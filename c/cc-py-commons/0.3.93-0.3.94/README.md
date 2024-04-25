# Comparing `tmp/cc_py_commons-0.3.93.tar.gz` & `tmp/cc_py_commons-0.3.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cc_py_commons-0.3.93.tar", last modified: Tue Apr  9 15:17:41 2024, max compression
+gzip compressed data, was "cc_py_commons-0.3.94.tar", last modified: Thu Apr 25 11:03:11 2024, max compression
```

## Comparing `cc_py_commons-0.3.93.tar` & `cc_py_commons-0.3.94.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.278895 cc_py_commons-0.3.93/
--rw-rw-r--   0 rof       (1001) rof       (1001)      210 2024-04-09 15:17:41.278895 cc_py_commons-0.3.93/PKG-INFO
--rw-rw-r--   0 rof       (1001) rof       (1001)     1118 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/README.md
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.262895 cc_py_commons-0.3.93/cc_py_commons/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/__init__.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.262895 cc_py_commons-0.3.93/cc_py_commons/bids/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/bids/__init__.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      802 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/bids/bid.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      300 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/bids/bid_history.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      471 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/bids/bid_history_schema.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     1332 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/bids/bid_schema.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.262895 cc_py_commons-0.3.93/cc_py_commons/carriers/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/carriers/__init__.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      233 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/carriers/account_carrier_map.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      687 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/carriers/account_carrier_map_schema.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     3094 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/carriers/carrier.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     2819 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/carriers/carrier_schema.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      429 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/carriers/contact.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      787 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/carriers/contact_schema.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.262895 cc_py_commons-0.3.93/cc_py_commons/config/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/config/__init__.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     6364 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/config/env.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     1364 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/config/mcleod_load_fields.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     1455 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/config/pc_miler_config.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.262895 cc_py_commons-0.3.93/cc_py_commons/db/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/db/__init__.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      566 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/db/connection.py
--rw-rw-r--   0 rof       (1001) rof       (1001)    13322 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/geolocate.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.266895 cc_py_commons-0.3.93/cc_py_commons/lanes/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/lanes/__init__.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      972 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/lanes/carrier_lane.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     1251 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/lanes/carrier_lane_schema.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      663 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/lanes/lane.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      941 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/lanes/lane_schema.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.266895 cc_py_commons-0.3.93/cc_py_commons/loads/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/loads/__init__.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      154 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/loads/equipment.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      384 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/loads/equipment_schema.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      965 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/loads/equipment_types.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      338 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/loads/freighthub_contact.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      442 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/loads/freighthub_contact_schema.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     3350 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/loads/load.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     4000 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/loads/load_schema.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      501 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/loads/load_status.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      286 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/loads/location.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      463 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/loads/location_schema.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      751 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/loads/map_load_response.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.270895 cc_py_commons-0.3.93/cc_py_commons/quotes/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/quotes/__init__.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     1967 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/quotes/quote.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     2638 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/quotes/quote_schema.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      501 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/quotes/quote_status.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.270895 cc_py_commons-0.3.93/cc_py_commons/rfp/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/rfp/__init__.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      145 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/rfp/rfp_status.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.270895 cc_py_commons-0.3.93/cc_py_commons/schemas/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/schemas/__init__.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      439 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/schemas/camel_case_schema.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.270895 cc_py_commons-0.3.93/cc_py_commons/services/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/__init__.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.270895 cc_py_commons-0.3.93/cc_py_commons/services/booking_agent/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/booking_agent/__init__.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      653 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/booking_agent/accept_bid.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      746 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/booking_agent/cancel_bid.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      671 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/booking_agent/constants.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      704 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/booking_agent/counter_bid.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      702 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/booking_agent/decline_bid.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      648 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/booking_agent/get_bid_by_amazon_order_id.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      943 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/booking_agent/get_quote.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      674 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/booking_agent/update_bid.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.270895 cc_py_commons-0.3.93/cc_py_commons/services/c4/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/c4/__init__.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      491 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/c4/amazon_session_token.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      147 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/c4/constants.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      922 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/c4/get_integration.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      681 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/c4/get_users_for_account.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      660 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/c4/refresh_amazon_token.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.270895 cc_py_commons-0.3.93/cc_py_commons/services/carrier_hub/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/carrier_hub/__init__.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      673 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/carrier_hub/get_carrier.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     1016 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/carrier_hub/list_carriers.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     1413 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/carrier_hub/list_contacts.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      724 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/carrier_hub/update_contact.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.274895 cc_py_commons-0.3.93/cc_py_commons/services/freight_hub/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/freight_hub/__init__.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      477 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/freight_hub/post_freight_hub_load.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.274895 cc_py_commons-0.3.93/cc_py_commons/services/mercury/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/mercury/__init__.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      571 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/mercury/get_green_screens_lane_price.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      553 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/mercury/get_lane_price.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      563 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/mercury/get_lane_price_for_bulk.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.274895 cc_py_commons-0.3.93/cc_py_commons/services/slack/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/slack/__init__.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     1044 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/services/slack/send_slack_message.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.274895 cc_py_commons-0.3.93/cc_py_commons/sns/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/sns/__init__.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      932 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/sns/book_load_notification.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.274895 cc_py_commons-0.3.93/cc_py_commons/sns/booking_agent/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/sns/booking_agent/__init__.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      971 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/sns/booking_agent/bid_counter_failure_notification.py
--rw-rw-r--   0 rof       (1001) rof       (1001)       77 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/sns/booking_agent/constants.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      747 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/sns/booking_agent/send_sns_notification.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      987 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/sns/booking_assistant_flow_notification.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      751 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/sns/import_movements_notification.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      901 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/sns/parsed_carrier_notification.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      269 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/sns/sns_service.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.274895 cc_py_commons-0.3.93/cc_py_commons/sqs/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/sqs/__init__.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     1152 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/sqs/booking_assistant_flow_event.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      440 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/sqs/sqs_service.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.274895 cc_py_commons-0.3.93/cc_py_commons/tests/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/tests/__init__.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      844 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/tests/test_case_conversion.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      760 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/tests/test_lambda_utils.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     2036 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/tests/test_map_transaction.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      475 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/tests/test_temperature_utils.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.278895 cc_py_commons-0.3.93/cc_py_commons/transactions/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/transactions/__init__.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      442 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/transactions/equipment_clas_schema.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      213 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/transactions/equipment_class.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      289 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/transactions/equipment_mapping.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      540 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/transactions/equipment_mapping_schema.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     3181 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/transactions/map_transaction.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     4931 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/transactions/transaction.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     5159 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/transactions/transaction_schema.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.278895 cc_py_commons-0.3.93/cc_py_commons/utils/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/utils/__init__.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     1519 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/utils/case_conversion.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     1168 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/utils/datadog_logger.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      759 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/utils/datetimes.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      723 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/utils/dimension_utils.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      513 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/utils/get_delivery_date.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      893 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/utils/json_logger.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      219 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/utils/lambda_utils.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     1051 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/utils/local_file.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      998 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/utils/logger.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     2026 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/utils/logger_v2.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     2792 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/utils/pc_miler_utils.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     1237 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/utils/price_utils.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     1044 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/utils/redis.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     2367 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/utils/s3_file.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      353 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/cc_py_commons/utils/temperature_utils.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-09 15:17:41.262895 cc_py_commons-0.3.93/cc_py_commons.egg-info/
--rw-rw-r--   0 rof       (1001) rof       (1001)      210 2024-04-09 15:17:41.000000 cc_py_commons-0.3.93/cc_py_commons.egg-info/PKG-INFO
--rw-rw-r--   0 rof       (1001) rof       (1001)     4989 2024-04-09 15:17:41.000000 cc_py_commons-0.3.93/cc_py_commons.egg-info/SOURCES.txt
--rw-rw-r--   0 rof       (1001) rof       (1001)        1 2024-04-09 15:17:41.000000 cc_py_commons-0.3.93/cc_py_commons.egg-info/dependency_links.txt
--rw-rw-r--   0 rof       (1001) rof       (1001)       66 2024-04-09 15:17:41.000000 cc_py_commons-0.3.93/cc_py_commons.egg-info/requires.txt
--rw-rw-r--   0 rof       (1001) rof       (1001)       14 2024-04-09 15:17:41.000000 cc_py_commons-0.3.93/cc_py_commons.egg-info/top_level.txt
--rw-rw-r--   0 rof       (1001) rof       (1001)       38 2024-04-09 15:17:41.278895 cc_py_commons-0.3.93/setup.cfg
--rw-rw-r--   0 rof       (1001) rof       (1001)      436 2024-04-09 15:17:15.000000 cc_py_commons-0.3.93/setup.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.137107 cc_py_commons-0.3.94/
+-rw-rw-r--   0 rof       (1001) rof       (1001)      210 2024-04-25 11:03:11.137107 cc_py_commons-0.3.94/PKG-INFO
+-rw-rw-r--   0 rof       (1001) rof       (1001)     1118 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/README.md
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.117107 cc_py_commons-0.3.94/cc_py_commons/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/__init__.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.117107 cc_py_commons-0.3.94/cc_py_commons/bids/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/bids/__init__.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      802 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/bids/bid.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      300 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/bids/bid_history.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      471 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/bids/bid_history_schema.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     1332 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/bids/bid_schema.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.121107 cc_py_commons-0.3.94/cc_py_commons/carriers/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/carriers/__init__.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      233 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/carriers/account_carrier_map.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      687 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/carriers/account_carrier_map_schema.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     3285 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/carriers/carrier.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     3038 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/carriers/carrier_schema.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      429 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/carriers/contact.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      787 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/carriers/contact_schema.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.121107 cc_py_commons-0.3.94/cc_py_commons/config/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/config/__init__.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     6364 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/config/env.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     1364 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/config/mcleod_load_fields.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     1455 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/config/pc_miler_config.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.121107 cc_py_commons-0.3.94/cc_py_commons/db/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/db/__init__.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      566 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/db/connection.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)    13322 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/geolocate.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.121107 cc_py_commons-0.3.94/cc_py_commons/lanes/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/lanes/__init__.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      972 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/lanes/carrier_lane.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     1251 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/lanes/carrier_lane_schema.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      663 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/lanes/lane.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      941 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/lanes/lane_schema.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.125107 cc_py_commons-0.3.94/cc_py_commons/loads/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/loads/__init__.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      154 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/loads/equipment.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      384 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/loads/equipment_schema.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      965 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/loads/equipment_types.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      338 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/loads/freighthub_contact.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      442 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/loads/freighthub_contact_schema.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     3350 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/loads/load.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     4000 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/loads/load_schema.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      501 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/loads/load_status.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      286 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/loads/location.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      463 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/loads/location_schema.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      751 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/loads/map_load_response.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.125107 cc_py_commons-0.3.94/cc_py_commons/quotes/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/quotes/__init__.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     1967 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/quotes/quote.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     2638 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/quotes/quote_schema.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      501 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/quotes/quote_status.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.125107 cc_py_commons-0.3.94/cc_py_commons/rfp/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/rfp/__init__.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      145 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/rfp/rfp_status.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.125107 cc_py_commons-0.3.94/cc_py_commons/schemas/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/schemas/__init__.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      439 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/schemas/camel_case_schema.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.125107 cc_py_commons-0.3.94/cc_py_commons/services/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/__init__.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.125107 cc_py_commons-0.3.94/cc_py_commons/services/booking_agent/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/booking_agent/__init__.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      653 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/booking_agent/accept_bid.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      746 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/booking_agent/cancel_bid.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      671 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/booking_agent/constants.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      704 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/booking_agent/counter_bid.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      702 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/booking_agent/decline_bid.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      648 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/booking_agent/get_bid_by_amazon_order_id.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      943 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/booking_agent/get_quote.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      674 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/booking_agent/update_bid.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.129107 cc_py_commons-0.3.94/cc_py_commons/services/c4/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/c4/__init__.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      491 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/c4/amazon_session_token.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      147 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/c4/constants.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      922 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/c4/get_integration.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      681 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/c4/get_users_for_account.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      660 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/c4/refresh_amazon_token.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.129107 cc_py_commons-0.3.94/cc_py_commons/services/carrier_hub/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/carrier_hub/__init__.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      673 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/carrier_hub/get_carrier.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     1016 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/carrier_hub/list_carriers.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     1413 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/carrier_hub/list_contacts.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      724 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/carrier_hub/update_contact.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.129107 cc_py_commons-0.3.94/cc_py_commons/services/freight_hub/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/freight_hub/__init__.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      477 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/freight_hub/post_freight_hub_load.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.129107 cc_py_commons-0.3.94/cc_py_commons/services/mercury/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/mercury/__init__.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      571 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/mercury/get_green_screens_lane_price.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      553 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/mercury/get_lane_price.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      563 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/mercury/get_lane_price_for_bulk.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.129107 cc_py_commons-0.3.94/cc_py_commons/services/slack/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/slack/__init__.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     1044 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/services/slack/send_slack_message.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.129107 cc_py_commons-0.3.94/cc_py_commons/sns/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/sns/__init__.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      932 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/sns/book_load_notification.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.133107 cc_py_commons-0.3.94/cc_py_commons/sns/booking_agent/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/sns/booking_agent/__init__.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      971 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/sns/booking_agent/bid_counter_failure_notification.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)       77 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/sns/booking_agent/constants.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      747 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/sns/booking_agent/send_sns_notification.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      987 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/sns/booking_assistant_flow_notification.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      751 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/sns/import_movements_notification.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      901 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/sns/parsed_carrier_notification.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      269 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/sns/sns_service.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.133107 cc_py_commons-0.3.94/cc_py_commons/sqs/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/sqs/__init__.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     1152 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/sqs/booking_assistant_flow_event.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      440 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/sqs/sqs_service.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.133107 cc_py_commons-0.3.94/cc_py_commons/tests/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/tests/__init__.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      844 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/tests/test_case_conversion.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      760 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/tests/test_lambda_utils.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     2036 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/tests/test_map_transaction.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      475 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/tests/test_temperature_utils.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.133107 cc_py_commons-0.3.94/cc_py_commons/transactions/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/transactions/__init__.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      442 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/transactions/equipment_clas_schema.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      213 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/transactions/equipment_class.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      289 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/transactions/equipment_mapping.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      540 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/transactions/equipment_mapping_schema.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     3181 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/transactions/map_transaction.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     4931 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/transactions/transaction.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     5159 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/transactions/transaction_schema.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.137107 cc_py_commons-0.3.94/cc_py_commons/utils/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/utils/__init__.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     1519 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/utils/case_conversion.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     1168 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/utils/datadog_logger.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      759 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/utils/datetimes.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      723 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/utils/dimension_utils.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      513 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/utils/get_delivery_date.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      893 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/utils/json_logger.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      219 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/utils/lambda_utils.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     1051 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/utils/local_file.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      998 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/utils/logger.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     2026 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/utils/logger_v2.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     2792 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/utils/pc_miler_utils.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     1237 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/utils/price_utils.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     1044 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/utils/redis.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     2367 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/utils/s3_file.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      353 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/cc_py_commons/utils/temperature_utils.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2024-04-25 11:03:11.117107 cc_py_commons-0.3.94/cc_py_commons.egg-info/
+-rw-rw-r--   0 rof       (1001) rof       (1001)      210 2024-04-25 11:03:11.000000 cc_py_commons-0.3.94/cc_py_commons.egg-info/PKG-INFO
+-rw-rw-r--   0 rof       (1001) rof       (1001)     4989 2024-04-25 11:03:11.000000 cc_py_commons-0.3.94/cc_py_commons.egg-info/SOURCES.txt
+-rw-rw-r--   0 rof       (1001) rof       (1001)        1 2024-04-25 11:03:11.000000 cc_py_commons-0.3.94/cc_py_commons.egg-info/dependency_links.txt
+-rw-rw-r--   0 rof       (1001) rof       (1001)       66 2024-04-25 11:03:11.000000 cc_py_commons-0.3.94/cc_py_commons.egg-info/requires.txt
+-rw-rw-r--   0 rof       (1001) rof       (1001)       14 2024-04-25 11:03:11.000000 cc_py_commons-0.3.94/cc_py_commons.egg-info/top_level.txt
+-rw-rw-r--   0 rof       (1001) rof       (1001)       38 2024-04-25 11:03:11.137107 cc_py_commons-0.3.94/setup.cfg
+-rw-rw-r--   0 rof       (1001) rof       (1001)      436 2024-04-25 11:02:48.000000 cc_py_commons-0.3.94/setup.py
```

### Comparing `cc_py_commons-0.3.93/README.md` & `cc_py_commons-0.3.94/README.md`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/bids/bid.py` & `cc_py_commons-0.3.94/cc_py_commons/bids/bid.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/bids/bid_schema.py` & `cc_py_commons-0.3.94/cc_py_commons/bids/bid_schema.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/carriers/account_carrier_map_schema.py` & `cc_py_commons-0.3.94/cc_py_commons/carriers/account_carrier_map_schema.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/carriers/carrier.py` & `cc_py_commons-0.3.94/cc_py_commons/carriers/carrier.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,7 +63,12 @@
   internal_remarks: str = field(default=None)
   contact: Contact = field(default=None)
   account_carrier_maps: List[AccountCarrierMap] = field(default_factory=lambda: [])
   lanes: List[Lane] = field(default_factory=lambda: [])
   carrier_manager_id: str = field(default=None)
   rmis_carrier: Dict = field(default=None)
   contacts: List[Contact] = field(default=None)
+  authority: str = field(default=None)
+  insurance: str = field(default=None)
+  operations: str = field(default=None)
+  safety: str = field(default=None)
+  overall: str = field(default=None)
```

