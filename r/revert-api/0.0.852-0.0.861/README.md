# Comparing `tmp/revert_api-0.0.852.tar.gz` & `tmp/revert_api-0.0.861.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revert_api-0.0.852.tar", max compression
+gzip compressed data, was "revert_api-0.0.861.tar", max compression
```

## Comparing `revert_api-0.0.852.tar` & `revert_api-0.0.861.tar`

### file list

```diff
@@ -1,242 +1,242 @@
--rw-r--r--   0        0        0     1688 2024-04-23 10:35:09.182742 revert_api-0.0.852/README.md
--rw-r--r--   0        0        0      404 2024-04-23 10:35:09.182742 revert_api-0.0.852/pyproject.toml
--rw-r--r--   0        0        0     2021 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/__init__.py
--rw-r--r--   0        0        0     3175 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/client.py
--rw-r--r--   0        0        0      519 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/core/api_error.py
--rw-r--r--   0        0        0      930 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      310 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/environment.py
--rw-r--r--   0        0        0        0 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/py.typed
--rw-r--r--   0        0        0     1988 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/__init__.py
--rw-r--r--   0        0        0      431 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/chat/__init__.py
--rw-r--r--   0        0        0     1075 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/chat/client.py
--rw-r--r--   0        0        0      449 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/chat/resources/__init__.py
--rw-r--r--   0        0        0      139 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/chat/resources/channels/__init__.py
--rw-r--r--   0        0        0     5785 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/chat/resources/channels/client.py
--rw-r--r--   0        0        0      155 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/chat/resources/channels/types/__init__.py
--rw-r--r--   0        0        0     1134 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/chat/resources/channels/types/get_channels_response.py
--rw-r--r--   0        0        0      221 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/chat/resources/messages/__init__.py
--rw-r--r--   0        0        0     5982 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/chat/resources/messages/client.py
--rw-r--r--   0        0        0      292 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/chat/resources/messages/types/__init__.py
--rw-r--r--   0        0        0      860 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/chat/resources/messages/types/createor_update_message_request.py
--rw-r--r--   0        0        0     1064 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/chat/resources/messages/types/createor_update_message_response.py
--rw-r--r--   0        0        0      133 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/chat/resources/users/__init__.py
--rw-r--r--   0        0        0     5743 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/chat/resources/users/client.py
--rw-r--r--   0        0        0      146 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/chat/resources/users/types/__init__.py
--rw-r--r--   0        0        0     1135 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/chat/resources/users/types/get_users_response.py
--rw-r--r--   0        0        0     2021 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/__init__.py
--rw-r--r--   0        0        0     2093 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/__init__.py
--rw-r--r--   0        0        0      381 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/associations/__init__.py
--rw-r--r--   0        0        0      515 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/associations/types/__init__.py
--rw-r--r--   0        0        0     1190 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/associations/types/company_association.py
--rw-r--r--   0        0        0     1341 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/associations/types/contact_association.py
--rw-r--r--   0        0        0     1327 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/associations/types/deal_association.py
--rw-r--r--   0        0        0     1378 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/associations/types/event_association.py
--rw-r--r--   0        0        0     1506 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/associations/types/lead_association.py
--rw-r--r--   0        0        0     1185 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/associations/types/task_association.py
--rw-r--r--   0        0        0      361 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/errors/__init__.py
--rw-r--r--   0        0        0      431 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/errors/errors/__init__.py
--rw-r--r--   0        0        0      277 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/errors/errors/bad_request_error.py
--rw-r--r--   0        0        0      281 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/errors/errors/internal_server_error.py
--rw-r--r--   0        0        0      275 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/errors/errors/not_found_error.py
--rw-r--r--   0        0        0      281 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/errors/errors/not_implemented_error.py
--rw-r--r--   0        0        0      279 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/errors/errors/un_authorized_error.py
--rw-r--r--   0        0        0      124 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/errors/types/__init__.py
--rw-r--r--   0        0        0      871 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/errors/types/base_error.py
--rw-r--r--   0        0        0      437 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/types/__init__.py
--rw-r--r--   0        0        0      607 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/types/types/__init__.py
--rw-r--r--   0        0        0     1308 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/types/types/account.py
--rw-r--r--   0        0        0     1420 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/types/types/app.py
--rw-r--r--   0        0        0      926 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/types/types/app_config.py
--rw-r--r--   0        0        0     1300 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/types/types/connection.py
--rw-r--r--   0        0        0      441 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/types/types/response_status.py
--rw-r--r--   0        0        0     1155 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/types/types/revert_user.py
--rw-r--r--   0        0        0     1286 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/types/types/standard_object.py
--rw-r--r--   0        0        0      889 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/types/types/ticket_priority.py
--rw-r--r--   0        0        0      638 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/types/types/ticket_status.py
--rw-r--r--   0        0        0     1207 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/types/types/tpid.py
--rw-r--r--   0        0        0     1021 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/__init__.py
--rw-r--r--   0        0        0     1537 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/__init__.py
--rw-r--r--   0        0        0     1213 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/channel.py
--rw-r--r--   0        0        0     1123 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/comment_ticket_write.py
--rw-r--r--   0        0        0     1594 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/common_unified_fields.py
--rw-r--r--   0        0        0     1729 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/company.py
--rw-r--r--   0        0        0     1057 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/company_address.py
--rw-r--r--   0        0        0      893 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/contact.py
--rw-r--r--   0        0        0     1294 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/contact_read.py
--rw-r--r--   0        0        0      950 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/contact_write.py
--rw-r--r--   0        0        0      881 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/deal.py
--rw-r--r--   0        0        0     1742 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/deal_read.py
--rw-r--r--   0        0        0      929 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/deal_write.py
--rw-r--r--   0        0        0      885 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/event.py
--rw-r--r--   0        0        0     1588 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/event_read.py
--rw-r--r--   0        0        0      936 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/event_write.py
--rw-r--r--   0        0        0      881 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/lead.py
--rw-r--r--   0        0        0     1279 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/lead_read.py
--rw-r--r--   0        0        0      929 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/lead_write.py
--rw-r--r--   0        0        0     1078 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/message.py
--rw-r--r--   0        0        0      881 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/note.py
--rw-r--r--   0        0        0      952 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/note_read.py
--rw-r--r--   0        0        0      929 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/note_write.py
--rw-r--r--   0        0        0      881 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/task.py
--rw-r--r--   0        0        0     1345 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/task_read.py
--rw-r--r--   0        0        0      909 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/task_ticket.py
--rw-r--r--   0        0        0     1912 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/task_ticket_write.py
--rw-r--r--   0        0        0      974 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/task_write.py
--rw-r--r--   0        0        0      884 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/user.py
--rw-r--r--   0        0        0     1231 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/user_chat.py
--rw-r--r--   0        0        0     1408 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/common/resources/unified/types/user_write.py
--rw-r--r--   0        0        0      867 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/connection/__init__.py
--rw-r--r--   0        0        0    34428 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/connection/client.py
--rw-r--r--   0        0        0     1279 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/connection/types/__init__.py
--rw-r--r--   0        0        0     1304 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/connection/types/connection_import.py
--rw-r--r--   0        0        0      477 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/connection/types/connection_status.py
--rw-r--r--   0        0        0      979 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/connection/types/create_connection_webhook_request.py
--rw-r--r--   0        0        0     1272 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/connection/types/create_connection_webhook_response.py
--rw-r--r--   0        0        0     1061 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/connection/types/delete_connection_response.py
--rw-r--r--   0        0        0     1142 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/connection/types/delete_connection_webhook_response.py
--rw-r--r--   0        0        0      198 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/connection/types/get_all_connection_response.py
--rw-r--r--   0        0        0     1264 2024-04-23 10:35:09.182742 revert_api-0.0.852/src/revert/resources/connection/types/get_connect_status_response.py
--rw-r--r--   0        0        0      889 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/connection/types/get_connection_response.py
--rw-r--r--   0        0        0     1163 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/connection/types/get_connection_webhook_response.py
--rw-r--r--   0        0        0      968 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/connection/types/import_connections_request_body.py
--rw-r--r--   0        0        0      972 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/connection/types/import_connections_response.py
--rw-r--r--   0        0        0     3061 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/__init__.py
--rw-r--r--   0        0        0     2536 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/client.py
--rw-r--r--   0        0        0     3207 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/__init__.py
--rw-r--r--   0        0        0      409 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/company/__init__.py
--rw-r--r--   0        0        0    23881 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/company/client.py
--rw-r--r--   0        0        0      563 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/company/types/__init__.py
--rw-r--r--   0        0        0     1007 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/company/types/create_or_update_company_request.py
--rw-r--r--   0        0        0     1020 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/company/types/create_or_update_company_response.py
--rw-r--r--   0        0        0     1135 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/company/types/get_companies_response.py
--rw-r--r--   0        0        0     1053 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/company/types/get_company_response.py
--rw-r--r--   0        0        0     1072 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/company/types/search_companies_response.py
--rw-r--r--   0        0        0      405 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/contact/__init__.py
--rw-r--r--   0        0        0    24439 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/contact/client.py
--rw-r--r--   0        0        0      557 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/contact/types/__init__.py
--rw-r--r--   0        0        0     1145 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/contact/types/create_or_update_contact_request.py
--rw-r--r--   0        0        0     1020 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/contact/types/create_or_update_contact_response.py
--rw-r--r--   0        0        0     1053 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/contact/types/get_contact_response.py
--rw-r--r--   0        0        0     1134 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/contact/types/get_contacts_response.py
--rw-r--r--   0        0        0     1071 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/contact/types/search_contacts_response.py
--rw-r--r--   0        0        0      375 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/deal/__init__.py
--rw-r--r--   0        0        0    23576 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/deal/client.py
--rw-r--r--   0        0        0      512 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/deal/types/__init__.py
--rw-r--r--   0        0        0     1133 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/deal/types/create_or_update_deal_request.py
--rw-r--r--   0        0        0     1017 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/deal/types/create_or_update_deal_response.py
--rw-r--r--   0        0        0     1041 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/deal/types/get_deal_response.py
--rw-r--r--   0        0        0     1122 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/deal/types/get_deals_response.py
--rw-r--r--   0        0        0     1059 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/deal/types/search_deals_response.py
--rw-r--r--   0        0        0      437 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/event/__init__.py
--rw-r--r--   0        0        0    27691 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/event/client.py
--rw-r--r--   0        0        0      609 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/event/types/__init__.py
--rw-r--r--   0        0        0     1137 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/event/types/create_or_update_event_request.py
--rw-r--r--   0        0        0     1018 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/event/types/create_or_update_event_response.py
--rw-r--r--   0        0        0      987 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/event/types/delete_event_response.py
--rw-r--r--   0        0        0     1045 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/event/types/get_event_response.py
--rw-r--r--   0        0        0     1126 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/event/types/get_events_response.py
--rw-r--r--   0        0        0     1063 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/event/types/search_events_response.py
--rw-r--r--   0        0        0      375 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/lead/__init__.py
--rw-r--r--   0        0        0    23576 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/lead/client.py
--rw-r--r--   0        0        0      512 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/lead/types/__init__.py
--rw-r--r--   0        0        0     1133 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/lead/types/create_or_update_lead_request.py
--rw-r--r--   0        0        0     1017 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/lead/types/create_or_update_lead_response.py
--rw-r--r--   0        0        0     1041 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/lead/types/get_lead_response.py
--rw-r--r--   0        0        0     1122 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/lead/types/get_leads_response.py
--rw-r--r--   0        0        0     1059 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/lead/types/search_leads_response.py
--rw-r--r--   0        0        0      375 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/note/__init__.py
--rw-r--r--   0        0        0    23576 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/note/client.py
--rw-r--r--   0        0        0      512 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/note/types/__init__.py
--rw-r--r--   0        0        0     1133 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/note/types/create_or_update_note_request.py
--rw-r--r--   0        0        0     1017 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/note/types/create_or_update_note_response.py
--rw-r--r--   0        0        0     1041 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/note/types/get_note_response.py
--rw-r--r--   0        0        0     1122 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/note/types/get_notes_response.py
--rw-r--r--   0        0        0     1059 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/note/types/search_notes_response.py
--rw-r--r--   0        0        0      465 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/properties/__init__.py
--rw-r--r--   0        0        0    10251 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/properties/client.py
--rw-r--r--   0        0        0      652 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/properties/types/__init__.py
--rw-r--r--   0        0        0      912 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/properties/types/field_details_type.py
--rw-r--r--   0        0        0     1026 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/properties/types/field_details_type_read.py
--rw-r--r--   0        0        0     1118 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/properties/types/field_details_type_request.py
--rw-r--r--   0        0        0      203 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/properties/types/get_object_properties_response.py
--rw-r--r--   0        0        0      183 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/properties/types/set_object_properties_request.py
--rw-r--r--   0        0        0      121 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/properties/types/set_object_properties_response.py
--rw-r--r--   0        0        0      173 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/proxy/__init__.py
--rw-r--r--   0        0        0     5499 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/proxy/client.py
--rw-r--r--   0        0        0      218 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/proxy/types/__init__.py
--rw-r--r--   0        0        0     1065 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/proxy/types/post_proxy_request_body.py
--rw-r--r--   0        0        0      883 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/proxy/types/proxy_response.py
--rw-r--r--   0        0        0      375 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/task/__init__.py
--rw-r--r--   0        0        0    23576 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/task/client.py
--rw-r--r--   0        0        0      512 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/task/types/__init__.py
--rw-r--r--   0        0        0     1133 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/task/types/create_or_update_task_request.py
--rw-r--r--   0        0        0     1017 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/task/types/create_or_update_task_response.py
--rw-r--r--   0        0        0     1041 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/task/types/get_task_response.py
--rw-r--r--   0        0        0     1122 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/task/types/get_tasks_response.py
--rw-r--r--   0        0        0     1059 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/task/types/search_tasks_response.py
--rw-r--r--   0        0        0      283 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/user/__init__.py
--rw-r--r--   0        0        0    14641 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/user/client.py
--rw-r--r--   0        0        0      411 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/user/types/__init__.py
--rw-r--r--   0        0        0     1133 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/user/types/create_or_update_user_request.py
--rw-r--r--   0        0        0     1017 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/user/types/create_or_update_user_response.py
--rw-r--r--   0        0        0     1041 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/user/types/get_user_response.py
--rw-r--r--   0        0        0     1122 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/crm/resources/user/types/get_users_response.py
--rw-r--r--   0        0        0      793 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/field_mapping/__init__.py
--rw-r--r--   0        0        0    22972 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/field_mapping/client.py
--rw-r--r--   0        0        0     1170 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/field_mapping/types/__init__.py
--rw-r--r--   0        0        0     1052 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/field_mapping/types/create_account_field_mapping_request_body.py
--rw-r--r--   0        0        0      980 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/field_mapping/types/create_account_field_mapping_response.py
--rw-r--r--   0        0        0     1157 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/field_mapping/types/create_field_mapping_request_body.py
--rw-r--r--   0        0        0      973 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/field_mapping/types/create_field_mapping_response.py
--rw-r--r--   0        0        0      986 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/field_mapping/types/delete_account_field_mapping_config_response.py
--rw-r--r--   0        0        0      990 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/field_mapping/types/delete_field_mapping_response.py
--rw-r--r--   0        0        0     1061 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/field_mapping/types/field_mapping_type.py
--rw-r--r--   0        0        0     1206 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/field_mapping/types/get_field_mapping_config_response.py
--rw-r--r--   0        0        0     1054 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/field_mapping/types/get_field_mappings_response.py
--rw-r--r--   0        0        0     1108 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/field_mapping/types/mappable_field_type.py
--rw-r--r--   0        0        0      191 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/metadata/__init__.py
--rw-r--r--   0        0        0     3656 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/metadata/client.py
--rw-r--r--   0        0        0      255 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/metadata/types/__init__.py
--rw-r--r--   0        0        0     1190 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/metadata/types/crm_metadata.py
--rw-r--r--   0        0        0      985 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/metadata/types/crm_metadata_response.py
--rw-r--r--   0        0        0      461 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/metadata/types/crm_status.py
--rw-r--r--   0        0        0      139 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/sync/__init__.py
--rw-r--r--   0        0        0     5258 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/sync/client.py
--rw-r--r--   0        0        0      155 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/sync/types/__init__.py
--rw-r--r--   0        0        0      966 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/sync/types/trigger_sync_response.py
--rw-r--r--   0        0        0      943 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/__init__.py
--rw-r--r--   0        0        0     1494 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/client.py
--rw-r--r--   0        0        0      973 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/__init__.py
--rw-r--r--   0        0        0      145 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/collection/__init__.py
--rw-r--r--   0        0        0     5829 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/collection/client.py
--rw-r--r--   0        0        0      164 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/collection/types/__init__.py
--rw-r--r--   0        0        0     1063 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/collection/types/get_collections_response.py
--rw-r--r--   0        0        0      307 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/comment/__init__.py
--rw-r--r--   0        0        0    19749 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/comment/client.py
--rw-r--r--   0        0        0      447 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/comment/types/__init__.py
--rw-r--r--   0        0        0      204 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/comment/types/create_or_update_comment_request.py
--rw-r--r--   0        0        0     1020 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/comment/types/create_or_update_comment_response.py
--rw-r--r--   0        0        0      992 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/comment/types/get_comment_response.py
--rw-r--r--   0        0        0     1060 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/comment/types/get_comments_response.py
--rw-r--r--   0        0        0      173 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/proxy/__init__.py
--rw-r--r--   0        0        0     5529 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/proxy/client.py
--rw-r--r--   0        0        0      218 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/proxy/types/__init__.py
--rw-r--r--   0        0        0     1065 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/proxy/types/post_proxy_request_body.py
--rw-r--r--   0        0        0      883 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/proxy/types/proxy_response.py
--rw-r--r--   0        0        0      283 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/task/__init__.py
--rw-r--r--   0        0        0    19908 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/task/client.py
--rw-r--r--   0        0        0      411 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/task/types/__init__.py
--rw-r--r--   0        0        0      192 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/task/types/create_or_update_task_request.py
--rw-r--r--   0        0        0     1017 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/task/types/create_or_update_task_response.py
--rw-r--r--   0        0        0     1060 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/task/types/get_task_response.py
--rw-r--r--   0        0        0     1141 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/task/types/get_tasks_response.py
--rw-r--r--   0        0        0      169 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/user/__init__.py
--rw-r--r--   0        0        0    10114 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/user/client.py
--rw-r--r--   0        0        0      212 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/user/types/__init__.py
--rw-r--r--   0        0        0      989 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/user/types/get_user_response.py
--rw-r--r--   0        0        0     1057 2024-04-23 10:35:09.186742 revert_api-0.0.852/src/revert/resources/ticket/resources/user/types/get_users_response.py
--rw-r--r--   0        0        0     2197 1970-01-01 00:00:00.000000 revert_api-0.0.852/PKG-INFO
+-rw-r--r--   0        0        0     1688 2024-04-25 13:24:05.190787 revert_api-0.0.861/README.md
+-rw-r--r--   0        0        0      404 2024-04-25 13:24:05.190787 revert_api-0.0.861/pyproject.toml
+-rw-r--r--   0        0        0     2021 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/__init__.py
+-rw-r--r--   0        0        0     3175 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/client.py
+-rw-r--r--   0        0        0      519 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/core/api_error.py
+-rw-r--r--   0        0        0      930 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      310 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/environment.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/py.typed
+-rw-r--r--   0        0        0     1988 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/resources/__init__.py
+-rw-r--r--   0        0        0      431 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/resources/chat/__init__.py
+-rw-r--r--   0        0        0     1075 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/resources/chat/client.py
+-rw-r--r--   0        0        0      449 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/resources/chat/resources/__init__.py
+-rw-r--r--   0        0        0      139 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/resources/chat/resources/channels/__init__.py
+-rw-r--r--   0        0        0     5785 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/resources/chat/resources/channels/client.py
+-rw-r--r--   0        0        0      155 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/resources/chat/resources/channels/types/__init__.py
+-rw-r--r--   0        0        0     1134 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/resources/chat/resources/channels/types/get_channels_response.py
+-rw-r--r--   0        0        0      221 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/resources/chat/resources/messages/__init__.py
+-rw-r--r--   0        0        0     5982 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/resources/chat/resources/messages/client.py
+-rw-r--r--   0        0        0      292 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/resources/chat/resources/messages/types/__init__.py
+-rw-r--r--   0        0        0      860 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/resources/chat/resources/messages/types/createor_update_message_request.py
+-rw-r--r--   0        0        0     1064 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/resources/chat/resources/messages/types/createor_update_message_response.py
+-rw-r--r--   0        0        0      133 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/resources/chat/resources/users/__init__.py
+-rw-r--r--   0        0        0     5743 2024-04-25 13:24:05.190787 revert_api-0.0.861/src/revert/resources/chat/resources/users/client.py
+-rw-r--r--   0        0        0      146 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/chat/resources/users/types/__init__.py
+-rw-r--r--   0        0        0     1135 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/chat/resources/users/types/get_users_response.py
+-rw-r--r--   0        0        0     2021 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/__init__.py
+-rw-r--r--   0        0        0     2093 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/__init__.py
+-rw-r--r--   0        0        0      381 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/associations/__init__.py
+-rw-r--r--   0        0        0      515 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/associations/types/__init__.py
+-rw-r--r--   0        0        0     1190 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/associations/types/company_association.py
+-rw-r--r--   0        0        0     1341 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/associations/types/contact_association.py
+-rw-r--r--   0        0        0     1327 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/associations/types/deal_association.py
+-rw-r--r--   0        0        0     1378 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/associations/types/event_association.py
+-rw-r--r--   0        0        0     1506 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/associations/types/lead_association.py
+-rw-r--r--   0        0        0     1185 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/associations/types/task_association.py
+-rw-r--r--   0        0        0      361 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/errors/__init__.py
+-rw-r--r--   0        0        0      431 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/errors/errors/__init__.py
+-rw-r--r--   0        0        0      277 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/errors/errors/bad_request_error.py
+-rw-r--r--   0        0        0      281 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/errors/errors/internal_server_error.py
+-rw-r--r--   0        0        0      275 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/errors/errors/not_found_error.py
+-rw-r--r--   0        0        0      281 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/errors/errors/not_implemented_error.py
+-rw-r--r--   0        0        0      279 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/errors/errors/un_authorized_error.py
+-rw-r--r--   0        0        0      124 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/errors/types/__init__.py
+-rw-r--r--   0        0        0      871 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/errors/types/base_error.py
+-rw-r--r--   0        0        0      437 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/types/__init__.py
+-rw-r--r--   0        0        0      607 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/types/types/__init__.py
+-rw-r--r--   0        0        0     1308 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/types/types/account.py
+-rw-r--r--   0        0        0     1420 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/types/types/app.py
+-rw-r--r--   0        0        0      926 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/types/types/app_config.py
+-rw-r--r--   0        0        0     1300 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/types/types/connection.py
+-rw-r--r--   0        0        0      441 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/types/types/response_status.py
+-rw-r--r--   0        0        0     1155 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/types/types/revert_user.py
+-rw-r--r--   0        0        0     1286 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/types/types/standard_object.py
+-rw-r--r--   0        0        0      889 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/types/types/ticket_priority.py
+-rw-r--r--   0        0        0      638 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/types/types/ticket_status.py
+-rw-r--r--   0        0        0     1207 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/types/types/tpid.py
+-rw-r--r--   0        0        0     1021 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/__init__.py
+-rw-r--r--   0        0        0     1537 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/__init__.py
+-rw-r--r--   0        0        0     1213 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/channel.py
+-rw-r--r--   0        0        0     1123 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/comment_ticket_write.py
+-rw-r--r--   0        0        0     1594 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/common_unified_fields.py
+-rw-r--r--   0        0        0     1729 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/company.py
+-rw-r--r--   0        0        0     1057 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/company_address.py
+-rw-r--r--   0        0        0      893 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/contact.py
+-rw-r--r--   0        0        0     1294 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/contact_read.py
+-rw-r--r--   0        0        0      950 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/contact_write.py
+-rw-r--r--   0        0        0      881 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/deal.py
+-rw-r--r--   0        0        0     1742 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/deal_read.py
+-rw-r--r--   0        0        0      929 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/deal_write.py
+-rw-r--r--   0        0        0      885 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/event.py
+-rw-r--r--   0        0        0     1588 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/event_read.py
+-rw-r--r--   0        0        0      936 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/event_write.py
+-rw-r--r--   0        0        0      881 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/lead.py
+-rw-r--r--   0        0        0     1279 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/lead_read.py
+-rw-r--r--   0        0        0      929 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/lead_write.py
+-rw-r--r--   0        0        0     1078 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/message.py
+-rw-r--r--   0        0        0      881 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/note.py
+-rw-r--r--   0        0        0      952 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/note_read.py
+-rw-r--r--   0        0        0      929 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/note_write.py
+-rw-r--r--   0        0        0      881 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/task.py
+-rw-r--r--   0        0        0     1345 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/task_read.py
+-rw-r--r--   0        0        0      909 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/task_ticket.py
+-rw-r--r--   0        0        0     1912 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/task_ticket_write.py
+-rw-r--r--   0        0        0      974 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/task_write.py
+-rw-r--r--   0        0        0      884 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/user.py
+-rw-r--r--   0        0        0     1231 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/user_chat.py
+-rw-r--r--   0        0        0     1408 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/common/resources/unified/types/user_write.py
+-rw-r--r--   0        0        0      867 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/connection/__init__.py
+-rw-r--r--   0        0        0    34428 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/connection/client.py
+-rw-r--r--   0        0        0     1279 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/connection/types/__init__.py
+-rw-r--r--   0        0        0     1304 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/connection/types/connection_import.py
+-rw-r--r--   0        0        0      477 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/connection/types/connection_status.py
+-rw-r--r--   0        0        0      979 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/connection/types/create_connection_webhook_request.py
+-rw-r--r--   0        0        0     1272 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/connection/types/create_connection_webhook_response.py
+-rw-r--r--   0        0        0     1061 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/connection/types/delete_connection_response.py
+-rw-r--r--   0        0        0     1142 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/connection/types/delete_connection_webhook_response.py
+-rw-r--r--   0        0        0      198 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/connection/types/get_all_connection_response.py
+-rw-r--r--   0        0        0     1264 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/connection/types/get_connect_status_response.py
+-rw-r--r--   0        0        0      889 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/connection/types/get_connection_response.py
+-rw-r--r--   0        0        0     1163 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/connection/types/get_connection_webhook_response.py
+-rw-r--r--   0        0        0      968 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/connection/types/import_connections_request_body.py
+-rw-r--r--   0        0        0      972 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/connection/types/import_connections_response.py
+-rw-r--r--   0        0        0     3061 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/__init__.py
+-rw-r--r--   0        0        0     2536 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/client.py
+-rw-r--r--   0        0        0     3207 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/__init__.py
+-rw-r--r--   0        0        0      409 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/company/__init__.py
+-rw-r--r--   0        0        0    24335 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/company/client.py
+-rw-r--r--   0        0        0      563 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/company/types/__init__.py
+-rw-r--r--   0        0        0     1007 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/company/types/create_or_update_company_request.py
+-rw-r--r--   0        0        0     1020 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/company/types/create_or_update_company_response.py
+-rw-r--r--   0        0        0     1135 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/company/types/get_companies_response.py
+-rw-r--r--   0        0        0     1053 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/company/types/get_company_response.py
+-rw-r--r--   0        0        0     1138 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/company/types/search_companies_response.py
+-rw-r--r--   0        0        0      405 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/contact/__init__.py
+-rw-r--r--   0        0        0    24893 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/contact/client.py
+-rw-r--r--   0        0        0      557 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/contact/types/__init__.py
+-rw-r--r--   0        0        0     1145 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/contact/types/create_or_update_contact_request.py
+-rw-r--r--   0        0        0     1020 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/contact/types/create_or_update_contact_response.py
+-rw-r--r--   0        0        0     1053 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/contact/types/get_contact_response.py
+-rw-r--r--   0        0        0     1134 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/contact/types/get_contacts_response.py
+-rw-r--r--   0        0        0     1137 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/contact/types/search_contacts_response.py
+-rw-r--r--   0        0        0      375 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/deal/__init__.py
+-rw-r--r--   0        0        0    24030 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/deal/client.py
+-rw-r--r--   0        0        0      512 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/deal/types/__init__.py
+-rw-r--r--   0        0        0     1133 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/deal/types/create_or_update_deal_request.py
+-rw-r--r--   0        0        0     1017 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/deal/types/create_or_update_deal_response.py
+-rw-r--r--   0        0        0     1041 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/deal/types/get_deal_response.py
+-rw-r--r--   0        0        0     1122 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/deal/types/get_deals_response.py
+-rw-r--r--   0        0        0     1125 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/deal/types/search_deals_response.py
+-rw-r--r--   0        0        0      437 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/event/__init__.py
+-rw-r--r--   0        0        0    28145 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/event/client.py
+-rw-r--r--   0        0        0      609 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/event/types/__init__.py
+-rw-r--r--   0        0        0     1137 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/event/types/create_or_update_event_request.py
+-rw-r--r--   0        0        0     1018 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/event/types/create_or_update_event_response.py
+-rw-r--r--   0        0        0      987 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/event/types/delete_event_response.py
+-rw-r--r--   0        0        0     1045 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/event/types/get_event_response.py
+-rw-r--r--   0        0        0     1126 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/event/types/get_events_response.py
+-rw-r--r--   0        0        0     1129 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/event/types/search_events_response.py
+-rw-r--r--   0        0        0      375 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/lead/__init__.py
+-rw-r--r--   0        0        0    24030 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/lead/client.py
+-rw-r--r--   0        0        0      512 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/lead/types/__init__.py
+-rw-r--r--   0        0        0     1133 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/lead/types/create_or_update_lead_request.py
+-rw-r--r--   0        0        0     1017 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/lead/types/create_or_update_lead_response.py
+-rw-r--r--   0        0        0     1041 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/lead/types/get_lead_response.py
+-rw-r--r--   0        0        0     1122 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/lead/types/get_leads_response.py
+-rw-r--r--   0        0        0     1125 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/lead/types/search_leads_response.py
+-rw-r--r--   0        0        0      375 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/note/__init__.py
+-rw-r--r--   0        0        0    24030 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/note/client.py
+-rw-r--r--   0        0        0      512 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/note/types/__init__.py
+-rw-r--r--   0        0        0     1133 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/note/types/create_or_update_note_request.py
+-rw-r--r--   0        0        0     1017 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/note/types/create_or_update_note_response.py
+-rw-r--r--   0        0        0     1041 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/note/types/get_note_response.py
+-rw-r--r--   0        0        0     1122 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/note/types/get_notes_response.py
+-rw-r--r--   0        0        0     1125 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/note/types/search_notes_response.py
+-rw-r--r--   0        0        0      465 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/properties/__init__.py
+-rw-r--r--   0        0        0    10251 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/properties/client.py
+-rw-r--r--   0        0        0      652 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/properties/types/__init__.py
+-rw-r--r--   0        0        0      912 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/properties/types/field_details_type.py
+-rw-r--r--   0        0        0     1026 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/properties/types/field_details_type_read.py
+-rw-r--r--   0        0        0     1118 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/properties/types/field_details_type_request.py
+-rw-r--r--   0        0        0      203 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/properties/types/get_object_properties_response.py
+-rw-r--r--   0        0        0      183 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/properties/types/set_object_properties_request.py
+-rw-r--r--   0        0        0      121 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/properties/types/set_object_properties_response.py
+-rw-r--r--   0        0        0      173 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/proxy/__init__.py
+-rw-r--r--   0        0        0     5499 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/proxy/client.py
+-rw-r--r--   0        0        0      218 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/proxy/types/__init__.py
+-rw-r--r--   0        0        0     1065 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/proxy/types/post_proxy_request_body.py
+-rw-r--r--   0        0        0      883 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/proxy/types/proxy_response.py
+-rw-r--r--   0        0        0      375 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/task/__init__.py
+-rw-r--r--   0        0        0    24030 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/task/client.py
+-rw-r--r--   0        0        0      512 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/task/types/__init__.py
+-rw-r--r--   0        0        0     1133 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/task/types/create_or_update_task_request.py
+-rw-r--r--   0        0        0     1017 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/task/types/create_or_update_task_response.py
+-rw-r--r--   0        0        0     1041 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/task/types/get_task_response.py
+-rw-r--r--   0        0        0     1122 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/task/types/get_tasks_response.py
+-rw-r--r--   0        0        0     1125 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/task/types/search_tasks_response.py
+-rw-r--r--   0        0        0      283 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/user/__init__.py
+-rw-r--r--   0        0        0    14641 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/user/client.py
+-rw-r--r--   0        0        0      411 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/user/types/__init__.py
+-rw-r--r--   0        0        0     1133 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/user/types/create_or_update_user_request.py
+-rw-r--r--   0        0        0     1017 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/user/types/create_or_update_user_response.py
+-rw-r--r--   0        0        0     1041 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/user/types/get_user_response.py
+-rw-r--r--   0        0        0     1122 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/crm/resources/user/types/get_users_response.py
+-rw-r--r--   0        0        0      793 2024-04-25 13:24:05.194787 revert_api-0.0.861/src/revert/resources/field_mapping/__init__.py
+-rw-r--r--   0        0        0    22972 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/field_mapping/client.py
+-rw-r--r--   0        0        0     1170 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/field_mapping/types/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/field_mapping/types/create_account_field_mapping_request_body.py
+-rw-r--r--   0        0        0      980 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/field_mapping/types/create_account_field_mapping_response.py
+-rw-r--r--   0        0        0     1157 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/field_mapping/types/create_field_mapping_request_body.py
+-rw-r--r--   0        0        0      973 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/field_mapping/types/create_field_mapping_response.py
+-rw-r--r--   0        0        0      986 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/field_mapping/types/delete_account_field_mapping_config_response.py
+-rw-r--r--   0        0        0      990 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/field_mapping/types/delete_field_mapping_response.py
+-rw-r--r--   0        0        0     1061 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/field_mapping/types/field_mapping_type.py
+-rw-r--r--   0        0        0     1206 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/field_mapping/types/get_field_mapping_config_response.py
+-rw-r--r--   0        0        0     1054 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/field_mapping/types/get_field_mappings_response.py
+-rw-r--r--   0        0        0     1108 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/field_mapping/types/mappable_field_type.py
+-rw-r--r--   0        0        0      191 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/metadata/__init__.py
+-rw-r--r--   0        0        0     3656 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/metadata/client.py
+-rw-r--r--   0        0        0      255 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/metadata/types/__init__.py
+-rw-r--r--   0        0        0     1190 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/metadata/types/crm_metadata.py
+-rw-r--r--   0        0        0      985 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/metadata/types/crm_metadata_response.py
+-rw-r--r--   0        0        0      461 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/metadata/types/crm_status.py
+-rw-r--r--   0        0        0      139 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/sync/__init__.py
+-rw-r--r--   0        0        0     5258 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/sync/client.py
+-rw-r--r--   0        0        0      155 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/sync/types/__init__.py
+-rw-r--r--   0        0        0      966 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/sync/types/trigger_sync_response.py
+-rw-r--r--   0        0        0      943 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/__init__.py
+-rw-r--r--   0        0        0     1494 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/client.py
+-rw-r--r--   0        0        0      973 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/collection/__init__.py
+-rw-r--r--   0        0        0     5829 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/collection/client.py
+-rw-r--r--   0        0        0      164 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/collection/types/__init__.py
+-rw-r--r--   0        0        0     1063 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/collection/types/get_collections_response.py
+-rw-r--r--   0        0        0      307 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/comment/__init__.py
+-rw-r--r--   0        0        0    19749 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/comment/client.py
+-rw-r--r--   0        0        0      447 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/comment/types/__init__.py
+-rw-r--r--   0        0        0      204 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/comment/types/create_or_update_comment_request.py
+-rw-r--r--   0        0        0     1020 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/comment/types/create_or_update_comment_response.py
+-rw-r--r--   0        0        0      992 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/comment/types/get_comment_response.py
+-rw-r--r--   0        0        0     1060 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/comment/types/get_comments_response.py
+-rw-r--r--   0        0        0      173 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/proxy/__init__.py
+-rw-r--r--   0        0        0     5529 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/proxy/client.py
+-rw-r--r--   0        0        0      218 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/proxy/types/__init__.py
+-rw-r--r--   0        0        0     1065 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/proxy/types/post_proxy_request_body.py
+-rw-r--r--   0        0        0      883 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/proxy/types/proxy_response.py
+-rw-r--r--   0        0        0      283 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/task/__init__.py
+-rw-r--r--   0        0        0    19908 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/task/client.py
+-rw-r--r--   0        0        0      411 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/task/types/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/task/types/create_or_update_task_request.py
+-rw-r--r--   0        0        0     1017 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/task/types/create_or_update_task_response.py
+-rw-r--r--   0        0        0     1060 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/task/types/get_task_response.py
+-rw-r--r--   0        0        0     1141 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/task/types/get_tasks_response.py
+-rw-r--r--   0        0        0      169 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/user/__init__.py
+-rw-r--r--   0        0        0    10114 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/user/client.py
+-rw-r--r--   0        0        0      212 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/user/types/__init__.py
+-rw-r--r--   0        0        0      989 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/user/types/get_user_response.py
+-rw-r--r--   0        0        0     1057 2024-04-25 13:24:05.198787 revert_api-0.0.861/src/revert/resources/ticket/resources/user/types/get_users_response.py
+-rw-r--r--   0        0        0     2197 1970-01-01 00:00:00.000000 revert_api-0.0.861/PKG-INFO
```

### Comparing `revert_api-0.0.852/README.md` & `revert_api-0.0.861/README.md`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/__init__.py` & `revert_api-0.0.861/src/revert/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/client.py` & `revert_api-0.0.861/src/revert/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/core/__init__.py` & `revert_api-0.0.861/src/revert/core/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/core/client_wrapper.py` & `revert_api-0.0.861/src/revert/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     def __init__(self, *, base_url: str):
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "revert-api",
-            "X-Fern-SDK-Version": "0.0.852",
+            "X-Fern-SDK-Version": "0.0.861",
         }
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `revert_api-0.0.852/src/revert/core/datetime_utils.py` & `revert_api-0.0.861/src/revert/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/core/jsonable_encoder.py` & `revert_api-0.0.861/src/revert/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/__init__.py` & `revert_api-0.0.861/src/revert/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/chat/client.py` & `revert_api-0.0.861/src/revert/resources/chat/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/chat/resources/channels/client.py` & `revert_api-0.0.861/src/revert/resources/chat/resources/channels/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/chat/resources/channels/types/get_channels_response.py` & `revert_api-0.0.861/src/revert/resources/chat/resources/channels/types/get_channels_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/chat/resources/messages/client.py` & `revert_api-0.0.861/src/revert/resources/chat/resources/messages/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/chat/resources/messages/types/createor_update_message_request.py` & `revert_api-0.0.861/src/revert/resources/chat/resources/messages/types/createor_update_message_request.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/chat/resources/messages/types/createor_update_message_response.py` & `revert_api-0.0.861/src/revert/resources/chat/resources/messages/types/createor_update_message_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/chat/resources/users/client.py` & `revert_api-0.0.861/src/revert/resources/chat/resources/users/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/chat/resources/users/types/get_users_response.py` & `revert_api-0.0.861/src/revert/resources/chat/resources/users/types/get_users_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/__init__.py` & `revert_api-0.0.861/src/revert/resources/common/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/__init__.py` & `revert_api-0.0.861/src/revert/resources/common/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/associations/types/__init__.py` & `revert_api-0.0.861/src/revert/resources/common/resources/associations/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/associations/types/company_association.py` & `revert_api-0.0.861/src/revert/resources/common/resources/associations/types/company_association.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/associations/types/contact_association.py` & `revert_api-0.0.861/src/revert/resources/common/resources/associations/types/contact_association.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/associations/types/deal_association.py` & `revert_api-0.0.861/src/revert/resources/common/resources/associations/types/deal_association.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/associations/types/event_association.py` & `revert_api-0.0.861/src/revert/resources/common/resources/associations/types/event_association.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/associations/types/lead_association.py` & `revert_api-0.0.861/src/revert/resources/common/resources/associations/types/lead_association.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/associations/types/task_association.py` & `revert_api-0.0.861/src/revert/resources/common/resources/associations/types/task_association.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/errors/types/base_error.py` & `revert_api-0.0.861/src/revert/resources/common/resources/errors/types/base_error.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/types/types/__init__.py` & `revert_api-0.0.861/src/revert/resources/common/resources/types/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/types/types/account.py` & `revert_api-0.0.861/src/revert/resources/common/resources/types/types/account.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/types/types/app.py` & `revert_api-0.0.861/src/revert/resources/common/resources/types/types/app.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/types/types/app_config.py` & `revert_api-0.0.861/src/revert/resources/common/resources/types/types/app_config.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/types/types/connection.py` & `revert_api-0.0.861/src/revert/resources/common/resources/types/types/connection.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/types/types/revert_user.py` & `revert_api-0.0.861/src/revert/resources/common/resources/types/types/revert_user.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/types/types/standard_object.py` & `revert_api-0.0.861/src/revert/resources/common/resources/types/types/standard_object.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/types/types/ticket_priority.py` & `revert_api-0.0.861/src/revert/resources/common/resources/types/types/ticket_priority.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/types/types/ticket_status.py` & `revert_api-0.0.861/src/revert/resources/common/resources/types/types/ticket_status.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/types/types/tpid.py` & `revert_api-0.0.861/src/revert/resources/common/resources/types/types/tpid.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/__init__.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/__init__.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/channel.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/channel.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/comment_ticket_write.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/comment_ticket_write.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/common_unified_fields.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/common_unified_fields.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/company.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/company.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/company_address.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/company_address.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/contact.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/contact.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/contact_read.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/contact_read.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/contact_write.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/contact_write.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/deal.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/deal.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/deal_read.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/deal_read.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/deal_write.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/deal_write.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/event.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/event.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/event_read.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/event_read.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/event_write.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/event_write.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/lead.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/lead.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/lead_read.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/lead_read.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/lead_write.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/lead_write.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/message.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/message.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/note.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/note.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/note_read.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/note_read.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/note_write.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/note_write.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/task.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/task.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/task_read.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/task_read.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/task_ticket.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/task_ticket.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/task_ticket_write.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/task_ticket_write.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/task_write.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/task_write.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/user.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/user.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/user_chat.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/user_chat.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/common/resources/unified/types/user_write.py` & `revert_api-0.0.861/src/revert/resources/common/resources/unified/types/user_write.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/connection/__init__.py` & `revert_api-0.0.861/src/revert/resources/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/connection/client.py` & `revert_api-0.0.861/src/revert/resources/connection/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/connection/types/__init__.py` & `revert_api-0.0.861/src/revert/resources/connection/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/connection/types/connection_import.py` & `revert_api-0.0.861/src/revert/resources/connection/types/connection_import.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/connection/types/create_connection_webhook_request.py` & `revert_api-0.0.861/src/revert/resources/connection/types/create_connection_webhook_request.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/connection/types/create_connection_webhook_response.py` & `revert_api-0.0.861/src/revert/resources/connection/types/create_connection_webhook_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/connection/types/delete_connection_response.py` & `revert_api-0.0.861/src/revert/resources/connection/types/delete_connection_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/connection/types/delete_connection_webhook_response.py` & `revert_api-0.0.861/src/revert/resources/connection/types/delete_connection_webhook_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/connection/types/get_connect_status_response.py` & `revert_api-0.0.861/src/revert/resources/connection/types/get_connect_status_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/connection/types/get_connection_response.py` & `revert_api-0.0.861/src/revert/resources/connection/types/get_connection_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/connection/types/get_connection_webhook_response.py` & `revert_api-0.0.861/src/revert/resources/connection/types/get_connection_webhook_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/connection/types/import_connections_request_body.py` & `revert_api-0.0.861/src/revert/resources/connection/types/import_connections_request_body.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/connection/types/import_connections_response.py` & `revert_api-0.0.861/src/revert/resources/connection/types/import_connections_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/__init__.py` & `revert_api-0.0.861/src/revert/resources/crm/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/client.py` & `revert_api-0.0.861/src/revert/resources/crm/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/__init__.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/company/client.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/deal/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,97 +8,96 @@
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .....core.jsonable_encoder import jsonable_encoder
 from .....core.remove_none_from_dict import remove_none_from_dict
 from ....common.resources.errors.errors.internal_server_error import InternalServerError
 from ....common.resources.errors.errors.not_found_error import NotFoundError
 from ....common.resources.errors.errors.un_authorized_error import UnAuthorizedError
 from ....common.resources.errors.types.base_error import BaseError
