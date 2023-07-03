# Comparing `tmp/ynab-api-2.0.0.tar.gz` & `tmp/ynab-api-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ynab-api-2.0.0.tar", last modified: Mon Jul  3 16:51:09 2023, max compression
+gzip compressed data, was "ynab-api-2.0.2.tar", last modified: Mon Jul  3 17:01:02 2023, max compression
```

## Comparing `ynab-api-2.0.0.tar` & `ynab-api-2.0.2.tar`

### file list

```diff
@@ -1,223 +1,223 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 16:51:09.379814 ynab-api-2.0.0/
--rw-rw-r--   0 david     (1000) david     (1000)      525 2023-07-03 16:51:09.379814 ynab-api-2.0.0/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)    13661 2023-07-03 16:46:53.000000 ynab-api-2.0.0/README.md
--rw-rw-r--   0 david     (1000) david     (1000)       69 2023-07-03 16:51:09.379814 ynab-api-2.0.0/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)     1448 2023-07-03 16:46:53.000000 ynab-api-2.0.0/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 16:51:09.367814 ynab-api-2.0.0/test/
--rw-rw-r--   0 david     (1000) david     (1000)      897 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_account.py
--rw-rw-r--   0 david     (1000) david     (1000)     1079 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_account_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1058 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_account_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)     1182 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_accounts_api.py
--rw-rw-r--   0 david     (1000) david     (1000)     1090 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_accounts_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1065 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_accounts_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)     2365 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_budget_detail.py
--rw-rw-r--   0 david     (1000) david     (1000)     1996 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_budget_detail_all_of.py
--rw-rw-r--   0 david     (1000) david     (1000)     1136 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_budget_detail_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1115 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_budget_detail_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)     1138 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_budget_settings.py
--rw-rw-r--   0 david     (1000) david     (1000)     1158 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_budget_settings_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1137 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_budget_settings_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)     1205 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_budget_summary.py
--rw-rw-r--   0 david     (1000) david     (1000)     1147 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_budget_summary_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1126 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_budget_summary_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)     1189 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_budgets_api.py
--rw-rw-r--   0 david     (1000) david     (1000)     1046 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_bulk_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1092 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_bulk_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)      991 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_bulk_response_data_bulk.py
--rw-rw-r--   0 david     (1000) david     (1000)     1069 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_bulk_transactions.py
--rw-rw-r--   0 david     (1000) david     (1000)     1422 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_categories_api.py
--rw-rw-r--   0 david     (1000) david     (1000)     1112 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_categories_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1162 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_categories_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)      904 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_category.py
--rw-rw-r--   0 david     (1000) david     (1000)      940 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_category_group.py
--rw-rw-r--   0 david     (1000) david     (1000)     1398 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_category_group_with_categories.py
--rw-rw-r--   0 david     (1000) david     (1000)     1156 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_category_group_with_categories_all_of.py
--rw-rw-r--   0 david     (1000) david     (1000)     1090 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_category_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1069 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_category_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)      947 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_currency_format.py
--rw-rw-r--   0 david     (1000) david     (1000)      919 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_date_format.py
--rw-rw-r--   0 david     (1000) david     (1000)      938 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_deprecated_api.py
--rw-rw-r--   0 david     (1000) david     (1000)      926 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_error_detail.py
--rw-rw-r--   0 david     (1000) david     (1000)     1032 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_error_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1225 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_hybrid_transaction.py
--rw-rw-r--   0 david     (1000) david     (1000)     1005 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_hybrid_transaction_all_of.py
--rw-rw-r--   0 david     (1000) david     (1000)     1202 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_hybrid_transactions_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1177 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_hybrid_transactions_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)     1213 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_month_detail.py
--rw-rw-r--   0 david     (1000) david     (1000)     1042 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_month_detail_all_of.py
--rw-rw-r--   0 david     (1000) david     (1000)     1125 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_month_detail_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1104 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_month_detail_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)     1158 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_month_summaries_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1129 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_month_summaries_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)      933 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_month_summary.py
--rw-rw-r--   0 david     (1000) david     (1000)     1046 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_months_api.py
--rw-rw-r--   0 david     (1000) david     (1000)      883 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payee.py
--rw-rw-r--   0 david     (1000) david     (1000)      940 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payee_location.py
--rw-rw-r--   0 david     (1000) david     (1000)     1147 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payee_location_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1126 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payee_location_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)     1290 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payee_locations_api.py
--rw-rw-r--   0 david     (1000) david     (1000)     1158 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payee_locations_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1133 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payee_locations_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)     1057 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payee_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1036 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payee_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)     1016 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payees_api.py
--rw-rw-r--   0 david     (1000) david     (1000)     1068 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payees_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1043 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payees_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)      926 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_account.py
--rw-rw-r--   0 david     (1000) david     (1000)     1068 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_account_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)     1136 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_category_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1098 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_category_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)      969 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_month_category.py
--rw-rw-r--   0 david     (1000) david     (1000)     1136 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_month_category_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)      976 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_sub_transaction.py
--rw-rw-r--   0 david     (1000) david     (1000)     1075 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_transaction.py
--rw-rw-r--   0 david     (1000) david     (1000)     1112 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_transaction_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)     1180 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_transactions_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1163 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_transactions_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)     1119 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_transactions_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)     1011 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_scheduled_sub_transaction.py
--rw-rw-r--   0 david     (1000) david     (1000)     1503 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_scheduled_transaction_detail.py
--rw-rw-r--   0 david     (1000) david     (1000)     1210 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_scheduled_transaction_detail_all_of.py
--rw-rw-r--   0 david     (1000) david     (1000)     1225 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_scheduled_transaction_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1228 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_scheduled_transaction_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)     1039 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_scheduled_transaction_summary.py
--rw-rw-r--   0 david     (1000) david     (1000)     1188 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_scheduled_transactions_api.py
--rw-rw-r--   0 david     (1000) david     (1000)     1236 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_scheduled_transactions_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1235 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_scheduled_transactions_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)      947 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_sub_transaction.py
--rw-rw-r--   0 david     (1000) david     (1000)     1328 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_transaction_detail.py
--rw-rw-r--   0 david     (1000) david     (1000)     1109 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_transaction_detail_all_of.py
--rw-rw-r--   0 david     (1000) david     (1000)     1123 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_transaction_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1127 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_transaction_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)      975 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_transaction_summary.py
--rw-rw-r--   0 david     (1000) david     (1000)     2273 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_transactions_api.py
--rw-rw-r--   0 david     (1000) david     (1000)     1202 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_transactions_import_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1061 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_transactions_import_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)     1134 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_transactions_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1134 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_transactions_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)     1333 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_update_transaction.py
--rw-rw-r--   0 david     (1000) david     (1000)     1005 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_update_transaction_all_of.py
--rw-rw-r--   0 david     (1000) david     (1000)     1141 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_update_transactions_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)      876 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_user.py
--rw-rw-r--   0 david     (1000) david     (1000)      861 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_user_api.py
--rw-rw-r--   0 david     (1000) david     (1000)     1046 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_user_response.py
--rw-rw-r--   0 david     (1000) david     (1000)     1025 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_user_response_data.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 16:51:09.367814 ynab-api-2.0.0/ynab_api/
--rw-rw-r--   0 david     (1000) david     (1000)      897 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 16:51:09.367814 ynab-api-2.0.0/ynab_api/api/
--rw-rw-r--   0 david     (1000) david     (1000)      213 2023-07-03 16:46:01.000000 ynab-api-2.0.0/ynab_api/api/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    14003 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/api/accounts_api.py
--rw-rw-r--   0 david     (1000) david     (1000)    14518 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/api/budgets_api.py
--rw-rw-r--   0 david     (1000) david     (1000)    20333 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/api/categories_api.py
--rw-rw-r--   0 david     (1000) david     (1000)     5668 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/api/deprecated_api.py
--rw-rw-r--   0 david     (1000) david     (1000)    11493 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/api/months_api.py
--rw-rw-r--   0 david     (1000) david     (1000)    14006 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/api/payee_locations_api.py
--rw-rw-r--   0 david     (1000) david     (1000)    11258 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/api/payees_api.py
--rw-rw-r--   0 david     (1000) david     (1000)    10380 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/api/scheduled_transactions_api.py
--rw-rw-r--   0 david     (1000) david     (1000)    46788 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/api/transactions_api.py
--rw-rw-r--   0 david     (1000) david     (1000)     4953 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/api/user_api.py
--rw-rw-r--   0 david     (1000) david     (1000)    37468 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/api_client.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 16:51:09.367814 ynab-api-2.0.0/ynab_api/apis/
--rw-rw-r--   0 david     (1000) david     (1000)      952 2023-07-03 16:46:01.000000 ynab-api-2.0.0/ynab_api/apis/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    17225 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/configuration.py
--rw-rw-r--   0 david     (1000) david     (1000)     5314 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/exceptions.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 16:51:09.379814 ynab-api-2.0.0/ynab_api/model/
--rw-rw-r--   0 david     (1000) david     (1000)      348 2023-07-03 16:46:01.000000 ynab-api-2.0.0/ynab_api/model/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    16686 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/account.py
--rw-rw-r--   0 david     (1000) david     (1000)    11651 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/account_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    11610 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/account_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)    11661 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/accounts_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    12053 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/accounts_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)    19151 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/budget_detail.py
--rw-rw-r--   0 david     (1000) david     (1000)    15032 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/budget_detail_all_of.py
--rw-rw-r--   0 david     (1000) david     (1000)    11702 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/budget_detail_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    12073 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/budget_detail_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)    12161 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/budget_settings.py
--rw-rw-r--   0 david     (1000) david     (1000)    11722 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/budget_settings_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    11692 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/budget_settings_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)    13786 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/budget_summary.py
--rw-rw-r--   0 david     (1000) david     (1000)    11712 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/budget_summary_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    11936 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/budget_summary_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)    11621 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/bulk_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    11662 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/bulk_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)    12417 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/bulk_response_data_bulk.py
--rw-rw-r--   0 david     (1000) david     (1000)    11719 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/bulk_transactions.py
--rw-rw-r--   0 david     (1000) david     (1000)    11681 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/categories_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    12279 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/categories_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)    18876 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/category.py
--rw-rw-r--   0 david     (1000) david     (1000)    12380 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/category_group.py
--rw-rw-r--   0 david     (1000) david     (1000)    14954 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/category_group_with_categories.py
--rw-rw-r--   0 david     (1000) david     (1000)    11935 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/category_group_with_categories_all_of.py
--rw-rw-r--   0 david     (1000) david     (1000)    11661 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/category_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    11631 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/category_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)    13725 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/currency_format.py
--rw-rw-r--   0 david     (1000) david     (1000)    11413 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/date_format.py
--rw-rw-r--   0 david     (1000) david     (1000)    11803 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/error_detail.py
--rw-rw-r--   0 david     (1000) david     (1000)    11599 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/error_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    20383 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/hybrid_transaction.py
--rw-rw-r--   0 david     (1000) david     (1000)    12976 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/hybrid_transaction_all_of.py
--rw-rw-r--   0 david     (1000) david     (1000)    11767 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/hybrid_transactions_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    11775 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/hybrid_transactions_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)    16149 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/month_detail.py
--rw-rw-r--   0 david     (1000) david     (1000)    11893 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/month_detail_all_of.py
--rw-rw-r--   0 david     (1000) david     (1000)    11692 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/month_detail_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    11629 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/month_detail_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)    11722 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/month_summaries_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    12085 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/month_summaries_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)    13983 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/month_summary.py
--rw-rw-r--   0 david     (1000) david     (1000)    12397 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/payee.py
--rw-rw-r--   0 david     (1000) david     (1000)    12601 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/payee_location.py
--rw-rw-r--   0 david     (1000) david     (1000)    11712 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/payee_location_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    11748 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/payee_location_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)    11722 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/payee_locations_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    11795 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/payee_locations_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)    11631 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/payee_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    11568 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/payee_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)    11641 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/payees_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    12011 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/payees_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)    12338 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_account.py
--rw-rw-r--   0 david     (1000) david     (1000)    11636 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_account_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)    11702 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_category_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    12066 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_category_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)    11530 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_month_category.py
--rw-rw-r--   0 david     (1000) david     (1000)    11708 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_month_category_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)    13410 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_sub_transaction.py
--rw-rw-r--   0 david     (1000) david     (1000)    19841 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_transaction.py
--rw-rw-r--   0 david     (1000) david     (1000)    11720 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_transaction_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)    11742 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_transactions_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    13485 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_transactions_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)    11900 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_transactions_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)    13697 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/scheduled_sub_transaction.py
--rw-rw-r--   0 david     (1000) david     (1000)    18477 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/scheduled_transaction_detail.py
--rw-rw-r--   0 david     (1000) david     (1000)    12720 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/scheduled_transaction_detail_all_of.py
--rw-rw-r--   0 david     (1000) david     (1000)    11787 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/scheduled_transaction_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    11977 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/scheduled_transaction_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)    15597 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/scheduled_transaction_summary.py
--rw-rw-r--   0 david     (1000) david     (1000)    11797 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/scheduled_transactions_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    12393 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/scheduled_transactions_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)    14331 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/sub_transaction.py
--rw-rw-r--   0 david     (1000) david     (1000)    19873 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/transaction_detail.py
--rw-rw-r--   0 david     (1000) david     (1000)    12609 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/transaction_detail_all_of.py
--rw-rw-r--   0 david     (1000) david     (1000)    11691 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/transaction_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    11737 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/transaction_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)    17120 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/transaction_summary.py
--rw-rw-r--   0 david     (1000) david     (1000)    11767 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/transactions_import_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    11701 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/transactions_import_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)    11701 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/transactions_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    12180 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/transactions_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)    21912 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/update_transaction.py
--rw-rw-r--   0 david     (1000) david     (1000)    11405 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/update_transaction_all_of.py
--rw-rw-r--   0 david     (1000) david     (1000)    11760 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/update_transactions_wrapper.py
--rw-rw-r--   0 david     (1000) david     (1000)    11351 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/user.py
--rw-rw-r--   0 david     (1000) david     (1000)    11621 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/user_response.py
--rw-rw-r--   0 david     (1000) david     (1000)    11547 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/user_response_data.py
--rw-rw-r--   0 david     (1000) david     (1000)    83377 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model_utils.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 16:51:09.379814 ynab-api-2.0.0/ynab_api/models/
--rw-rw-r--   0 david     (1000) david     (1000)     6525 2023-07-03 16:46:01.000000 ynab-api-2.0.0/ynab_api/models/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    13847 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/rest.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 16:51:09.367814 ynab-api-2.0.0/ynab_api.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)      525 2023-07-03 16:51:09.000000 ynab-api-2.0.0/ynab_api.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     7689 2023-07-03 16:51:09.000000 ynab-api-2.0.0/ynab_api.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-07-03 16:51:09.000000 ynab-api-2.0.0/ynab_api.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       32 2023-07-03 16:51:09.000000 ynab-api-2.0.0/ynab_api.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)        9 2023-07-03 16:51:09.000000 ynab-api-2.0.0/ynab_api.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 17:01:02.982567 ynab-api-2.0.2/
+-rw-rw-r--   0 david     (1000) david     (1000)      543 2023-07-03 17:01:02.982567 ynab-api-2.0.2/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)    14061 2023-07-03 16:55:13.000000 ynab-api-2.0.2/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)       69 2023-07-03 17:01:02.982567 ynab-api-2.0.2/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)     1466 2023-07-03 16:59:52.000000 ynab-api-2.0.2/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 17:01:02.974567 ynab-api-2.0.2/test/
+-rw-rw-r--   0 david     (1000) david     (1000)      897 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_account.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1079 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_account_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1058 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_account_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1182 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_accounts_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1090 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_accounts_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1065 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_accounts_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2365 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_budget_detail.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1996 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_budget_detail_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1136 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_budget_detail_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1115 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_budget_detail_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1138 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_budget_settings.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1158 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_budget_settings_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1137 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_budget_settings_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1205 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_budget_summary.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1147 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_budget_summary_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1126 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_budget_summary_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1189 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_budgets_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1046 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_bulk_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1092 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_bulk_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)      991 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_bulk_response_data_bulk.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1069 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_bulk_transactions.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1422 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_categories_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1112 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_categories_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1162 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_categories_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)      904 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_category.py
+-rw-rw-r--   0 david     (1000) david     (1000)      940 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_category_group.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1398 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_category_group_with_categories.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1156 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_category_group_with_categories_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1090 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_category_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1069 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_category_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)      947 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_currency_format.py
+-rw-rw-r--   0 david     (1000) david     (1000)      919 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_date_format.py
+-rw-rw-r--   0 david     (1000) david     (1000)      938 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_deprecated_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)      926 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_error_detail.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1032 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_error_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1225 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_hybrid_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1005 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_hybrid_transaction_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1202 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_hybrid_transactions_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1177 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_hybrid_transactions_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1213 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_month_detail.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1042 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_month_detail_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1125 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_month_detail_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1104 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_month_detail_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1158 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_month_summaries_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1129 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_month_summaries_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)      933 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_month_summary.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1046 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_months_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)      883 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_payee.py
+-rw-rw-r--   0 david     (1000) david     (1000)      940 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_payee_location.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1147 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_payee_location_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1126 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_payee_location_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1290 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_payee_locations_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1158 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_payee_locations_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1133 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_payee_locations_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1057 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_payee_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1036 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_payee_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1016 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_payees_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1068 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_payees_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1043 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_payees_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)      926 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_save_account.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1068 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_save_account_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1136 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_save_category_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1098 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_save_category_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)      969 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_save_month_category.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1136 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_save_month_category_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)      976 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_save_sub_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1075 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_save_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1112 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_save_transaction_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1180 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_save_transactions_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1163 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_save_transactions_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1119 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_save_transactions_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1011 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_scheduled_sub_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1503 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_scheduled_transaction_detail.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1210 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_scheduled_transaction_detail_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1225 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_scheduled_transaction_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1228 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_scheduled_transaction_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1039 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_scheduled_transaction_summary.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1188 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_scheduled_transactions_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1236 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_scheduled_transactions_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1235 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_scheduled_transactions_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)      947 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_sub_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1328 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_transaction_detail.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1109 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_transaction_detail_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1123 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_transaction_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1127 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_transaction_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)      975 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_transaction_summary.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2273 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_transactions_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1202 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_transactions_import_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1061 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_transactions_import_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1134 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_transactions_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1134 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_transactions_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1333 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_update_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1005 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_update_transaction_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1141 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_update_transactions_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)      876 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_user.py
+-rw-rw-r--   0 david     (1000) david     (1000)      861 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_user_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1046 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_user_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1025 2023-07-03 16:46:01.000000 ynab-api-2.0.2/test/test_user_response_data.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 17:01:02.974567 ynab-api-2.0.2/ynab_api/
+-rw-rw-r--   0 david     (1000) david     (1000)      897 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 17:01:02.974567 ynab-api-2.0.2/ynab_api/api/
+-rw-rw-r--   0 david     (1000) david     (1000)      213 2023-07-03 16:46:01.000000 ynab-api-2.0.2/ynab_api/api/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    14690 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/api/accounts_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)    14800 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/api/budgets_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)    21654 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/api/categories_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5809 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/api/deprecated_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12326 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/api/months_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)    14684 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/api/payee_locations_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12144 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/api/payees_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10940 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/api/scheduled_transactions_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)    50244 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/api/transactions_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4953 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/api/user_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)    37468 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/api_client.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 17:01:02.974567 ynab-api-2.0.2/ynab_api/apis/
+-rw-rw-r--   0 david     (1000) david     (1000)      952 2023-07-03 16:46:01.000000 ynab-api-2.0.2/ynab_api/apis/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    17225 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/configuration.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5314 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/exceptions.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 17:01:02.982567 ynab-api-2.0.2/ynab_api/model/
+-rw-rw-r--   0 david     (1000) david     (1000)      348 2023-07-03 16:46:01.000000 ynab-api-2.0.2/ynab_api/model/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    17258 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/account.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11651 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/account_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11610 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/account_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11661 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/accounts_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12131 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/accounts_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    19541 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/budget_detail.py
+-rw-rw-r--   0 david     (1000) david     (1000)    15032 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/budget_detail_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11702 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/budget_detail_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12151 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/budget_detail_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12161 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/budget_settings.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11722 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/budget_settings_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11692 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/budget_settings_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    14176 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/budget_summary.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11712 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/budget_summary_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11936 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/budget_summary_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11621 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/bulk_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11662 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/bulk_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12483 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/bulk_response_data_bulk.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11719 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/bulk_transactions.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11681 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/categories_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12357 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/categories_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    20150 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/category.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12536 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/category_group.py
+-rw-rw-r--   0 david     (1000) david     (1000)    15110 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/category_group_with_categories.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11935 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/category_group_with_categories_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11661 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/category_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11631 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/category_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    14193 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/currency_format.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11491 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/date_format.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12037 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/error_detail.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11599 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/error_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    21865 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/hybrid_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13392 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/hybrid_transaction_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11767 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/hybrid_transactions_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11775 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/hybrid_transactions_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    16617 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/month_detail.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11893 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/month_detail_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11692 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/month_detail_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11629 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/month_detail_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11722 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/month_summaries_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12163 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/month_summaries_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    14451 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/month_summary.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12631 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/payee.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12913 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/payee_location.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11712 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/payee_location_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11748 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/payee_location_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11722 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/payee_locations_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11795 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/payee_locations_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11631 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/payee_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11568 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/payee_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11641 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/payees_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12089 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/payees_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12598 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/save_account.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11636 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/save_account_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11702 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/save_category_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12144 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/save_category_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11608 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/save_month_category.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11708 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/save_month_category_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13800 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/save_sub_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)    20673 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/save_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11720 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/save_transaction_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11742 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/save_transactions_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13629 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/save_transactions_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11900 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/save_transactions_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)    14243 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/scheduled_sub_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)    19621 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/scheduled_transaction_detail.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12954 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/scheduled_transaction_detail_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11787 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/scheduled_transaction_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11977 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/scheduled_transaction_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    16507 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/scheduled_transaction_summary.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11797 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/scheduled_transactions_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12471 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/scheduled_transactions_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    15111 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/sub_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)    21173 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/transaction_detail.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12843 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/transaction_detail_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11691 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/transaction_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11737 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/transaction_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    18186 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/transaction_summary.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11767 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/transactions_import_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11734 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/transactions_import_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11701 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/transactions_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12258 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/transactions_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    22822 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/update_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11483 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/update_transaction_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11760 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/update_transactions_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11429 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/user.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11621 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/user_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11547 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model/user_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    83377 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/model_utils.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 17:01:02.982567 ynab-api-2.0.2/ynab_api/models/
+-rw-rw-r--   0 david     (1000) david     (1000)     6525 2023-07-03 16:46:01.000000 ynab-api-2.0.2/ynab_api/models/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13847 2023-07-03 16:55:13.000000 ynab-api-2.0.2/ynab_api/rest.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 17:01:02.974567 ynab-api-2.0.2/ynab_api.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)      543 2023-07-03 17:01:02.000000 ynab-api-2.0.2/ynab_api.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     7689 2023-07-03 17:01:02.000000 ynab-api-2.0.2/ynab_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-07-03 17:01:02.000000 ynab-api-2.0.2/ynab_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       32 2023-07-03 17:01:02.000000 ynab-api-2.0.2/ynab_api.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        9 2023-07-03 17:01:02.000000 ynab-api-2.0.2/ynab_api.egg-info/top_level.txt
```

### Comparing `ynab-api-2.0.0/PKG-INFO` & `ynab-api-2.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ynab-api
-Version: 2.0.0
+Version: 2.0.2
 Summary: YNAB API Endpoints
 Home-page: 
-Author: David Lerner
-Author-email: dmlerner@gmail.com
+Author: OpenAPI Generator community
+Author-email: team@openapitools.org
 Keywords: OpenAPI,OpenAPI-Generator,YNAB API Endpoints
 Requires-Python: >=3.6
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
```

### Comparing `ynab-api-2.0.0/README.md` & `ynab-api-2.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,119 +1,100 @@
 # ynab-api
-
 Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.0
+- API version: 2.0.3
 - Package version: 1.0.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python >= 3.6
 
 ## Installation & Usage
-
 ### pip install
 
-```sh
-pip install git+https://github.com/dmlerner/ynab-api.git
-```
-
-NOTE: If you get issues about nullability or things being not set, consider installed the "nullfix" branch:
+If the python package is hosted on a repository, you can install directly using:
 
 ```sh
-pip install git+https://github.com/dmlerner/ynab-api.git@nullfix
+pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
 ```