### Comparing `cc_py_commons-0.3.93/cc_py_commons/carriers/carrier_schema.py` & `cc_py_commons-0.3.94/cc_py_commons/carriers/carrier_schema.py`

 * *Files 24% similar despite different names*

```diff
@@ -53,11 +53,16 @@
   contact = fields.Nested(ContactSchema, allow_none=True)
   account_carrier_maps = fields.List(fields.Nested(AccountCarrierMapSchema))
   lanes = fields.List(fields.Nested(LaneSchema))
   equipment_preferences = fields.List(fields.String)
   no_dispatch = fields.Boolean(allow_none=True)
   rmis_carrier = fields.Dict(allow_none=True, cls_or_instance=fields.Raw())
   contacts = fields.List(fields.Nested(ContactSchema, allow_none=True))
-  
+  authority = fields.String(allow_none=True)
+  insurance = fields.String(allow_none=True)
+  operations = fields.String(allow_none=True)
+  safety = fields.String(allow_none=True)
+  overall = fields.String(allow_none=True)
+
   @post_load
   def make_bid(self, data, **kwargs):
       return Carrier(**data)
```

### Comparing `cc_py_commons-0.3.93/cc_py_commons/carriers/contact_schema.py` & `cc_py_commons-0.3.94/cc_py_commons/carriers/contact_schema.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/config/env.py` & `cc_py_commons-0.3.94/cc_py_commons/config/env.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/config/mcleod_load_fields.py` & `cc_py_commons-0.3.94/cc_py_commons/config/mcleod_load_fields.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/config/pc_miler_config.py` & `cc_py_commons-0.3.94/cc_py_commons/config/pc_miler_config.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/db/connection.py` & `cc_py_commons-0.3.94/cc_py_commons/db/connection.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/geolocate.py` & `cc_py_commons-0.3.94/cc_py_commons/geolocate.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/lanes/carrier_lane.py` & `cc_py_commons-0.3.94/cc_py_commons/lanes/carrier_lane.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/lanes/carrier_lane_schema.py` & `cc_py_commons-0.3.94/cc_py_commons/lanes/carrier_lane_schema.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/lanes/lane.py` & `cc_py_commons-0.3.94/cc_py_commons/lanes/lane.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/lanes/lane_schema.py` & `cc_py_commons-0.3.94/cc_py_commons/lanes/lane_schema.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/loads/equipment_types.py` & `cc_py_commons-0.3.94/cc_py_commons/loads/equipment_types.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/loads/load.py` & `cc_py_commons-0.3.94/cc_py_commons/loads/load.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/loads/load_schema.py` & `cc_py_commons-0.3.94/cc_py_commons/loads/load_schema.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/loads/map_load_response.py` & `cc_py_commons-0.3.94/cc_py_commons/loads/map_load_response.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/quotes/quote.py` & `cc_py_commons-0.3.94/cc_py_commons/quotes/quote.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/quotes/quote_schema.py` & `cc_py_commons-0.3.94/cc_py_commons/quotes/quote_schema.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/services/booking_agent/accept_bid.py` & `cc_py_commons-0.3.94/cc_py_commons/services/booking_agent/accept_bid.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/services/booking_agent/cancel_bid.py` & `cc_py_commons-0.3.94/cc_py_commons/services/booking_agent/cancel_bid.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/services/booking_agent/constants.py` & `cc_py_commons-0.3.94/cc_py_commons/services/booking_agent/constants.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/services/booking_agent/counter_bid.py` & `cc_py_commons-0.3.94/cc_py_commons/services/booking_agent/counter_bid.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/services/booking_agent/decline_bid.py` & `cc_py_commons-0.3.94/cc_py_commons/services/booking_agent/decline_bid.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/services/booking_agent/get_bid_by_amazon_order_id.py` & `cc_py_commons-0.3.94/cc_py_commons/services/booking_agent/get_bid_by_amazon_order_id.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/services/booking_agent/get_quote.py` & `cc_py_commons-0.3.94/cc_py_commons/services/booking_agent/get_quote.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/services/booking_agent/update_bid.py` & `cc_py_commons-0.3.94/cc_py_commons/services/booking_agent/update_bid.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/services/c4/get_integration.py` & `cc_py_commons-0.3.94/cc_py_commons/services/c4/get_integration.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/services/c4/get_users_for_account.py` & `cc_py_commons-0.3.94/cc_py_commons/services/c4/get_users_for_account.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/services/c4/refresh_amazon_token.py` & `cc_py_commons-0.3.94/cc_py_commons/services/c4/refresh_amazon_token.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/services/carrier_hub/get_carrier.py` & `cc_py_commons-0.3.94/cc_py_commons/services/carrier_hub/get_carrier.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/services/carrier_hub/list_carriers.py` & `cc_py_commons-0.3.94/cc_py_commons/services/carrier_hub/list_carriers.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/services/carrier_hub/list_contacts.py` & `cc_py_commons-0.3.94/cc_py_commons/services/carrier_hub/list_contacts.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/services/carrier_hub/update_contact.py` & `cc_py_commons-0.3.94/cc_py_commons/services/carrier_hub/update_contact.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/services/mercury/get_green_screens_lane_price.py` & `cc_py_commons-0.3.94/cc_py_commons/services/mercury/get_green_screens_lane_price.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/services/mercury/get_lane_price.py` & `cc_py_commons-0.3.94/cc_py_commons/services/mercury/get_lane_price.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/services/mercury/get_lane_price_for_bulk.py` & `cc_py_commons-0.3.94/cc_py_commons/services/mercury/get_lane_price_for_bulk.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/services/slack/send_slack_message.py` & `cc_py_commons-0.3.94/cc_py_commons/services/slack/send_slack_message.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/sns/book_load_notification.py` & `cc_py_commons-0.3.94/cc_py_commons/sns/book_load_notification.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/sns/booking_agent/bid_counter_failure_notification.py` & `cc_py_commons-0.3.94/cc_py_commons/sns/booking_agent/bid_counter_failure_notification.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/sns/booking_agent/send_sns_notification.py` & `cc_py_commons-0.3.94/cc_py_commons/sns/booking_agent/send_sns_notification.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/sns/booking_assistant_flow_notification.py` & `cc_py_commons-0.3.94/cc_py_commons/sns/booking_assistant_flow_notification.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/sns/import_movements_notification.py` & `cc_py_commons-0.3.94/cc_py_commons/sns/import_movements_notification.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/sns/parsed_carrier_notification.py` & `cc_py_commons-0.3.94/cc_py_commons/sns/parsed_carrier_notification.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/sqs/booking_assistant_flow_event.py` & `cc_py_commons-0.3.94/cc_py_commons/sqs/booking_assistant_flow_event.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/tests/test_case_conversion.py` & `cc_py_commons-0.3.94/cc_py_commons/tests/test_case_conversion.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/tests/test_lambda_utils.py` & `cc_py_commons-0.3.94/cc_py_commons/tests/test_lambda_utils.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/tests/test_map_transaction.py` & `cc_py_commons-0.3.94/cc_py_commons/tests/test_map_transaction.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/transactions/equipment_mapping_schema.py` & `cc_py_commons-0.3.94/cc_py_commons/transactions/equipment_mapping_schema.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/transactions/map_transaction.py` & `cc_py_commons-0.3.94/cc_py_commons/transactions/map_transaction.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/transactions/transaction.py` & `cc_py_commons-0.3.94/cc_py_commons/transactions/transaction.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/transactions/transaction_schema.py` & `cc_py_commons-0.3.94/cc_py_commons/transactions/transaction_schema.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/utils/case_conversion.py` & `cc_py_commons-0.3.94/cc_py_commons/utils/case_conversion.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/utils/datadog_logger.py` & `cc_py_commons-0.3.94/cc_py_commons/utils/datadog_logger.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/utils/datetimes.py` & `cc_py_commons-0.3.94/cc_py_commons/utils/datetimes.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/utils/dimension_utils.py` & `cc_py_commons-0.3.94/cc_py_commons/utils/dimension_utils.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/utils/get_delivery_date.py` & `cc_py_commons-0.3.94/cc_py_commons/utils/get_delivery_date.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/utils/json_logger.py` & `cc_py_commons-0.3.94/cc_py_commons/utils/json_logger.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/utils/local_file.py` & `cc_py_commons-0.3.94/cc_py_commons/utils/local_file.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/utils/logger.py` & `cc_py_commons-0.3.94/cc_py_commons/utils/logger.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/utils/logger_v2.py` & `cc_py_commons-0.3.94/cc_py_commons/utils/logger_v2.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/utils/pc_miler_utils.py` & `cc_py_commons-0.3.94/cc_py_commons/utils/pc_miler_utils.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/utils/price_utils.py` & `cc_py_commons-0.3.94/cc_py_commons/utils/price_utils.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/utils/redis.py` & `cc_py_commons-0.3.94/cc_py_commons/utils/redis.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons/utils/s3_file.py` & `cc_py_commons-0.3.94/cc_py_commons/utils/s3_file.py`

 * *Files identical despite different names*

### Comparing `cc_py_commons-0.3.93/cc_py_commons.egg-info/SOURCES.txt` & `cc_py_commons-0.3.94/cc_py_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