-from ....common.resources.unified.types.company import Company
-from .types.create_or_update_company_request import CreateOrUpdateCompanyRequest
-from .types.create_or_update_company_response import CreateOrUpdateCompanyResponse
-from .types.get_companies_response import GetCompaniesResponse
-from .types.get_company_response import GetCompanyResponse
-from .types.search_companies_response import SearchCompaniesResponse
+from .types.create_or_update_deal_request import CreateOrUpdateDealRequest
+from .types.create_or_update_deal_response import CreateOrUpdateDealResponse
+from .types.get_deal_response import GetDealResponse
+from .types.get_deals_response import GetDealsResponse
+from .types.search_deals_response import SearchDealsResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class CompanyClient:
+class DealClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def get_company(
+    def get_deal(
         self,
         id: str,
         *,
         fields: typing.Optional[str] = None,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> GetCompanyResponse:
+    ) -> GetDealResponse:
         """
-        Get details of a company
+        Get details of a deal
 
         Parameters:
-            - id: str. The unique `id` of the company in the CRM.
+            - id: str.
 
             - fields: typing.Optional[str].
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/companies/{id}"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/deals/{id}"),
             params=remove_none_from_dict({"fields": fields}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetCompanyResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(GetDealResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_companies(
+    def get_deals(
         self,
         *,
         fields: typing.Optional[str] = None,
         page_size: typing.Optional[str] = None,
         cursor: typing.Optional[str] = None,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> GetCompaniesResponse:
+    ) -> GetDealsResponse:
         """
-        Get all the companies
+        Get all the deals
 
         Parameters:
             - fields: typing.Optional[str].
 
             - page_size: typing.Optional[str].
 
             - cursor: typing.Optional[str].
@@ -107,259 +106,265 @@
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/companies"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/deals"),
             params=remove_none_from_dict({"fields": fields, "pageSize": page_size, "cursor": cursor}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetCompaniesResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(GetDealsResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create_company(
+    def create_deal(
         self,
         *,
-        request: CreateOrUpdateCompanyRequest,
+        request: CreateOrUpdateDealRequest,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> CreateOrUpdateCompanyResponse:
+    ) -> CreateOrUpdateDealResponse:
         """
-        Create a new company
+        Create a new deal
 
         Parameters:
-            - request: CreateOrUpdateCompanyRequest.
+            - request: CreateOrUpdateDealRequest.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/companies"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/deals"),
             json=jsonable_encoder(request),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CreateOrUpdateCompanyResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateOrUpdateDealResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update_company(
+    def update_deal(
         self,
         id: str,
         *,
-        request: Company,
+        request: CreateOrUpdateDealRequest,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> CreateOrUpdateCompanyResponse:
+    ) -> CreateOrUpdateDealResponse:
         """
-        Update a company
+        Update a deal
 
         Parameters:
             - id: str.
 
-            - request: Company.
+            - request: CreateOrUpdateDealRequest.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/companies/{id}"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/deals/{id}"),
             json=jsonable_encoder(request),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CreateOrUpdateCompanyResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateOrUpdateDealResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def search_companies(
+    def search_deals(
         self,
         *,
         fields: typing.Optional[str] = None,
+        page_size: typing.Optional[str] = None,
+        cursor: typing.Optional[str] = None,
         search_criteria: typing.Any,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> SearchCompaniesResponse:
+    ) -> SearchDealsResponse:
         """
-        Search for companies
+        Search for deals
 
         Parameters:
             - fields: typing.Optional[str].
 
+            - page_size: typing.Optional[str].
+
+            - cursor: typing.Optional[str].
+
             - search_criteria: typing.Any.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/companies/search"),
-            params=remove_none_from_dict({"fields": fields}),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/deals/search"),
+            params=remove_none_from_dict({"fields": fields, "pageSize": page_size, "cursor": cursor}),
             json=jsonable_encoder({"searchCriteria": search_criteria}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(SearchCompaniesResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(SearchDealsResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncCompanyClient:
+class AsyncDealClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def get_company(
+    async def get_deal(
         self,
         id: str,
         *,
         fields: typing.Optional[str] = None,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> GetCompanyResponse:
+    ) -> GetDealResponse:
         """
-        Get details of a company
+        Get details of a deal
 
         Parameters:
-            - id: str. The unique `id` of the company in the CRM.
+            - id: str.
 
             - fields: typing.Optional[str].
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/companies/{id}"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/deals/{id}"),
             params=remove_none_from_dict({"fields": fields}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetCompanyResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(GetDealResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_companies(
+    async def get_deals(
         self,
         *,
         fields: typing.Optional[str] = None,
         page_size: typing.Optional[str] = None,
         cursor: typing.Optional[str] = None,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> GetCompaniesResponse:
+    ) -> GetDealsResponse:
         """
-        Get all the companies
+        Get all the deals
 
         Parameters:
             - fields: typing.Optional[str].
 
             - page_size: typing.Optional[str].
 
             - cursor: typing.Optional[str].
@@ -368,179 +373,185 @@
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/companies"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/deals"),
             params=remove_none_from_dict({"fields": fields, "pageSize": page_size, "cursor": cursor}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetCompaniesResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(GetDealsResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create_company(
+    async def create_deal(
         self,
         *,
-        request: CreateOrUpdateCompanyRequest,
+        request: CreateOrUpdateDealRequest,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> CreateOrUpdateCompanyResponse:
+    ) -> CreateOrUpdateDealResponse:
         """
-        Create a new company
+        Create a new deal
 
         Parameters:
-            - request: CreateOrUpdateCompanyRequest.
+            - request: CreateOrUpdateDealRequest.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/companies"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/deals"),
             json=jsonable_encoder(request),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CreateOrUpdateCompanyResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateOrUpdateDealResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update_company(
+    async def update_deal(
         self,
         id: str,
         *,
-        request: Company,
+        request: CreateOrUpdateDealRequest,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> CreateOrUpdateCompanyResponse:
+    ) -> CreateOrUpdateDealResponse:
         """
-        Update a company
+        Update a deal
 
         Parameters:
             - id: str.
 
-            - request: Company.
+            - request: CreateOrUpdateDealRequest.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/companies/{id}"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/deals/{id}"),
             json=jsonable_encoder(request),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CreateOrUpdateCompanyResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateOrUpdateDealResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def search_companies(
+    async def search_deals(
         self,
         *,
         fields: typing.Optional[str] = None,
+        page_size: typing.Optional[str] = None,
+        cursor: typing.Optional[str] = None,
         search_criteria: typing.Any,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> SearchCompaniesResponse:
+    ) -> SearchDealsResponse:
         """
-        Search for companies
+        Search for deals
 
         Parameters:
             - fields: typing.Optional[str].
 
+            - page_size: typing.Optional[str].
+
+            - cursor: typing.Optional[str].
+
             - search_criteria: typing.Any.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/companies/search"),
-            params=remove_none_from_dict({"fields": fields}),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/deals/search"),
+            params=remove_none_from_dict({"fields": fields, "pageSize": page_size, "cursor": cursor}),
             json=jsonable_encoder({"searchCriteria": search_criteria}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(SearchCompaniesResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(SearchDealsResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
```

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/company/types/__init__.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/company/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/company/types/create_or_update_company_request.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/company/types/create_or_update_company_request.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/company/types/create_or_update_company_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/company/types/create_or_update_company_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/company/types/get_companies_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/company/types/get_companies_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/company/types/get_company_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/company/types/get_company_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/company/types/search_companies_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/lead/types/get_lead_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ......core.datetime_utils import serialize_datetime
 from .....common.resources.types.types.response_status import ResponseStatus
-from .....common.resources.unified.types.company import Company
+from .....common.resources.unified.types.lead import Lead
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class SearchCompaniesResponse(pydantic.BaseModel):
+class GetLeadResponse(pydantic.BaseModel):
     status: ResponseStatus
-    results: typing.List[Company]
+    result: Lead
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/contact/client.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/contact/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,37 +240,43 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def search_contacts(
         self,
         *,
         fields: typing.Optional[str] = None,
+        page_size: typing.Optional[str] = None,
+        cursor: typing.Optional[str] = None,
         search_criteria: typing.Any,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
     ) -> SearchContactsResponse:
         """
         Search for contacts
 
         Parameters:
             - fields: typing.Optional[str].
 
+            - page_size: typing.Optional[str].
+
+            - cursor: typing.Optional[str].
+
             - search_criteria: typing.Any.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/contacts/search"),
-            params=remove_none_from_dict({"fields": fields}),
+            params=remove_none_from_dict({"fields": fields, "pageSize": page_size, "cursor": cursor}),
             json=jsonable_encoder({"searchCriteria": search_criteria}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
@@ -505,37 +511,43 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def search_contacts(
         self,
         *,
         fields: typing.Optional[str] = None,
+        page_size: typing.Optional[str] = None,
+        cursor: typing.Optional[str] = None,
         search_criteria: typing.Any,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
     ) -> SearchContactsResponse:
         """
         Search for contacts
 
         Parameters:
             - fields: typing.Optional[str].
 
+            - page_size: typing.Optional[str].
+
+            - cursor: typing.Optional[str].
+
             - search_criteria: typing.Any.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/contacts/search"),
-            params=remove_none_from_dict({"fields": fields}),
+            params=remove_none_from_dict({"fields": fields, "pageSize": page_size, "cursor": cursor}),
             json=jsonable_encoder({"searchCriteria": search_criteria}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
```

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/contact/types/__init__.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/contact/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/contact/types/create_or_update_contact_request.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/contact/types/create_or_update_contact_request.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/contact/types/create_or_update_contact_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/contact/types/create_or_update_contact_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/contact/types/get_contact_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/contact/types/get_contact_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/contact/types/get_contacts_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/contact/types/get_contacts_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/contact/types/search_contacts_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/deal/types/search_deals_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ......core.datetime_utils import serialize_datetime
 from .....common.resources.types.types.response_status import ResponseStatus
-from .....common.resources.unified.types.contact import Contact
+from .....common.resources.unified.types.deal import Deal
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class SearchContactsResponse(pydantic.BaseModel):
+class SearchDealsResponse(pydantic.BaseModel):
     status: ResponseStatus
-    results: typing.List[Contact]
+    next: typing.Optional[str]
+    previous: typing.Optional[str]
+    results: typing.List[Deal]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/deal/client.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/note/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,96 +8,96 @@
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .....core.jsonable_encoder import jsonable_encoder
 from .....core.remove_none_from_dict import remove_none_from_dict
 from ....common.resources.errors.errors.internal_server_error import InternalServerError
 from ....common.resources.errors.errors.not_found_error import NotFoundError
 from ....common.resources.errors.errors.un_authorized_error import UnAuthorizedError
 from ....common.resources.errors.types.base_error import BaseError
-from .types.create_or_update_deal_request import CreateOrUpdateDealRequest
-from .types.create_or_update_deal_response import CreateOrUpdateDealResponse
-from .types.get_deal_response import GetDealResponse
-from .types.get_deals_response import GetDealsResponse
-from .types.search_deals_response import SearchDealsResponse
+from .types.create_or_update_note_request import CreateOrUpdateNoteRequest
+from .types.create_or_update_note_response import CreateOrUpdateNoteResponse
+from .types.get_note_response import GetNoteResponse
+from .types.get_notes_response import GetNotesResponse
+from .types.search_notes_response import SearchNotesResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class DealClient:
+class NoteClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def get_deal(
+    def get_note(
         self,
         id: str,
         *,
         fields: typing.Optional[str] = None,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> GetDealResponse:
+    ) -> GetNoteResponse:
         """
-        Get details of a deal
+        Get details of a note
 
         Parameters:
             - id: str.
 
             - fields: typing.Optional[str].
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/deals/{id}"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/notes/{id}"),
             params=remove_none_from_dict({"fields": fields}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetDealResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(GetNoteResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_deals(
+    def get_notes(
         self,
         *,
         fields: typing.Optional[str] = None,
         page_size: typing.Optional[str] = None,
         cursor: typing.Optional[str] = None,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> GetDealsResponse:
+    ) -> GetNotesResponse:
         """
-        Get all the deals
+        Get all the notes
 
         Parameters:
             - fields: typing.Optional[str].
 
             - page_size: typing.Optional[str].
 
             - cursor: typing.Optional[str].
@@ -106,259 +106,265 @@
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/deals"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/notes"),
             params=remove_none_from_dict({"fields": fields, "pageSize": page_size, "cursor": cursor}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetDealsResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(GetNotesResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create_deal(
+    def create_note(
         self,
         *,
-        request: CreateOrUpdateDealRequest,
+        request: CreateOrUpdateNoteRequest,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> CreateOrUpdateDealResponse:
+    ) -> CreateOrUpdateNoteResponse:
         """
-        Create a new deal
+        Create a new note
 
         Parameters:
-            - request: CreateOrUpdateDealRequest.
+            - request: CreateOrUpdateNoteRequest.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/deals"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/notes"),
             json=jsonable_encoder(request),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CreateOrUpdateDealResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateOrUpdateNoteResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update_deal(
+    def update_note(
         self,
         id: str,
         *,
-        request: CreateOrUpdateDealRequest,
+        request: CreateOrUpdateNoteRequest,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> CreateOrUpdateDealResponse:
+    ) -> CreateOrUpdateNoteResponse:
         """
-        Update a deal
+        Update a note
 
         Parameters:
             - id: str.
 
-            - request: CreateOrUpdateDealRequest.
+            - request: CreateOrUpdateNoteRequest.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/deals/{id}"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/notes/{id}"),
             json=jsonable_encoder(request),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CreateOrUpdateDealResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateOrUpdateNoteResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def search_deals(
+    def search_notes(
         self,
         *,
         fields: typing.Optional[str] = None,
+        page_size: typing.Optional[str] = None,
+        cursor: typing.Optional[str] = None,
         search_criteria: typing.Any,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> SearchDealsResponse:
+    ) -> SearchNotesResponse:
         """
-        Search for deals
+        Search for notes
 
         Parameters:
             - fields: typing.Optional[str].
 
+            - page_size: typing.Optional[str].
+
+            - cursor: typing.Optional[str].
+
             - search_criteria: typing.Any.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/deals/search"),
-            params=remove_none_from_dict({"fields": fields}),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/notes/search"),
+            params=remove_none_from_dict({"fields": fields, "pageSize": page_size, "cursor": cursor}),
             json=jsonable_encoder({"searchCriteria": search_criteria}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(SearchDealsResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(SearchNotesResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncDealClient:
+class AsyncNoteClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def get_deal(
+    async def get_note(
         self,
         id: str,
         *,
         fields: typing.Optional[str] = None,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> GetDealResponse:
+    ) -> GetNoteResponse:
         """
-        Get details of a deal
+        Get details of a note
 
         Parameters:
             - id: str.
 
             - fields: typing.Optional[str].
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/deals/{id}"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/notes/{id}"),
             params=remove_none_from_dict({"fields": fields}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetDealResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(GetNoteResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_deals(
+    async def get_notes(
         self,
         *,
         fields: typing.Optional[str] = None,
         page_size: typing.Optional[str] = None,
         cursor: typing.Optional[str] = None,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> GetDealsResponse:
+    ) -> GetNotesResponse:
         """
-        Get all the deals
+        Get all the notes
 
         Parameters:
             - fields: typing.Optional[str].
 
             - page_size: typing.Optional[str].
 
             - cursor: typing.Optional[str].
@@ -367,179 +373,185 @@
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/deals"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/notes"),
             params=remove_none_from_dict({"fields": fields, "pageSize": page_size, "cursor": cursor}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetDealsResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(GetNotesResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create_deal(
+    async def create_note(
         self,
         *,
-        request: CreateOrUpdateDealRequest,
+        request: CreateOrUpdateNoteRequest,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> CreateOrUpdateDealResponse:
+    ) -> CreateOrUpdateNoteResponse:
         """
-        Create a new deal
+        Create a new note
 
         Parameters:
-            - request: CreateOrUpdateDealRequest.
+            - request: CreateOrUpdateNoteRequest.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/deals"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/notes"),
             json=jsonable_encoder(request),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CreateOrUpdateDealResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateOrUpdateNoteResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update_deal(
+    async def update_note(
         self,
         id: str,
         *,
-        request: CreateOrUpdateDealRequest,
+        request: CreateOrUpdateNoteRequest,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> CreateOrUpdateDealResponse:
+    ) -> CreateOrUpdateNoteResponse:
         """
-        Update a deal
+        Update a note
 
         Parameters:
             - id: str.
 
-            - request: CreateOrUpdateDealRequest.
+            - request: CreateOrUpdateNoteRequest.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/deals/{id}"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/notes/{id}"),
             json=jsonable_encoder(request),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CreateOrUpdateDealResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateOrUpdateNoteResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def search_deals(
+    async def search_notes(
         self,
         *,
         fields: typing.Optional[str] = None,
+        page_size: typing.Optional[str] = None,
+        cursor: typing.Optional[str] = None,
         search_criteria: typing.Any,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> SearchDealsResponse:
+    ) -> SearchNotesResponse:
         """
-        Search for deals
+        Search for notes
 
         Parameters:
             - fields: typing.Optional[str].
 
+            - page_size: typing.Optional[str].
+
+            - cursor: typing.Optional[str].
+
             - search_criteria: typing.Any.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/deals/search"),
-            params=remove_none_from_dict({"fields": fields}),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/notes/search"),
+            params=remove_none_from_dict({"fields": fields, "pageSize": page_size, "cursor": cursor}),
             json=jsonable_encoder({"searchCriteria": search_criteria}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(SearchDealsResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(SearchNotesResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
```

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/deal/types/__init__.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/deal/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/deal/types/create_or_update_deal_request.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/deal/types/create_or_update_deal_request.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/deal/types/create_or_update_deal_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/deal/types/create_or_update_deal_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/deal/types/get_deal_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/deal/types/get_deal_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/deal/types/get_deals_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/deal/types/get_deals_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/deal/types/search_deals_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/event/types/search_events_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ......core.datetime_utils import serialize_datetime
 from .....common.resources.types.types.response_status import ResponseStatus
-from .....common.resources.unified.types.deal import Deal
+from .....common.resources.unified.types.event import Event
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class SearchDealsResponse(pydantic.BaseModel):
+class SearchEventsResponse(pydantic.BaseModel):
     status: ResponseStatus
-    results: typing.List[Deal]
+    next: typing.Optional[str]
+    previous: typing.Optional[str]
+    results: typing.List[Event]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/event/client.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/event/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,37 +236,43 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def search_events(
         self,
         *,
         fields: typing.Optional[str] = None,
+        page_size: typing.Optional[str] = None,
+        cursor: typing.Optional[str] = None,
         search_criteria: typing.Any,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
     ) -> SearchEventsResponse:
         """
         Search for events
 
         Parameters:
             - fields: typing.Optional[str].
 
+            - page_size: typing.Optional[str].
+
+            - cursor: typing.Optional[str].
+
             - search_criteria: typing.Any.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/events/search"),
-            params=remove_none_from_dict({"fields": fields}),
+            params=remove_none_from_dict({"fields": fields, "pageSize": page_size, "cursor": cursor}),
             json=jsonable_encoder({"searchCriteria": search_criteria}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
@@ -539,37 +545,43 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def search_events(
         self,
         *,
         fields: typing.Optional[str] = None,
+        page_size: typing.Optional[str] = None,
+        cursor: typing.Optional[str] = None,
         search_criteria: typing.Any,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
     ) -> SearchEventsResponse:
         """
         Search for events
 
         Parameters:
             - fields: typing.Optional[str].
 
+            - page_size: typing.Optional[str].
+
+            - cursor: typing.Optional[str].
+
             - search_criteria: typing.Any.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/events/search"),
-            params=remove_none_from_dict({"fields": fields}),
+            params=remove_none_from_dict({"fields": fields, "pageSize": page_size, "cursor": cursor}),
             json=jsonable_encoder({"searchCriteria": search_criteria}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
```

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/event/types/__init__.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/event/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/event/types/create_or_update_event_request.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/event/types/create_or_update_event_request.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/event/types/create_or_update_event_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/event/types/create_or_update_event_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/event/types/delete_event_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/event/types/delete_event_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/event/types/get_event_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/event/types/get_event_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/event/types/get_events_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/event/types/get_events_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/event/types/search_events_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/note/types/get_note_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ......core.datetime_utils import serialize_datetime
 from .....common.resources.types.types.response_status import ResponseStatus
-from .....common.resources.unified.types.event import Event
+from .....common.resources.unified.types.note import Note
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class SearchEventsResponse(pydantic.BaseModel):
+class GetNoteResponse(pydantic.BaseModel):
     status: ResponseStatus
-    results: typing.List[Event]
+    result: Note
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/lead/client.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/lead/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,37 +235,43 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def search_leads(
         self,
         *,
         fields: typing.Optional[str] = None,
+        page_size: typing.Optional[str] = None,
+        cursor: typing.Optional[str] = None,
         search_criteria: typing.Any,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
     ) -> SearchLeadsResponse:
         """
         Search for leads
 
         Parameters:
             - fields: typing.Optional[str].
 
+            - page_size: typing.Optional[str].
+
+            - cursor: typing.Optional[str].
+
             - search_criteria: typing.Any.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/leads/search"),
-            params=remove_none_from_dict({"fields": fields}),
+            params=remove_none_from_dict({"fields": fields, "pageSize": page_size, "cursor": cursor}),
             json=jsonable_encoder({"searchCriteria": search_criteria}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
@@ -496,37 +502,43 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def search_leads(
         self,
         *,
         fields: typing.Optional[str] = None,
+        page_size: typing.Optional[str] = None,
+        cursor: typing.Optional[str] = None,
         search_criteria: typing.Any,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
     ) -> SearchLeadsResponse:
         """
         Search for leads
 
         Parameters:
             - fields: typing.Optional[str].
 
+            - page_size: typing.Optional[str].
+
+            - cursor: typing.Optional[str].
+
             - search_criteria: typing.Any.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/leads/search"),
-            params=remove_none_from_dict({"fields": fields}),
+            params=remove_none_from_dict({"fields": fields, "pageSize": page_size, "cursor": cursor}),
             json=jsonable_encoder({"searchCriteria": search_criteria}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
```

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/lead/types/__init__.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/lead/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/lead/types/create_or_update_lead_request.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/lead/types/create_or_update_lead_request.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/lead/types/create_or_update_lead_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/lead/types/create_or_update_lead_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/lead/types/get_lead_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/user/types/get_user_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ......core.datetime_utils import serialize_datetime
 from .....common.resources.types.types.response_status import ResponseStatus
-from .....common.resources.unified.types.lead import Lead
+from .....common.resources.unified.types.user import User
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class GetLeadResponse(pydantic.BaseModel):
+class GetUserResponse(pydantic.BaseModel):
     status: ResponseStatus
-    result: Lead
+    result: User
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/lead/types/get_leads_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/lead/types/get_leads_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/lead/types/search_leads_response.py` & `revert_api-0.0.861/src/revert/resources/ticket/resources/task/types/get_task_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ......core.datetime_utils import serialize_datetime
 from .....common.resources.types.types.response_status import ResponseStatus
-from .....common.resources.unified.types.lead import Lead
+from .....common.resources.unified.types.task_ticket import TaskTicket
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class SearchLeadsResponse(pydantic.BaseModel):
+class GetTaskResponse(pydantic.BaseModel):
     status: ResponseStatus
-    results: typing.List[Lead]
+    result: TaskTicket
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/note/client.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/company/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,96 +8,97 @@
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .....core.jsonable_encoder import jsonable_encoder
 from .....core.remove_none_from_dict import remove_none_from_dict
 from ....common.resources.errors.errors.internal_server_error import InternalServerError
 from ....common.resources.errors.errors.not_found_error import NotFoundError
 from ....common.resources.errors.errors.un_authorized_error import UnAuthorizedError
 from ....common.resources.errors.types.base_error import BaseError
-from .types.create_or_update_note_request import CreateOrUpdateNoteRequest
-from .types.create_or_update_note_response import CreateOrUpdateNoteResponse
-from .types.get_note_response import GetNoteResponse
-from .types.get_notes_response import GetNotesResponse
-from .types.search_notes_response import SearchNotesResponse
+from ....common.resources.unified.types.company import Company
+from .types.create_or_update_company_request import CreateOrUpdateCompanyRequest
+from .types.create_or_update_company_response import CreateOrUpdateCompanyResponse
+from .types.get_companies_response import GetCompaniesResponse
+from .types.get_company_response import GetCompanyResponse
+from .types.search_companies_response import SearchCompaniesResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class NoteClient:
+class CompanyClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def get_note(
+    def get_company(
         self,
         id: str,
         *,
         fields: typing.Optional[str] = None,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> GetNoteResponse:
+    ) -> GetCompanyResponse:
         """
-        Get details of a note
+        Get details of a company
 
         Parameters:
-            - id: str.
+            - id: str. The unique `id` of the company in the CRM.
 
             - fields: typing.Optional[str].
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/notes/{id}"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/companies/{id}"),
             params=remove_none_from_dict({"fields": fields}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetNoteResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(GetCompanyResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_notes(
+    def get_companies(
         self,
         *,
         fields: typing.Optional[str] = None,
         page_size: typing.Optional[str] = None,
         cursor: typing.Optional[str] = None,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> GetNotesResponse:
+    ) -> GetCompaniesResponse:
         """
-        Get all the notes
+        Get all the companies
 
         Parameters:
             - fields: typing.Optional[str].
 
             - page_size: typing.Optional[str].
 
             - cursor: typing.Optional[str].
@@ -106,259 +107,265 @@
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/notes"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/companies"),
             params=remove_none_from_dict({"fields": fields, "pageSize": page_size, "cursor": cursor}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetNotesResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(GetCompaniesResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create_note(
+    def create_company(
         self,
         *,
-        request: CreateOrUpdateNoteRequest,
+        request: CreateOrUpdateCompanyRequest,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> CreateOrUpdateNoteResponse:
+    ) -> CreateOrUpdateCompanyResponse:
         """
-        Create a new note
+        Create a new company
 
         Parameters:
-            - request: CreateOrUpdateNoteRequest.
+            - request: CreateOrUpdateCompanyRequest.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/notes"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/companies"),
             json=jsonable_encoder(request),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CreateOrUpdateNoteResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateOrUpdateCompanyResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update_note(
+    def update_company(
         self,
         id: str,
         *,
-        request: CreateOrUpdateNoteRequest,
+        request: Company,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> CreateOrUpdateNoteResponse:
+    ) -> CreateOrUpdateCompanyResponse:
         """
-        Update a note
+        Update a company
 
         Parameters:
             - id: str.
 
-            - request: CreateOrUpdateNoteRequest.
+            - request: Company.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/notes/{id}"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/companies/{id}"),
             json=jsonable_encoder(request),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CreateOrUpdateNoteResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateOrUpdateCompanyResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def search_notes(
+    def search_companies(
         self,
         *,
         fields: typing.Optional[str] = None,
+        page_size: typing.Optional[str] = None,
+        cursor: typing.Optional[str] = None,
         search_criteria: typing.Any,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> SearchNotesResponse:
+    ) -> SearchCompaniesResponse:
         """
-        Search for notes
+        Search for companies
 
         Parameters:
             - fields: typing.Optional[str].
 
+            - page_size: typing.Optional[str].
+
+            - cursor: typing.Optional[str].
+
             - search_criteria: typing.Any.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/notes/search"),
-            params=remove_none_from_dict({"fields": fields}),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/companies/search"),
+            params=remove_none_from_dict({"fields": fields, "pageSize": page_size, "cursor": cursor}),
             json=jsonable_encoder({"searchCriteria": search_criteria}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(SearchNotesResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(SearchCompaniesResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncNoteClient:
+class AsyncCompanyClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def get_note(
+    async def get_company(
         self,
         id: str,
         *,
         fields: typing.Optional[str] = None,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> GetNoteResponse:
+    ) -> GetCompanyResponse:
         """
-        Get details of a note
+        Get details of a company
 
         Parameters:
-            - id: str.
+            - id: str. The unique `id` of the company in the CRM.
 
             - fields: typing.Optional[str].
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/notes/{id}"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/companies/{id}"),
             params=remove_none_from_dict({"fields": fields}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetNoteResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(GetCompanyResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_notes(
+    async def get_companies(
         self,
         *,
         fields: typing.Optional[str] = None,
         page_size: typing.Optional[str] = None,
         cursor: typing.Optional[str] = None,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> GetNotesResponse:
+    ) -> GetCompaniesResponse:
         """
-        Get all the notes
+        Get all the companies
 
         Parameters:
             - fields: typing.Optional[str].
 
             - page_size: typing.Optional[str].
 
             - cursor: typing.Optional[str].
@@ -367,179 +374,185 @@
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/notes"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/companies"),
             params=remove_none_from_dict({"fields": fields, "pageSize": page_size, "cursor": cursor}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetNotesResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(GetCompaniesResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create_note(
+    async def create_company(
         self,
         *,
-        request: CreateOrUpdateNoteRequest,
+        request: CreateOrUpdateCompanyRequest,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> CreateOrUpdateNoteResponse:
+    ) -> CreateOrUpdateCompanyResponse:
         """
-        Create a new note
+        Create a new company
 
         Parameters:
-            - request: CreateOrUpdateNoteRequest.
+            - request: CreateOrUpdateCompanyRequest.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/notes"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/companies"),
             json=jsonable_encoder(request),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CreateOrUpdateNoteResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateOrUpdateCompanyResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update_note(
+    async def update_company(
         self,
         id: str,
         *,
-        request: CreateOrUpdateNoteRequest,
+        request: Company,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> CreateOrUpdateNoteResponse:
+    ) -> CreateOrUpdateCompanyResponse:
         """
-        Update a note
+        Update a company
 
         Parameters:
             - id: str.
 
-            - request: CreateOrUpdateNoteRequest.
+            - request: Company.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/notes/{id}"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"crm/companies/{id}"),
             json=jsonable_encoder(request),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CreateOrUpdateNoteResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateOrUpdateCompanyResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def search_notes(
+    async def search_companies(
         self,
         *,
         fields: typing.Optional[str] = None,
+        page_size: typing.Optional[str] = None,
+        cursor: typing.Optional[str] = None,
         search_criteria: typing.Any,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
-    ) -> SearchNotesResponse:
+    ) -> SearchCompaniesResponse:
         """
-        Search for notes
+        Search for companies
 
         Parameters:
             - fields: typing.Optional[str].
 
+            - page_size: typing.Optional[str].
+
+            - cursor: typing.Optional[str].
+
             - search_criteria: typing.Any.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/notes/search"),
-            params=remove_none_from_dict({"fields": fields}),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/companies/search"),
+            params=remove_none_from_dict({"fields": fields, "pageSize": page_size, "cursor": cursor}),
             json=jsonable_encoder({"searchCriteria": search_criteria}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
                 }
             ),
             timeout=None,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(SearchNotesResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(SearchCompaniesResponse, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnAuthorizedError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(BaseError, _response.json()))  # type: ignore
         try:
```

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/note/types/__init__.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/note/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/note/types/create_or_update_note_request.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/note/types/create_or_update_note_request.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/note/types/create_or_update_note_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/note/types/create_or_update_note_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/note/types/get_note_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/task/types/get_task_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ......core.datetime_utils import serialize_datetime
 from .....common.resources.types.types.response_status import ResponseStatus
-from .....common.resources.unified.types.note import Note
+from .....common.resources.unified.types.task import Task
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class GetNoteResponse(pydantic.BaseModel):
+class GetTaskResponse(pydantic.BaseModel):
     status: ResponseStatus
-    result: Note
+    result: Task
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/note/types/get_notes_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/note/types/get_notes_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/note/types/search_notes_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/company/types/search_companies_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ......core.datetime_utils import serialize_datetime
 from .....common.resources.types.types.response_status import ResponseStatus
-from .....common.resources.unified.types.note import Note
+from .....common.resources.unified.types.company import Company
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class SearchNotesResponse(pydantic.BaseModel):
+class SearchCompaniesResponse(pydantic.BaseModel):
     status: ResponseStatus
-    results: typing.List[Note]
+    next: typing.Optional[str]
+    previous: typing.Optional[str]
+    results: typing.List[Company]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/properties/client.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/properties/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/properties/types/__init__.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/properties/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/properties/types/field_details_type.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/properties/types/field_details_type.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/properties/types/field_details_type_read.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/properties/types/field_details_type_read.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/properties/types/field_details_type_request.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/properties/types/field_details_type_request.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/proxy/client.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/proxy/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/proxy/types/post_proxy_request_body.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/proxy/types/post_proxy_request_body.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/proxy/types/proxy_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/proxy/types/proxy_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/task/client.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/task/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,37 +235,43 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def search_tasks(
         self,
         *,
         fields: typing.Optional[str] = None,
+        page_size: typing.Optional[str] = None,
+        cursor: typing.Optional[str] = None,
         search_criteria: typing.Any,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
     ) -> SearchTasksResponse:
         """
         Search for tasks
 
         Parameters:
             - fields: typing.Optional[str].
 
+            - page_size: typing.Optional[str].
+
+            - cursor: typing.Optional[str].
+
             - search_criteria: typing.Any.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/tasks/search"),
-            params=remove_none_from_dict({"fields": fields}),
+            params=remove_none_from_dict({"fields": fields, "pageSize": page_size, "cursor": cursor}),
             json=jsonable_encoder({"searchCriteria": search_criteria}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
@@ -496,37 +502,43 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def search_tasks(
         self,
         *,
         fields: typing.Optional[str] = None,
+        page_size: typing.Optional[str] = None,
+        cursor: typing.Optional[str] = None,
         search_criteria: typing.Any,
         x_revert_api_token: str,
         x_revert_t_id: str,
         x_api_version: typing.Optional[str] = None,
     ) -> SearchTasksResponse:
         """
         Search for tasks
 
         Parameters:
             - fields: typing.Optional[str].
 
+            - page_size: typing.Optional[str].
+
+            - cursor: typing.Optional[str].
+
             - search_criteria: typing.Any.
 
             - x_revert_api_token: str. Your official API key for accessing revert apis.
 
             - x_revert_t_id: str. The unique customer id used when the customer linked their account.
 
             - x_api_version: typing.Optional[str]. Optional Revert API version you're using. If missing we default to the latest version of the API.
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "crm/tasks/search"),
-            params=remove_none_from_dict({"fields": fields}),
+            params=remove_none_from_dict({"fields": fields, "pageSize": page_size, "cursor": cursor}),
             json=jsonable_encoder({"searchCriteria": search_criteria}),
             headers=remove_none_from_dict(
                 {
                     **self._client_wrapper.get_headers(),
                     "x-revert-api-token": x_revert_api_token,
                     "x-revert-t-id": x_revert_t_id,
                     "x-api-version": x_api_version,
```

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/task/types/__init__.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/task/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/task/types/create_or_update_task_request.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/task/types/create_or_update_task_request.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/task/types/create_or_update_task_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/task/types/create_or_update_task_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/task/types/get_task_response.py` & `revert_api-0.0.861/src/revert/resources/field_mapping/types/create_field_mapping_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ......core.datetime_utils import serialize_datetime
-from .....common.resources.types.types.response_status import ResponseStatus
-from .....common.resources.unified.types.task import Task
+from ....core.datetime_utils import serialize_datetime
+from ...common.resources.types.types.response_status import ResponseStatus
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class GetTaskResponse(pydantic.BaseModel):
+class CreateFieldMappingResponse(pydantic.BaseModel):
     status: ResponseStatus
-    result: Task
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/task/types/get_tasks_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/task/types/get_tasks_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/task/types/search_tasks_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/lead/types/search_leads_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ......core.datetime_utils import serialize_datetime
 from .....common.resources.types.types.response_status import ResponseStatus
-from .....common.resources.unified.types.task import Task
+from .....common.resources.unified.types.lead import Lead
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class SearchTasksResponse(pydantic.BaseModel):
+class SearchLeadsResponse(pydantic.BaseModel):
     status: ResponseStatus
-    results: typing.List[Task]
+    next: typing.Optional[str]
+    previous: typing.Optional[str]
+    results: typing.List[Lead]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/user/client.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/user/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/user/types/create_or_update_user_request.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/user/types/create_or_update_user_request.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/user/types/create_or_update_user_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/user/types/create_or_update_user_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/user/types/get_user_response.py` & `revert_api-0.0.861/src/revert/resources/ticket/resources/user/types/get_user_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ......core.datetime_utils import serialize_datetime
 from .....common.resources.types.types.response_status import ResponseStatus
-from .....common.resources.unified.types.user import User
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class GetUserResponse(pydantic.BaseModel):
     status: ResponseStatus
-    result: User
+    result: typing.Any
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `revert_api-0.0.852/src/revert/resources/crm/resources/user/types/get_users_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/user/types/get_users_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/field_mapping/__init__.py` & `revert_api-0.0.861/src/revert/resources/field_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/field_mapping/client.py` & `revert_api-0.0.861/src/revert/resources/field_mapping/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/field_mapping/types/__init__.py` & `revert_api-0.0.861/src/revert/resources/field_mapping/types/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/field_mapping/types/create_account_field_mapping_request_body.py` & `revert_api-0.0.861/src/revert/resources/field_mapping/types/create_account_field_mapping_request_body.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/field_mapping/types/create_account_field_mapping_response.py` & `revert_api-0.0.861/src/revert/resources/field_mapping/types/create_account_field_mapping_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/field_mapping/types/create_field_mapping_request_body.py` & `revert_api-0.0.861/src/revert/resources/field_mapping/types/create_field_mapping_request_body.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/field_mapping/types/create_field_mapping_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/note/types/search_notes_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ...common.resources.types.types.response_status import ResponseStatus
+from ......core.datetime_utils import serialize_datetime
+from .....common.resources.types.types.response_status import ResponseStatus
+from .....common.resources.unified.types.note import Note
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class CreateFieldMappingResponse(pydantic.BaseModel):
+class SearchNotesResponse(pydantic.BaseModel):
     status: ResponseStatus
+    next: typing.Optional[str]
+    previous: typing.Optional[str]
+    results: typing.List[Note]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `revert_api-0.0.852/src/revert/resources/field_mapping/types/delete_account_field_mapping_config_response.py` & `revert_api-0.0.861/src/revert/resources/field_mapping/types/delete_account_field_mapping_config_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/field_mapping/types/delete_field_mapping_response.py` & `revert_api-0.0.861/src/revert/resources/field_mapping/types/delete_field_mapping_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/field_mapping/types/field_mapping_type.py` & `revert_api-0.0.861/src/revert/resources/field_mapping/types/field_mapping_type.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/field_mapping/types/get_field_mapping_config_response.py` & `revert_api-0.0.861/src/revert/resources/field_mapping/types/get_field_mapping_config_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/field_mapping/types/get_field_mappings_response.py` & `revert_api-0.0.861/src/revert/resources/field_mapping/types/get_field_mappings_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/field_mapping/types/mappable_field_type.py` & `revert_api-0.0.861/src/revert/resources/field_mapping/types/mappable_field_type.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/metadata/client.py` & `revert_api-0.0.861/src/revert/resources/metadata/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/metadata/types/crm_metadata.py` & `revert_api-0.0.861/src/revert/resources/metadata/types/crm_metadata.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/metadata/types/crm_metadata_response.py` & `revert_api-0.0.861/src/revert/resources/metadata/types/crm_metadata_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/sync/client.py` & `revert_api-0.0.861/src/revert/resources/sync/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/sync/types/trigger_sync_response.py` & `revert_api-0.0.861/src/revert/resources/sync/types/trigger_sync_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/ticket/__init__.py` & `revert_api-0.0.861/src/revert/resources/ticket/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/ticket/client.py` & `revert_api-0.0.861/src/revert/resources/ticket/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/ticket/resources/__init__.py` & `revert_api-0.0.861/src/revert/resources/ticket/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/ticket/resources/collection/client.py` & `revert_api-0.0.861/src/revert/resources/ticket/resources/collection/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/ticket/resources/collection/types/get_collections_response.py` & `revert_api-0.0.861/src/revert/resources/ticket/resources/collection/types/get_collections_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/ticket/resources/comment/client.py` & `revert_api-0.0.861/src/revert/resources/ticket/resources/comment/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/ticket/resources/comment/types/create_or_update_comment_response.py` & `revert_api-0.0.861/src/revert/resources/ticket/resources/comment/types/create_or_update_comment_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/ticket/resources/comment/types/get_comment_response.py` & `revert_api-0.0.861/src/revert/resources/ticket/resources/comment/types/get_comment_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/ticket/resources/comment/types/get_comments_response.py` & `revert_api-0.0.861/src/revert/resources/ticket/resources/comment/types/get_comments_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/ticket/resources/proxy/client.py` & `revert_api-0.0.861/src/revert/resources/ticket/resources/proxy/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/ticket/resources/proxy/types/post_proxy_request_body.py` & `revert_api-0.0.861/src/revert/resources/ticket/resources/proxy/types/post_proxy_request_body.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/ticket/resources/proxy/types/proxy_response.py` & `revert_api-0.0.861/src/revert/resources/ticket/resources/proxy/types/proxy_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/ticket/resources/task/client.py` & `revert_api-0.0.861/src/revert/resources/ticket/resources/task/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/ticket/resources/task/types/create_or_update_task_response.py` & `revert_api-0.0.861/src/revert/resources/ticket/resources/task/types/create_or_update_task_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/ticket/resources/task/types/get_task_response.py` & `revert_api-0.0.861/src/revert/resources/ticket/resources/task/types/get_tasks_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class GetTaskResponse(pydantic.BaseModel):
+class GetTasksResponse(pydantic.BaseModel):
     status: ResponseStatus
-    result: TaskTicket
+    next: typing.Optional[str]
+    previous: typing.Optional[str]
+    results: typing.List[TaskTicket]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `revert_api-0.0.852/src/revert/resources/ticket/resources/task/types/get_tasks_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/task/types/search_tasks_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ......core.datetime_utils import serialize_datetime
 from .....common.resources.types.types.response_status import ResponseStatus
-from .....common.resources.unified.types.task_ticket import TaskTicket
+from .....common.resources.unified.types.task import Task
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class GetTasksResponse(pydantic.BaseModel):
+class SearchTasksResponse(pydantic.BaseModel):
     status: ResponseStatus
     next: typing.Optional[str]
     previous: typing.Optional[str]
-    results: typing.List[TaskTicket]
+    results: typing.List[Task]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `revert_api-0.0.852/src/revert/resources/ticket/resources/user/client.py` & `revert_api-0.0.861/src/revert/resources/ticket/resources/user/client.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/src/revert/resources/ticket/resources/user/types/get_user_response.py` & `revert_api-0.0.861/src/revert/resources/crm/resources/contact/types/search_contacts_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ......core.datetime_utils import serialize_datetime
 from .....common.resources.types.types.response_status import ResponseStatus
+from .....common.resources.unified.types.contact import Contact
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class GetUserResponse(pydantic.BaseModel):
+class SearchContactsResponse(pydantic.BaseModel):
     status: ResponseStatus
-    result: typing.Any
+    next: typing.Optional[str]
+    previous: typing.Optional[str]
+    results: typing.List[Contact]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `revert_api-0.0.852/src/revert/resources/ticket/resources/user/types/get_users_response.py` & `revert_api-0.0.861/src/revert/resources/ticket/resources/user/types/get_users_response.py`

 * *Files identical despite different names*

### Comparing `revert_api-0.0.852/PKG-INFO` & `revert_api-0.0.861/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revert-api
-Version: 0.0.852
+Version: 0.0.861
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