-
-(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/dmlerner/ynab-api.git`)
+(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
 
 Then import the package:
-
 ```python
 import ynab_api
 ```
 
-NOTE: the pip package `ynab_api` is an old, non-working version of this.
-I am working to get it updated, but am locked out of that account.
-
 ### Setuptools
 
 Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
 
 ```sh
 python setup.py install --user
 ```
-
 (or `sudo python setup.py install` to install the package for all users)
 
 Then import the package:
-
 ```python
 import ynab_api
 ```
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
-```
-python ynabdemo.py
-```
-
-## Sample usage (ynabdemo.py)
-
 ```python
-import json
+
+import time
 import ynab_api
 from pprint import pprint
 from ynab_api.api import accounts_api
-'''
-secrets.json should be manually generated as:
+from ynab_api.model.account_response import AccountResponse
+from ynab_api.model.accounts_response import AccountsResponse
+from ynab_api.model.error_response import ErrorResponse
+from ynab_api.model.save_account_wrapper import SaveAccountWrapper
+# Defining the host is optional and defaults to https://api.youneedabudget.com/v1
+# See configuration.py for a list of all supported configuration parameters.
+configuration = ynab_api.Configuration(
+    host = "https://api.youneedabudget.com/v1"
+)
 
-{
-   "budget_id":"xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx"
-   "api_key":"xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
-}
-
-To get an api_key:
-Sign in to the YNAB web app
-and go to the "Account Settings" page
-and then to the "Developer Settings" page.
-Under the "Personal Access Tokens" section,
-click "New Token", enter your password
-and click "Generate" to get an access token.
-
-To get your budget_id:
-Sign in to the YNAB web app and go the budget of interest.
-Copy YOUR_BUDGET_ID from the url:
-https://app.youneedabudget.com/YOUR_BUDGET_ID/budget
-
-Or, populate the fields directly in your code.
-'''
-
-with open('secrets.json') as f:
-    secrets = json.load(f)
-budget_id = secrets['budget_id']
-api_key = secrets['api_key']
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure API key authorization: bearer
+configuration.api_key['bearer'] = 'YOUR_API_KEY'
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['bearer'] = 'Bearer'
 
-configuration = ynab_api.Configuration(
-    host="https://api.youneedabudget.com/v1")
-configuration.api_key['bearer'] = api_key
-configuration.api_key_prefix['bearer'] = 'Bearer'
 
+# Enter a context with an instance of the API client
 with ynab_api.ApiClient(configuration) as api_client:
+    # Create an instance of the API class
     api_instance = accounts_api.AccountsApi(api_client)
+    budget_id = "budget_id_example" # str, none_type | The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget)
+data = SaveAccountWrapper(
+        account=SaveAccount(
+            name="name_example",
+            type="checking",
+            balance=1,
+        ),
+    ) # SaveAccountWrapper | The account to create.
 
     try:
-        api_response = api_instance.get_accounts(budget_id)
+        # Create a new account
+        api_response = api_instance.create_account(budget_id, data)
         pprint(api_response)
     except ynab_api.ApiException as e:
-        print("Exception: %s\n" % e)
+        print("Exception when calling AccountsApi->create_account: %s\n" % e)
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://api.youneedabudget.com/v1*
 
 Class | Method | HTTP request | Description
@@ -145,131 +126,134 @@
 *TransactionsApi* | [**get_transactions_by_category**](docs/TransactionsApi.md#get_transactions_by_category) | **GET** /budgets/{budget_id}/categories/{category_id}/transactions | List category transactions
 *TransactionsApi* | [**get_transactions_by_payee**](docs/TransactionsApi.md#get_transactions_by_payee) | **GET** /budgets/{budget_id}/payees/{payee_id}/transactions | List payee transactions
 *TransactionsApi* | [**import_transactions**](docs/TransactionsApi.md#import_transactions) | **POST** /budgets/{budget_id}/transactions/import | Import transactions
 *TransactionsApi* | [**update_transaction**](docs/TransactionsApi.md#update_transaction) | **PUT** /budgets/{budget_id}/transactions/{transaction_id} | Updates an existing transaction
 *TransactionsApi* | [**update_transactions**](docs/TransactionsApi.md#update_transactions) | **PATCH** /budgets/{budget_id}/transactions | Update multiple transactions
 *UserApi* | [**get_user**](docs/UserApi.md#get_user) | **GET** /user | User info
 
+
 ## Documentation For Models
 
-- [Account](docs/Account.md)
-- [AccountResponse](docs/AccountResponse.md)
-- [AccountResponseData](docs/AccountResponseData.md)
-- [AccountsResponse](docs/AccountsResponse.md)
-- [AccountsResponseData](docs/AccountsResponseData.md)
-- [BudgetDetail](docs/BudgetDetail.md)
-- [BudgetDetailAllOf](docs/BudgetDetailAllOf.md)
-- [BudgetDetailResponse](docs/BudgetDetailResponse.md)
-- [BudgetDetailResponseData](docs/BudgetDetailResponseData.md)
-- [BudgetSettings](docs/BudgetSettings.md)
-- [BudgetSettingsResponse](docs/BudgetSettingsResponse.md)
-- [BudgetSettingsResponseData](docs/BudgetSettingsResponseData.md)
-- [BudgetSummary](docs/BudgetSummary.md)
-- [BudgetSummaryResponse](docs/BudgetSummaryResponse.md)
-- [BudgetSummaryResponseData](docs/BudgetSummaryResponseData.md)
-- [BulkResponse](docs/BulkResponse.md)
-- [BulkResponseData](docs/BulkResponseData.md)
-- [BulkResponseDataBulk](docs/BulkResponseDataBulk.md)
-- [BulkTransactions](docs/BulkTransactions.md)
-- [CategoriesResponse](docs/CategoriesResponse.md)
-- [CategoriesResponseData](docs/CategoriesResponseData.md)
-- [Category](docs/Category.md)
-- [CategoryGroup](docs/CategoryGroup.md)
-- [CategoryGroupWithCategories](docs/CategoryGroupWithCategories.md)
-- [CategoryGroupWithCategoriesAllOf](docs/CategoryGroupWithCategoriesAllOf.md)
-- [CategoryResponse](docs/CategoryResponse.md)
-- [CategoryResponseData](docs/CategoryResponseData.md)
-- [CurrencyFormat](docs/CurrencyFormat.md)
-- [DateFormat](docs/DateFormat.md)
-- [ErrorDetail](docs/ErrorDetail.md)
-- [ErrorResponse](docs/ErrorResponse.md)
-- [HybridTransaction](docs/HybridTransaction.md)
-- [HybridTransactionAllOf](docs/HybridTransactionAllOf.md)
-- [HybridTransactionsResponse](docs/HybridTransactionsResponse.md)
-- [HybridTransactionsResponseData](docs/HybridTransactionsResponseData.md)
-- [MonthDetail](docs/MonthDetail.md)
-- [MonthDetailAllOf](docs/MonthDetailAllOf.md)
-- [MonthDetailResponse](docs/MonthDetailResponse.md)
-- [MonthDetailResponseData](docs/MonthDetailResponseData.md)
-- [MonthSummariesResponse](docs/MonthSummariesResponse.md)
-- [MonthSummariesResponseData](docs/MonthSummariesResponseData.md)
-- [MonthSummary](docs/MonthSummary.md)
-- [Payee](docs/Payee.md)
-- [PayeeLocation](docs/PayeeLocation.md)
-- [PayeeLocationResponse](docs/PayeeLocationResponse.md)
-- [PayeeLocationResponseData](docs/PayeeLocationResponseData.md)
-- [PayeeLocationsResponse](docs/PayeeLocationsResponse.md)
-- [PayeeLocationsResponseData](docs/PayeeLocationsResponseData.md)
-- [PayeeResponse](docs/PayeeResponse.md)
-- [PayeeResponseData](docs/PayeeResponseData.md)
-- [PayeesResponse](docs/PayeesResponse.md)
-- [PayeesResponseData](docs/PayeesResponseData.md)
-- [SaveAccount](docs/SaveAccount.md)
-- [SaveAccountWrapper](docs/SaveAccountWrapper.md)
-- [SaveCategoryResponse](docs/SaveCategoryResponse.md)
-- [SaveCategoryResponseData](docs/SaveCategoryResponseData.md)
-- [SaveMonthCategory](docs/SaveMonthCategory.md)
-- [SaveMonthCategoryWrapper](docs/SaveMonthCategoryWrapper.md)
-- [SaveSubTransaction](docs/SaveSubTransaction.md)
-- [SaveTransaction](docs/SaveTransaction.md)
-- [SaveTransactionWrapper](docs/SaveTransactionWrapper.md)
-- [SaveTransactionsResponse](docs/SaveTransactionsResponse.md)
-- [SaveTransactionsResponseData](docs/SaveTransactionsResponseData.md)
-- [SaveTransactionsWrapper](docs/SaveTransactionsWrapper.md)
-- [ScheduledSubTransaction](docs/ScheduledSubTransaction.md)
-- [ScheduledTransactionDetail](docs/ScheduledTransactionDetail.md)
-- [ScheduledTransactionDetailAllOf](docs/ScheduledTransactionDetailAllOf.md)
-- [ScheduledTransactionResponse](docs/ScheduledTransactionResponse.md)
-- [ScheduledTransactionResponseData](docs/ScheduledTransactionResponseData.md)
-- [ScheduledTransactionSummary](docs/ScheduledTransactionSummary.md)
-- [ScheduledTransactionsResponse](docs/ScheduledTransactionsResponse.md)
-- [ScheduledTransactionsResponseData](docs/ScheduledTransactionsResponseData.md)
-- [SubTransaction](docs/SubTransaction.md)
-- [TransactionDetail](docs/TransactionDetail.md)
-- [TransactionDetailAllOf](docs/TransactionDetailAllOf.md)
-- [TransactionResponse](docs/TransactionResponse.md)
-- [TransactionResponseData](docs/TransactionResponseData.md)
-- [TransactionSummary](docs/TransactionSummary.md)
-- [TransactionsImportResponse](docs/TransactionsImportResponse.md)
-- [TransactionsImportResponseData](docs/TransactionsImportResponseData.md)
-- [TransactionsResponse](docs/TransactionsResponse.md)
-- [TransactionsResponseData](docs/TransactionsResponseData.md)
-- [UpdateTransaction](docs/UpdateTransaction.md)
-- [UpdateTransactionAllOf](docs/UpdateTransactionAllOf.md)
-- [UpdateTransactionsWrapper](docs/UpdateTransactionsWrapper.md)
-- [User](docs/User.md)
-- [UserResponse](docs/UserResponse.md)
-- [UserResponseData](docs/UserResponseData.md)
+ - [Account](docs/Account.md)
+ - [AccountResponse](docs/AccountResponse.md)
+ - [AccountResponseData](docs/AccountResponseData.md)
+ - [AccountsResponse](docs/AccountsResponse.md)
+ - [AccountsResponseData](docs/AccountsResponseData.md)
+ - [BudgetDetail](docs/BudgetDetail.md)
+ - [BudgetDetailAllOf](docs/BudgetDetailAllOf.md)
+ - [BudgetDetailResponse](docs/BudgetDetailResponse.md)
+ - [BudgetDetailResponseData](docs/BudgetDetailResponseData.md)
+ - [BudgetSettings](docs/BudgetSettings.md)
+ - [BudgetSettingsResponse](docs/BudgetSettingsResponse.md)
+ - [BudgetSettingsResponseData](docs/BudgetSettingsResponseData.md)
+ - [BudgetSummary](docs/BudgetSummary.md)
+ - [BudgetSummaryResponse](docs/BudgetSummaryResponse.md)
+ - [BudgetSummaryResponseData](docs/BudgetSummaryResponseData.md)
+ - [BulkResponse](docs/BulkResponse.md)
+ - [BulkResponseData](docs/BulkResponseData.md)
+ - [BulkResponseDataBulk](docs/BulkResponseDataBulk.md)
+ - [BulkTransactions](docs/BulkTransactions.md)
+ - [CategoriesResponse](docs/CategoriesResponse.md)
+ - [CategoriesResponseData](docs/CategoriesResponseData.md)
+ - [Category](docs/Category.md)
+ - [CategoryGroup](docs/CategoryGroup.md)
+ - [CategoryGroupWithCategories](docs/CategoryGroupWithCategories.md)
+ - [CategoryGroupWithCategoriesAllOf](docs/CategoryGroupWithCategoriesAllOf.md)
+ - [CategoryResponse](docs/CategoryResponse.md)
+ - [CategoryResponseData](docs/CategoryResponseData.md)
+ - [CurrencyFormat](docs/CurrencyFormat.md)
+ - [DateFormat](docs/DateFormat.md)
+ - [ErrorDetail](docs/ErrorDetail.md)
+ - [ErrorResponse](docs/ErrorResponse.md)
+ - [HybridTransaction](docs/HybridTransaction.md)
+ - [HybridTransactionAllOf](docs/HybridTransactionAllOf.md)
+ - [HybridTransactionsResponse](docs/HybridTransactionsResponse.md)
+ - [HybridTransactionsResponseData](docs/HybridTransactionsResponseData.md)
+ - [MonthDetail](docs/MonthDetail.md)
+ - [MonthDetailAllOf](docs/MonthDetailAllOf.md)
+ - [MonthDetailResponse](docs/MonthDetailResponse.md)
+ - [MonthDetailResponseData](docs/MonthDetailResponseData.md)
+ - [MonthSummariesResponse](docs/MonthSummariesResponse.md)
+ - [MonthSummariesResponseData](docs/MonthSummariesResponseData.md)
+ - [MonthSummary](docs/MonthSummary.md)
+ - [Payee](docs/Payee.md)
+ - [PayeeLocation](docs/PayeeLocation.md)
+ - [PayeeLocationResponse](docs/PayeeLocationResponse.md)
+ - [PayeeLocationResponseData](docs/PayeeLocationResponseData.md)
+ - [PayeeLocationsResponse](docs/PayeeLocationsResponse.md)
+ - [PayeeLocationsResponseData](docs/PayeeLocationsResponseData.md)
+ - [PayeeResponse](docs/PayeeResponse.md)
+ - [PayeeResponseData](docs/PayeeResponseData.md)
+ - [PayeesResponse](docs/PayeesResponse.md)
+ - [PayeesResponseData](docs/PayeesResponseData.md)
+ - [SaveAccount](docs/SaveAccount.md)
+ - [SaveAccountWrapper](docs/SaveAccountWrapper.md)
+ - [SaveCategoryResponse](docs/SaveCategoryResponse.md)
+ - [SaveCategoryResponseData](docs/SaveCategoryResponseData.md)
+ - [SaveMonthCategory](docs/SaveMonthCategory.md)
+ - [SaveMonthCategoryWrapper](docs/SaveMonthCategoryWrapper.md)
+ - [SaveSubTransaction](docs/SaveSubTransaction.md)
+ - [SaveTransaction](docs/SaveTransaction.md)
+ - [SaveTransactionWrapper](docs/SaveTransactionWrapper.md)
+ - [SaveTransactionsResponse](docs/SaveTransactionsResponse.md)
+ - [SaveTransactionsResponseData](docs/SaveTransactionsResponseData.md)
+ - [SaveTransactionsWrapper](docs/SaveTransactionsWrapper.md)
+ - [ScheduledSubTransaction](docs/ScheduledSubTransaction.md)
+ - [ScheduledTransactionDetail](docs/ScheduledTransactionDetail.md)
+ - [ScheduledTransactionDetailAllOf](docs/ScheduledTransactionDetailAllOf.md)
+ - [ScheduledTransactionResponse](docs/ScheduledTransactionResponse.md)
+ - [ScheduledTransactionResponseData](docs/ScheduledTransactionResponseData.md)
+ - [ScheduledTransactionSummary](docs/ScheduledTransactionSummary.md)
+ - [ScheduledTransactionsResponse](docs/ScheduledTransactionsResponse.md)
+ - [ScheduledTransactionsResponseData](docs/ScheduledTransactionsResponseData.md)
+ - [SubTransaction](docs/SubTransaction.md)
+ - [TransactionDetail](docs/TransactionDetail.md)
+ - [TransactionDetailAllOf](docs/TransactionDetailAllOf.md)
+ - [TransactionResponse](docs/TransactionResponse.md)
+ - [TransactionResponseData](docs/TransactionResponseData.md)
+ - [TransactionSummary](docs/TransactionSummary.md)
+ - [TransactionsImportResponse](docs/TransactionsImportResponse.md)
+ - [TransactionsImportResponseData](docs/TransactionsImportResponseData.md)
+ - [TransactionsResponse](docs/TransactionsResponse.md)
+ - [TransactionsResponseData](docs/TransactionsResponseData.md)
+ - [UpdateTransaction](docs/UpdateTransaction.md)
+ - [UpdateTransactionAllOf](docs/UpdateTransactionAllOf.md)
+ - [UpdateTransactionsWrapper](docs/UpdateTransactionsWrapper.md)
+ - [User](docs/User.md)
+ - [UserResponse](docs/UserResponse.md)
+ - [UserResponseData](docs/UserResponseData.md)
+
 
 ## Documentation For Authorization
 
+
 ## bearer
 
 - **Type**: API key
 - **API key parameter name**: Authorization
 - **Location**: HTTP header
 
+
 ## Author
 
-David Lerner
 
-## Notes for Large OpenAPI documents
 
+
+## Notes for Large OpenAPI documents
 If the OpenAPI document is large, imports in ynab_api.apis and ynab_api.models may fail with a
 RecursionError indicating the maximum recursion limit has been exceeded. In that case, there are a couple of solutions:
 
 Solution 1:
 Use specific imports for apis and models like:
-
 - `from ynab_api.api.default_api import DefaultApi`
 - `from ynab_api.model.pet import Pet`
 
 Solution 2:
 Before importing the package, adjust the maximum recursion limit as shown below:
-
 ```
 import sys
 sys.setrecursionlimit(1500)
 import ynab_api
 from ynab_api.apis import *
 from ynab_api.models import *
 ```
+
```

### Comparing `ynab-api-2.0.0/setup.py` & `ynab-api-2.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 2.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "ynab-api"
-VERSION = "2.0.0"
+VERSION = "2.0.2"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -22,16 +22,16 @@
     "urllib3 >= 1.25.3",
     "python-dateutil",
 ]
 
 setup(name=NAME,
       version=VERSION,
       description="YNAB API Endpoints",
-      author="David Lerner",
-      author_email="dmlerner@gmail.com",
+      author="OpenAPI Generator community",
+      author_email="team@openapitools.org",
       url="",
       keywords=["OpenAPI", "OpenAPI-Generator", "YNAB API Endpoints"],
       python_requires=">=3.6",
       install_requires=REQUIRES,
       packages=find_packages(exclude=["test", "tests"]),
       include_package_data=True,
       long_description="""\
```

### Comparing `ynab-api-2.0.0/test/test_account.py` & `ynab-api-2.0.2/test/test_account.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_account_response.py` & `ynab-api-2.0.2/test/test_account_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_account_response_data.py` & `ynab-api-2.0.2/test/test_account_response_data.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_accounts_api.py` & `ynab-api-2.0.2/test/test_accounts_api.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_accounts_response.py` & `ynab-api-2.0.2/test/test_accounts_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_accounts_response_data.py` & `ynab-api-2.0.2/test/test_accounts_response_data.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_budget_detail.py` & `ynab-api-2.0.2/test/test_budget_detail.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_budget_detail_all_of.py` & `ynab-api-2.0.2/test/test_budget_detail_all_of.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_budget_detail_response.py` & `ynab-api-2.0.2/test/test_budget_detail_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_budget_detail_response_data.py` & `ynab-api-2.0.2/test/test_budget_detail_response_data.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_budget_settings.py` & `ynab-api-2.0.2/test/test_budget_settings.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_budget_settings_response.py` & `ynab-api-2.0.2/test/test_budget_settings_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_budget_settings_response_data.py` & `ynab-api-2.0.2/test/test_budget_settings_response_data.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_budget_summary.py` & `ynab-api-2.0.2/test/test_budget_summary.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_budget_summary_response.py` & `ynab-api-2.0.2/test/test_budget_summary_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_budget_summary_response_data.py` & `ynab-api-2.0.2/test/test_budget_summary_response_data.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_budgets_api.py` & `ynab-api-2.0.2/test/test_budgets_api.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_bulk_response.py` & `ynab-api-2.0.2/test/test_bulk_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_bulk_response_data.py` & `ynab-api-2.0.2/test/test_bulk_response_data.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_bulk_response_data_bulk.py` & `ynab-api-2.0.2/test/test_bulk_response_data_bulk.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_bulk_transactions.py` & `ynab-api-2.0.2/test/test_bulk_transactions.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_categories_api.py` & `ynab-api-2.0.2/test/test_categories_api.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_categories_response.py` & `ynab-api-2.0.2/test/test_categories_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_categories_response_data.py` & `ynab-api-2.0.2/test/test_categories_response_data.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_category.py` & `ynab-api-2.0.2/test/test_category.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_category_group.py` & `ynab-api-2.0.2/test/test_category_group.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_category_group_with_categories.py` & `ynab-api-2.0.2/test/test_category_group_with_categories.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_category_group_with_categories_all_of.py` & `ynab-api-2.0.2/test/test_category_group_with_categories_all_of.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_category_response.py` & `ynab-api-2.0.2/test/test_category_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_category_response_data.py` & `ynab-api-2.0.2/test/test_category_response_data.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_currency_format.py` & `ynab-api-2.0.2/test/test_currency_format.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_date_format.py` & `ynab-api-2.0.2/test/test_date_format.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_deprecated_api.py` & `ynab-api-2.0.2/test/test_deprecated_api.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_error_detail.py` & `ynab-api-2.0.2/test/test_error_detail.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_error_response.py` & `ynab-api-2.0.2/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_hybrid_transaction.py` & `ynab-api-2.0.2/test/test_hybrid_transaction.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_hybrid_transaction_all_of.py` & `ynab-api-2.0.2/test/test_hybrid_transaction_all_of.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_hybrid_transactions_response.py` & `ynab-api-2.0.2/test/test_hybrid_transactions_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_hybrid_transactions_response_data.py` & `ynab-api-2.0.2/test/test_hybrid_transactions_response_data.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_month_detail.py` & `ynab-api-2.0.2/test/test_month_detail.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_month_detail_all_of.py` & `ynab-api-2.0.2/test/test_month_detail_all_of.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_month_detail_response.py` & `ynab-api-2.0.2/test/test_month_detail_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_month_detail_response_data.py` & `ynab-api-2.0.2/test/test_month_detail_response_data.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_month_summaries_response.py` & `ynab-api-2.0.2/test/test_month_summaries_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_month_summaries_response_data.py` & `ynab-api-2.0.2/test/test_month_summaries_response_data.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_month_summary.py` & `ynab-api-2.0.2/test/test_month_summary.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_months_api.py` & `ynab-api-2.0.2/test/test_months_api.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_payee.py` & `ynab-api-2.0.2/test/test_payee.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_payee_location.py` & `ynab-api-2.0.2/test/test_payee_location.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_payee_location_response.py` & `ynab-api-2.0.2/test/test_payee_location_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_payee_location_response_data.py` & `ynab-api-2.0.2/test/test_payee_location_response_data.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_payee_locations_api.py` & `ynab-api-2.0.2/test/test_payee_locations_api.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_payee_locations_response.py` & `ynab-api-2.0.2/test/test_payee_locations_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_payee_locations_response_data.py` & `ynab-api-2.0.2/test/test_payee_locations_response_data.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_payee_response.py` & `ynab-api-2.0.2/test/test_payee_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_payee_response_data.py` & `ynab-api-2.0.2/test/test_payee_response_data.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_payees_api.py` & `ynab-api-2.0.2/test/test_payees_api.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_payees_response.py` & `ynab-api-2.0.2/test/test_payees_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_payees_response_data.py` & `ynab-api-2.0.2/test/test_payees_response_data.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_save_account.py` & `ynab-api-2.0.2/test/test_save_account.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_save_account_wrapper.py` & `ynab-api-2.0.2/test/test_save_account_wrapper.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_save_category_response.py` & `ynab-api-2.0.2/test/test_save_category_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_save_category_response_data.py` & `ynab-api-2.0.2/test/test_save_category_response_data.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_save_month_category.py` & `ynab-api-2.0.2/test/test_save_month_category.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_save_month_category_wrapper.py` & `ynab-api-2.0.2/test/test_save_month_category_wrapper.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_save_sub_transaction.py` & `ynab-api-2.0.2/test/test_save_sub_transaction.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_save_transaction.py` & `ynab-api-2.0.2/test/test_save_transaction.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_save_transaction_wrapper.py` & `ynab-api-2.0.2/test/test_save_transaction_wrapper.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_save_transactions_response.py` & `ynab-api-2.0.2/test/test_save_transactions_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_save_transactions_response_data.py` & `ynab-api-2.0.2/test/test_save_transactions_response_data.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_save_transactions_wrapper.py` & `ynab-api-2.0.2/test/test_save_transactions_wrapper.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_scheduled_sub_transaction.py` & `ynab-api-2.0.2/test/test_scheduled_sub_transaction.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_scheduled_transaction_detail.py` & `ynab-api-2.0.2/test/test_scheduled_transaction_detail.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_scheduled_transaction_detail_all_of.py` & `ynab-api-2.0.2/test/test_scheduled_transaction_detail_all_of.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_scheduled_transaction_response.py` & `ynab-api-2.0.2/test/test_scheduled_transaction_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_scheduled_transaction_response_data.py` & `ynab-api-2.0.2/test/test_scheduled_transaction_response_data.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_scheduled_transaction_summary.py` & `ynab-api-2.0.2/test/test_scheduled_transaction_summary.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_scheduled_transactions_api.py` & `ynab-api-2.0.2/test/test_scheduled_transactions_api.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_scheduled_transactions_response.py` & `ynab-api-2.0.2/test/test_scheduled_transactions_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_scheduled_transactions_response_data.py` & `ynab-api-2.0.2/test/test_scheduled_transactions_response_data.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_sub_transaction.py` & `ynab-api-2.0.2/test/test_sub_transaction.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_transaction_detail.py` & `ynab-api-2.0.2/test/test_transaction_detail.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_transaction_detail_all_of.py` & `ynab-api-2.0.2/test/test_transaction_detail_all_of.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_transaction_response.py` & `ynab-api-2.0.2/test/test_transaction_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_transaction_response_data.py` & `ynab-api-2.0.2/test/test_transaction_response_data.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_transaction_summary.py` & `ynab-api-2.0.2/test/test_transaction_summary.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_transactions_api.py` & `ynab-api-2.0.2/test/test_transactions_api.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_transactions_import_response.py` & `ynab-api-2.0.2/test/test_transactions_import_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_transactions_import_response_data.py` & `ynab-api-2.0.2/test/test_transactions_import_response_data.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_transactions_response.py` & `ynab-api-2.0.2/test/test_transactions_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_transactions_response_data.py` & `ynab-api-2.0.2/test/test_transactions_response_data.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_update_transaction.py` & `ynab-api-2.0.2/test/test_update_transaction.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_update_transaction_all_of.py` & `ynab-api-2.0.2/test/test_update_transaction_all_of.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_update_transactions_wrapper.py` & `ynab-api-2.0.2/test/test_update_transactions_wrapper.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_user.py` & `ynab-api-2.0.2/test/test_user.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_user_api.py` & `ynab-api-2.0.2/test/test_user_api.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_user_response.py` & `ynab-api-2.0.2/test/test_user_response.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/test/test_user_response_data.py` & `ynab-api-2.0.2/test/test_user_response_data.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/ynab_api/__init__.py` & `ynab-api-2.0.2/ynab_api/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # flake8: noqa
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 __version__ = "1.0.0"
 
 # import ApiClient
 from ynab_api.api_client import ApiClient
```

### Comparing `ynab-api-2.0.0/ynab_api/api/accounts_api.py` & `ynab-api-2.0.2/ynab_api/api/accounts_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.api_client import ApiClient, Endpoint as _Endpoint
@@ -44,23 +44,28 @@
                     'budget_id',
                     'data',
                 ],
                 'required': [
                     'budget_id',
                     'data',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                ],
                 'enum': [],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {},
                 'openapi_types': {
-                    'budget_id': (str, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
                     'data': (SaveAccountWrapper, ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                 },
                 'location_map': {
                     'budget_id': 'path',
@@ -87,24 +92,33 @@
                     'budget_id',
                     'account_id',
                 ],
                 'required': [
                     'budget_id',
                     'account_id',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                    'account_id',
+                ],
                 'enum': [],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {},
                 'openapi_types': {
-                    'budget_id': (str, ),
-                    'account_id': (str, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
+                    'account_id': (
+                        str,
+                        none_type,
+                    ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                     'account_id': 'account_id',
                 },
                 'location_map': {
                     'budget_id': 'path',
@@ -130,24 +144,33 @@
                 'all': [
                     'budget_id',
                     'last_knowledge_of_server',
                 ],
                 'required': [
                     'budget_id',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                    'last_knowledge_of_server',
+                ],
                 'enum': [],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {},
                 'openapi_types': {
-                    'budget_id': (str, ),
-                    'last_knowledge_of_server': (int, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
+                    'last_knowledge_of_server': (
+                        int,
+                        none_type,
+                    ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                     'last_knowledge_of_server': 'last_knowledge_of_server',
                 },
                 'location_map': {
                     'budget_id': 'path',
@@ -168,15 +191,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_account(budget_id, data, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget)
+            budget_id (str, none_type): The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget)
             data (SaveAccountWrapper): The account to create.
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -222,16 +245,16 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_account_by_id(budget_id, account_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
-            account_id (str): The id of the account
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            account_id (str, none_type): The id of the account
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -276,18 +299,18 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_accounts(budget_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
 
         Keyword Args:
-            last_knowledge_of_server (int): The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.. [optional]
+            last_knowledge_of_server (int, none_type): The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `ynab-api-2.0.0/ynab_api/api/budgets_api.py` & `ynab-api-2.0.2/ynab_api/api/budgets_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.api_client import ApiClient, Endpoint as _Endpoint
@@ -43,23 +43,28 @@
                 'all': [
                     'budget_id',
                     'last_knowledge_of_server',
                 ],
                 'required': [
                     'budget_id',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                ],
                 'enum': [],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {},
                 'openapi_types': {
-                    'budget_id': (str, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
                     'last_knowledge_of_server': (int, ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                     'last_knowledge_of_server': 'last_knowledge_of_server',
                 },
                 'location_map': {
@@ -85,23 +90,28 @@
             params_map={
                 'all': [
                     'budget_id',
                 ],
                 'required': [
                     'budget_id',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                ],
                 'enum': [],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {},
                 'openapi_types': {
-                    'budget_id': (str, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                 },
                 'location_map': {
                     'budget_id': 'path',
                 },
@@ -164,15 +174,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_budget_by_id(budget_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
 
         Keyword Args:
             last_knowledge_of_server (int): The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -216,15 +226,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_budget_settings_by_id(budget_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
```

### Comparing `ynab-api-2.0.0/ynab_api/api/categories_api.py` & `ynab-api-2.0.2/ynab_api/api/categories_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.api_client import ApiClient, Endpoint as _Endpoint
@@ -44,24 +44,33 @@
                 'all': [
                     'budget_id',
                     'last_knowledge_of_server',
                 ],
                 'required': [
                     'budget_id',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                    'last_knowledge_of_server',
+                ],
                 'enum': [],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {},
                 'openapi_types': {
-                    'budget_id': (str, ),
-                    'last_knowledge_of_server': (int, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
+                    'last_knowledge_of_server': (
+                        int,
+                        none_type,
+                    ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                     'last_knowledge_of_server': 'last_knowledge_of_server',
                 },
                 'location_map': {
                     'budget_id': 'path',
@@ -89,24 +98,33 @@
                     'budget_id',
                     'category_id',
                 ],
                 'required': [
                     'budget_id',
                     'category_id',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                    'category_id',
+                ],
                 'enum': [],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {},
                 'openapi_types': {
-                    'budget_id': (str, ),
-                    'category_id': (str, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
+                    'category_id': (
+                        str,
+                        none_type,
+                    ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                     'category_id': 'category_id',
                 },
                 'location_map': {
                     'budget_id': 'path',
@@ -136,25 +154,38 @@
                     'category_id',
                 ],
                 'required': [
                     'budget_id',
                     'month',
                     'category_id',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                    'month',
+                    'category_id',
+                ],
                 'enum': [],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {},
                 'openapi_types': {
-                    'budget_id': (str, ),
-                    'month': (date, ),
-                    'category_id': (str, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
+                    'month': (
+                        date,
+                        none_type,
+                    ),
+                    'category_id': (
+                        str,
+                        none_type,
+                    ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                     'month': 'month',
                     'category_id': 'category_id',
                 },
                 'location_map': {
@@ -188,25 +219,38 @@
                 ],
                 'required': [
                     'budget_id',
                     'month',
                     'category_id',
                     'data',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                    'month',
+                    'category_id',
+                ],
                 'enum': [],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {},
                 'openapi_types': {
-                    'budget_id': (str, ),
-                    'month': (date, ),
-                    'category_id': (str, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
+                    'month': (
+                        date,
+                        none_type,
+                    ),
+                    'category_id': (
+                        str,
+                        none_type,
+                    ),
                     'data': (SaveMonthCategoryWrapper, ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                     'month': 'month',
                     'category_id': 'category_id',
                 },
@@ -231,18 +275,18 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_categories(budget_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
 
         Keyword Args:
-            last_knowledge_of_server (int): The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.. [optional]
+            last_knowledge_of_server (int, none_type): The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -283,16 +327,16 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_category_by_id(budget_id, category_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
-            category_id (str): The id of the category
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            category_id (str, none_type): The id of the category
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -338,17 +382,17 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_month_category_by_id(budget_id, month, category_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
-            month (date): The budget month in ISO format (e.g. 2016-12-01) (\"current\" can also be used to specify the current calendar month (UTC))
-            category_id (str): The id of the category
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            month (date, none_type): The budget month in ISO format (e.g. 2016-12-01) (\"current\" can also be used to specify the current calendar month (UTC))
+            category_id (str, none_type): The id of the category
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -397,17 +441,17 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_month_category(budget_id, month, category_id, data, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
-            month (date): The budget month in ISO format (e.g. 2016-12-01) (\"current\" can also be used to specify the current calendar month (UTC))
-            category_id (str): The id of the category
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            month (date, none_type): The budget month in ISO format (e.g. 2016-12-01) (\"current\" can also be used to specify the current calendar month (UTC))
+            category_id (str, none_type): The id of the category
             data (SaveMonthCategoryWrapper): The category to update.  Only `budgeted` amount can be updated and any other fields specified will be ignored.
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
```

### Comparing `ynab-api-2.0.0/ynab_api/api/deprecated_api.py` & `ynab-api-2.0.2/ynab_api/api/deprecated_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.api_client import ApiClient, Endpoint as _Endpoint
@@ -43,23 +43,28 @@
                     'budget_id',
                     'transactions',
                 ],
                 'required': [
                     'budget_id',
                     'transactions',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                ],
                 'enum': [],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {},
                 'openapi_types': {
-                    'budget_id': (str, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
                     'transactions': (BulkTransactions, ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                 },
                 'location_map': {
                     'budget_id': 'path',
@@ -80,15 +85,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.bulk_create_transactions(budget_id, transactions, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
             transactions (BulkTransactions): The list of transactions to create
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
```

### Comparing `ynab-api-2.0.0/ynab_api/api/months_api.py` & `ynab-api-2.0.2/ynab_api/api/months_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.api_client import ApiClient, Endpoint as _Endpoint
@@ -46,25 +46,33 @@
                                                            'budget_id',
                                                            'month',
                                                        ],
                                                        'required': [
                                                            'budget_id',
                                                            'month',
                                                        ],
-                                                       'nullable': [],
+                                                       'nullable': [
+                                                           'budget_id',
+                                                           'month',
+                                                       ],
                                                        'enum': [],
                                                        'validation': []
                                                    },
                                                    root_map={
                                                        'validations': {},
                                                        'allowed_values': {},
                                                        'openapi_types': {
-                                                           'budget_id':
-                                                           (str, ),
-                                                           'month': (date, ),
+                                                           'budget_id': (
+                                                               str,
+                                                               none_type,
+                                                           ),
+                                                           'month': (
+                                                               date,
+                                                               none_type,
+                                                           ),
                                                        },
                                                        'attribute_map': {
                                                            'budget_id':
                                                            'budget_id',
                                                            'month': 'month',
                                                        },
                                                        'location_map': {
@@ -93,24 +101,33 @@
                 'all': [
                     'budget_id',
                     'last_knowledge_of_server',
                 ],
                 'required': [
                     'budget_id',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                    'last_knowledge_of_server',
+                ],
                 'enum': [],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {},
                 'openapi_types': {
-                    'budget_id': (str, ),
-                    'last_knowledge_of_server': (int, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
+                    'last_knowledge_of_server': (
+                        int,
+                        none_type,
+                    ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                     'last_knowledge_of_server': 'last_knowledge_of_server',
                 },
                 'location_map': {
                     'budget_id': 'path',
@@ -131,16 +148,16 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_budget_month(budget_id, month, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
-            month (date): The budget month in ISO format (e.g. 2016-12-01) (\"current\" can also be used to specify the current calendar month (UTC))
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            month (date, none_type): The budget month in ISO format (e.g. 2016-12-01) (\"current\" can also be used to specify the current calendar month (UTC))
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -185,18 +202,18 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_budget_months(budget_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
 
         Keyword Args:
-            last_knowledge_of_server (int): The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.. [optional]
+            last_knowledge_of_server (int, none_type): The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `ynab-api-2.0.0/ynab_api/api/payee_locations_api.py` & `ynab-api-2.0.2/ynab_api/api/payee_locations_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.api_client import ApiClient, Endpoint as _Endpoint
@@ -44,24 +44,33 @@
                     'budget_id',
                     'payee_location_id',
                 ],
                 'required': [
                     'budget_id',
                     'payee_location_id',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                    'payee_location_id',
+                ],
                 'enum': [],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {},
                 'openapi_types': {
-                    'budget_id': (str, ),
-                    'payee_location_id': (str, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
+                    'payee_location_id': (
+                        str,
+                        none_type,
+                    ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                     'payee_location_id': 'payee_location_id',
                 },
                 'location_map': {
                     'budget_id': 'path',
@@ -86,23 +95,28 @@
             params_map={
                 'all': [
                     'budget_id',
                 ],
                 'required': [
                     'budget_id',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                ],
                 'enum': [],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {},
                 'openapi_types': {
-                    'budget_id': (str, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                 },
                 'location_map': {
                     'budget_id': 'path',
                 },
@@ -128,24 +142,33 @@
                     'budget_id',
                     'payee_id',
                 ],
                 'required': [
                     'budget_id',
                     'payee_id',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                    'payee_id',
+                ],
                 'enum': [],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {},
                 'openapi_types': {
-                    'budget_id': (str, ),
-                    'payee_id': (str, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
+                    'payee_id': (
+                        str,
+                        none_type,
+                    ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                     'payee_id': 'payee_id',
                 },
                 'location_map': {
                     'budget_id': 'path',
@@ -166,16 +189,16 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_payee_location_by_id(budget_id, payee_location_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
-            payee_location_id (str): id of payee location
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            payee_location_id (str, none_type): id of payee location
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -221,15 +244,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_payee_locations(budget_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -272,16 +295,16 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_payee_locations_by_payee(budget_id, payee_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
-            payee_id (str): id of payee
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            payee_id (str, none_type): id of payee
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
```

### Comparing `ynab-api-2.0.0/ynab_api/api/payees_api.py` & `ynab-api-2.0.2/ynab_api/api/payees_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.api_client import ApiClient, Endpoint as _Endpoint
@@ -46,24 +46,33 @@
                                                           'budget_id',
                                                           'payee_id',
                                                       ],
                                                       'required': [
                                                           'budget_id',
                                                           'payee_id',
                                                       ],
-                                                      'nullable': [],
+                                                      'nullable': [
+                                                          'budget_id',
+                                                          'payee_id',
+                                                      ],
                                                       'enum': [],
                                                       'validation': []
                                                   },
                                                   root_map={
                                                       'validations': {},
                                                       'allowed_values': {},
                                                       'openapi_types': {
-                                                          'budget_id': (str, ),
-                                                          'payee_id': (str, ),
+                                                          'budget_id': (
+                                                              str,
+                                                              none_type,
+                                                          ),
+                                                          'payee_id': (
+                                                              str,
+                                                              none_type,
+                                                          ),
                                                       },
                                                       'attribute_map': {
                                                           'budget_id':
                                                           'budget_id',
                                                           'payee_id':
                                                           'payee_id',
                                                       },
@@ -93,24 +102,33 @@
                 'all': [
                     'budget_id',
                     'last_knowledge_of_server',
                 ],
                 'required': [
                     'budget_id',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                    'last_knowledge_of_server',
+                ],
                 'enum': [],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {},
                 'openapi_types': {
-                    'budget_id': (str, ),
-                    'last_knowledge_of_server': (int, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
+                    'last_knowledge_of_server': (
+                        int,
+                        none_type,
+                    ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                     'last_knowledge_of_server': 'last_knowledge_of_server',
                 },
                 'location_map': {
                     'budget_id': 'path',
@@ -131,16 +149,16 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_payee_by_id(budget_id, payee_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
-            payee_id (str): The id of the payee
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            payee_id (str, none_type): The id of the payee
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -185,18 +203,18 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_payees(budget_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
 
         Keyword Args:
-            last_knowledge_of_server (int): The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.. [optional]
+            last_knowledge_of_server (int, none_type): The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `ynab-api-2.0.0/ynab_api/api/scheduled_transactions_api.py` & `ynab-api-2.0.2/ynab_api/api/scheduled_transactions_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.api_client import ApiClient, Endpoint as _Endpoint
@@ -44,24 +44,33 @@
                     'budget_id',
                     'scheduled_transaction_id',
                 ],
                 'required': [
                     'budget_id',
                     'scheduled_transaction_id',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                    'scheduled_transaction_id',
+                ],
                 'enum': [],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {},
                 'openapi_types': {
-                    'budget_id': (str, ),
-                    'scheduled_transaction_id': (str, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
+                    'scheduled_transaction_id': (
+                        str,
+                        none_type,
+                    ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                     'scheduled_transaction_id': 'scheduled_transaction_id',
                 },
                 'location_map': {
                     'budget_id': 'path',
@@ -87,24 +96,33 @@
                 'all': [
                     'budget_id',
                     'last_knowledge_of_server',
                 ],
                 'required': [
                     'budget_id',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                    'last_knowledge_of_server',
+                ],
                 'enum': [],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {},
                 'openapi_types': {
-                    'budget_id': (str, ),
-                    'last_knowledge_of_server': (int, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
+                    'last_knowledge_of_server': (
+                        int,
+                        none_type,
+                    ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                     'last_knowledge_of_server': 'last_knowledge_of_server',
                 },
                 'location_map': {
                     'budget_id': 'path',
@@ -126,16 +144,16 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_scheduled_transaction_by_id(budget_id, scheduled_transaction_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
-            scheduled_transaction_id (str): The id of the scheduled transaction
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            scheduled_transaction_id (str, none_type): The id of the scheduled transaction
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -181,18 +199,18 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_scheduled_transactions(budget_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
 
         Keyword Args:
-            last_knowledge_of_server (int): The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.. [optional]
+            last_knowledge_of_server (int, none_type): The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `ynab-api-2.0.0/ynab_api/api/transactions_api.py` & `ynab-api-2.0.2/ynab_api/api/transactions_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.api_client import ApiClient, Endpoint as _Endpoint
@@ -49,23 +49,28 @@
                     'budget_id',
                     'data',
                 ],
                 'required': [
                     'budget_id',
                     'data',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                ],
                 'enum': [],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {},
                 'openapi_types': {
-                    'budget_id': (str, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
                     'data': (SaveTransactionsWrapper, ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                 },
                 'location_map': {
                     'budget_id': 'path',
@@ -93,24 +98,33 @@
                     'budget_id',
                     'transaction_id',
                 ],
                 'required': [
                     'budget_id',
                     'transaction_id',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                    'transaction_id',
+                ],
                 'enum': [],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {},
                 'openapi_types': {
-                    'budget_id': (str, ),
-                    'transaction_id': (str, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
+                    'transaction_id': (
+                        str,
+                        none_type,
+                    ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                     'transaction_id': 'transaction_id',
                 },
                 'location_map': {
                     'budget_id': 'path',
@@ -138,33 +152,51 @@
                     'since_date',
                     'type',
                     'last_knowledge_of_server',
                 ],
                 'required': [
                     'budget_id',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                    'since_date',
+                    'type',
+                    'last_knowledge_of_server',
+                ],
                 'enum': [
                     'type',
                 ],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {
                     ('type', ): {
+                        'None': None,
                         "UNCATEGORIZED": "uncategorized",
                         "UNAPPROVED": "unapproved"
                     },
                 },
                 'openapi_types': {
-                    'budget_id': (str, ),
-                    'since_date': (date, ),
-                    'type': (str, ),
-                    'last_knowledge_of_server': (int, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
+                    'since_date': (
+                        date,
+                        none_type,
+                    ),
+                    'type': (
+                        str,
+                        none_type,
+                    ),
+                    'last_knowledge_of_server': (
+                        int,
+                        none_type,
+                    ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                     'since_date': 'since_date',
                     'type': 'type',
                     'last_knowledge_of_server': 'last_knowledge_of_server',
                 },
@@ -199,34 +231,56 @@
                     'type',
                     'last_knowledge_of_server',
                 ],
                 'required': [
                     'budget_id',
                     'account_id',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                    'account_id',
+                    'since_date',
+                    'type',
+                    'last_knowledge_of_server',
+                ],
                 'enum': [
                     'type',
                 ],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {
                     ('type', ): {
+                        'None': None,
                         "UNCATEGORIZED": "uncategorized",
                         "UNAPPROVED": "unapproved"
                     },
                 },
                 'openapi_types': {
-                    'budget_id': (str, ),
-                    'account_id': (str, ),
-                    'since_date': (date, ),
-                    'type': (str, ),
-                    'last_knowledge_of_server': (int, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
+                    'account_id': (
+                        str,
+                        none_type,
+                    ),
+                    'since_date': (
+                        date,
+                        none_type,
+                    ),
+                    'type': (
+                        str,
+                        none_type,
+                    ),
+                    'last_knowledge_of_server': (
+                        int,
+                        none_type,
+                    ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                     'account_id': 'account_id',
                     'since_date': 'since_date',
                     'type': 'type',
                     'last_knowledge_of_server': 'last_knowledge_of_server',
@@ -263,34 +317,56 @@
                     'type',
                     'last_knowledge_of_server',
                 ],
                 'required': [
                     'budget_id',
                     'category_id',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                    'category_id',
+                    'since_date',
+                    'type',
+                    'last_knowledge_of_server',
+                ],
                 'enum': [
                     'type',
                 ],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {
                     ('type', ): {
+                        'None': None,
                         "UNCATEGORIZED": "uncategorized",
                         "UNAPPROVED": "unapproved"
                     },
                 },
                 'openapi_types': {
-                    'budget_id': (str, ),
-                    'category_id': (str, ),
-                    'since_date': (date, ),
-                    'type': (str, ),
-                    'last_knowledge_of_server': (int, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
+                    'category_id': (
+                        str,
+                        none_type,
+                    ),
+                    'since_date': (
+                        date,
+                        none_type,
+                    ),
+                    'type': (
+                        str,
+                        none_type,
+                    ),
+                    'last_knowledge_of_server': (
+                        int,
+                        none_type,
+                    ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                     'category_id': 'category_id',
                     'since_date': 'since_date',
                     'type': 'type',
                     'last_knowledge_of_server': 'last_knowledge_of_server',
@@ -327,34 +403,56 @@
                     'type',
                     'last_knowledge_of_server',
                 ],
                 'required': [
                     'budget_id',
                     'payee_id',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                    'payee_id',
+                    'since_date',
+                    'type',
+                    'last_knowledge_of_server',
+                ],
                 'enum': [
                     'type',
                 ],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {
                     ('type', ): {
+                        'None': None,
                         "UNCATEGORIZED": "uncategorized",
                         "UNAPPROVED": "unapproved"
                     },
                 },
                 'openapi_types': {
-                    'budget_id': (str, ),
-                    'payee_id': (str, ),
-                    'since_date': (date, ),
-                    'type': (str, ),
-                    'last_knowledge_of_server': (int, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
+                    'payee_id': (
+                        str,
+                        none_type,
+                    ),
+                    'since_date': (
+                        date,
+                        none_type,
+                    ),
+                    'type': (
+                        str,
+                        none_type,
+                    ),
+                    'last_knowledge_of_server': (
+                        int,
+                        none_type,
+                    ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                     'payee_id': 'payee_id',
                     'since_date': 'since_date',
                     'type': 'type',
                     'last_knowledge_of_server': 'last_knowledge_of_server',
@@ -385,23 +483,28 @@
             params_map={
                 'all': [
                     'budget_id',
                 ],
                 'required': [
                     'budget_id',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                ],
                 'enum': [],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {},
                 'openapi_types': {
-                    'budget_id': (str, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                 },
                 'location_map': {
                     'budget_id': 'path',
                 },
@@ -429,23 +532,28 @@
                     'data',
                 ],
                 'required': [
                     'budget_id',
                     'transaction_id',
                     'data',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                ],
                 'enum': [],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {},
                 'openapi_types': {
-                    'budget_id': (str, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
                     'transaction_id': (str, ),
                     'data': (SaveTransactionWrapper, ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                     'transaction_id': 'transaction_id',
                 },
@@ -475,23 +583,28 @@
                     'budget_id',
                     'data',
                 ],
                 'required': [
                     'budget_id',
                     'data',
                 ],
-                'nullable': [],
+                'nullable': [
+                    'budget_id',
+                ],
                 'enum': [],
                 'validation': []
             },
             root_map={
                 'validations': {},
                 'allowed_values': {},
                 'openapi_types': {
-                    'budget_id': (str, ),
+                    'budget_id': (
+                        str,
+                        none_type,
+                    ),
                     'data': (UpdateTransactionsWrapper, ),
                 },
                 'attribute_map': {
                     'budget_id': 'budget_id',
                 },
                 'location_map': {
                     'budget_id': 'path',
@@ -512,15 +625,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_transaction(budget_id, data, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
             data (SaveTransactionsWrapper): The transaction or transactions to create.  To create a single transaction you can specify a value for the `transaction` object and to create multiple transactions you can specify an array of `transactions`.  It is expected that you will only provide a value for one of these objects.
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -566,16 +679,16 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_transaction_by_id(budget_id, transaction_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
-            transaction_id (str): The id of the transaction
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            transaction_id (str, none_type): The id of the transaction
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -621,20 +734,20 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_transactions(budget_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
 
         Keyword Args:
-            since_date (date): If specified, only transactions on or after this date will be included.  The date should be ISO formatted (e.g. 2016-12-30).. [optional]
-            type (str): If specified, only transactions of the specified type will be included. \"uncategorized\" and \"unapproved\" are currently supported.. [optional]
-            last_knowledge_of_server (int): The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.. [optional]
+            since_date (date, none_type): If specified, only transactions on or after this date will be included.  The date should be ISO formatted (e.g. 2016-12-30).. [optional]
+            type (str, none_type): If specified, only transactions of the specified type will be included. \"uncategorized\" and \"unapproved\" are currently supported.. [optional]
+            last_knowledge_of_server (int, none_type): The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -675,21 +788,21 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_transactions_by_account(budget_id, account_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
-            account_id (str): The id of the account
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            account_id (str, none_type): The id of the account
 
         Keyword Args:
-            since_date (date): If specified, only transactions on or after this date will be included.  The date should be ISO formatted (e.g. 2016-12-30).. [optional]
-            type (str): If specified, only transactions of the specified type will be included. \"uncategorized\" and \"unapproved\" are currently supported.. [optional]
-            last_knowledge_of_server (int): The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.. [optional]
+            since_date (date, none_type): If specified, only transactions on or after this date will be included.  The date should be ISO formatted (e.g. 2016-12-30).. [optional]
+            type (str, none_type): If specified, only transactions of the specified type will be included. \"uncategorized\" and \"unapproved\" are currently supported.. [optional]
+            last_knowledge_of_server (int, none_type): The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -733,21 +846,21 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_transactions_by_category(budget_id, category_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
-            category_id (str): The id of the category
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            category_id (str, none_type): The id of the category
 
         Keyword Args:
-            since_date (date): If specified, only transactions on or after this date will be included.  The date should be ISO formatted (e.g. 2016-12-30).. [optional]
-            type (str): If specified, only transactions of the specified type will be included. \"uncategorized\" and \"unapproved\" are currently supported.. [optional]
-            last_knowledge_of_server (int): The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.. [optional]
+            since_date (date, none_type): If specified, only transactions on or after this date will be included.  The date should be ISO formatted (e.g. 2016-12-30).. [optional]
+            type (str, none_type): If specified, only transactions of the specified type will be included. \"uncategorized\" and \"unapproved\" are currently supported.. [optional]
+            last_knowledge_of_server (int, none_type): The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -791,21 +904,21 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_transactions_by_payee(budget_id, payee_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
-            payee_id (str): The id of the payee
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            payee_id (str, none_type): The id of the payee
 
         Keyword Args:
-            since_date (date): If specified, only transactions on or after this date will be included.  The date should be ISO formatted (e.g. 2016-12-30).. [optional]
-            type (str): If specified, only transactions of the specified type will be included. \"uncategorized\" and \"unapproved\" are currently supported.. [optional]
-            last_knowledge_of_server (int): The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.. [optional]
+            since_date (date, none_type): If specified, only transactions on or after this date will be included.  The date should be ISO formatted (e.g. 2016-12-30).. [optional]
+            type (str, none_type): If specified, only transactions of the specified type will be included. \"uncategorized\" and \"unapproved\" are currently supported.. [optional]
+            last_knowledge_of_server (int, none_type): The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -849,15 +962,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.import_transactions(budget_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -900,15 +1013,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_transaction(budget_id, transaction_id, data, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
             transaction_id (str): The id of the transaction
             data (SaveTransactionWrapper): The transaction to update
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -957,15 +1070,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_transactions(budget_id, data, async_req=True)
         >>> result = thread.get()
 
         Args:
-            budget_id (str): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
+            budget_id (str, none_type): The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget).
             data (UpdateTransactionsWrapper): The transactions to update. Each transaction must have either an `id` or `import_id` specified. If `id` is specified as null an `import_id` value can be provided which will allow transaction(s) to be updated by their `import_id`. If an `id` is specified, it will always be used for lookup.
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
```

### Comparing `ynab-api-2.0.0/ynab_api/api/user_api.py` & `ynab-api-2.0.2/ynab_api/api/user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.api_client import ApiClient, Endpoint as _Endpoint
```

### Comparing `ynab-api-2.0.0/ynab_api/api_client.py` & `ynab-api-2.0.2/ynab_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import json
 import atexit
 import mimetypes
 from multiprocessing.pool import ThreadPool
```

### Comparing `ynab-api-2.0.0/ynab_api/apis/__init__.py` & `ynab-api-2.0.2/ynab_api/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/ynab_api/configuration.py` & `ynab-api-2.0.2/ynab_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import copy
 import logging
 import multiprocessing
 import sys
@@ -403,15 +403,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0.0\n"\
+               "Version of the API: 2.0.3\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `ynab-api-2.0.0/ynab_api/exceptions.py` & `ynab-api-2.0.2/ynab_api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `ynab-api-2.0.0/ynab_api/model/account.py` & `ynab-api-2.0.2/ynab_api/model/account.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -41,14 +41,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('type', ): {
+            'None': None,
             'CHECKING': "checking",
             'SAVINGS': "savings",
             'CASH': "cash",
             'CREDITCARD': "creditCard",
             'LINEOFCREDIT': "lineOfCredit",
             'OTHERASSET': "otherAsset",
             'OTHERLIABILITY': "otherLiability",
@@ -88,23 +89,44 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (str, ),  # noqa: E501
-            'name': (str, ),  # noqa: E501
-            'type': (str, ),  # noqa: E501
+            'id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'name': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'type': (
+                str,
+                none_type,
+            ),  # noqa: E501
             'on_budget': (bool, ),  # noqa: E501
             'closed': (bool, ),  # noqa: E501
-            'balance': (int, ),  # noqa: E501
-            'cleared_balance': (int, ),  # noqa: E501
-            'uncleared_balance': (int, ),  # noqa: E501
-            'transfer_payee_id': (str, ),  # noqa: E501
+            'balance': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'cleared_balance': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'uncleared_balance': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'transfer_payee_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
             'deleted': (bool, ),  # noqa: E501
             'note': (
                 str,
                 none_type,
             ),  # noqa: E501
             'direct_import_linked': (bool, ),  # noqa: E501
             'direct_import_in_error': (bool, ),  # noqa: E501
@@ -139,23 +161,23 @@
     def _from_openapi_data(cls, id, name, type, on_budget, closed, balance,
                            cleared_balance, uncleared_balance,
                            transfer_payee_id, deleted, *args,
                            **kwargs):  # noqa: E501
         """Account - a model defined in OpenAPI
 
         Args:
-            id (str):
-            name (str):
-            type (str): The type of account. Note: payPal, merchantAccount, investmentAccount, and mortgage types have been deprecated and will be removed in the future.
+            id (str, none_type):
+            name (str, none_type):
+            type (str, none_type): The type of account. Note: payPal, merchantAccount, investmentAccount, and mortgage types have been deprecated and will be removed in the future.
             on_budget (bool): Whether this account is on budget or not
             closed (bool): Whether this account is closed or not
-            balance (int): The current balance of the account in milliunits format
-            cleared_balance (int): The current cleared balance of the account in milliunits format
-            uncleared_balance (int): The current uncleared balance of the account in milliunits format
-            transfer_payee_id (str): The payee id which should be used when transferring to this account
+            balance (int, none_type): The current balance of the account in milliunits format
+            cleared_balance (int, none_type): The current cleared balance of the account in milliunits format
+            uncleared_balance (int, none_type): The current uncleared balance of the account in milliunits format
+            transfer_payee_id (str, none_type): The payee id which should be used when transferring to this account
             deleted (bool): Whether or not the account has been deleted.  Deleted accounts will only be included in delta requests.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -249,23 +271,23 @@
     @convert_js_args_to_python_args
     def __init__(self, id, name, type, on_budget, closed, balance,
                  cleared_balance, uncleared_balance, transfer_payee_id,
                  deleted, *args, **kwargs):  # noqa: E501
         """Account - a model defined in OpenAPI
 
         Args:
-            id (str):
-            name (str):
-            type (str): The type of account. Note: payPal, merchantAccount, investmentAccount, and mortgage types have been deprecated and will be removed in the future.
+            id (str, none_type):
+            name (str, none_type):
+            type (str, none_type): The type of account. Note: payPal, merchantAccount, investmentAccount, and mortgage types have been deprecated and will be removed in the future.
             on_budget (bool): Whether this account is on budget or not
             closed (bool): Whether this account is closed or not
-            balance (int): The current balance of the account in milliunits format
-            cleared_balance (int): The current cleared balance of the account in milliunits format
-            uncleared_balance (int): The current uncleared balance of the account in milliunits format
-            transfer_payee_id (str): The payee id which should be used when transferring to this account
+            balance (int, none_type): The current balance of the account in milliunits format
+            cleared_balance (int, none_type): The current cleared balance of the account in milliunits format
+            uncleared_balance (int, none_type): The current uncleared balance of the account in milliunits format
+            transfer_payee_id (str, none_type): The payee id which should be used when transferring to this account
             deleted (bool): Whether or not the account has been deleted.  Deleted accounts will only be included in delta requests.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `ynab-api-2.0.0/ynab_api/model/account_response.py` & `ynab-api-2.0.2/ynab_api/model/account_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/account_response_data.py` & `ynab-api-2.0.2/ynab_api/model/account_response_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/accounts_response.py` & `ynab-api-2.0.2/ynab_api/model/accounts_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/accounts_response_data.py` & `ynab-api-2.0.2/ynab_api/model/accounts_response_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -82,15 +82,18 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'accounts': ([Account], ),  # noqa: E501
-            'server_knowledge': (int, ),  # noqa: E501
+            'server_knowledge': (
+                int,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -106,15 +109,15 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, accounts, server_knowledge, *args,
                            **kwargs):  # noqa: E501
         """AccountsResponseData - a model defined in OpenAPI
 
         Args:
             accounts ([Account]):
-            server_knowledge (int): The knowledge of the server
+            server_knowledge (int, none_type): The knowledge of the server
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -196,15 +199,15 @@
     @convert_js_args_to_python_args
     def __init__(self, accounts, server_knowledge, *args,
                  **kwargs):  # noqa: E501
         """AccountsResponseData - a model defined in OpenAPI
 
         Args:
             accounts ([Account]):
-            server_knowledge (int): The knowledge of the server
+            server_knowledge (int, none_type): The knowledge of the server
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `ynab-api-2.0.0/ynab_api/model/budget_detail.py` & `ynab-api-2.0.2/ynab_api/model/budget_detail.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -107,19 +107,34 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'id': (str, ),  # noqa: E501
-            'name': (str, ),  # noqa: E501
-            'last_modified_on': (datetime, ),  # noqa: E501
-            'first_month': (date, ),  # noqa: E501
-            'last_month': (date, ),  # noqa: E501
+            'id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'name': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'last_modified_on': (
+                datetime,
+                none_type,
+            ),  # noqa: E501
+            'first_month': (
+                date,
+                none_type,
+            ),  # noqa: E501
+            'last_month': (
+                date,
+                none_type,
+            ),  # noqa: E501
             'date_format': (DateFormat, ),  # noqa: E501
             'currency_format': (CurrencyFormat, ),  # noqa: E501
             'accounts': ([Account], ),  # noqa: E501
             'payees': ([Payee], ),  # noqa: E501
             'payee_locations': ([PayeeLocation], ),  # noqa: E501
             'category_groups': ([CategoryGroup], ),  # noqa: E501
             'categories': ([Category], ),  # noqa: E501
@@ -160,16 +175,16 @@
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """BudgetDetail - a model defined in OpenAPI
 
         Keyword Args:
-            id (str):
-            name (str):
+            id (str, none_type):
+            name (str, none_type):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -192,17 +207,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            last_modified_on (datetime): The last time any changes were made to the budget from either a web or mobile client. [optional]  # noqa: E501
-            first_month (date): The earliest budget month. [optional]  # noqa: E501
-            last_month (date): The latest budget month. [optional]  # noqa: E501
+            last_modified_on (datetime, none_type): The last time any changes were made to the budget from either a web or mobile client. [optional]  # noqa: E501
+            first_month (date, none_type): The earliest budget month. [optional]  # noqa: E501
+            last_month (date, none_type): The latest budget month. [optional]  # noqa: E501
             date_format (DateFormat): [optional]  # noqa: E501
             currency_format (CurrencyFormat): [optional]  # noqa: E501
             accounts ([Account]): [optional]  # noqa: E501
             payees ([Payee]): [optional]  # noqa: E501
             payee_locations ([PayeeLocation]): [optional]  # noqa: E501
             category_groups ([CategoryGroup]): [optional]  # noqa: E501
             categories ([Category]): [optional]  # noqa: E501
@@ -277,16 +292,16 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
         """BudgetDetail - a model defined in OpenAPI
 
         Keyword Args:
-            id (str):
-            name (str):
+            id (str, none_type):
+            name (str, none_type):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -309,17 +324,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            last_modified_on (datetime): The last time any changes were made to the budget from either a web or mobile client. [optional]  # noqa: E501
-            first_month (date): The earliest budget month. [optional]  # noqa: E501
-            last_month (date): The latest budget month. [optional]  # noqa: E501
+            last_modified_on (datetime, none_type): The last time any changes were made to the budget from either a web or mobile client. [optional]  # noqa: E501
+            first_month (date, none_type): The earliest budget month. [optional]  # noqa: E501
+            last_month (date, none_type): The latest budget month. [optional]  # noqa: E501
             date_format (DateFormat): [optional]  # noqa: E501
             currency_format (CurrencyFormat): [optional]  # noqa: E501
             accounts ([Account]): [optional]  # noqa: E501
             payees ([Payee]): [optional]  # noqa: E501
             payee_locations ([PayeeLocation]): [optional]  # noqa: E501
             category_groups ([CategoryGroup]): [optional]  # noqa: E501
             categories ([Category]): [optional]  # noqa: E501
```

### Comparing `ynab-api-2.0.0/ynab_api/model/budget_detail_all_of.py` & `ynab-api-2.0.2/ynab_api/model/budget_detail_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/budget_detail_response.py` & `ynab-api-2.0.2/ynab_api/model/budget_detail_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/budget_detail_response_data.py` & `ynab-api-2.0.2/ynab_api/model/budget_detail_response_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -82,15 +82,18 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'budget': (BudgetDetail, ),  # noqa: E501
-            'server_knowledge': (int, ),  # noqa: E501
+            'server_knowledge': (
+                int,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -106,15 +109,15 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, budget, server_knowledge, *args,
                            **kwargs):  # noqa: E501
         """BudgetDetailResponseData - a model defined in OpenAPI
 
         Args:
             budget (BudgetDetail):
-            server_knowledge (int): The knowledge of the server
+            server_knowledge (int, none_type): The knowledge of the server
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -196,15 +199,15 @@
     @convert_js_args_to_python_args
     def __init__(self, budget, server_knowledge, *args,
                  **kwargs):  # noqa: E501
         """BudgetDetailResponseData - a model defined in OpenAPI
 
         Args:
             budget (BudgetDetail):
-            server_knowledge (int): The knowledge of the server
+            server_knowledge (int, none_type): The knowledge of the server
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `ynab-api-2.0.0/ynab_api/model/budget_settings.py` & `ynab-api-2.0.2/ynab_api/model/budget_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/budget_settings_response.py` & `ynab-api-2.0.2/ynab_api/model/budget_settings_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/budget_settings_response_data.py` & `ynab-api-2.0.2/ynab_api/model/budget_settings_response_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/budget_summary.py` & `ynab-api-2.0.2/ynab_api/model/budget_summary.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -85,19 +85,34 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'id': (str, ),  # noqa: E501
-            'name': (str, ),  # noqa: E501
-            'last_modified_on': (datetime, ),  # noqa: E501
-            'first_month': (date, ),  # noqa: E501
-            'last_month': (date, ),  # noqa: E501
+            'id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'name': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'last_modified_on': (
+                datetime,
+                none_type,
+            ),  # noqa: E501
+            'first_month': (
+                date,
+                none_type,
+            ),  # noqa: E501
+            'last_month': (
+                date,
+                none_type,
+            ),  # noqa: E501
             'date_format': (DateFormat, ),  # noqa: E501
             'currency_format': (CurrencyFormat, ),  # noqa: E501
             'accounts': ([Account], ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
@@ -120,16 +135,16 @@
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, id, name, *args, **kwargs):  # noqa: E501
         """BudgetSummary - a model defined in OpenAPI
 
         Args:
-            id (str):
-            name (str):
+            id (str, none_type):
+            name (str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -154,17 +169,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            last_modified_on (datetime): The last time any changes were made to the budget from either a web or mobile client. [optional]  # noqa: E501
-            first_month (date): The earliest budget month. [optional]  # noqa: E501
-            last_month (date): The latest budget month. [optional]  # noqa: E501
+            last_modified_on (datetime, none_type): The last time any changes were made to the budget from either a web or mobile client. [optional]  # noqa: E501
+            first_month (date, none_type): The earliest budget month. [optional]  # noqa: E501
+            last_month (date, none_type): The latest budget month. [optional]  # noqa: E501
             date_format (DateFormat): [optional]  # noqa: E501
             currency_format (CurrencyFormat): [optional]  # noqa: E501
             accounts ([Account]): The budget accounts (only included if `include_accounts=true` specified as query parameter). [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -215,16 +230,16 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, id, name, *args, **kwargs):  # noqa: E501
         """BudgetSummary - a model defined in OpenAPI
 
         Args:
-            id (str):
-            name (str):
+            id (str, none_type):
+            name (str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -249,17 +264,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            last_modified_on (datetime): The last time any changes were made to the budget from either a web or mobile client. [optional]  # noqa: E501
-            first_month (date): The earliest budget month. [optional]  # noqa: E501
-            last_month (date): The latest budget month. [optional]  # noqa: E501
+            last_modified_on (datetime, none_type): The last time any changes were made to the budget from either a web or mobile client. [optional]  # noqa: E501
+            first_month (date, none_type): The earliest budget month. [optional]  # noqa: E501
+            last_month (date, none_type): The latest budget month. [optional]  # noqa: E501
             date_format (DateFormat): [optional]  # noqa: E501
             currency_format (CurrencyFormat): [optional]  # noqa: E501
             accounts ([Account]): The budget accounts (only included if `include_accounts=true` specified as query parameter). [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
```

### Comparing `ynab-api-2.0.0/ynab_api/model/budget_summary_response.py` & `ynab-api-2.0.2/ynab_api/model/budget_summary_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/budget_summary_response_data.py` & `ynab-api-2.0.2/ynab_api/model/budget_summary_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/bulk_response.py` & `ynab-api-2.0.2/ynab_api/model/bulk_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/bulk_response_data.py` & `ynab-api-2.0.2/ynab_api/model/bulk_response_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/bulk_response_data_bulk.py` & `ynab-api-2.0.2/ynab_api/model/bulk_response_data_bulk.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -74,16 +74,16 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'transaction_ids': ([str], ),  # noqa: E501
-            'duplicate_import_ids': ([str], ),  # noqa: E501
+            'transaction_ids': ([str, none_type], ),  # noqa: E501
+            'duplicate_import_ids': ([str, none_type], ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -98,16 +98,16 @@
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, transaction_ids, duplicate_import_ids, *args,
                            **kwargs):  # noqa: E501
         """BulkResponseDataBulk - a model defined in OpenAPI
 
         Args:
-            transaction_ids ([str]): The list of Transaction ids that were created.
-            duplicate_import_ids ([str]): If any Transactions were not created because they had an `import_id` matching a transaction already on the same account, the specified import_id(s) will be included in this list.
+            transaction_ids ([str, none_type]): The list of Transaction ids that were created.
+            duplicate_import_ids ([str, none_type]): If any Transactions were not created because they had an `import_id` matching a transaction already on the same account, the specified import_id(s) will be included in this list.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -188,16 +188,16 @@
 
     @convert_js_args_to_python_args
     def __init__(self, transaction_ids, duplicate_import_ids, *args,
                  **kwargs):  # noqa: E501
         """BulkResponseDataBulk - a model defined in OpenAPI
 
         Args:
-            transaction_ids ([str]): The list of Transaction ids that were created.
-            duplicate_import_ids ([str]): If any Transactions were not created because they had an `import_id` matching a transaction already on the same account, the specified import_id(s) will be included in this list.
+            transaction_ids ([str, none_type]): The list of Transaction ids that were created.
+            duplicate_import_ids ([str, none_type]): If any Transactions were not created because they had an `import_id` matching a transaction already on the same account, the specified import_id(s) will be included in this list.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `ynab-api-2.0.0/ynab_api/model/bulk_transactions.py` & `ynab-api-2.0.2/ynab_api/model/bulk_transactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/categories_response.py` & `ynab-api-2.0.2/ynab_api/model/categories_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/categories_response_data.py` & `ynab-api-2.0.2/ynab_api/model/categories_response_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -82,15 +82,18 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'category_groups': ([CategoryGroupWithCategories], ),  # noqa: E501
-            'server_knowledge': (int, ),  # noqa: E501
+            'server_knowledge': (
+                int,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -106,15 +109,15 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, category_groups, server_knowledge, *args,
                            **kwargs):  # noqa: E501
         """CategoriesResponseData - a model defined in OpenAPI
 
         Args:
             category_groups ([CategoryGroupWithCategories]):
-            server_knowledge (int): The knowledge of the server
+            server_knowledge (int, none_type): The knowledge of the server
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -196,15 +199,15 @@
     @convert_js_args_to_python_args
     def __init__(self, category_groups, server_knowledge, *args,
                  **kwargs):  # noqa: E501
         """CategoriesResponseData - a model defined in OpenAPI
 
         Args:
             category_groups ([CategoryGroupWithCategories]):
-            server_knowledge (int): The knowledge of the server
+            server_knowledge (int, none_type): The knowledge of the server
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `ynab-api-2.0.0/ynab_api/model/category.py` & `ynab-api-2.0.2/ynab_api/model/category.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -41,14 +41,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('goal_type', ): {
+            'None': None,
             'TB': "TB",
             'TBD': "TBD",
             'MF': "MF",
             'NEED': "NEED",
         },
     }
 
@@ -81,36 +82,84 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (str, ),  # noqa: E501
-            'category_group_id': (str, ),  # noqa: E501
-            'name': (str, ),  # noqa: E501
+            'id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'category_group_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'name': (
+                str,
+                none_type,
+            ),  # noqa: E501
             'hidden': (bool, ),  # noqa: E501
-            'budgeted': (int, ),  # noqa: E501
-            'activity': (int, ),  # noqa: E501
-            'balance': (int, ),  # noqa: E501
+            'budgeted': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'activity': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'balance': (
+                int,
+                none_type,
+            ),  # noqa: E501
             'deleted': (bool, ),  # noqa: E501
-            'original_category_group_id': (str, ),  # noqa: E501
+            'original_category_group_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
             'note': (
                 str,
                 none_type,
             ),  # noqa: E501
-            'goal_type': (str, ),  # noqa: E501
-            'goal_creation_month': (date, ),  # noqa: E501
-            'goal_target': (int, ),  # noqa: E501
-            'goal_target_month': (date, ),  # noqa: E501
-            'goal_percentage_complete': (int, ),  # noqa: E501
-            'goal_months_to_budget': (int, ),  # noqa: E501
-            'goal_under_funded': (int, ),  # noqa: E501
-            'goal_overall_funded': (int, ),  # noqa: E501
-            'goal_overall_left': (int, ),  # noqa: E501
+            'goal_type': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'goal_creation_month': (
+                date,
+                none_type,
+            ),  # noqa: E501
+            'goal_target': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'goal_target_month': (
+                date,
+                none_type,
+            ),  # noqa: E501
+            'goal_percentage_complete': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'goal_months_to_budget': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'goal_under_funded': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'goal_overall_funded': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'goal_overall_left': (
+                int,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -144,21 +193,21 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, id, category_group_id, name, hidden, budgeted,
                            activity, balance, deleted, *args,
                            **kwargs):  # noqa: E501
         """Category - a model defined in OpenAPI
 
         Args:
-            id (str):
-            category_group_id (str):
-            name (str):
+            id (str, none_type):
+            category_group_id (str, none_type):
+            name (str, none_type):
             hidden (bool): Whether or not the category is hidden
-            budgeted (int): Budgeted amount in milliunits format
-            activity (int): Activity amount in milliunits format
-            balance (int): Balance in milliunits format
+            budgeted (int, none_type): Budgeted amount in milliunits format
+            activity (int, none_type): Activity amount in milliunits format
+            balance (int, none_type): Balance in milliunits format
             deleted (bool): Whether or not the category has been deleted.  Deleted categories will only be included in delta requests.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -184,25 +233,25 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            original_category_group_id (str): If category is hidden this is the id of the category group it originally belonged to before it was hidden.. [optional]  # noqa: E501
+            original_category_group_id (str, none_type): If category is hidden this is the id of the category group it originally belonged to before it was hidden.. [optional]  # noqa: E501
             note (str, none_type): [optional]  # noqa: E501
-            goal_type (str): The type of goal, if the category has a goal (TB='Target Category Balance', TBD='Target Category Balance by Date', MF='Monthly Funding', NEED='Plan Your Spending'). [optional]  # noqa: E501
-            goal_creation_month (date): The month a goal was created. [optional]  # noqa: E501
-            goal_target (int): The goal target amount in milliunits. [optional]  # noqa: E501
-            goal_target_month (date): The original target month for the goal to be completed.  Only some goal types specify this date.. [optional]  # noqa: E501
-            goal_percentage_complete (int): The percentage completion of the goal. [optional]  # noqa: E501
-            goal_months_to_budget (int): The number of months, including the current month, left in the current goal period.. [optional]  # noqa: E501
-            goal_under_funded (int): The amount of funding still needed in the current month to stay on track towards completing the goal within the current goal period.  This amount will generally correspond to the 'Underfunded' amount in the web and mobile clients except when viewing a category with a Needed for Spending Goal in a future month.  The web and mobile clients will ignore any funding from a prior goal period when viewing category with a Needed for Spending Goal in a future month.. [optional]  # noqa: E501
-            goal_overall_funded (int): The total amount funded towards the goal within the current goal period.. [optional]  # noqa: E501
-            goal_overall_left (int): The amount of funding still needed to complete the goal within the current goal period.. [optional]  # noqa: E501
+            goal_type (str, none_type): The type of goal, if the category has a goal (TB='Target Category Balance', TBD='Target Category Balance by Date', MF='Monthly Funding', NEED='Plan Your Spending'). [optional]  # noqa: E501
+            goal_creation_month (date, none_type): The month a goal was created. [optional]  # noqa: E501
+            goal_target (int, none_type): The goal target amount in milliunits. [optional]  # noqa: E501
+            goal_target_month (date, none_type): The original target month for the goal to be completed.  Only some goal types specify this date.. [optional]  # noqa: E501
+            goal_percentage_complete (int, none_type): The percentage completion of the goal. [optional]  # noqa: E501
+            goal_months_to_budget (int, none_type): The number of months, including the current month, left in the current goal period.. [optional]  # noqa: E501
+            goal_under_funded (int, none_type): The amount of funding still needed in the current month to stay on track towards completing the goal within the current goal period.  This amount will generally correspond to the 'Underfunded' amount in the web and mobile clients except when viewing a category with a Needed for Spending Goal in a future month.  The web and mobile clients will ignore any funding from a prior goal period when viewing category with a Needed for Spending Goal in a future month.. [optional]  # noqa: E501
+            goal_overall_funded (int, none_type): The total amount funded towards the goal within the current goal period.. [optional]  # noqa: E501
+            goal_overall_left (int, none_type): The amount of funding still needed to complete the goal within the current goal period.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -257,21 +306,21 @@
 
     @convert_js_args_to_python_args
     def __init__(self, id, category_group_id, name, hidden, budgeted, activity,
                  balance, deleted, *args, **kwargs):  # noqa: E501
         """Category - a model defined in OpenAPI
 
         Args:
-            id (str):
-            category_group_id (str):
-            name (str):
+            id (str, none_type):
+            category_group_id (str, none_type):
+            name (str, none_type):
             hidden (bool): Whether or not the category is hidden
-            budgeted (int): Budgeted amount in milliunits format
-            activity (int): Activity amount in milliunits format
-            balance (int): Balance in milliunits format
+            budgeted (int, none_type): Budgeted amount in milliunits format
+            activity (int, none_type): Activity amount in milliunits format
+            balance (int, none_type): Balance in milliunits format
             deleted (bool): Whether or not the category has been deleted.  Deleted categories will only be included in delta requests.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -297,25 +346,25 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            original_category_group_id (str): If category is hidden this is the id of the category group it originally belonged to before it was hidden.. [optional]  # noqa: E501
+            original_category_group_id (str, none_type): If category is hidden this is the id of the category group it originally belonged to before it was hidden.. [optional]  # noqa: E501
             note (str, none_type): [optional]  # noqa: E501
-            goal_type (str): The type of goal, if the category has a goal (TB='Target Category Balance', TBD='Target Category Balance by Date', MF='Monthly Funding', NEED='Plan Your Spending'). [optional]  # noqa: E501
-            goal_creation_month (date): The month a goal was created. [optional]  # noqa: E501
-            goal_target (int): The goal target amount in milliunits. [optional]  # noqa: E501
-            goal_target_month (date): The original target month for the goal to be completed.  Only some goal types specify this date.. [optional]  # noqa: E501
-            goal_percentage_complete (int): The percentage completion of the goal. [optional]  # noqa: E501
-            goal_months_to_budget (int): The number of months, including the current month, left in the current goal period.. [optional]  # noqa: E501
-            goal_under_funded (int): The amount of funding still needed in the current month to stay on track towards completing the goal within the current goal period.  This amount will generally correspond to the 'Underfunded' amount in the web and mobile clients except when viewing a category with a Needed for Spending Goal in a future month.  The web and mobile clients will ignore any funding from a prior goal period when viewing category with a Needed for Spending Goal in a future month.. [optional]  # noqa: E501
-            goal_overall_funded (int): The total amount funded towards the goal within the current goal period.. [optional]  # noqa: E501
-            goal_overall_left (int): The amount of funding still needed to complete the goal within the current goal period.. [optional]  # noqa: E501
+            goal_type (str, none_type): The type of goal, if the category has a goal (TB='Target Category Balance', TBD='Target Category Balance by Date', MF='Monthly Funding', NEED='Plan Your Spending'). [optional]  # noqa: E501
+            goal_creation_month (date, none_type): The month a goal was created. [optional]  # noqa: E501
+            goal_target (int, none_type): The goal target amount in milliunits. [optional]  # noqa: E501
+            goal_target_month (date, none_type): The original target month for the goal to be completed.  Only some goal types specify this date.. [optional]  # noqa: E501
+            goal_percentage_complete (int, none_type): The percentage completion of the goal. [optional]  # noqa: E501
+            goal_months_to_budget (int, none_type): The number of months, including the current month, left in the current goal period.. [optional]  # noqa: E501
+            goal_under_funded (int, none_type): The amount of funding still needed in the current month to stay on track towards completing the goal within the current goal period.  This amount will generally correspond to the 'Underfunded' amount in the web and mobile clients except when viewing a category with a Needed for Spending Goal in a future month.  The web and mobile clients will ignore any funding from a prior goal period when viewing category with a Needed for Spending Goal in a future month.. [optional]  # noqa: E501
+            goal_overall_funded (int, none_type): The total amount funded towards the goal within the current goal period.. [optional]  # noqa: E501
+            goal_overall_left (int, none_type): The amount of funding still needed to complete the goal within the current goal period.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ynab-api-2.0.0/ynab_api/model/category_group.py` & `ynab-api-2.0.2/ynab_api/model/category_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -74,16 +74,22 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (str, ),  # noqa: E501
-            'name': (str, ),  # noqa: E501
+            'id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'name': (
+                str,
+                none_type,
+            ),  # noqa: E501
             'hidden': (bool, ),  # noqa: E501
             'deleted': (bool, ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
@@ -102,16 +108,16 @@
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, id, name, hidden, deleted, *args,
                            **kwargs):  # noqa: E501
         """CategoryGroup - a model defined in OpenAPI
 
         Args:
-            id (str):
-            name (str):
+            id (str, none_type):
+            name (str, none_type):
             hidden (bool): Whether or not the category group is hidden
             deleted (bool): Whether or not the category group has been deleted.  Deleted category groups will only be included in delta requests.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -196,16 +202,16 @@
 
     @convert_js_args_to_python_args
     def __init__(self, id, name, hidden, deleted, *args,
                  **kwargs):  # noqa: E501
         """CategoryGroup - a model defined in OpenAPI
 
         Args:
-            id (str):
-            name (str):
+            id (str, none_type):
+            name (str, none_type):
             hidden (bool): Whether or not the category group is hidden
             deleted (bool): Whether or not the category group has been deleted.  Deleted category groups will only be included in delta requests.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
```

### Comparing `ynab-api-2.0.0/ynab_api/model/category_group_with_categories.py` & `ynab-api-2.0.2/ynab_api/model/category_group_with_categories.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -86,16 +86,22 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'id': (str, ),  # noqa: E501
-            'name': (str, ),  # noqa: E501
+            'id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'name': (
+                str,
+                none_type,
+            ),  # noqa: E501
             'hidden': (bool, ),  # noqa: E501
             'deleted': (bool, ),  # noqa: E501
             'categories': ([Category], ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
@@ -113,16 +119,16 @@
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """CategoryGroupWithCategories - a model defined in OpenAPI
 
         Keyword Args:
-            id (str):
-            name (str):
+            id (str, none_type):
+            name (str, none_type):
             hidden (bool): Whether or not the category group is hidden
             deleted (bool): Whether or not the category group has been deleted.  Deleted category groups will only be included in delta requests.
             categories ([Category]): Category group categories.  Amounts (budgeted, activity, balance, etc.) are specific to the current budget month (UTC).
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -218,16 +224,16 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
         """CategoryGroupWithCategories - a model defined in OpenAPI
 
         Keyword Args:
-            id (str):
-            name (str):
+            id (str, none_type):
+            name (str, none_type):
             hidden (bool): Whether or not the category group is hidden
             deleted (bool): Whether or not the category group has been deleted.  Deleted category groups will only be included in delta requests.
             categories ([Category]): Category group categories.  Amounts (budgeted, activity, balance, etc.) are specific to the current budget month (UTC).
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `ynab-api-2.0.0/ynab_api/model/category_group_with_categories_all_of.py` & `ynab-api-2.0.2/ynab_api/model/category_group_with_categories_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/category_response.py` & `ynab-api-2.0.2/ynab_api/model/category_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/category_response_data.py` & `ynab-api-2.0.2/ynab_api/model/category_response_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/currency_format.py` & `ynab-api-2.0.2/ynab_api/model/currency_format.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -74,21 +74,39 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'iso_code': (str, ),  # noqa: E501
-            'example_format': (str, ),  # noqa: E501
-            'decimal_digits': (int, ),  # noqa: E501
-            'decimal_separator': (str, ),  # noqa: E501
+            'iso_code': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'example_format': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'decimal_digits': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'decimal_separator': (
+                str,
+                none_type,
+            ),  # noqa: E501
             'symbol_first': (bool, ),  # noqa: E501
-            'group_separator': (str, ),  # noqa: E501
-            'currency_symbol': (str, ),  # noqa: E501
+            'group_separator': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'currency_symbol': (
+                str,
+                none_type,
+            ),  # noqa: E501
             'display_symbol': (bool, ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -112,21 +130,21 @@
     def _from_openapi_data(cls, iso_code, example_format, decimal_digits,
                            decimal_separator, symbol_first, group_separator,
                            currency_symbol, display_symbol, *args,
                            **kwargs):  # noqa: E501
         """CurrencyFormat - a model defined in OpenAPI
 
         Args:
-            iso_code (str):
-            example_format (str):
-            decimal_digits (int):
-            decimal_separator (str):
+            iso_code (str, none_type):
+            example_format (str, none_type):
+            decimal_digits (int, none_type):
+            decimal_separator (str, none_type):
             symbol_first (bool):
-            group_separator (str):
-            currency_symbol (str):
+            group_separator (str, none_type):
+            currency_symbol (str, none_type):
             display_symbol (bool):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -216,21 +234,21 @@
     def __init__(self, iso_code, example_format, decimal_digits,
                  decimal_separator, symbol_first, group_separator,
                  currency_symbol, display_symbol, *args,
                  **kwargs):  # noqa: E501
         """CurrencyFormat - a model defined in OpenAPI
 
         Args:
-            iso_code (str):
-            example_format (str):
-            decimal_digits (int):
-            decimal_separator (str):
+            iso_code (str, none_type):
+            example_format (str, none_type):
+            decimal_digits (int, none_type):
+            decimal_separator (str, none_type):
             symbol_first (bool):
-            group_separator (str):
-            currency_symbol (str):
+            group_separator (str, none_type):
+            currency_symbol (str, none_type):
             display_symbol (bool):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `ynab-api-2.0.0/ynab_api/model/date_format.py` & `ynab-api-2.0.2/ynab_api/model/date_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -74,15 +74,18 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'format': (str, ),  # noqa: E501
+            'format': (
+                str,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -95,15 +98,15 @@
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, format, *args, **kwargs):  # noqa: E501
         """DateFormat - a model defined in OpenAPI
 
         Args:
-            format (str):
+            format (str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -182,15 +185,15 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, format, *args, **kwargs):  # noqa: E501
         """DateFormat - a model defined in OpenAPI
 
         Args:
-            format (str):
+            format (str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `ynab-api-2.0.0/ynab_api/model/error_detail.py` & `ynab-api-2.0.2/ynab_api/model/error_detail.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -74,17 +74,26 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (str, ),  # noqa: E501
-            'name': (str, ),  # noqa: E501
-            'detail': (str, ),  # noqa: E501
+            'id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'name': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'detail': (
+                str,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -100,17 +109,17 @@
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, id, name, detail, *args,
                            **kwargs):  # noqa: E501
         """ErrorDetail - a model defined in OpenAPI
 
         Args:
-            id (str):
-            name (str):
-            detail (str):
+            id (str, none_type):
+            name (str, none_type):
+            detail (str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -191,17 +200,17 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, id, name, detail, *args, **kwargs):  # noqa: E501
         """ErrorDetail - a model defined in OpenAPI
 
         Args:
-            id (str):
-            name (str):
-            detail (str):
+            id (str, none_type):
+            name (str, none_type):
+            detail (str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `ynab-api-2.0.0/ynab_api/model/error_response.py` & `ynab-api-2.0.2/ynab_api/model/error_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/hybrid_transaction.py` & `ynab-api-2.0.2/ynab_api/model/transaction_detail.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -16,21 +16,23 @@
     file_type, none_type, validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from ynab_api.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from ynab_api.model.hybrid_transaction_all_of import HybridTransactionAllOf
+    from ynab_api.model.sub_transaction import SubTransaction
+    from ynab_api.model.transaction_detail_all_of import TransactionDetailAllOf
     from ynab_api.model.transaction_summary import TransactionSummary
-    globals()['HybridTransactionAllOf'] = HybridTransactionAllOf
+    globals()['SubTransaction'] = SubTransaction
+    globals()['TransactionDetailAllOf'] = TransactionDetailAllOf
     globals()['TransactionSummary'] = TransactionSummary
 
 
-class HybridTransaction(ModelComposed):
+class TransactionDetail(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -48,23 +50,21 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('cleared', ): {
+            'None': None,
             'CLEARED': "cleared",
             'UNCLEARED': "uncleared",
             'RECONCILED': "reconciled",
         },
-        ('type', ): {
-            'TRANSACTION': "transaction",
-            'SUBTRANSACTION': "subtransaction",
-        },
         ('flag_color', ): {
+            'None': None,
             'RED': "red",
             'ORANGE': "orange",
             'YELLOW': "yellow",
             'GREEN': "green",
             'BLUE': "blue",
             'PURPLE': "purple",
         },
@@ -101,80 +101,126 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'id': (str, ),  # noqa: E501
-            'date': (date, ),  # noqa: E501
-            'amount': (int, ),  # noqa: E501
-            'cleared': (str, ),  # noqa: E501
+            'id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'date': (
+                date,
+                none_type,
+            ),  # noqa: E501
+            'amount': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'cleared': (
+                str,
+                none_type,
+            ),  # noqa: E501
             'approved': (bool, ),  # noqa: E501
-            'account_id': (str, ),  # noqa: E501
+            'account_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
             'deleted': (bool, ),  # noqa: E501
-            'type': (str, ),  # noqa: E501
-            'account_name': (str, ),  # noqa: E501
-            'memo': (str, ),  # noqa: E501
-            'flag_color': (str, ),  # noqa: E501
-            'payee_id': (str, ),  # noqa: E501
-            'category_id': (str, ),  # noqa: E501
-            'transfer_account_id': (str, ),  # noqa: E501
-            'transfer_transaction_id': (str, ),  # noqa: E501
-            'matched_transaction_id': (str, ),  # noqa: E501
-            'import_id': (str, ),  # noqa: E501
-            'parent_transaction_id': (str, ),  # noqa: E501
-            'payee_name': (str, ),  # noqa: E501
-            'category_name': (str, ),  # noqa: E501
+            'account_name': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'subtransactions': ([SubTransaction], ),  # noqa: E501
+            'memo': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'flag_color': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'payee_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'category_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'transfer_account_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'transfer_transaction_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'matched_transaction_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'import_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'payee_name': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'category_name': (
+                str,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'date': 'date',  # noqa: E501
         'amount': 'amount',  # noqa: E501
         'cleared': 'cleared',  # noqa: E501
         'approved': 'approved',  # noqa: E501
         'account_id': 'account_id',  # noqa: E501
         'deleted': 'deleted',  # noqa: E501
-        'type': 'type',  # noqa: E501
         'account_name': 'account_name',  # noqa: E501
+        'subtransactions': 'subtransactions',  # noqa: E501
         'memo': 'memo',  # noqa: E501
         'flag_color': 'flag_color',  # noqa: E501
         'payee_id': 'payee_id',  # noqa: E501
         'category_id': 'category_id',  # noqa: E501
         'transfer_account_id': 'transfer_account_id',  # noqa: E501
         'transfer_transaction_id': 'transfer_transaction_id',  # noqa: E501
         'matched_transaction_id': 'matched_transaction_id',  # noqa: E501
         'import_id': 'import_id',  # noqa: E501
-        'parent_transaction_id': 'parent_transaction_id',  # noqa: E501
         'payee_name': 'payee_name',  # noqa: E501
         'category_name': 'category_name',  # noqa: E501
     }
 
     read_only_vars = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """HybridTransaction - a model defined in OpenAPI
+        """TransactionDetail - a model defined in OpenAPI
 
         Keyword Args:
-            id (str):
-            date (date): The transaction date in ISO format (e.g. 2016-12-01)
-            amount (int): The transaction amount in milliunits format
-            cleared (str): The cleared status of the transaction
+            id (str, none_type):
+            date (date, none_type): The transaction date in ISO format (e.g. 2016-12-01)
+            amount (int, none_type): The transaction amount in milliunits format
+            cleared (str, none_type): The cleared status of the transaction
             approved (bool): Whether or not the transaction is approved
-            account_id (str):
+            account_id (str, none_type):
             deleted (bool): Whether or not the transaction has been deleted.  Deleted transactions will only be included in delta requests.
-            type (str): Whether the hybrid transaction represents a regular transaction or a subtransaction
-            account_name (str):
+            account_name (str, none_type):
+            subtransactions ([SubTransaction]): If a split transaction, the subtransactions.
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -197,25 +243,24 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            memo (str): [optional]  # noqa: E501
-            flag_color (str): The transaction flag. [optional]  # noqa: E501
-            payee_id (str): [optional]  # noqa: E501
-            category_id (str): [optional]  # noqa: E501
-            transfer_account_id (str): If a transfer transaction, the account to which it transfers. [optional]  # noqa: E501
-            transfer_transaction_id (str): If a transfer transaction, the id of transaction on the other side of the transfer. [optional]  # noqa: E501
-            matched_transaction_id (str): If transaction is matched, the id of the matched transaction. [optional]  # noqa: E501
-            import_id (str): If the Transaction was imported, this field is a unique (by account) import identifier.  If this transaction was imported through File Based Import or Direct Import and not through the API, the import_id will have the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'.  For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.. [optional]  # noqa: E501
-            parent_transaction_id (str): For subtransaction types, this is the id of the parent transaction.  For transaction types, this id will be always be null.. [optional]  # noqa: E501
-            payee_name (str): [optional]  # noqa: E501
-            category_name (str): [optional]  # noqa: E501
+            memo (str, none_type): [optional]  # noqa: E501
+            flag_color (str, none_type): The transaction flag. [optional]  # noqa: E501
+            payee_id (str, none_type): [optional]  # noqa: E501
+            category_id (str, none_type): [optional]  # noqa: E501
+            transfer_account_id (str, none_type): If a transfer transaction, the account to which it transfers. [optional]  # noqa: E501
+            transfer_transaction_id (str, none_type): If a transfer transaction, the id of transaction on the other side of the transfer. [optional]  # noqa: E501
+            matched_transaction_id (str, none_type): If transaction is matched, the id of the matched transaction. [optional]  # noqa: E501
+            import_id (str, none_type): If the Transaction was imported, this field is a unique (by account) import identifier.  If this transaction was imported through File Based Import or Direct Import and not through the API, the import_id will have the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'.  For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.. [optional]  # noqa: E501
+            payee_name (str, none_type): [optional]  # noqa: E501
+            category_name (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -275,26 +320,26 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """HybridTransaction - a model defined in OpenAPI
+        """TransactionDetail - a model defined in OpenAPI
 
         Keyword Args:
-            id (str):
-            date (date): The transaction date in ISO format (e.g. 2016-12-01)
-            amount (int): The transaction amount in milliunits format
-            cleared (str): The cleared status of the transaction
+            id (str, none_type):
+            date (date, none_type): The transaction date in ISO format (e.g. 2016-12-01)
+            amount (int, none_type): The transaction amount in milliunits format
+            cleared (str, none_type): The cleared status of the transaction
             approved (bool): Whether or not the transaction is approved
-            account_id (str):
+            account_id (str, none_type):
             deleted (bool): Whether or not the transaction has been deleted.  Deleted transactions will only be included in delta requests.
-            type (str): Whether the hybrid transaction represents a regular transaction or a subtransaction
-            account_name (str):
+            account_name (str, none_type):
+            subtransactions ([SubTransaction]): If a split transaction, the subtransactions.
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -317,25 +362,24 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            memo (str): [optional]  # noqa: E501
-            flag_color (str): The transaction flag. [optional]  # noqa: E501
-            payee_id (str): [optional]  # noqa: E501
-            category_id (str): [optional]  # noqa: E501
-            transfer_account_id (str): If a transfer transaction, the account to which it transfers. [optional]  # noqa: E501
-            transfer_transaction_id (str): If a transfer transaction, the id of transaction on the other side of the transfer. [optional]  # noqa: E501
-            matched_transaction_id (str): If transaction is matched, the id of the matched transaction. [optional]  # noqa: E501
-            import_id (str): If the Transaction was imported, this field is a unique (by account) import identifier.  If this transaction was imported through File Based Import or Direct Import and not through the API, the import_id will have the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'.  For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.. [optional]  # noqa: E501
-            parent_transaction_id (str): For subtransaction types, this is the id of the parent transaction.  For transaction types, this id will be always be null.. [optional]  # noqa: E501
-            payee_name (str): [optional]  # noqa: E501
-            category_name (str): [optional]  # noqa: E501
+            memo (str, none_type): [optional]  # noqa: E501
+            flag_color (str, none_type): The transaction flag. [optional]  # noqa: E501
+            payee_id (str, none_type): [optional]  # noqa: E501
+            category_id (str, none_type): [optional]  # noqa: E501
+            transfer_account_id (str, none_type): If a transfer transaction, the account to which it transfers. [optional]  # noqa: E501
+            transfer_transaction_id (str, none_type): If a transfer transaction, the id of transaction on the other side of the transfer. [optional]  # noqa: E501
+            matched_transaction_id (str, none_type): If transaction is matched, the id of the matched transaction. [optional]  # noqa: E501
+            import_id (str, none_type): If the Transaction was imported, this field is a unique (by account) import identifier.  If this transaction was imported through File Based Import or Direct Import and not through the API, the import_id will have the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'.  For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.. [optional]  # noqa: E501
+            payee_name (str, none_type): [optional]  # noqa: E501
+            category_name (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -394,12 +438,12 @@
         # code would be run when this module is imported, and these composed
         # classes don't exist yet because their module has not finished
         # loading
         lazy_import()
         return {
             'anyOf': [],
             'allOf': [
-                HybridTransactionAllOf,
+                TransactionDetailAllOf,
                 TransactionSummary,
             ],
             'oneOf': [],
         }
```

### Comparing `ynab-api-2.0.0/ynab_api/model/hybrid_transaction_all_of.py` & `ynab-api-2.0.2/ynab_api/model/save_transaction_wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -15,15 +15,20 @@
     change_keys_js_to_python, convert_js_args_to_python_args, date, datetime,
     file_type, none_type, validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from ynab_api.exceptions import ApiAttributeError
 
 
-class HybridTransactionAllOf(ModelNormal):
+def lazy_import():
+    from ynab_api.model.save_transaction import SaveTransaction
+    globals()['SaveTransaction'] = SaveTransaction
+
+
+class SaveTransactionWrapper(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -39,29 +44,25 @@
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
-    allowed_values = {
-        ('type', ): {
-            'TRANSACTION': "transaction",
-            'SUBTRANSACTION': "subtransaction",
-        },
-    }
+    allowed_values = {}
 
     validations = {}
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (
             bool,
             date,
             datetime,
             dict,
             float,
             int,
@@ -78,47 +79,38 @@
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'type': (str, ),  # noqa: E501
-            'account_name': (str, ),  # noqa: E501
-            'parent_transaction_id': (str, ),  # noqa: E501
-            'payee_name': (str, ),  # noqa: E501
-            'category_name': (str, ),  # noqa: E501
+            'transaction': (SaveTransaction, ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
-        'type': 'type',  # noqa: E501
-        'account_name': 'account_name',  # noqa: E501
-        'parent_transaction_id': 'parent_transaction_id',  # noqa: E501
-        'payee_name': 'payee_name',  # noqa: E501
-        'category_name': 'category_name',  # noqa: E501
+        'transaction': 'transaction',  # noqa: E501
     }
 
     read_only_vars = {}
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, type, account_name, *args,
-                           **kwargs):  # noqa: E501
-        """HybridTransactionAllOf - a model defined in OpenAPI
+    def _from_openapi_data(cls, transaction, *args, **kwargs):  # noqa: E501
+        """SaveTransactionWrapper - a model defined in OpenAPI
 
         Args:
-            type (str): Whether the hybrid transaction represents a regular transaction or a subtransaction
-            account_name (str):
+            transaction (SaveTransaction):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,17 +135,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            parent_transaction_id (str): For subtransaction types, this is the id of the parent transaction.  For transaction types, this id will be always be null.. [optional]  # noqa: E501
-            payee_name (str): [optional]  # noqa: E501
-            category_name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -175,16 +164,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (
             self.__class__, )
 
-        self.type = type
-        self.account_name = account_name
+        self.transaction = transaction
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -197,20 +185,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, type, account_name, *args, **kwargs):  # noqa: E501
-        """HybridTransactionAllOf - a model defined in OpenAPI
+    def __init__(self, transaction, *args, **kwargs):  # noqa: E501
+        """SaveTransactionWrapper - a model defined in OpenAPI
 
         Args:
-            type (str): Whether the hybrid transaction represents a regular transaction or a subtransaction
-            account_name (str):
+            transaction (SaveTransaction):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -235,17 +222,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            parent_transaction_id (str): For subtransaction types, this is the id of the parent transaction.  For transaction types, this id will be always be null.. [optional]  # noqa: E501
-            payee_name (str): [optional]  # noqa: E501
-            category_name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -265,16 +249,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (
             self.__class__, )
 
-        self.type = type
-        self.account_name = account_name
+        self.transaction = transaction
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `ynab-api-2.0.0/ynab_api/model/hybrid_transactions_response.py` & `ynab-api-2.0.2/ynab_api/model/hybrid_transactions_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/hybrid_transactions_response_data.py` & `ynab-api-2.0.2/ynab_api/model/hybrid_transactions_response_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/month_detail.py` & `ynab-api-2.0.2/ynab_api/model/month_detail.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -85,26 +85,44 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'month': (date, ),  # noqa: E501
-            'income': (int, ),  # noqa: E501
-            'budgeted': (int, ),  # noqa: E501
-            'activity': (int, ),  # noqa: E501
-            'to_be_budgeted': (int, ),  # noqa: E501
+            'month': (
+                date,
+                none_type,
+            ),  # noqa: E501
+            'income': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'budgeted': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'activity': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'to_be_budgeted': (
+                int,
+                none_type,
+            ),  # noqa: E501
             'deleted': (bool, ),  # noqa: E501
             'categories': ([Category], ),  # noqa: E501
             'note': (
                 str,
                 none_type,
             ),  # noqa: E501
-            'age_of_money': (int, ),  # noqa: E501
+            'age_of_money': (
+                int,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -123,19 +141,19 @@
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """MonthDetail - a model defined in OpenAPI
 
         Keyword Args:
-            month (date):
-            income (int): The total amount of transactions categorized to 'Inflow: Ready to Assign' in the month
-            budgeted (int): The total amount budgeted in the month
-            activity (int): The total amount of transactions in the month, excluding those categorized to 'Inflow: Ready to Assign'
-            to_be_budgeted (int): The available amount for 'Ready to Assign'
+            month (date, none_type):
+            income (int, none_type): The total amount of transactions categorized to 'Inflow: Ready to Assign' in the month
+            budgeted (int, none_type): The total amount budgeted in the month
+            activity (int, none_type): The total amount of transactions in the month, excluding those categorized to 'Inflow: Ready to Assign'
+            to_be_budgeted (int, none_type): The available amount for 'Ready to Assign'
             deleted (bool): Whether or not the month has been deleted.  Deleted months will only be included in delta requests.
             categories ([Category]): The budget month categories.  Amounts (budgeted, activity, balance, etc.) are specific to the {month} parameter specified.
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -161,15 +179,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             note (str, none_type): [optional]  # noqa: E501
-            age_of_money (int): The Age of Money as of the month. [optional]  # noqa: E501
+            age_of_money (int, none_type): The Age of Money as of the month. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -232,19 +250,19 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
         """MonthDetail - a model defined in OpenAPI
 
         Keyword Args:
-            month (date):
-            income (int): The total amount of transactions categorized to 'Inflow: Ready to Assign' in the month
-            budgeted (int): The total amount budgeted in the month
-            activity (int): The total amount of transactions in the month, excluding those categorized to 'Inflow: Ready to Assign'
-            to_be_budgeted (int): The available amount for 'Ready to Assign'
+            month (date, none_type):
+            income (int, none_type): The total amount of transactions categorized to 'Inflow: Ready to Assign' in the month
+            budgeted (int, none_type): The total amount budgeted in the month
+            activity (int, none_type): The total amount of transactions in the month, excluding those categorized to 'Inflow: Ready to Assign'
+            to_be_budgeted (int, none_type): The available amount for 'Ready to Assign'
             deleted (bool): Whether or not the month has been deleted.  Deleted months will only be included in delta requests.
             categories ([Category]): The budget month categories.  Amounts (budgeted, activity, balance, etc.) are specific to the {month} parameter specified.
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -270,15 +288,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             note (str, none_type): [optional]  # noqa: E501
-            age_of_money (int): The Age of Money as of the month. [optional]  # noqa: E501
+            age_of_money (int, none_type): The Age of Money as of the month. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ynab-api-2.0.0/ynab_api/model/month_detail_all_of.py` & `ynab-api-2.0.2/ynab_api/model/month_detail_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/month_detail_response.py` & `ynab-api-2.0.2/ynab_api/model/month_detail_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/month_detail_response_data.py` & `ynab-api-2.0.2/ynab_api/model/month_detail_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/month_summaries_response.py` & `ynab-api-2.0.2/ynab_api/model/month_summaries_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/month_summaries_response_data.py` & `ynab-api-2.0.2/ynab_api/model/month_summaries_response_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -82,15 +82,18 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'months': ([MonthSummary], ),  # noqa: E501
-            'server_knowledge': (int, ),  # noqa: E501
+            'server_knowledge': (
+                int,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -106,15 +109,15 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, months, server_knowledge, *args,
                            **kwargs):  # noqa: E501
         """MonthSummariesResponseData - a model defined in OpenAPI
 
         Args:
             months ([MonthSummary]):
-            server_knowledge (int): The knowledge of the server
+            server_knowledge (int, none_type): The knowledge of the server
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -196,15 +199,15 @@
     @convert_js_args_to_python_args
     def __init__(self, months, server_knowledge, *args,
                  **kwargs):  # noqa: E501
         """MonthSummariesResponseData - a model defined in OpenAPI
 
         Args:
             months ([MonthSummary]):
-            server_knowledge (int): The knowledge of the server
+            server_knowledge (int, none_type): The knowledge of the server
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `ynab-api-2.0.0/ynab_api/model/month_summary.py` & `ynab-api-2.0.2/ynab_api/model/month_summary.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -74,25 +74,43 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'month': (date, ),  # noqa: E501
-            'income': (int, ),  # noqa: E501
-            'budgeted': (int, ),  # noqa: E501
-            'activity': (int, ),  # noqa: E501
-            'to_be_budgeted': (int, ),  # noqa: E501
+            'month': (
+                date,
+                none_type,
+            ),  # noqa: E501
+            'income': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'budgeted': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'activity': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'to_be_budgeted': (
+                int,
+                none_type,
+            ),  # noqa: E501
             'deleted': (bool, ),  # noqa: E501
             'note': (
                 str,
                 none_type,
             ),  # noqa: E501
-            'age_of_money': (int, ),  # noqa: E501
+            'age_of_money': (
+                int,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -114,19 +132,19 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, month, income, budgeted, activity,
                            to_be_budgeted, deleted, *args,
                            **kwargs):  # noqa: E501
         """MonthSummary - a model defined in OpenAPI
 
         Args:
-            month (date):
-            income (int): The total amount of transactions categorized to 'Inflow: Ready to Assign' in the month
-            budgeted (int): The total amount budgeted in the month
-            activity (int): The total amount of transactions in the month, excluding those categorized to 'Inflow: Ready to Assign'
-            to_be_budgeted (int): The available amount for 'Ready to Assign'
+            month (date, none_type):
+            income (int, none_type): The total amount of transactions categorized to 'Inflow: Ready to Assign' in the month
+            budgeted (int, none_type): The total amount budgeted in the month
+            activity (int, none_type): The total amount of transactions in the month, excluding those categorized to 'Inflow: Ready to Assign'
+            to_be_budgeted (int, none_type): The available amount for 'Ready to Assign'
             deleted (bool): Whether or not the month has been deleted.  Deleted months will only be included in delta requests.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -153,15 +171,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             note (str, none_type): [optional]  # noqa: E501
-            age_of_money (int): The Age of Money as of the month. [optional]  # noqa: E501
+            age_of_money (int, none_type): The Age of Money as of the month. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -214,19 +232,19 @@
 
     @convert_js_args_to_python_args
     def __init__(self, month, income, budgeted, activity, to_be_budgeted,
                  deleted, *args, **kwargs):  # noqa: E501
         """MonthSummary - a model defined in OpenAPI
 
         Args:
-            month (date):
-            income (int): The total amount of transactions categorized to 'Inflow: Ready to Assign' in the month
-            budgeted (int): The total amount budgeted in the month
-            activity (int): The total amount of transactions in the month, excluding those categorized to 'Inflow: Ready to Assign'
-            to_be_budgeted (int): The available amount for 'Ready to Assign'
+            month (date, none_type):
+            income (int, none_type): The total amount of transactions categorized to 'Inflow: Ready to Assign' in the month
+            budgeted (int, none_type): The total amount budgeted in the month
+            activity (int, none_type): The total amount of transactions in the month, excluding those categorized to 'Inflow: Ready to Assign'
+            to_be_budgeted (int, none_type): The available amount for 'Ready to Assign'
             deleted (bool): Whether or not the month has been deleted.  Deleted months will only be included in delta requests.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -253,15 +271,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             note (str, none_type): [optional]  # noqa: E501
-            age_of_money (int): The Age of Money as of the month. [optional]  # noqa: E501
+            age_of_money (int, none_type): The Age of Money as of the month. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ynab-api-2.0.0/ynab_api/model/payee.py` & `ynab-api-2.0.2/ynab_api/model/payee.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -74,18 +74,27 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (str, ),  # noqa: E501
-            'name': (str, ),  # noqa: E501
+            'id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'name': (
+                str,
+                none_type,
+            ),  # noqa: E501
             'deleted': (bool, ),  # noqa: E501
-            'transfer_account_id': (str, ),  # noqa: E501
+            'transfer_account_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -102,16 +111,16 @@
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, id, name, deleted, *args,
                            **kwargs):  # noqa: E501
         """Payee - a model defined in OpenAPI
 
         Args:
-            id (str):
-            name (str):
+            id (str, none_type):
+            name (str, none_type):
             deleted (bool): Whether or not the payee has been deleted.  Deleted payees will only be included in delta requests.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -137,15 +146,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            transfer_account_id (str): If a transfer payee, the `account_id` to which this payee transfers to. [optional]  # noqa: E501
+            transfer_account_id (str, none_type): If a transfer payee, the `account_id` to which this payee transfers to. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -194,16 +203,16 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, id, name, deleted, *args, **kwargs):  # noqa: E501
         """Payee - a model defined in OpenAPI
 
         Args:
-            id (str):
-            name (str):
+            id (str, none_type):
+            name (str, none_type):
             deleted (bool): Whether or not the payee has been deleted.  Deleted payees will only be included in delta requests.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -229,15 +238,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            transfer_account_id (str): If a transfer payee, the `account_id` to which this payee transfers to. [optional]  # noqa: E501
+            transfer_account_id (str, none_type): If a transfer payee, the `account_id` to which this payee transfers to. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ynab-api-2.0.0/ynab_api/model/payee_location.py` & `ynab-api-2.0.2/ynab_api/model/save_account.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -15,15 +15,15 @@
     change_keys_js_to_python, convert_js_args_to_python_args, date, datetime,
     file_type, none_type, validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from ynab_api.exceptions import ApiAttributeError
 
 
-class PayeeLocation(ModelNormal):
+class SaveAccount(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -39,15 +39,26 @@
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
-    allowed_values = {}
+    allowed_values = {
+        ('type', ): {
+            'None': None,
+            'CHECKING': "checking",
+            'SAVINGS': "savings",
+            'CREDITCARD': "creditCard",
+            'CASH': "cash",
+            'LINEOFCREDIT': "lineOfCredit",
+            'OTHERASSET': "otherAsset",
+            'OTHERLIABILITY': "otherLiability",
+        },
+    }
 
     validations = {}
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
@@ -74,49 +85,52 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (str, ),  # noqa: E501
-            'payee_id': (str, ),  # noqa: E501
-            'latitude': (str, ),  # noqa: E501
-            'longitude': (str, ),  # noqa: E501
-            'deleted': (bool, ),  # noqa: E501
+            'name': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'type': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'balance': (
+                int,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'payee_id': 'payee_id',  # noqa: E501
-        'latitude': 'latitude',  # noqa: E501
-        'longitude': 'longitude',  # noqa: E501
-        'deleted': 'deleted',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'balance': 'balance',  # noqa: E501
     }
 
     read_only_vars = {}
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, payee_id, latitude, longitude, deleted,
-                           *args, **kwargs):  # noqa: E501
-        """PayeeLocation - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, type, balance, *args,
+                           **kwargs):  # noqa: E501
+        """SaveAccount - a model defined in OpenAPI
 
         Args:
-            id (str):
-            payee_id (str):
-            latitude (str):
-            longitude (str):
-            deleted (bool): Whether or not the payee location has been deleted.  Deleted payee locations will only be included in delta requests.
+            name (str, none_type): The name of the account
+            type (str, none_type): The account type
+            balance (int, none_type): The current balance of the account in milliunits format
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -170,19 +184,17 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (
             self.__class__, )
 
-        self.id = id
-        self.payee_id = payee_id
-        self.latitude = latitude
-        self.longitude = longitude
-        self.deleted = deleted
+        self.name = name
+        self.type = type
+        self.balance = balance
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -195,24 +207,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, payee_id, latitude, longitude, deleted, *args,
-                 **kwargs):  # noqa: E501
-        """PayeeLocation - a model defined in OpenAPI
+    def __init__(self, name, type, balance, *args, **kwargs):  # noqa: E501
+        """SaveAccount - a model defined in OpenAPI
 
         Args:
-            id (str):
-            payee_id (str):
-            latitude (str):
-            longitude (str):
-            deleted (bool): Whether or not the payee location has been deleted.  Deleted payee locations will only be included in delta requests.
+            name (str, none_type): The name of the account
+            type (str, none_type): The account type
+            balance (int, none_type): The current balance of the account in milliunits format
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -264,19 +273,17 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (
             self.__class__, )
 
-        self.id = id
-        self.payee_id = payee_id
-        self.latitude = latitude
-        self.longitude = longitude
-        self.deleted = deleted
+        self.name = name
+        self.type = type
+        self.balance = balance
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `ynab-api-2.0.0/ynab_api/model/payee_location_response.py` & `ynab-api-2.0.2/ynab_api/model/payee_location_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/payee_location_response_data.py` & `ynab-api-2.0.2/ynab_api/model/payee_location_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/payee_locations_response.py` & `ynab-api-2.0.2/ynab_api/model/payee_locations_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/payee_locations_response_data.py` & `ynab-api-2.0.2/ynab_api/model/payee_locations_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/payee_response.py` & `ynab-api-2.0.2/ynab_api/model/payee_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/payee_response_data.py` & `ynab-api-2.0.2/ynab_api/model/payee_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/payees_response.py` & `ynab-api-2.0.2/ynab_api/model/payees_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/payees_response_data.py` & `ynab-api-2.0.2/ynab_api/model/payees_response_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -82,15 +82,18 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'payees': ([Payee], ),  # noqa: E501
-            'server_knowledge': (int, ),  # noqa: E501
+            'server_knowledge': (
+                int,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -106,15 +109,15 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, payees, server_knowledge, *args,
                            **kwargs):  # noqa: E501
         """PayeesResponseData - a model defined in OpenAPI
 
         Args:
             payees ([Payee]):
-            server_knowledge (int): The knowledge of the server
+            server_knowledge (int, none_type): The knowledge of the server
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -196,15 +199,15 @@
     @convert_js_args_to_python_args
     def __init__(self, payees, server_knowledge, *args,
                  **kwargs):  # noqa: E501
         """PayeesResponseData - a model defined in OpenAPI
 
         Args:
             payees ([Payee]):
-            server_knowledge (int): The knowledge of the server
+            server_knowledge (int, none_type): The knowledge of the server
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `ynab-api-2.0.0/ynab_api/model/save_account.py` & `ynab-api-2.0.2/ynab_api/model/transaction_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -15,15 +15,20 @@
     change_keys_js_to_python, convert_js_args_to_python_args, date, datetime,
     file_type, none_type, validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from ynab_api.exceptions import ApiAttributeError
 
 
-class SaveAccount(ModelNormal):
+def lazy_import():
+    from ynab_api.model.transaction_response_data import TransactionResponseData
+    globals()['TransactionResponseData'] = TransactionResponseData
+
+
+class TransactionResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -39,34 +44,25 @@
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
-    allowed_values = {
-        ('type', ): {
-            'CHECKING': "checking",
-            'SAVINGS': "savings",
-            'CREDITCARD': "creditCard",
-            'CASH': "cash",
-            'LINEOFCREDIT': "lineOfCredit",
-            'OTHERASSET': "otherAsset",
-            'OTHERLIABILITY': "otherLiability",
-        },
-    }
+    allowed_values = {}
 
     validations = {}
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (
             bool,
             date,
             datetime,
             dict,
             float,
             int,
@@ -83,44 +79,38 @@
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'name': (str, ),  # noqa: E501
-            'type': (str, ),  # noqa: E501
-            'balance': (int, ),  # noqa: E501
+            'data': (TransactionResponseData, ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
-        'type': 'type',  # noqa: E501
-        'balance': 'balance',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {}
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, type, balance, *args,
-                           **kwargs):  # noqa: E501
-        """SaveAccount - a model defined in OpenAPI
+    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
+        """TransactionResponse - a model defined in OpenAPI
 
         Args:
-            name (str): The name of the account
-            type (str): The account type
-            balance (int): The current balance of the account in milliunits format
+            data (TransactionResponseData):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -174,17 +164,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (
             self.__class__, )
 
-        self.name = name
-        self.type = type
-        self.balance = balance
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -197,21 +185,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, type, balance, *args, **kwargs):  # noqa: E501
-        """SaveAccount - a model defined in OpenAPI
+    def __init__(self, data, *args, **kwargs):  # noqa: E501
+        """TransactionResponse - a model defined in OpenAPI
 
         Args:
-            name (str): The name of the account
-            type (str): The account type
-            balance (int): The current balance of the account in milliunits format
+            data (TransactionResponseData):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -263,17 +249,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (
             self.__class__, )
 
-        self.name = name
-        self.type = type
-        self.balance = balance
+        self.data = data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `ynab-api-2.0.0/ynab_api/model/save_account_wrapper.py` & `ynab-api-2.0.2/ynab_api/model/save_account_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/save_category_response.py` & `ynab-api-2.0.2/ynab_api/model/save_category_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/save_category_response_data.py` & `ynab-api-2.0.2/ynab_api/model/save_category_response_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -82,15 +82,18 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'category': (Category, ),  # noqa: E501
-            'server_knowledge': (int, ),  # noqa: E501
+            'server_knowledge': (
+                int,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -106,15 +109,15 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, category, server_knowledge, *args,
                            **kwargs):  # noqa: E501
         """SaveCategoryResponseData - a model defined in OpenAPI
 
         Args:
             category (Category):
-            server_knowledge (int): The knowledge of the server
+            server_knowledge (int, none_type): The knowledge of the server
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -196,15 +199,15 @@
     @convert_js_args_to_python_args
     def __init__(self, category, server_knowledge, *args,
                  **kwargs):  # noqa: E501
         """SaveCategoryResponseData - a model defined in OpenAPI
 
         Args:
             category (Category):
-            server_knowledge (int): The knowledge of the server
+            server_knowledge (int, none_type): The knowledge of the server
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `ynab-api-2.0.0/ynab_api/model/save_month_category.py` & `ynab-api-2.0.2/ynab_api/model/save_month_category.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -74,15 +74,18 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'budgeted': (int, ),  # noqa: E501
+            'budgeted': (
+                int,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -95,15 +98,15 @@
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, budgeted, *args, **kwargs):  # noqa: E501
         """SaveMonthCategory - a model defined in OpenAPI
 
         Args:
-            budgeted (int): Budgeted amount in milliunits format
+            budgeted (int, none_type): Budgeted amount in milliunits format
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -182,15 +185,15 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, budgeted, *args, **kwargs):  # noqa: E501
         """SaveMonthCategory - a model defined in OpenAPI
 
         Args:
-            budgeted (int): Budgeted amount in milliunits format
+            budgeted (int, none_type): Budgeted amount in milliunits format
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `ynab-api-2.0.0/ynab_api/model/save_month_category_wrapper.py` & `ynab-api-2.0.2/ynab_api/model/save_month_category_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/save_sub_transaction.py` & `ynab-api-2.0.2/ynab_api/model/save_sub_transaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -81,19 +81,34 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'amount': (int, ),  # noqa: E501
-            'payee_id': (str, ),  # noqa: E501
-            'payee_name': (str, ),  # noqa: E501
-            'category_id': (str, ),  # noqa: E501
-            'memo': (str, ),  # noqa: E501
+            'amount': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'payee_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'payee_name': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'category_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'memo': (
+                str,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -110,15 +125,15 @@
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, amount, *args, **kwargs):  # noqa: E501
         """SaveSubTransaction - a model defined in OpenAPI
 
         Args:
-            amount (int): The subtransaction amount in milliunits format.
+            amount (int, none_type): The subtransaction amount in milliunits format.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,18 +158,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            payee_id (str): The payee for the subtransaction.. [optional]  # noqa: E501
-            payee_name (str): The payee name.  If a `payee_name` value is provided and `payee_id` has a null value, the `payee_name` value will be used to resolve the payee by either (1) a matching payee rename rule (only if import_id is also specified on parent transaction) or (2) a payee with the same name or (3) creation of a new payee.. [optional]  # noqa: E501
-            category_id (str): The category for the subtransaction.  Credit Card Payment categories are not permitted and will be ignored if supplied.. [optional]  # noqa: E501
-            memo (str): [optional]  # noqa: E501
+            payee_id (str, none_type): The payee for the subtransaction.. [optional]  # noqa: E501
+            payee_name (str, none_type): The payee name.  If a `payee_name` value is provided and `payee_id` has a null value, the `payee_name` value will be used to resolve the payee by either (1) a matching payee rename rule (only if import_id is also specified on parent transaction) or (2) a payee with the same name or (3) creation of a new payee.. [optional]  # noqa: E501
+            category_id (str, none_type): The category for the subtransaction.  Credit Card Payment categories are not permitted and will be ignored if supplied.. [optional]  # noqa: E501
+            memo (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -201,15 +216,15 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, amount, *args, **kwargs):  # noqa: E501
         """SaveSubTransaction - a model defined in OpenAPI
 
         Args:
-            amount (int): The subtransaction amount in milliunits format.
+            amount (int, none_type): The subtransaction amount in milliunits format.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -234,18 +249,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            payee_id (str): The payee for the subtransaction.. [optional]  # noqa: E501
-            payee_name (str): The payee name.  If a `payee_name` value is provided and `payee_id` has a null value, the `payee_name` value will be used to resolve the payee by either (1) a matching payee rename rule (only if import_id is also specified on parent transaction) or (2) a payee with the same name or (3) creation of a new payee.. [optional]  # noqa: E501
-            category_id (str): The category for the subtransaction.  Credit Card Payment categories are not permitted and will be ignored if supplied.. [optional]  # noqa: E501
-            memo (str): [optional]  # noqa: E501
+            payee_id (str, none_type): The payee for the subtransaction.. [optional]  # noqa: E501
+            payee_name (str, none_type): The payee name.  If a `payee_name` value is provided and `payee_id` has a null value, the `payee_name` value will be used to resolve the payee by either (1) a matching payee rename rule (only if import_id is also specified on parent transaction) or (2) a payee with the same name or (3) creation of a new payee.. [optional]  # noqa: E501
+            category_id (str, none_type): The category for the subtransaction.  Credit Card Payment categories are not permitted and will be ignored if supplied.. [optional]  # noqa: E501
+            memo (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ynab-api-2.0.0/ynab_api/model/save_transaction.py` & `ynab-api-2.0.2/ynab_api/model/update_transaction.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -17,18 +17,22 @@
 )
 from ..model_utils import OpenApiModel
 from ynab_api.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from ynab_api.model.save_sub_transaction import SaveSubTransaction
+    from ynab_api.model.save_transaction import SaveTransaction
+    from ynab_api.model.update_transaction_all_of import UpdateTransactionAllOf
     globals()['SaveSubTransaction'] = SaveSubTransaction
+    globals()['SaveTransaction'] = SaveTransaction
+    globals()['UpdateTransactionAllOf'] = UpdateTransactionAllOf
 
 
-class SaveTransaction(ModelNormal):
+class UpdateTransaction(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -46,19 +50,21 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('cleared', ): {
+            'None': None,
             'CLEARED': "cleared",
             'UNCLEARED': "uncleared",
             'RECONCILED': "reconciled",
         },
         ('flag_color', ): {
+            'None': None,
             'RED': "red",
             'ORANGE': "orange",
             'YELLOW': "yellow",
             'GREEN': "green",
             'BLUE': "blue",
             'PURPLE': "purple",
         },
@@ -105,33 +111,68 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'account_id': (str, ),  # noqa: E501
-            'date': (date, ),  # noqa: E501
-            'amount': (int, ),  # noqa: E501
-            'payee_id': (str, ),  # noqa: E501
-            'payee_name': (str, ),  # noqa: E501
-            'category_id': (str, ),  # noqa: E501
-            'memo': (str, ),  # noqa: E501
-            'cleared': (str, ),  # noqa: E501
+            'id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'account_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'date': (
+                date,
+                none_type,
+            ),  # noqa: E501
+            'amount': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'payee_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'payee_name': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'category_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'memo': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'cleared': (
+                str,
+                none_type,
+            ),  # noqa: E501
             'approved': (bool, ),  # noqa: E501
-            'flag_color': (str, ),  # noqa: E501
-            'import_id': (str, ),  # noqa: E501
+            'flag_color': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'import_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
             'subtransactions': ([SaveSubTransaction], ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
+        'id': 'id',  # noqa: E501
         'account_id': 'account_id',  # noqa: E501
         'date': 'date',  # noqa: E501
         'amount': 'amount',  # noqa: E501
         'payee_id': 'payee_id',  # noqa: E501
         'payee_name': 'payee_name',  # noqa: E501
         'category_id': 'category_id',  # noqa: E501
         'memo': 'memo',  # noqa: E501
@@ -140,28 +181,24 @@
         'flag_color': 'flag_color',  # noqa: E501
         'import_id': 'import_id',  # noqa: E501
         'subtransactions': 'subtransactions',  # noqa: E501
     }
 
     read_only_vars = {}
 
-    _composed_schemas = {}
-
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, account_id, date, amount, *args,
-                           **kwargs):  # noqa: E501
-        """SaveTransaction - a model defined in OpenAPI
-
-        Args:
-            account_id (str):
-            date (date): The transaction date in ISO format (e.g. 2016-12-01).  Future dates (scheduled transactions) are not permitted.  Split transaction dates cannot be changed and if a different date is supplied it will be ignored.
-            amount (int): The transaction amount in milliunits format.  Split transaction amounts cannot be changed and if a different amount is supplied it will be ignored.
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """UpdateTransaction - a model defined in OpenAPI
 
         Keyword Args:
+            id (str, none_type):
+            account_id (str, none_type):
+            date (date, none_type): The transaction date in ISO format (e.g. 2016-12-01).  Future dates (scheduled transactions) are not permitted.  Split transaction dates cannot be changed and if a different date is supplied it will be ignored.
+            amount (int, none_type): The transaction amount in milliunits format.  Split transaction amounts cannot be changed and if a different amount is supplied it will be ignored.
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -184,22 +221,22 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            payee_id (str): The payee for the transaction.  To create a transfer between two accounts, use the account transfer payee pointing to the target account.  Account transfer payees are specified as `tranfer_payee_id` on the account resource.. [optional]  # noqa: E501
-            payee_name (str): The payee name.  If a `payee_name` value is provided and `payee_id` has a null value, the `payee_name` value will be used to resolve the payee by either (1) a matching payee rename rule (only if `import_id` is also specified) or (2) a payee with the same name or (3) creation of a new payee.. [optional]  # noqa: E501
-            category_id (str): The category for the transaction.  To configure a split transaction, you can specify null for `category_id` and provide a `subtransactions` array as part of the transaction object.  If an existing transaction is a split, the `category_id` cannot be changed.  Credit Card Payment categories are not permitted and will be ignored if supplied.. [optional]  # noqa: E501
-            memo (str): [optional]  # noqa: E501
-            cleared (str): The cleared status of the transaction. [optional]  # noqa: E501
+            payee_id (str, none_type): The payee for the transaction.  To create a transfer between two accounts, use the account transfer payee pointing to the target account.  Account transfer payees are specified as `tranfer_payee_id` on the account resource.. [optional]  # noqa: E501
+            payee_name (str, none_type): The payee name.  If a `payee_name` value is provided and `payee_id` has a null value, the `payee_name` value will be used to resolve the payee by either (1) a matching payee rename rule (only if `import_id` is also specified) or (2) a payee with the same name or (3) creation of a new payee.. [optional]  # noqa: E501
+            category_id (str, none_type): The category for the transaction.  To configure a split transaction, you can specify null for `category_id` and provide a `subtransactions` array as part of the transaction object.  If an existing transaction is a split, the `category_id` cannot be changed.  Credit Card Payment categories are not permitted and will be ignored if supplied.. [optional]  # noqa: E501
+            memo (str, none_type): [optional]  # noqa: E501
+            cleared (str, none_type): The cleared status of the transaction. [optional]  # noqa: E501
             approved (bool): Whether or not the transaction is approved.  If not supplied, transaction will be unapproved by default.. [optional]  # noqa: E501
-            flag_color (str): The transaction flag. [optional]  # noqa: E501
-            import_id (str): If specified, the new transaction will be assigned this `import_id` and considered \"imported\".  We will also attempt to match this imported transaction to an existing \"user-entered\" transation on the same account, with the same amount, and with a date +/-10 days from the imported transaction date.<br><br>Transactions imported through File Based Import or Direct Import (not through the API) are assigned an import_id in the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'. For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.  Using a consistent format will prevent duplicates through Direct Import and File Based Import.<br><br>If import_id is omitted or specified as null, the transaction will be treated as a \"user-entered\" transaction. As such, it will be eligible to be matched against transactions later being imported (via DI, FBI, or API).. [optional]  # noqa: E501
+            flag_color (str, none_type): The transaction flag. [optional]  # noqa: E501
+            import_id (str, none_type): If specified, the new transaction will be assigned this `import_id` and considered \"imported\".  We will also attempt to match this imported transaction to an existing \"user-entered\" transation on the same account, with the same amount, and with a date +/-10 days from the imported transaction date.<br><br>Transactions imported through File Based Import or Direct Import (not through the API) are assigned an import_id in the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'. For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.  Using a consistent format will prevent duplicates through Direct Import and File Based Import.<br><br>If import_id is omitted or specified as null, the transaction will be treated as a \"user-entered\" transaction. As such, it will be eligible to be matched against transactions later being imported (via DI, FBI, or API).. [optional]  # noqa: E501
             subtransactions ([SaveSubTransaction]): An array of subtransactions to configure a transaction as a split.  Updating `subtransactions` on an existing split transaction is not supported.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -222,47 +259,59 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (
             self.__class__, )
 
-        self.account_id = account_id
-        self.date = date
-        self.amount = amount
+        constant_args = {
+            '_check_type': _check_type,
+            '_path_to_item': _path_to_item,
+            '_spec_property_naming': _spec_property_naming,
+            '_configuration': _configuration,
+            '_visited_composed_classes': self._visited_composed_classes,
+        }
+        composed_info = validate_get_composed_info(constant_args, kwargs, self)
+        self._composed_instances = composed_info[0]
+        self._var_name_to_model_instances = composed_info[1]
+        self._additional_properties_model_instances = composed_info[2]
+        discarded_args = composed_info[3]
+
         for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
+            if var_name in discarded_args and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
+                        self._additional_properties_model_instances:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
+
         return self
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
+        '_composed_instances',
+        '_var_name_to_model_instances',
+        '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, account_id, date, amount, *args,
-                 **kwargs):  # noqa: E501
-        """SaveTransaction - a model defined in OpenAPI
-
-        Args:
-            account_id (str):
-            date (date): The transaction date in ISO format (e.g. 2016-12-01).  Future dates (scheduled transactions) are not permitted.  Split transaction dates cannot be changed and if a different date is supplied it will be ignored.
-            amount (int): The transaction amount in milliunits format.  Split transaction amounts cannot be changed and if a different amount is supplied it will be ignored.
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """UpdateTransaction - a model defined in OpenAPI
 
         Keyword Args:
+            id (str, none_type):
+            account_id (str, none_type):
+            date (date, none_type): The transaction date in ISO format (e.g. 2016-12-01).  Future dates (scheduled transactions) are not permitted.  Split transaction dates cannot be changed and if a different date is supplied it will be ignored.
+            amount (int, none_type): The transaction amount in milliunits format.  Split transaction amounts cannot be changed and if a different amount is supplied it will be ignored.
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -285,22 +334,22 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            payee_id (str): The payee for the transaction.  To create a transfer between two accounts, use the account transfer payee pointing to the target account.  Account transfer payees are specified as `tranfer_payee_id` on the account resource.. [optional]  # noqa: E501
-            payee_name (str): The payee name.  If a `payee_name` value is provided and `payee_id` has a null value, the `payee_name` value will be used to resolve the payee by either (1) a matching payee rename rule (only if `import_id` is also specified) or (2) a payee with the same name or (3) creation of a new payee.. [optional]  # noqa: E501
-            category_id (str): The category for the transaction.  To configure a split transaction, you can specify null for `category_id` and provide a `subtransactions` array as part of the transaction object.  If an existing transaction is a split, the `category_id` cannot be changed.  Credit Card Payment categories are not permitted and will be ignored if supplied.. [optional]  # noqa: E501
-            memo (str): [optional]  # noqa: E501
-            cleared (str): The cleared status of the transaction. [optional]  # noqa: E501
+            payee_id (str, none_type): The payee for the transaction.  To create a transfer between two accounts, use the account transfer payee pointing to the target account.  Account transfer payees are specified as `tranfer_payee_id` on the account resource.. [optional]  # noqa: E501
+            payee_name (str, none_type): The payee name.  If a `payee_name` value is provided and `payee_id` has a null value, the `payee_name` value will be used to resolve the payee by either (1) a matching payee rename rule (only if `import_id` is also specified) or (2) a payee with the same name or (3) creation of a new payee.. [optional]  # noqa: E501
+            category_id (str, none_type): The category for the transaction.  To configure a split transaction, you can specify null for `category_id` and provide a `subtransactions` array as part of the transaction object.  If an existing transaction is a split, the `category_id` cannot be changed.  Credit Card Payment categories are not permitted and will be ignored if supplied.. [optional]  # noqa: E501
+            memo (str, none_type): [optional]  # noqa: E501
+            cleared (str, none_type): The cleared status of the transaction. [optional]  # noqa: E501
             approved (bool): Whether or not the transaction is approved.  If not supplied, transaction will be unapproved by default.. [optional]  # noqa: E501
-            flag_color (str): The transaction flag. [optional]  # noqa: E501
-            import_id (str): If specified, the new transaction will be assigned this `import_id` and considered \"imported\".  We will also attempt to match this imported transaction to an existing \"user-entered\" transation on the same account, with the same amount, and with a date +/-10 days from the imported transaction date.<br><br>Transactions imported through File Based Import or Direct Import (not through the API) are assigned an import_id in the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'. For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.  Using a consistent format will prevent duplicates through Direct Import and File Based Import.<br><br>If import_id is omitted or specified as null, the transaction will be treated as a \"user-entered\" transaction. As such, it will be eligible to be matched against transactions later being imported (via DI, FBI, or API).. [optional]  # noqa: E501
+            flag_color (str, none_type): The transaction flag. [optional]  # noqa: E501
+            import_id (str, none_type): If specified, the new transaction will be assigned this `import_id` and considered \"imported\".  We will also attempt to match this imported transaction to an existing \"user-entered\" transation on the same account, with the same amount, and with a date +/-10 days from the imported transaction date.<br><br>Transactions imported through File Based Import or Direct Import (not through the API) are assigned an import_id in the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'. For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.  Using a consistent format will prevent duplicates through Direct Import and File Based Import.<br><br>If import_id is omitted or specified as null, the transaction will be treated as a \"user-entered\" transaction. As such, it will be eligible to be matched against transactions later being imported (via DI, FBI, or API).. [optional]  # noqa: E501
             subtransactions ([SaveSubTransaction]): An array of subtransactions to configure a transaction as a split.  Updating `subtransactions` on an existing split transaction is not supported.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -321,22 +370,51 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (
             self.__class__, )
 
-        self.account_id = account_id
-        self.date = date
-        self.amount = amount
+        constant_args = {
+            '_check_type': _check_type,
+            '_path_to_item': _path_to_item,
+            '_spec_property_naming': _spec_property_naming,
+            '_configuration': _configuration,
+            '_visited_composed_classes': self._visited_composed_classes,
+        }
+        composed_info = validate_get_composed_info(constant_args, kwargs, self)
+        self._composed_instances = composed_info[0]
+        self._var_name_to_model_instances = composed_info[1]
+        self._additional_properties_model_instances = composed_info[2]
+        discarded_args = composed_info[3]
+
         for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
+            if var_name in discarded_args and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
+                        self._additional_properties_model_instances:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
             if var_name in self.read_only_vars:
                 raise ApiAttributeError(
                     f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
                     f"class with read only attributes.")
+
+    @cached_property
+    def _composed_schemas():
+        # we need this here to make our import statements work
+        # we must store _composed_schemas in here so the code is only run
+        # when we invoke this method. If we kept this at the class
+        # level we would get an error because the class level
+        # code would be run when this module is imported, and these composed
+        # classes don't exist yet because their module has not finished
+        # loading
+        lazy_import()
+        return {
+            'anyOf': [],
+            'allOf': [
+                SaveTransaction,
+                UpdateTransactionAllOf,
+            ],
+            'oneOf': [],
+        }
```

### Comparing `ynab-api-2.0.0/ynab_api/model/save_transaction_wrapper.py` & `ynab-api-2.0.2/ynab_api/model/transaction_response_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -16,19 +16,19 @@
     file_type, none_type, validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from ynab_api.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from ynab_api.model.save_transaction import SaveTransaction
-    globals()['SaveTransaction'] = SaveTransaction
+    from ynab_api.model.transaction_detail import TransactionDetail
+    globals()['TransactionDetail'] = TransactionDetail
 
 
-class SaveTransactionWrapper(ModelNormal):
+class TransactionResponseData(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -81,15 +81,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'transaction': (SaveTransaction, ),  # noqa: E501
+            'transaction': (TransactionDetail, ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -99,18 +99,18 @@
     read_only_vars = {}
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, transaction, *args, **kwargs):  # noqa: E501
-        """SaveTransactionWrapper - a model defined in OpenAPI
+        """TransactionResponseData - a model defined in OpenAPI
 
         Args:
-            transaction (SaveTransaction):
+            transaction (TransactionDetail):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -186,18 +186,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, transaction, *args, **kwargs):  # noqa: E501
-        """SaveTransactionWrapper - a model defined in OpenAPI
+        """TransactionResponseData - a model defined in OpenAPI
 
         Args:
-            transaction (SaveTransaction):
+            transaction (TransactionDetail):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `ynab-api-2.0.0/ynab_api/model/save_transactions_response.py` & `ynab-api-2.0.2/ynab_api/model/save_transactions_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/save_transactions_response_data.py` & `ynab-api-2.0.2/ynab_api/model/save_transactions_response_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -81,19 +81,22 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'transaction_ids': ([str], ),  # noqa: E501
-            'server_knowledge': (int, ),  # noqa: E501
+            'transaction_ids': ([str, none_type], ),  # noqa: E501
+            'server_knowledge': (
+                int,
+                none_type,
+            ),  # noqa: E501
             'transaction': (TransactionDetail, ),  # noqa: E501
             'transactions': ([TransactionDetail], ),  # noqa: E501
-            'duplicate_import_ids': ([str], ),  # noqa: E501
+            'duplicate_import_ids': ([str, none_type], ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -111,16 +114,16 @@
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, transaction_ids, server_knowledge, *args,
                            **kwargs):  # noqa: E501
         """SaveTransactionsResponseData - a model defined in OpenAPI
 
         Args:
-            transaction_ids ([str]): The transaction ids that were saved
-            server_knowledge (int): The knowledge of the server
+            transaction_ids ([str, none_type]): The transaction ids that were saved
+            server_knowledge (int, none_type): The knowledge of the server
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -147,15 +150,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             transaction (TransactionDetail): [optional]  # noqa: E501
             transactions ([TransactionDetail]): If multiple transactions were specified, the transactions that were saved. [optional]  # noqa: E501
-            duplicate_import_ids ([str]): If multiple transactions were specified, a list of import_ids that were not created because of an existing `import_id` found on the same account. [optional]  # noqa: E501
+            duplicate_import_ids ([str, none_type]): If multiple transactions were specified, a list of import_ids that were not created because of an existing `import_id` found on the same account. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -204,16 +207,16 @@
 
     @convert_js_args_to_python_args
     def __init__(self, transaction_ids, server_knowledge, *args,
                  **kwargs):  # noqa: E501
         """SaveTransactionsResponseData - a model defined in OpenAPI
 
         Args:
-            transaction_ids ([str]): The transaction ids that were saved
-            server_knowledge (int): The knowledge of the server
+            transaction_ids ([str, none_type]): The transaction ids that were saved
+            server_knowledge (int, none_type): The knowledge of the server
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -240,15 +243,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             transaction (TransactionDetail): [optional]  # noqa: E501
             transactions ([TransactionDetail]): If multiple transactions were specified, the transactions that were saved. [optional]  # noqa: E501
-            duplicate_import_ids ([str]): If multiple transactions were specified, a list of import_ids that were not created because of an existing `import_id` found on the same account. [optional]  # noqa: E501
+            duplicate_import_ids ([str, none_type]): If multiple transactions were specified, a list of import_ids that were not created because of an existing `import_id` found on the same account. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ynab-api-2.0.0/ynab_api/model/save_transactions_wrapper.py` & `ynab-api-2.0.2/ynab_api/model/save_transactions_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/scheduled_sub_transaction.py` & `ynab-api-2.0.2/ynab_api/model/payee_location.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -15,15 +15,15 @@
     change_keys_js_to_python, convert_js_args_to_python_args, date, datetime,
     file_type, none_type, validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from ynab_api.exceptions import ApiAttributeError
 
 
-class ScheduledSubTransaction(ModelNormal):
+class PayeeLocation(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -74,54 +74,61 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (str, ),  # noqa: E501
-            'scheduled_transaction_id': (str, ),  # noqa: E501
-            'amount': (int, ),  # noqa: E501
+            'id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'payee_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'latitude': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'longitude': (
+                str,
+                none_type,
+            ),  # noqa: E501
             'deleted': (bool, ),  # noqa: E501
-            'memo': (str, ),  # noqa: E501
-            'payee_id': (str, ),  # noqa: E501
-            'category_id': (str, ),  # noqa: E501
-            'transfer_account_id': (str, ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
         'id': 'id',  # noqa: E501
-        'scheduled_transaction_id': 'scheduled_transaction_id',  # noqa: E501
-        'amount': 'amount',  # noqa: E501
-        'deleted': 'deleted',  # noqa: E501
-        'memo': 'memo',  # noqa: E501
         'payee_id': 'payee_id',  # noqa: E501
-        'category_id': 'category_id',  # noqa: E501
-        'transfer_account_id': 'transfer_account_id',  # noqa: E501
+        'latitude': 'latitude',  # noqa: E501
+        'longitude': 'longitude',  # noqa: E501
+        'deleted': 'deleted',  # noqa: E501
     }
 
     read_only_vars = {}
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, scheduled_transaction_id, amount, deleted,
+    def _from_openapi_data(cls, id, payee_id, latitude, longitude, deleted,
                            *args, **kwargs):  # noqa: E501
-        """ScheduledSubTransaction - a model defined in OpenAPI
+        """PayeeLocation - a model defined in OpenAPI
 
         Args:
-            id (str):
-            scheduled_transaction_id (str):
-            amount (int): The scheduled subtransaction amount in milliunits format
-            deleted (bool): Whether or not the scheduled subtransaction has been deleted.  Deleted scheduled subtransactions will only be included in delta requests.
+            id (str, none_type):
+            payee_id (str, none_type):
+            latitude (str, none_type):
+            longitude (str, none_type):
+            deleted (bool): Whether or not the payee location has been deleted.  Deleted payee locations will only be included in delta requests.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -146,18 +153,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            memo (str): [optional]  # noqa: E501
-            payee_id (str): [optional]  # noqa: E501
-            category_id (str): [optional]  # noqa: E501
-            transfer_account_id (str): If a transfer, the account_id which the scheduled subtransaction transfers to. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -180,16 +183,17 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (
             self.__class__, )
 
         self.id = id
-        self.scheduled_transaction_id = scheduled_transaction_id
-        self.amount = amount
+        self.payee_id = payee_id
+        self.latitude = latitude
+        self.longitude = longitude
         self.deleted = deleted
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
@@ -203,23 +207,24 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, scheduled_transaction_id, amount, deleted, *args,
+    def __init__(self, id, payee_id, latitude, longitude, deleted, *args,
                  **kwargs):  # noqa: E501
-        """ScheduledSubTransaction - a model defined in OpenAPI
+        """PayeeLocation - a model defined in OpenAPI
 
         Args:
-            id (str):
-            scheduled_transaction_id (str):
-            amount (int): The scheduled subtransaction amount in milliunits format
-            deleted (bool): Whether or not the scheduled subtransaction has been deleted.  Deleted scheduled subtransactions will only be included in delta requests.
+            id (str, none_type):
+            payee_id (str, none_type):
+            latitude (str, none_type):
+            longitude (str, none_type):
+            deleted (bool): Whether or not the payee location has been deleted.  Deleted payee locations will only be included in delta requests.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -244,18 +249,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            memo (str): [optional]  # noqa: E501
-            payee_id (str): [optional]  # noqa: E501
-            category_id (str): [optional]  # noqa: E501
-            transfer_account_id (str): If a transfer, the account_id which the scheduled subtransaction transfers to. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -276,16 +277,17 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (
             self.__class__, )
 
         self.id = id
-        self.scheduled_transaction_id = scheduled_transaction_id
-        self.amount = amount
+        self.payee_id = payee_id
+        self.latitude = latitude
+        self.longitude = longitude
         self.deleted = deleted
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
```

### Comparing `ynab-api-2.0.0/ynab_api/model/scheduled_transaction_detail.py` & `ynab-api-2.0.2/ynab_api/model/scheduled_transaction_detail.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -51,14 +51,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('frequency', ): {
+            'None': None,
             'NEVER': "never",
             'DAILY': "daily",
             'WEEKLY': "weekly",
             'EVERYOTHERWEEK': "everyOtherWeek",
             'TWICEAMONTH': "twiceAMonth",
             'EVERY4WEEKS': "every4Weeks",
             'MONTHLY': "monthly",
@@ -66,14 +67,15 @@
             'EVERY3MONTHS': "every3Months",
             'EVERY4MONTHS': "every4Months",
             'TWICEAYEAR': "twiceAYear",
             'YEARLY': "yearly",
             'EVERYOTHERYEAR': "everyOtherYear",
         },
         ('flag_color', ): {
+            'None': None,
             'RED': "red",
             'ORANGE': "orange",
             'YELLOW': "yellow",
             'GREEN': "green",
             'BLUE': "blue",
             'PURPLE': "purple",
         },
@@ -110,30 +112,72 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'id': (str, ),  # noqa: E501
-            'date_first': (date, ),  # noqa: E501
-            'date_next': (date, ),  # noqa: E501
-            'frequency': (str, ),  # noqa: E501
-            'amount': (int, ),  # noqa: E501
-            'account_id': (str, ),  # noqa: E501
+            'id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'date_first': (
+                date,
+                none_type,
+            ),  # noqa: E501
+            'date_next': (
+                date,
+                none_type,
+            ),  # noqa: E501
+            'frequency': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'amount': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'account_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
             'deleted': (bool, ),  # noqa: E501
-            'account_name': (str, ),  # noqa: E501
+            'account_name': (
+                str,
+                none_type,
+            ),  # noqa: E501
             'subtransactions': ([ScheduledSubTransaction], ),  # noqa: E501
-            'memo': (str, ),  # noqa: E501
-            'flag_color': (str, ),  # noqa: E501
-            'payee_id': (str, ),  # noqa: E501
-            'category_id': (str, ),  # noqa: E501
-            'transfer_account_id': (str, ),  # noqa: E501
-            'payee_name': (str, ),  # noqa: E501
-            'category_name': (str, ),  # noqa: E501
+            'memo': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'flag_color': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'payee_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'category_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'transfer_account_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'payee_name': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'category_name': (
+                str,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -159,22 +203,22 @@
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """ScheduledTransactionDetail - a model defined in OpenAPI
 
         Keyword Args:
-            id (str):
-            date_first (date): The first date for which the Scheduled Transaction was scheduled.
-            date_next (date): The next date for which the Scheduled Transaction is scheduled.
-            frequency (str):
-            amount (int): The scheduled transaction amount in milliunits format
-            account_id (str):
+            id (str, none_type):
+            date_first (date, none_type): The first date for which the Scheduled Transaction was scheduled.
+            date_next (date, none_type): The next date for which the Scheduled Transaction is scheduled.
+            frequency (str, none_type):
+            amount (int, none_type): The scheduled transaction amount in milliunits format
+            account_id (str, none_type):
             deleted (bool): Whether or not the scheduled transaction has been deleted.  Deleted scheduled transactions will only be included in delta requests.
-            account_name (str):
+            account_name (str, none_type):
             subtransactions ([ScheduledSubTransaction]): If a split scheduled transaction, the subtransactions.
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -198,21 +242,21 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            memo (str): [optional]  # noqa: E501
-            flag_color (str): The scheduled transaction flag. [optional]  # noqa: E501
-            payee_id (str): [optional]  # noqa: E501
-            category_id (str): [optional]  # noqa: E501
-            transfer_account_id (str): If a transfer, the account_id which the scheduled transaction transfers to. [optional]  # noqa: E501
-            payee_name (str): [optional]  # noqa: E501
-            category_name (str): [optional]  # noqa: E501
+            memo (str, none_type): [optional]  # noqa: E501
+            flag_color (str, none_type): The scheduled transaction flag. [optional]  # noqa: E501
+            payee_id (str, none_type): [optional]  # noqa: E501
+            category_id (str, none_type): [optional]  # noqa: E501
+            transfer_account_id (str, none_type): If a transfer, the account_id which the scheduled transaction transfers to. [optional]  # noqa: E501
+            payee_name (str, none_type): [optional]  # noqa: E501
+            category_name (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -275,22 +319,22 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
         """ScheduledTransactionDetail - a model defined in OpenAPI
 
         Keyword Args:
-            id (str):
-            date_first (date): The first date for which the Scheduled Transaction was scheduled.
-            date_next (date): The next date for which the Scheduled Transaction is scheduled.
-            frequency (str):
-            amount (int): The scheduled transaction amount in milliunits format
-            account_id (str):
+            id (str, none_type):
+            date_first (date, none_type): The first date for which the Scheduled Transaction was scheduled.
+            date_next (date, none_type): The next date for which the Scheduled Transaction is scheduled.
+            frequency (str, none_type):
+            amount (int, none_type): The scheduled transaction amount in milliunits format
+            account_id (str, none_type):
             deleted (bool): Whether or not the scheduled transaction has been deleted.  Deleted scheduled transactions will only be included in delta requests.
-            account_name (str):
+            account_name (str, none_type):
             subtransactions ([ScheduledSubTransaction]): If a split scheduled transaction, the subtransactions.
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -314,21 +358,21 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            memo (str): [optional]  # noqa: E501
-            flag_color (str): The scheduled transaction flag. [optional]  # noqa: E501
-            payee_id (str): [optional]  # noqa: E501
-            category_id (str): [optional]  # noqa: E501
-            transfer_account_id (str): If a transfer, the account_id which the scheduled transaction transfers to. [optional]  # noqa: E501
-            payee_name (str): [optional]  # noqa: E501
-            category_name (str): [optional]  # noqa: E501
+            memo (str, none_type): [optional]  # noqa: E501
+            flag_color (str, none_type): The scheduled transaction flag. [optional]  # noqa: E501
+            payee_id (str, none_type): [optional]  # noqa: E501
+            category_id (str, none_type): [optional]  # noqa: E501
+            transfer_account_id (str, none_type): If a transfer, the account_id which the scheduled transaction transfers to. [optional]  # noqa: E501
+            payee_name (str, none_type): [optional]  # noqa: E501
+            category_name (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ynab-api-2.0.0/ynab_api/model/scheduled_transaction_detail_all_of.py` & `ynab-api-2.0.2/ynab_api/model/transaction_detail_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -16,19 +16,19 @@
     file_type, none_type, validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from ynab_api.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from ynab_api.model.scheduled_sub_transaction import ScheduledSubTransaction
-    globals()['ScheduledSubTransaction'] = ScheduledSubTransaction
+    from ynab_api.model.sub_transaction import SubTransaction
+    globals()['SubTransaction'] = SubTransaction
 
 
-class ScheduledTransactionDetailAllOf(ModelNormal):
+class TransactionDetailAllOf(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -81,18 +81,27 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'account_name': (str, ),  # noqa: E501
-            'subtransactions': ([ScheduledSubTransaction], ),  # noqa: E501
-            'payee_name': (str, ),  # noqa: E501
-            'category_name': (str, ),  # noqa: E501
+            'account_name': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'subtransactions': ([SubTransaction], ),  # noqa: E501
+            'payee_name': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'category_name': (
+                str,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -106,19 +115,19 @@
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, account_name, subtransactions, *args,
                            **kwargs):  # noqa: E501
-        """ScheduledTransactionDetailAllOf - a model defined in OpenAPI
+        """TransactionDetailAllOf - a model defined in OpenAPI
 
         Args:
-            account_name (str):
-            subtransactions ([ScheduledSubTransaction]): If a split scheduled transaction, the subtransactions.
+            account_name (str, none_type):
+            subtransactions ([SubTransaction]): If a split transaction, the subtransactions.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,16 +152,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            payee_name (str): [optional]  # noqa: E501
-            category_name (str): [optional]  # noqa: E501
+            payee_name (str, none_type): [optional]  # noqa: E501
+            category_name (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -198,19 +207,19 @@
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, account_name, subtransactions, *args,
                  **kwargs):  # noqa: E501
-        """ScheduledTransactionDetailAllOf - a model defined in OpenAPI
+        """TransactionDetailAllOf - a model defined in OpenAPI
 
         Args:
-            account_name (str):
-            subtransactions ([ScheduledSubTransaction]): If a split scheduled transaction, the subtransactions.
+            account_name (str, none_type):
+            subtransactions ([SubTransaction]): If a split transaction, the subtransactions.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -235,16 +244,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            payee_name (str): [optional]  # noqa: E501
-            category_name (str): [optional]  # noqa: E501
+            payee_name (str, none_type): [optional]  # noqa: E501
+            category_name (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ynab-api-2.0.0/ynab_api/model/scheduled_transaction_response.py` & `ynab-api-2.0.2/ynab_api/model/scheduled_transaction_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/scheduled_transaction_response_data.py` & `ynab-api-2.0.2/ynab_api/model/scheduled_transaction_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/scheduled_transaction_summary.py` & `ynab-api-2.0.2/ynab_api/model/scheduled_transaction_summary.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -41,14 +41,15 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('frequency', ): {
+            'None': None,
             'NEVER': "never",
             'DAILY': "daily",
             'WEEKLY': "weekly",
             'EVERYOTHERWEEK': "everyOtherWeek",
             'TWICEAMONTH': "twiceAMonth",
             'EVERY4WEEKS': "every4Weeks",
             'MONTHLY': "monthly",
@@ -56,14 +57,15 @@
             'EVERY3MONTHS': "every3Months",
             'EVERY4MONTHS': "every4Months",
             'TWICEAYEAR': "twiceAYear",
             'YEARLY': "yearly",
             'EVERYOTHERYEAR': "everyOtherYear",
         },
         ('flag_color', ): {
+            'None': None,
             'RED': "red",
             'ORANGE': "orange",
             'YELLOW': "yellow",
             'GREEN': "green",
             'BLUE': "blue",
             'PURPLE': "purple",
         },
@@ -98,26 +100,59 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (str, ),  # noqa: E501
-            'date_first': (date, ),  # noqa: E501
-            'date_next': (date, ),  # noqa: E501
-            'frequency': (str, ),  # noqa: E501
-            'amount': (int, ),  # noqa: E501
-            'account_id': (str, ),  # noqa: E501
+            'id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'date_first': (
+                date,
+                none_type,
+            ),  # noqa: E501
+            'date_next': (
+                date,
+                none_type,
+            ),  # noqa: E501
+            'frequency': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'amount': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'account_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
             'deleted': (bool, ),  # noqa: E501
-            'memo': (str, ),  # noqa: E501
-            'flag_color': (str, ),  # noqa: E501
-            'payee_id': (str, ),  # noqa: E501
-            'category_id': (str, ),  # noqa: E501
-            'transfer_account_id': (str, ),  # noqa: E501
+            'memo': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'flag_color': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'payee_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'category_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'transfer_account_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -142,20 +177,20 @@
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, id, date_first, date_next, frequency, amount,
                            account_id, deleted, *args, **kwargs):  # noqa: E501
         """ScheduledTransactionSummary - a model defined in OpenAPI
 
         Args:
-            id (str):
-            date_first (date): The first date for which the Scheduled Transaction was scheduled.
-            date_next (date): The next date for which the Scheduled Transaction is scheduled.
-            frequency (str):
-            amount (int): The scheduled transaction amount in milliunits format
-            account_id (str):
+            id (str, none_type):
+            date_first (date, none_type): The first date for which the Scheduled Transaction was scheduled.
+            date_next (date, none_type): The next date for which the Scheduled Transaction is scheduled.
+            frequency (str, none_type):
+            amount (int, none_type): The scheduled transaction amount in milliunits format
+            account_id (str, none_type):
             deleted (bool): Whether or not the scheduled transaction has been deleted.  Deleted scheduled transactions will only be included in delta requests.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -181,19 +216,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            memo (str): [optional]  # noqa: E501
-            flag_color (str): The scheduled transaction flag. [optional]  # noqa: E501
-            payee_id (str): [optional]  # noqa: E501
-            category_id (str): [optional]  # noqa: E501
-            transfer_account_id (str): If a transfer, the account_id which the scheduled transaction transfers to. [optional]  # noqa: E501
+            memo (str, none_type): [optional]  # noqa: E501
+            flag_color (str, none_type): The scheduled transaction flag. [optional]  # noqa: E501
+            payee_id (str, none_type): [optional]  # noqa: E501
+            category_id (str, none_type): [optional]  # noqa: E501
+            transfer_account_id (str, none_type): If a transfer, the account_id which the scheduled transaction transfers to. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -247,20 +282,20 @@
 
     @convert_js_args_to_python_args
     def __init__(self, id, date_first, date_next, frequency, amount,
                  account_id, deleted, *args, **kwargs):  # noqa: E501
         """ScheduledTransactionSummary - a model defined in OpenAPI
 
         Args:
-            id (str):
-            date_first (date): The first date for which the Scheduled Transaction was scheduled.
-            date_next (date): The next date for which the Scheduled Transaction is scheduled.
-            frequency (str):
-            amount (int): The scheduled transaction amount in milliunits format
-            account_id (str):
+            id (str, none_type):
+            date_first (date, none_type): The first date for which the Scheduled Transaction was scheduled.
+            date_next (date, none_type): The next date for which the Scheduled Transaction is scheduled.
+            frequency (str, none_type):
+            amount (int, none_type): The scheduled transaction amount in milliunits format
+            account_id (str, none_type):
             deleted (bool): Whether or not the scheduled transaction has been deleted.  Deleted scheduled transactions will only be included in delta requests.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -286,19 +321,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            memo (str): [optional]  # noqa: E501
-            flag_color (str): The scheduled transaction flag. [optional]  # noqa: E501
-            payee_id (str): [optional]  # noqa: E501
-            category_id (str): [optional]  # noqa: E501
-            transfer_account_id (str): If a transfer, the account_id which the scheduled transaction transfers to. [optional]  # noqa: E501
+            memo (str, none_type): [optional]  # noqa: E501
+            flag_color (str, none_type): The scheduled transaction flag. [optional]  # noqa: E501
+            payee_id (str, none_type): [optional]  # noqa: E501
+            category_id (str, none_type): [optional]  # noqa: E501
+            transfer_account_id (str, none_type): If a transfer, the account_id which the scheduled transaction transfers to. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ynab-api-2.0.0/ynab_api/model/scheduled_transactions_response.py` & `ynab-api-2.0.2/ynab_api/model/scheduled_transactions_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/scheduled_transactions_response_data.py` & `ynab-api-2.0.2/ynab_api/model/scheduled_transactions_response_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -83,15 +83,18 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'scheduled_transactions':
             ([ScheduledTransactionDetail], ),  # noqa: E501
-            'server_knowledge': (int, ),  # noqa: E501
+            'server_knowledge': (
+                int,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -107,15 +110,15 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, scheduled_transactions, server_knowledge,
                            *args, **kwargs):  # noqa: E501
         """ScheduledTransactionsResponseData - a model defined in OpenAPI
 
         Args:
             scheduled_transactions ([ScheduledTransactionDetail]):
-            server_knowledge (int): The knowledge of the server
+            server_knowledge (int, none_type): The knowledge of the server
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -197,15 +200,15 @@
     @convert_js_args_to_python_args
     def __init__(self, scheduled_transactions, server_knowledge, *args,
                  **kwargs):  # noqa: E501
         """ScheduledTransactionsResponseData - a model defined in OpenAPI
 
         Args:
             scheduled_transactions ([ScheduledTransactionDetail]):
-            server_knowledge (int): The knowledge of the server
+            server_knowledge (int, none_type): The knowledge of the server
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `ynab-api-2.0.0/ynab_api/model/sub_transaction.py` & `ynab-api-2.0.2/ynab_api/model/scheduled_sub_transaction.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -15,15 +15,15 @@
     change_keys_js_to_python, convert_js_args_to_python_args, date, datetime,
     file_type, none_type, validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from ynab_api.exceptions import ApiAttributeError
 
 
-class SubTransaction(ModelNormal):
+class ScheduledSubTransaction(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -74,60 +74,75 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (str, ),  # noqa: E501
-            'transaction_id': (str, ),  # noqa: E501
-            'amount': (int, ),  # noqa: E501
+            'id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'scheduled_transaction_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'amount': (
+                int,
+                none_type,
+            ),  # noqa: E501
             'deleted': (bool, ),  # noqa: E501
-            'memo': (str, ),  # noqa: E501
-            'payee_id': (str, ),  # noqa: E501
-            'payee_name': (str, ),  # noqa: E501
-            'category_id': (str, ),  # noqa: E501
-            'category_name': (str, ),  # noqa: E501
-            'transfer_account_id': (str, ),  # noqa: E501
-            'transfer_transaction_id': (str, ),  # noqa: E501
+            'memo': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'payee_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'category_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'transfer_account_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
         'id': 'id',  # noqa: E501
-        'transaction_id': 'transaction_id',  # noqa: E501
+        'scheduled_transaction_id': 'scheduled_transaction_id',  # noqa: E501
         'amount': 'amount',  # noqa: E501
         'deleted': 'deleted',  # noqa: E501
         'memo': 'memo',  # noqa: E501
         'payee_id': 'payee_id',  # noqa: E501
-        'payee_name': 'payee_name',  # noqa: E501
         'category_id': 'category_id',  # noqa: E501
-        'category_name': 'category_name',  # noqa: E501
         'transfer_account_id': 'transfer_account_id',  # noqa: E501
-        'transfer_transaction_id': 'transfer_transaction_id',  # noqa: E501
     }
 
     read_only_vars = {}
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, transaction_id, amount, deleted, *args,
-                           **kwargs):  # noqa: E501
-        """SubTransaction - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, scheduled_transaction_id, amount, deleted,
+                           *args, **kwargs):  # noqa: E501
+        """ScheduledSubTransaction - a model defined in OpenAPI
 
         Args:
-            id (str):
-            transaction_id (str):
-            amount (int): The subtransaction amount in milliunits format
-            deleted (bool): Whether or not the subtransaction has been deleted.  Deleted subtransactions will only be included in delta requests.
+            id (str, none_type):
+            scheduled_transaction_id (str, none_type):
+            amount (int, none_type): The scheduled subtransaction amount in milliunits format
+            deleted (bool): Whether or not the scheduled subtransaction has been deleted.  Deleted scheduled subtransactions will only be included in delta requests.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -152,21 +167,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            memo (str): [optional]  # noqa: E501
-            payee_id (str): [optional]  # noqa: E501
-            payee_name (str): [optional]  # noqa: E501
-            category_id (str): [optional]  # noqa: E501
-            category_name (str): [optional]  # noqa: E501
-            transfer_account_id (str): If a transfer, the account_id which the subtransaction transfers to. [optional]  # noqa: E501
-            transfer_transaction_id (str): If a transfer, the id of transaction on the other side of the transfer. [optional]  # noqa: E501
+            memo (str, none_type): [optional]  # noqa: E501
+            payee_id (str, none_type): [optional]  # noqa: E501
+            category_id (str, none_type): [optional]  # noqa: E501
+            transfer_account_id (str, none_type): If a transfer, the account_id which the scheduled subtransaction transfers to. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -189,15 +201,15 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (
             self.__class__, )
 
         self.id = id
-        self.transaction_id = transaction_id
+        self.scheduled_transaction_id = scheduled_transaction_id
         self.amount = amount
         self.deleted = deleted
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
@@ -212,23 +224,23 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, transaction_id, amount, deleted, *args,
+    def __init__(self, id, scheduled_transaction_id, amount, deleted, *args,
                  **kwargs):  # noqa: E501
-        """SubTransaction - a model defined in OpenAPI
+        """ScheduledSubTransaction - a model defined in OpenAPI
 
         Args:
-            id (str):
-            transaction_id (str):
-            amount (int): The subtransaction amount in milliunits format
-            deleted (bool): Whether or not the subtransaction has been deleted.  Deleted subtransactions will only be included in delta requests.
+            id (str, none_type):
+            scheduled_transaction_id (str, none_type):
+            amount (int, none_type): The scheduled subtransaction amount in milliunits format
+            deleted (bool): Whether or not the scheduled subtransaction has been deleted.  Deleted scheduled subtransactions will only be included in delta requests.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -253,21 +265,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            memo (str): [optional]  # noqa: E501
-            payee_id (str): [optional]  # noqa: E501
-            payee_name (str): [optional]  # noqa: E501
-            category_id (str): [optional]  # noqa: E501
-            category_name (str): [optional]  # noqa: E501
-            transfer_account_id (str): If a transfer, the account_id which the subtransaction transfers to. [optional]  # noqa: E501
-            transfer_transaction_id (str): If a transfer, the id of transaction on the other side of the transfer. [optional]  # noqa: E501
+            memo (str, none_type): [optional]  # noqa: E501
+            payee_id (str, none_type): [optional]  # noqa: E501
+            category_id (str, none_type): [optional]  # noqa: E501
+            transfer_account_id (str, none_type): If a transfer, the account_id which the scheduled subtransaction transfers to. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -288,15 +297,15 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (
             self.__class__, )
 
         self.id = id
-        self.transaction_id = transaction_id
+        self.scheduled_transaction_id = scheduled_transaction_id
         self.amount = amount
         self.deleted = deleted
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
```

### Comparing `ynab-api-2.0.0/ynab_api/model/transaction_detail.py` & `ynab-api-2.0.2/ynab_api/model/hybrid_transaction.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -16,23 +16,21 @@
     file_type, none_type, validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from ynab_api.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from ynab_api.model.sub_transaction import SubTransaction
-    from ynab_api.model.transaction_detail_all_of import TransactionDetailAllOf
+    from ynab_api.model.hybrid_transaction_all_of import HybridTransactionAllOf
     from ynab_api.model.transaction_summary import TransactionSummary
-    globals()['SubTransaction'] = SubTransaction
-    globals()['TransactionDetailAllOf'] = TransactionDetailAllOf
+    globals()['HybridTransactionAllOf'] = HybridTransactionAllOf
     globals()['TransactionSummary'] = TransactionSummary
 
 
-class TransactionDetail(ModelComposed):
+class HybridTransaction(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -50,19 +48,26 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('cleared', ): {
+            'None': None,
             'CLEARED': "cleared",
             'UNCLEARED': "uncleared",
             'RECONCILED': "reconciled",
         },
+        ('type', ): {
+            'None': None,
+            'TRANSACTION': "transaction",
+            'SUBTRANSACTION': "subtransaction",
+        },
         ('flag_color', ): {
+            'None': None,
             'RED': "red",
             'ORANGE': "orange",
             'YELLOW': "yellow",
             'GREEN': "green",
             'BLUE': "blue",
             'PURPLE': "purple",
         },
@@ -99,78 +104,134 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'id': (str, ),  # noqa: E501
-            'date': (date, ),  # noqa: E501
-            'amount': (int, ),  # noqa: E501
-            'cleared': (str, ),  # noqa: E501
+            'id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'date': (
+                date,
+                none_type,
+            ),  # noqa: E501
+            'amount': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'cleared': (
+                str,
+                none_type,
+            ),  # noqa: E501
             'approved': (bool, ),  # noqa: E501
-            'account_id': (str, ),  # noqa: E501
+            'account_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
             'deleted': (bool, ),  # noqa: E501
-            'account_name': (str, ),  # noqa: E501
-            'subtransactions': ([SubTransaction], ),  # noqa: E501
-            'memo': (str, ),  # noqa: E501
-            'flag_color': (str, ),  # noqa: E501
-            'payee_id': (str, ),  # noqa: E501
-            'category_id': (str, ),  # noqa: E501
-            'transfer_account_id': (str, ),  # noqa: E501
-            'transfer_transaction_id': (str, ),  # noqa: E501
-            'matched_transaction_id': (str, ),  # noqa: E501
-            'import_id': (str, ),  # noqa: E501
-            'payee_name': (str, ),  # noqa: E501
-            'category_name': (str, ),  # noqa: E501
+            'type': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'account_name': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'memo': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'flag_color': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'payee_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'category_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'transfer_account_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'transfer_transaction_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'matched_transaction_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'import_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'parent_transaction_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'payee_name': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'category_name': (
+                str,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'date': 'date',  # noqa: E501
         'amount': 'amount',  # noqa: E501
         'cleared': 'cleared',  # noqa: E501
         'approved': 'approved',  # noqa: E501
         'account_id': 'account_id',  # noqa: E501
         'deleted': 'deleted',  # noqa: E501
+        'type': 'type',  # noqa: E501
         'account_name': 'account_name',  # noqa: E501
-        'subtransactions': 'subtransactions',  # noqa: E501
         'memo': 'memo',  # noqa: E501
         'flag_color': 'flag_color',  # noqa: E501
         'payee_id': 'payee_id',  # noqa: E501
         'category_id': 'category_id',  # noqa: E501
         'transfer_account_id': 'transfer_account_id',  # noqa: E501
         'transfer_transaction_id': 'transfer_transaction_id',  # noqa: E501
         'matched_transaction_id': 'matched_transaction_id',  # noqa: E501
         'import_id': 'import_id',  # noqa: E501
+        'parent_transaction_id': 'parent_transaction_id',  # noqa: E501
         'payee_name': 'payee_name',  # noqa: E501
         'category_name': 'category_name',  # noqa: E501
     }
 
     read_only_vars = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TransactionDetail - a model defined in OpenAPI
+        """HybridTransaction - a model defined in OpenAPI
 
         Keyword Args:
-            id (str):
-            date (date): The transaction date in ISO format (e.g. 2016-12-01)
-            amount (int): The transaction amount in milliunits format
-            cleared (str): The cleared status of the transaction
+            id (str, none_type):
+            date (date, none_type): The transaction date in ISO format (e.g. 2016-12-01)
+            amount (int, none_type): The transaction amount in milliunits format
+            cleared (str, none_type): The cleared status of the transaction
             approved (bool): Whether or not the transaction is approved
-            account_id (str):
+            account_id (str, none_type):
             deleted (bool): Whether or not the transaction has been deleted.  Deleted transactions will only be included in delta requests.
-            account_name (str):
-            subtransactions ([SubTransaction]): If a split transaction, the subtransactions.
+            type (str, none_type): Whether the hybrid transaction represents a regular transaction or a subtransaction
+            account_name (str, none_type):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -193,24 +254,25 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            memo (str): [optional]  # noqa: E501
-            flag_color (str): The transaction flag. [optional]  # noqa: E501
-            payee_id (str): [optional]  # noqa: E501
-            category_id (str): [optional]  # noqa: E501
-            transfer_account_id (str): If a transfer transaction, the account to which it transfers. [optional]  # noqa: E501
-            transfer_transaction_id (str): If a transfer transaction, the id of transaction on the other side of the transfer. [optional]  # noqa: E501
-            matched_transaction_id (str): If transaction is matched, the id of the matched transaction. [optional]  # noqa: E501
-            import_id (str): If the Transaction was imported, this field is a unique (by account) import identifier.  If this transaction was imported through File Based Import or Direct Import and not through the API, the import_id will have the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'.  For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.. [optional]  # noqa: E501
-            payee_name (str): [optional]  # noqa: E501
-            category_name (str): [optional]  # noqa: E501
+            memo (str, none_type): [optional]  # noqa: E501
+            flag_color (str, none_type): The transaction flag. [optional]  # noqa: E501
+            payee_id (str, none_type): [optional]  # noqa: E501
+            category_id (str, none_type): [optional]  # noqa: E501
+            transfer_account_id (str, none_type): If a transfer transaction, the account to which it transfers. [optional]  # noqa: E501
+            transfer_transaction_id (str, none_type): If a transfer transaction, the id of transaction on the other side of the transfer. [optional]  # noqa: E501
+            matched_transaction_id (str, none_type): If transaction is matched, the id of the matched transaction. [optional]  # noqa: E501
+            import_id (str, none_type): If the Transaction was imported, this field is a unique (by account) import identifier.  If this transaction was imported through File Based Import or Direct Import and not through the API, the import_id will have the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'.  For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.. [optional]  # noqa: E501
+            parent_transaction_id (str, none_type): For subtransaction types, this is the id of the parent transaction.  For transaction types, this id will be always be null.. [optional]  # noqa: E501
+            payee_name (str, none_type): [optional]  # noqa: E501
+            category_name (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -270,26 +332,26 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TransactionDetail - a model defined in OpenAPI
+        """HybridTransaction - a model defined in OpenAPI
 
         Keyword Args:
-            id (str):
-            date (date): The transaction date in ISO format (e.g. 2016-12-01)
-            amount (int): The transaction amount in milliunits format
-            cleared (str): The cleared status of the transaction
+            id (str, none_type):
+            date (date, none_type): The transaction date in ISO format (e.g. 2016-12-01)
+            amount (int, none_type): The transaction amount in milliunits format
+            cleared (str, none_type): The cleared status of the transaction
             approved (bool): Whether or not the transaction is approved
-            account_id (str):
+            account_id (str, none_type):
             deleted (bool): Whether or not the transaction has been deleted.  Deleted transactions will only be included in delta requests.
-            account_name (str):
-            subtransactions ([SubTransaction]): If a split transaction, the subtransactions.
+            type (str, none_type): Whether the hybrid transaction represents a regular transaction or a subtransaction
+            account_name (str, none_type):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -312,24 +374,25 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            memo (str): [optional]  # noqa: E501
-            flag_color (str): The transaction flag. [optional]  # noqa: E501
-            payee_id (str): [optional]  # noqa: E501
-            category_id (str): [optional]  # noqa: E501
-            transfer_account_id (str): If a transfer transaction, the account to which it transfers. [optional]  # noqa: E501
-            transfer_transaction_id (str): If a transfer transaction, the id of transaction on the other side of the transfer. [optional]  # noqa: E501
-            matched_transaction_id (str): If transaction is matched, the id of the matched transaction. [optional]  # noqa: E501
-            import_id (str): If the Transaction was imported, this field is a unique (by account) import identifier.  If this transaction was imported through File Based Import or Direct Import and not through the API, the import_id will have the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'.  For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.. [optional]  # noqa: E501
-            payee_name (str): [optional]  # noqa: E501
-            category_name (str): [optional]  # noqa: E501
+            memo (str, none_type): [optional]  # noqa: E501
+            flag_color (str, none_type): The transaction flag. [optional]  # noqa: E501
+            payee_id (str, none_type): [optional]  # noqa: E501
+            category_id (str, none_type): [optional]  # noqa: E501
+            transfer_account_id (str, none_type): If a transfer transaction, the account to which it transfers. [optional]  # noqa: E501
+            transfer_transaction_id (str, none_type): If a transfer transaction, the id of transaction on the other side of the transfer. [optional]  # noqa: E501
+            matched_transaction_id (str, none_type): If transaction is matched, the id of the matched transaction. [optional]  # noqa: E501
+            import_id (str, none_type): If the Transaction was imported, this field is a unique (by account) import identifier.  If this transaction was imported through File Based Import or Direct Import and not through the API, the import_id will have the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'.  For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.. [optional]  # noqa: E501
+            parent_transaction_id (str, none_type): For subtransaction types, this is the id of the parent transaction.  For transaction types, this id will be always be null.. [optional]  # noqa: E501
+            payee_name (str, none_type): [optional]  # noqa: E501
+            category_name (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -388,12 +451,12 @@
         # code would be run when this module is imported, and these composed
         # classes don't exist yet because their module has not finished
         # loading
         lazy_import()
         return {
             'anyOf': [],
             'allOf': [
-                TransactionDetailAllOf,
+                HybridTransactionAllOf,
                 TransactionSummary,
             ],
             'oneOf': [],
         }
```

### Comparing `ynab-api-2.0.0/ynab_api/model/transaction_detail_all_of.py` & `ynab-api-2.0.2/ynab_api/model/scheduled_transaction_detail_all_of.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -16,19 +16,19 @@
     file_type, none_type, validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from ynab_api.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from ynab_api.model.sub_transaction import SubTransaction
-    globals()['SubTransaction'] = SubTransaction
+    from ynab_api.model.scheduled_sub_transaction import ScheduledSubTransaction
+    globals()['ScheduledSubTransaction'] = ScheduledSubTransaction
 
 
-class TransactionDetailAllOf(ModelNormal):
+class ScheduledTransactionDetailAllOf(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -81,18 +81,27 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'account_name': (str, ),  # noqa: E501
-            'subtransactions': ([SubTransaction], ),  # noqa: E501
-            'payee_name': (str, ),  # noqa: E501
-            'category_name': (str, ),  # noqa: E501
+            'account_name': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'subtransactions': ([ScheduledSubTransaction], ),  # noqa: E501
+            'payee_name': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'category_name': (
+                str,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -106,19 +115,19 @@
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, account_name, subtransactions, *args,
                            **kwargs):  # noqa: E501
-        """TransactionDetailAllOf - a model defined in OpenAPI
+        """ScheduledTransactionDetailAllOf - a model defined in OpenAPI
 
         Args:
-            account_name (str):
-            subtransactions ([SubTransaction]): If a split transaction, the subtransactions.
+            account_name (str, none_type):
+            subtransactions ([ScheduledSubTransaction]): If a split scheduled transaction, the subtransactions.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,16 +152,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            payee_name (str): [optional]  # noqa: E501
-            category_name (str): [optional]  # noqa: E501
+            payee_name (str, none_type): [optional]  # noqa: E501
+            category_name (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -198,19 +207,19 @@
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, account_name, subtransactions, *args,
                  **kwargs):  # noqa: E501
-        """TransactionDetailAllOf - a model defined in OpenAPI
+        """ScheduledTransactionDetailAllOf - a model defined in OpenAPI
 
         Args:
-            account_name (str):
-            subtransactions ([SubTransaction]): If a split transaction, the subtransactions.
+            account_name (str, none_type):
+            subtransactions ([ScheduledSubTransaction]): If a split scheduled transaction, the subtransactions.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -235,16 +244,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            payee_name (str): [optional]  # noqa: E501
-            category_name (str): [optional]  # noqa: E501
+            payee_name (str, none_type): [optional]  # noqa: E501
+            category_name (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ynab-api-2.0.0/ynab_api/model/transaction_response.py` & `ynab-api-2.0.2/ynab_api/model/transactions_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -16,19 +16,19 @@
     file_type, none_type, validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from ynab_api.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from ynab_api.model.transaction_response_data import TransactionResponseData
-    globals()['TransactionResponseData'] = TransactionResponseData
+    from ynab_api.model.transactions_response_data import TransactionsResponseData
+    globals()['TransactionsResponseData'] = TransactionsResponseData
 
 
-class TransactionResponse(ModelNormal):
+class TransactionsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -81,15 +81,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (TransactionResponseData, ),  # noqa: E501
+            'data': (TransactionsResponseData, ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -99,18 +99,18 @@
     read_only_vars = {}
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """TransactionResponse - a model defined in OpenAPI
+        """TransactionsResponse - a model defined in OpenAPI
 
         Args:
-            data (TransactionResponseData):
+            data (TransactionsResponseData):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -186,18 +186,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """TransactionResponse - a model defined in OpenAPI
+        """TransactionsResponse - a model defined in OpenAPI
 
         Args:
-            data (TransactionResponseData):
+            data (TransactionsResponseData):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `ynab-api-2.0.0/ynab_api/model/transaction_response_data.py` & `ynab-api-2.0.2/ynab_api/model/update_transactions_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -16,19 +16,19 @@
     file_type, none_type, validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from ynab_api.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from ynab_api.model.transaction_detail import TransactionDetail
-    globals()['TransactionDetail'] = TransactionDetail
+    from ynab_api.model.update_transaction import UpdateTransaction
+    globals()['UpdateTransaction'] = UpdateTransaction
 
 
-class TransactionResponseData(ModelNormal):
+class UpdateTransactionsWrapper(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -81,36 +81,36 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'transaction': (TransactionDetail, ),  # noqa: E501
+            'transactions': ([UpdateTransaction], ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
-        'transaction': 'transaction',  # noqa: E501
+        'transactions': 'transactions',  # noqa: E501
     }
 
     read_only_vars = {}
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, transaction, *args, **kwargs):  # noqa: E501
-        """TransactionResponseData - a model defined in OpenAPI
+    def _from_openapi_data(cls, transactions, *args, **kwargs):  # noqa: E501
+        """UpdateTransactionsWrapper - a model defined in OpenAPI
 
         Args:
-            transaction (TransactionDetail):
+            transactions ([UpdateTransaction]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -164,15 +164,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (
             self.__class__, )
 
-        self.transaction = transaction
+        self.transactions = transactions
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -185,19 +185,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, transaction, *args, **kwargs):  # noqa: E501
-        """TransactionResponseData - a model defined in OpenAPI
+    def __init__(self, transactions, *args, **kwargs):  # noqa: E501
+        """UpdateTransactionsWrapper - a model defined in OpenAPI
 
         Args:
-            transaction (TransactionDetail):
+            transactions ([UpdateTransaction]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -249,15 +249,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (
             self.__class__, )
 
-        self.transaction = transaction
+        self.transactions = transactions
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `ynab-api-2.0.0/ynab_api/model/transaction_summary.py` & `ynab-api-2.0.2/ynab_api/model/hybrid_transaction_all_of.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -15,15 +15,15 @@
     change_keys_js_to_python, convert_js_args_to_python_args, date, datetime,
     file_type, none_type, validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from ynab_api.exceptions import ApiAttributeError
 
 
-class TransactionSummary(ModelNormal):
+class HybridTransactionAllOf(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -40,26 +40,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('cleared', ): {
-            'CLEARED': "cleared",
-            'UNCLEARED': "uncleared",
-            'RECONCILED': "reconciled",
-        },
-        ('flag_color', ): {
-            'RED': "red",
-            'ORANGE': "orange",
-            'YELLOW': "yellow",
-            'GREEN': "green",
-            'BLUE': "blue",
-            'PURPLE': "purple",
+        ('type', ): {
+            'None': None,
+            'TRANSACTION': "transaction",
+            'SUBTRANSACTION': "subtransaction",
         },
     }
 
     validations = {}
 
     @cached_property
     def additional_properties_type():
@@ -88,71 +80,61 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (str, ),  # noqa: E501
-            'date': (date, ),  # noqa: E501
-            'amount': (int, ),  # noqa: E501
-            'cleared': (str, ),  # noqa: E501
-            'approved': (bool, ),  # noqa: E501
-            'account_id': (str, ),  # noqa: E501
-            'deleted': (bool, ),  # noqa: E501
-            'memo': (str, ),  # noqa: E501
-            'flag_color': (str, ),  # noqa: E501
-            'payee_id': (str, ),  # noqa: E501
-            'category_id': (str, ),  # noqa: E501
-            'transfer_account_id': (str, ),  # noqa: E501
-            'transfer_transaction_id': (str, ),  # noqa: E501
-            'matched_transaction_id': (str, ),  # noqa: E501
-            'import_id': (str, ),  # noqa: E501
+            'type': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'account_name': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'parent_transaction_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'payee_name': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'category_name': (
+                str,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'date': 'date',  # noqa: E501
-        'amount': 'amount',  # noqa: E501
-        'cleared': 'cleared',  # noqa: E501
-        'approved': 'approved',  # noqa: E501
-        'account_id': 'account_id',  # noqa: E501
-        'deleted': 'deleted',  # noqa: E501
-        'memo': 'memo',  # noqa: E501
-        'flag_color': 'flag_color',  # noqa: E501
-        'payee_id': 'payee_id',  # noqa: E501
-        'category_id': 'category_id',  # noqa: E501
-        'transfer_account_id': 'transfer_account_id',  # noqa: E501
-        'transfer_transaction_id': 'transfer_transaction_id',  # noqa: E501
-        'matched_transaction_id': 'matched_transaction_id',  # noqa: E501
-        'import_id': 'import_id',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'account_name': 'account_name',  # noqa: E501
+        'parent_transaction_id': 'parent_transaction_id',  # noqa: E501
+        'payee_name': 'payee_name',  # noqa: E501
+        'category_name': 'category_name',  # noqa: E501
     }
 
     read_only_vars = {}
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, date, amount, cleared, approved,
-                           account_id, deleted, *args, **kwargs):  # noqa: E501
-        """TransactionSummary - a model defined in OpenAPI
+    def _from_openapi_data(cls, type, account_name, *args,
+                           **kwargs):  # noqa: E501
+        """HybridTransactionAllOf - a model defined in OpenAPI
 
         Args:
-            id (str):
-            date (date): The transaction date in ISO format (e.g. 2016-12-01)
-            amount (int): The transaction amount in milliunits format
-            cleared (str): The cleared status of the transaction
-            approved (bool): Whether or not the transaction is approved
-            account_id (str):
-            deleted (bool): Whether or not the transaction has been deleted.  Deleted transactions will only be included in delta requests.
+            type (str, none_type): Whether the hybrid transaction represents a regular transaction or a subtransaction
+            account_name (str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -177,22 +159,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            memo (str): [optional]  # noqa: E501
-            flag_color (str): The transaction flag. [optional]  # noqa: E501
-            payee_id (str): [optional]  # noqa: E501
-            category_id (str): [optional]  # noqa: E501
-            transfer_account_id (str): If a transfer transaction, the account to which it transfers. [optional]  # noqa: E501
-            transfer_transaction_id (str): If a transfer transaction, the id of transaction on the other side of the transfer. [optional]  # noqa: E501
-            matched_transaction_id (str): If transaction is matched, the id of the matched transaction. [optional]  # noqa: E501
-            import_id (str): If the Transaction was imported, this field is a unique (by account) import identifier.  If this transaction was imported through File Based Import or Direct Import and not through the API, the import_id will have the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'.  For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.. [optional]  # noqa: E501
+            parent_transaction_id (str, none_type): For subtransaction types, this is the id of the parent transaction.  For transaction types, this id will be always be null.. [optional]  # noqa: E501
+            payee_name (str, none_type): [optional]  # noqa: E501
+            category_name (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -214,21 +191,16 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (
             self.__class__, )
 
-        self.id = id
-        self.date = date
-        self.amount = amount
-        self.cleared = cleared
-        self.approved = approved
-        self.account_id = account_id
-        self.deleted = deleted
+        self.type = type
+        self.account_name = account_name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -241,26 +213,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, date, amount, cleared, approved, account_id,
-                 deleted, *args, **kwargs):  # noqa: E501
-        """TransactionSummary - a model defined in OpenAPI
+    def __init__(self, type, account_name, *args, **kwargs):  # noqa: E501
+        """HybridTransactionAllOf - a model defined in OpenAPI
 
         Args:
-            id (str):
-            date (date): The transaction date in ISO format (e.g. 2016-12-01)
-            amount (int): The transaction amount in milliunits format
-            cleared (str): The cleared status of the transaction
-            approved (bool): Whether or not the transaction is approved
-            account_id (str):
-            deleted (bool): Whether or not the transaction has been deleted.  Deleted transactions will only be included in delta requests.
+            type (str, none_type): Whether the hybrid transaction represents a regular transaction or a subtransaction
+            account_name (str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -285,22 +251,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            memo (str): [optional]  # noqa: E501
-            flag_color (str): The transaction flag. [optional]  # noqa: E501
-            payee_id (str): [optional]  # noqa: E501
-            category_id (str): [optional]  # noqa: E501
-            transfer_account_id (str): If a transfer transaction, the account to which it transfers. [optional]  # noqa: E501
-            transfer_transaction_id (str): If a transfer transaction, the id of transaction on the other side of the transfer. [optional]  # noqa: E501
-            matched_transaction_id (str): If transaction is matched, the id of the matched transaction. [optional]  # noqa: E501
-            import_id (str): If the Transaction was imported, this field is a unique (by account) import identifier.  If this transaction was imported through File Based Import or Direct Import and not through the API, the import_id will have the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'.  For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.. [optional]  # noqa: E501
+            parent_transaction_id (str, none_type): For subtransaction types, this is the id of the parent transaction.  For transaction types, this id will be always be null.. [optional]  # noqa: E501
+            payee_name (str, none_type): [optional]  # noqa: E501
+            category_name (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -320,21 +281,16 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (
             self.__class__, )
 
-        self.id = id
-        self.date = date
-        self.amount = amount
-        self.cleared = cleared
-        self.approved = approved
-        self.account_id = account_id
-        self.deleted = deleted
+        self.type = type
+        self.account_name = account_name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `ynab-api-2.0.0/ynab_api/model/transactions_import_response.py` & `ynab-api-2.0.2/ynab_api/model/transactions_import_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
```

### Comparing `ynab-api-2.0.0/ynab_api/model/transactions_import_response_data.py` & `ynab-api-2.0.2/ynab_api/model/transactions_import_response_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -74,15 +74,15 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'transaction_ids': ([str], ),  # noqa: E501
+            'transaction_ids': ([str, none_type], ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -96,15 +96,15 @@
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, transaction_ids, *args,
                            **kwargs):  # noqa: E501
         """TransactionsImportResponseData - a model defined in OpenAPI
 
         Args:
-            transaction_ids ([str]): The list of transaction ids that were imported.
+            transaction_ids ([str, none_type]): The list of transaction ids that were imported.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -183,15 +183,15 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, transaction_ids, *args, **kwargs):  # noqa: E501
         """TransactionsImportResponseData - a model defined in OpenAPI
 
         Args:
-            transaction_ids ([str]): The list of transaction ids that were imported.
+            transaction_ids ([str, none_type]): The list of transaction ids that were imported.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `ynab-api-2.0.0/ynab_api/model/transactions_response.py` & `ynab-api-2.0.2/ynab_api/model/user_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -16,19 +16,19 @@
     file_type, none_type, validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from ynab_api.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from ynab_api.model.transactions_response_data import TransactionsResponseData
-    globals()['TransactionsResponseData'] = TransactionsResponseData
+    from ynab_api.model.user_response_data import UserResponseData
+    globals()['UserResponseData'] = UserResponseData
 
 
-class TransactionsResponse(ModelNormal):
+class UserResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -81,15 +81,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (TransactionsResponseData, ),  # noqa: E501
+            'data': (UserResponseData, ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -99,18 +99,18 @@
     read_only_vars = {}
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """TransactionsResponse - a model defined in OpenAPI
+        """UserResponse - a model defined in OpenAPI
 
         Args:
-            data (TransactionsResponseData):
+            data (UserResponseData):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -186,18 +186,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """TransactionsResponse - a model defined in OpenAPI
+        """UserResponse - a model defined in OpenAPI
 
         Args:
-            data (TransactionsResponseData):
+            data (UserResponseData):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `ynab-api-2.0.0/ynab_api/model/transactions_response_data.py` & `ynab-api-2.0.2/ynab_api/model/transactions_response_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -82,15 +82,18 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'transactions': ([TransactionDetail], ),  # noqa: E501
-            'server_knowledge': (int, ),  # noqa: E501
+            'server_knowledge': (
+                int,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -106,15 +109,15 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, transactions, server_knowledge, *args,
                            **kwargs):  # noqa: E501
         """TransactionsResponseData - a model defined in OpenAPI
 
         Args:
             transactions ([TransactionDetail]):
-            server_knowledge (int): The knowledge of the server
+            server_knowledge (int, none_type): The knowledge of the server
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -196,15 +199,15 @@
     @convert_js_args_to_python_args
     def __init__(self, transactions, server_knowledge, *args,
                  **kwargs):  # noqa: E501
         """TransactionsResponseData - a model defined in OpenAPI
 
         Args:
             transactions ([TransactionDetail]):
-            server_knowledge (int): The knowledge of the server
+            server_knowledge (int, none_type): The knowledge of the server
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `ynab-api-2.0.0/ynab_api/model/update_transaction.py` & `ynab-api-2.0.2/ynab_api/model/save_transaction.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -17,22 +17,18 @@
 )
 from ..model_utils import OpenApiModel
 from ynab_api.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from ynab_api.model.save_sub_transaction import SaveSubTransaction
-    from ynab_api.model.save_transaction import SaveTransaction
-    from ynab_api.model.update_transaction_all_of import UpdateTransactionAllOf
     globals()['SaveSubTransaction'] = SaveSubTransaction
-    globals()['SaveTransaction'] = SaveTransaction
-    globals()['UpdateTransactionAllOf'] = UpdateTransactionAllOf
 
 
-class UpdateTransaction(ModelComposed):
+class SaveTransaction(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -50,19 +46,21 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('cleared', ): {
+            'None': None,
             'CLEARED': "cleared",
             'UNCLEARED': "uncleared",
             'RECONCILED': "reconciled",
         },
         ('flag_color', ): {
+            'None': None,
             'RED': "red",
             'ORANGE': "orange",
             'YELLOW': "yellow",
             'GREEN': "green",
             'BLUE': "blue",
             'PURPLE': "purple",
         },
@@ -109,35 +107,63 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'id': (str, ),  # noqa: E501
-            'account_id': (str, ),  # noqa: E501
-            'date': (date, ),  # noqa: E501
-            'amount': (int, ),  # noqa: E501
-            'payee_id': (str, ),  # noqa: E501
-            'payee_name': (str, ),  # noqa: E501
-            'category_id': (str, ),  # noqa: E501
-            'memo': (str, ),  # noqa: E501
-            'cleared': (str, ),  # noqa: E501
+            'account_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'date': (
+                date,
+                none_type,
+            ),  # noqa: E501
+            'amount': (
+                int,
+                none_type,
+            ),  # noqa: E501
+            'payee_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'payee_name': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'category_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'memo': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'cleared': (
+                str,
+                none_type,
+            ),  # noqa: E501
             'approved': (bool, ),  # noqa: E501
-            'flag_color': (str, ),  # noqa: E501
-            'import_id': (str, ),  # noqa: E501
+            'flag_color': (
+                str,
+                none_type,
+            ),  # noqa: E501
+            'import_id': (
+                str,
+                none_type,
+            ),  # noqa: E501
             'subtransactions': ([SaveSubTransaction], ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
         'account_id': 'account_id',  # noqa: E501
         'date': 'date',  # noqa: E501
         'amount': 'amount',  # noqa: E501
         'payee_id': 'payee_id',  # noqa: E501
         'payee_name': 'payee_name',  # noqa: E501
         'category_id': 'category_id',  # noqa: E501
         'memo': 'memo',  # noqa: E501
@@ -146,24 +172,28 @@
         'flag_color': 'flag_color',  # noqa: E501
         'import_id': 'import_id',  # noqa: E501
         'subtransactions': 'subtransactions',  # noqa: E501
     }
 
     read_only_vars = {}
 
+    _composed_schemas = {}
+
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UpdateTransaction - a model defined in OpenAPI
+    def _from_openapi_data(cls, account_id, date, amount, *args,
+                           **kwargs):  # noqa: E501
+        """SaveTransaction - a model defined in OpenAPI
+
+        Args:
+            account_id (str, none_type):
+            date (date, none_type): The transaction date in ISO format (e.g. 2016-12-01).  Future dates (scheduled transactions) are not permitted.  Split transaction dates cannot be changed and if a different date is supplied it will be ignored.
+            amount (int, none_type): The transaction amount in milliunits format.  Split transaction amounts cannot be changed and if a different amount is supplied it will be ignored.
 
         Keyword Args:
-            id (str):
-            account_id (str):
-            date (date): The transaction date in ISO format (e.g. 2016-12-01).  Future dates (scheduled transactions) are not permitted.  Split transaction dates cannot be changed and if a different date is supplied it will be ignored.
-            amount (int): The transaction amount in milliunits format.  Split transaction amounts cannot be changed and if a different amount is supplied it will be ignored.
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -186,22 +216,22 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            payee_id (str): The payee for the transaction.  To create a transfer between two accounts, use the account transfer payee pointing to the target account.  Account transfer payees are specified as `tranfer_payee_id` on the account resource.. [optional]  # noqa: E501
-            payee_name (str): The payee name.  If a `payee_name` value is provided and `payee_id` has a null value, the `payee_name` value will be used to resolve the payee by either (1) a matching payee rename rule (only if `import_id` is also specified) or (2) a payee with the same name or (3) creation of a new payee.. [optional]  # noqa: E501
-            category_id (str): The category for the transaction.  To configure a split transaction, you can specify null for `category_id` and provide a `subtransactions` array as part of the transaction object.  If an existing transaction is a split, the `category_id` cannot be changed.  Credit Card Payment categories are not permitted and will be ignored if supplied.. [optional]  # noqa: E501
-            memo (str): [optional]  # noqa: E501
-            cleared (str): The cleared status of the transaction. [optional]  # noqa: E501
+            payee_id (str, none_type): The payee for the transaction.  To create a transfer between two accounts, use the account transfer payee pointing to the target account.  Account transfer payees are specified as `tranfer_payee_id` on the account resource.. [optional]  # noqa: E501
+            payee_name (str, none_type): The payee name.  If a `payee_name` value is provided and `payee_id` has a null value, the `payee_name` value will be used to resolve the payee by either (1) a matching payee rename rule (only if `import_id` is also specified) or (2) a payee with the same name or (3) creation of a new payee.. [optional]  # noqa: E501
+            category_id (str, none_type): The category for the transaction.  To configure a split transaction, you can specify null for `category_id` and provide a `subtransactions` array as part of the transaction object.  If an existing transaction is a split, the `category_id` cannot be changed.  Credit Card Payment categories are not permitted and will be ignored if supplied.. [optional]  # noqa: E501
+            memo (str, none_type): [optional]  # noqa: E501
+            cleared (str, none_type): The cleared status of the transaction. [optional]  # noqa: E501
             approved (bool): Whether or not the transaction is approved.  If not supplied, transaction will be unapproved by default.. [optional]  # noqa: E501
-            flag_color (str): The transaction flag. [optional]  # noqa: E501
-            import_id (str): If specified, the new transaction will be assigned this `import_id` and considered \"imported\".  We will also attempt to match this imported transaction to an existing \"user-entered\" transation on the same account, with the same amount, and with a date +/-10 days from the imported transaction date.<br><br>Transactions imported through File Based Import or Direct Import (not through the API) are assigned an import_id in the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'. For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.  Using a consistent format will prevent duplicates through Direct Import and File Based Import.<br><br>If import_id is omitted or specified as null, the transaction will be treated as a \"user-entered\" transaction. As such, it will be eligible to be matched against transactions later being imported (via DI, FBI, or API).. [optional]  # noqa: E501
+            flag_color (str, none_type): The transaction flag. [optional]  # noqa: E501
+            import_id (str, none_type): If specified, the new transaction will be assigned this `import_id` and considered \"imported\".  We will also attempt to match this imported transaction to an existing \"user-entered\" transation on the same account, with the same amount, and with a date +/-10 days from the imported transaction date.<br><br>Transactions imported through File Based Import or Direct Import (not through the API) are assigned an import_id in the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'. For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.  Using a consistent format will prevent duplicates through Direct Import and File Based Import.<br><br>If import_id is omitted or specified as null, the transaction will be treated as a \"user-entered\" transaction. As such, it will be eligible to be matched against transactions later being imported (via DI, FBI, or API).. [optional]  # noqa: E501
             subtransactions ([SaveSubTransaction]): An array of subtransactions to configure a transaction as a split.  Updating `subtransactions` on an existing split transaction is not supported.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -224,59 +254,47 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (
             self.__class__, )
 
-        constant_args = {
-            '_check_type': _check_type,
-            '_path_to_item': _path_to_item,
-            '_spec_property_naming': _spec_property_naming,
-            '_configuration': _configuration,
-            '_visited_composed_classes': self._visited_composed_classes,
-        }
-        composed_info = validate_get_composed_info(constant_args, kwargs, self)
-        self._composed_instances = composed_info[0]
-        self._var_name_to_model_instances = composed_info[1]
-        self._additional_properties_model_instances = composed_info[2]
-        discarded_args = composed_info[3]
-
+        self.account_id = account_id
+        self.date = date
+        self.amount = amount
         for var_name, var_value in kwargs.items():
-            if var_name in discarded_args and \
+            if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self._additional_properties_model_instances:
+                        self.additional_properties_type is None:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
-
         return self
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
-        '_composed_instances',
-        '_var_name_to_model_instances',
-        '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """UpdateTransaction - a model defined in OpenAPI
+    def __init__(self, account_id, date, amount, *args,
+                 **kwargs):  # noqa: E501
+        """SaveTransaction - a model defined in OpenAPI
+
+        Args:
+            account_id (str, none_type):
+            date (date, none_type): The transaction date in ISO format (e.g. 2016-12-01).  Future dates (scheduled transactions) are not permitted.  Split transaction dates cannot be changed and if a different date is supplied it will be ignored.
+            amount (int, none_type): The transaction amount in milliunits format.  Split transaction amounts cannot be changed and if a different amount is supplied it will be ignored.
 
         Keyword Args:
-            id (str):
-            account_id (str):
-            date (date): The transaction date in ISO format (e.g. 2016-12-01).  Future dates (scheduled transactions) are not permitted.  Split transaction dates cannot be changed and if a different date is supplied it will be ignored.
-            amount (int): The transaction amount in milliunits format.  Split transaction amounts cannot be changed and if a different amount is supplied it will be ignored.
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -299,22 +317,22 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            payee_id (str): The payee for the transaction.  To create a transfer between two accounts, use the account transfer payee pointing to the target account.  Account transfer payees are specified as `tranfer_payee_id` on the account resource.. [optional]  # noqa: E501
-            payee_name (str): The payee name.  If a `payee_name` value is provided and `payee_id` has a null value, the `payee_name` value will be used to resolve the payee by either (1) a matching payee rename rule (only if `import_id` is also specified) or (2) a payee with the same name or (3) creation of a new payee.. [optional]  # noqa: E501
-            category_id (str): The category for the transaction.  To configure a split transaction, you can specify null for `category_id` and provide a `subtransactions` array as part of the transaction object.  If an existing transaction is a split, the `category_id` cannot be changed.  Credit Card Payment categories are not permitted and will be ignored if supplied.. [optional]  # noqa: E501
-            memo (str): [optional]  # noqa: E501
-            cleared (str): The cleared status of the transaction. [optional]  # noqa: E501
+            payee_id (str, none_type): The payee for the transaction.  To create a transfer between two accounts, use the account transfer payee pointing to the target account.  Account transfer payees are specified as `tranfer_payee_id` on the account resource.. [optional]  # noqa: E501
+            payee_name (str, none_type): The payee name.  If a `payee_name` value is provided and `payee_id` has a null value, the `payee_name` value will be used to resolve the payee by either (1) a matching payee rename rule (only if `import_id` is also specified) or (2) a payee with the same name or (3) creation of a new payee.. [optional]  # noqa: E501
+            category_id (str, none_type): The category for the transaction.  To configure a split transaction, you can specify null for `category_id` and provide a `subtransactions` array as part of the transaction object.  If an existing transaction is a split, the `category_id` cannot be changed.  Credit Card Payment categories are not permitted and will be ignored if supplied.. [optional]  # noqa: E501
+            memo (str, none_type): [optional]  # noqa: E501
+            cleared (str, none_type): The cleared status of the transaction. [optional]  # noqa: E501
             approved (bool): Whether or not the transaction is approved.  If not supplied, transaction will be unapproved by default.. [optional]  # noqa: E501
-            flag_color (str): The transaction flag. [optional]  # noqa: E501
-            import_id (str): If specified, the new transaction will be assigned this `import_id` and considered \"imported\".  We will also attempt to match this imported transaction to an existing \"user-entered\" transation on the same account, with the same amount, and with a date +/-10 days from the imported transaction date.<br><br>Transactions imported through File Based Import or Direct Import (not through the API) are assigned an import_id in the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'. For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.  Using a consistent format will prevent duplicates through Direct Import and File Based Import.<br><br>If import_id is omitted or specified as null, the transaction will be treated as a \"user-entered\" transaction. As such, it will be eligible to be matched against transactions later being imported (via DI, FBI, or API).. [optional]  # noqa: E501
+            flag_color (str, none_type): The transaction flag. [optional]  # noqa: E501
+            import_id (str, none_type): If specified, the new transaction will be assigned this `import_id` and considered \"imported\".  We will also attempt to match this imported transaction to an existing \"user-entered\" transation on the same account, with the same amount, and with a date +/-10 days from the imported transaction date.<br><br>Transactions imported through File Based Import or Direct Import (not through the API) are assigned an import_id in the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'. For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.  Using a consistent format will prevent duplicates through Direct Import and File Based Import.<br><br>If import_id is omitted or specified as null, the transaction will be treated as a \"user-entered\" transaction. As such, it will be eligible to be matched against transactions later being imported (via DI, FBI, or API).. [optional]  # noqa: E501
             subtransactions ([SaveSubTransaction]): An array of subtransactions to configure a transaction as a split.  Updating `subtransactions` on an existing split transaction is not supported.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -335,51 +353,22 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (
             self.__class__, )
 
-        constant_args = {
-            '_check_type': _check_type,
-            '_path_to_item': _path_to_item,
-            '_spec_property_naming': _spec_property_naming,
-            '_configuration': _configuration,
-            '_visited_composed_classes': self._visited_composed_classes,
-        }
-        composed_info = validate_get_composed_info(constant_args, kwargs, self)
-        self._composed_instances = composed_info[0]
-        self._var_name_to_model_instances = composed_info[1]
-        self._additional_properties_model_instances = composed_info[2]
-        discarded_args = composed_info[3]
-
+        self.account_id = account_id
+        self.date = date
+        self.amount = amount
         for var_name, var_value in kwargs.items():
-            if var_name in discarded_args and \
+            if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self._additional_properties_model_instances:
+                        self.additional_properties_type is None:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
             if var_name in self.read_only_vars:
                 raise ApiAttributeError(
                     f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
                     f"class with read only attributes.")
-
-    @cached_property
-    def _composed_schemas():
-        # we need this here to make our import statements work
-        # we must store _composed_schemas in here so the code is only run
-        # when we invoke this method. If we kept this at the class
-        # level we would get an error because the class level
-        # code would be run when this module is imported, and these composed
-        # classes don't exist yet because their module has not finished
-        # loading
-        lazy_import()
-        return {
-            'anyOf': [],
-            'allOf': [
-                SaveTransaction,
-                UpdateTransactionAllOf,
-            ],
-            'oneOf': [],
-        }
```

### Comparing `ynab-api-2.0.0/ynab_api/model/update_transaction_all_of.py` & `ynab-api-2.0.2/ynab_api/model/update_transaction_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -74,15 +74,18 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (str, ),  # noqa: E501
+            'id': (
+                str,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
@@ -95,15 +98,15 @@
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, id, *args, **kwargs):  # noqa: E501
         """UpdateTransactionAllOf - a model defined in OpenAPI
 
         Args:
-            id (str):
+            id (str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -182,15 +185,15 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, id, *args, **kwargs):  # noqa: E501
         """UpdateTransactionAllOf - a model defined in OpenAPI
 
         Args:
-            id (str):
+            id (str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `ynab-api-2.0.0/ynab_api/model/update_transactions_wrapper.py` & `ynab-api-2.0.2/ynab_api/model/user.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -15,20 +15,15 @@
     change_keys_js_to_python, convert_js_args_to_python_args, date, datetime,
     file_type, none_type, validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from ynab_api.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from ynab_api.model.update_transaction import UpdateTransaction
-    globals()['UpdateTransaction'] = UpdateTransaction
-
-
-class UpdateTransactionsWrapper(ModelNormal):
+class User(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -54,15 +49,14 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (
             bool,
             date,
             datetime,
             dict,
             float,
             int,
@@ -79,38 +73,40 @@
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'transactions': ([UpdateTransaction], ),  # noqa: E501
+            'id': (
+                str,
+                none_type,
+            ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
-        'transactions': 'transactions',  # noqa: E501
+        'id': 'id',  # noqa: E501
     }
 
     read_only_vars = {}
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, transactions, *args, **kwargs):  # noqa: E501
-        """UpdateTransactionsWrapper - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, *args, **kwargs):  # noqa: E501
+        """User - a model defined in OpenAPI
 
         Args:
-            transactions ([UpdateTransaction]):
+            id (str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -164,15 +160,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (
             self.__class__, )
 
-        self.transactions = transactions
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -185,19 +181,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, transactions, *args, **kwargs):  # noqa: E501
-        """UpdateTransactionsWrapper - a model defined in OpenAPI
+    def __init__(self, id, *args, **kwargs):  # noqa: E501
+        """User - a model defined in OpenAPI
 
         Args:
-            transactions ([UpdateTransaction]):
+            id (str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -249,15 +245,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (
             self.__class__, )
 
-        self.transactions = transactions
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `ynab-api-2.0.0/ynab_api/model/user.py` & `ynab-api-2.0.2/ynab_api/model/user_response_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
 from ynab_api.model_utils import (  # noqa: F401
@@ -15,15 +15,20 @@
     change_keys_js_to_python, convert_js_args_to_python_args, date, datetime,
     file_type, none_type, validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from ynab_api.exceptions import ApiAttributeError
 
 
-class User(ModelNormal):
+def lazy_import():
+    from ynab_api.model.user import User
+    globals()['User'] = User
+
+
+class UserResponseData(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,14 +54,15 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (
             bool,
             date,
             datetime,
             dict,
             float,
             int,
@@ -73,37 +79,38 @@
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'id': (str, ),  # noqa: E501
+            'user': (User, ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
+        'user': 'user',  # noqa: E501
     }
 
     read_only_vars = {}
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, *args, **kwargs):  # noqa: E501
-        """User - a model defined in OpenAPI
+    def _from_openapi_data(cls, user, *args, **kwargs):  # noqa: E501
+        """UserResponseData - a model defined in OpenAPI
 
         Args:
-            id (str):
+            user (User):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -157,15 +164,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (
             self.__class__, )
 
-        self.id = id
+        self.user = user
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -178,19 +185,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, *args, **kwargs):  # noqa: E501
-        """User - a model defined in OpenAPI
+    def __init__(self, user, *args, **kwargs):  # noqa: E501
+        """UserResponseData - a model defined in OpenAPI
 
         Args:
-            id (str):
+            user (User):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -242,15 +249,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (
             self.__class__, )
 
-        self.id = id
+        self.user = user
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `ynab-api-2.0.0/ynab_api/model_utils.py` & `ynab-api-2.0.2/ynab_api/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
 import io
```

### Comparing `ynab-api-2.0.0/ynab_api/models/__init__.py` & `ynab-api-2.0.2/ynab_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ynab-api-2.0.0/ynab_api/rest.py` & `ynab-api-2.0.2/ynab_api/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.3
     Generated by: https://openapi-generator.tech
 """
 
 import io
 import json
 import logging
 import re
```

### Comparing `ynab-api-2.0.0/ynab_api.egg-info/PKG-INFO` & `ynab-api-2.0.2/ynab_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ynab-api
-Version: 2.0.0
+Version: 2.0.2
 Summary: YNAB API Endpoints
 Home-page: 
-Author: David Lerner
-Author-email: dmlerner@gmail.com
+Author: OpenAPI Generator community
+Author-email: team@openapitools.org
 Keywords: OpenAPI,OpenAPI-Generator,YNAB API Endpoints
 Requires-Python: >=3.6
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
```

### Comparing `ynab-api-2.0.0/ynab_api.egg-info/SOURCES.txt` & `ynab-api-2.0.2/ynab_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

