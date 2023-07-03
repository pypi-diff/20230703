# Comparing `tmp/ynab-api-1.0.0.tar.gz` & `tmp/ynab-api-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ynab-api-1.0.0.tar", last modified: Fri Nov 22 00:28:14 2019, max compression
+gzip compressed data, was "ynab-api-2.0.0.tar", last modified: Mon Jul  3 16:51:09 2023, max compression
```

## Comparing `ynab-api-1.0.0.tar` & `ynab-api-2.0.0.tar`

### file list

```diff
@@ -1,209 +1,223 @@
-drwxrwxrwx   0 david     (1000) david     (1000)        0 2019-11-22 00:28:14.000000 ynab-api-1.0.0/
--rwxrwxrwx   0 david     (1000) david     (1000)    14530 2019-11-22 00:28:14.000000 ynab-api-1.0.0/PKG-INFO
--rwxrwxrwx   0 david     (1000) david     (1000)    12081 2019-11-22 00:08:24.000000 ynab-api-1.0.0/README.md
--rwxrwxrwx   0 david     (1000) david     (1000)       79 2019-11-22 00:28:14.000000 ynab-api-1.0.0/setup.cfg
--rwxrwxrwx   0 david     (1000) david     (1000)     1475 2019-11-22 00:28:09.000000 ynab-api-1.0.0/setup.py
-drwxrwxrwx   0 david     (1000) david     (1000)        0 2019-11-22 00:28:14.000000 ynab-api-1.0.0/test/
--rwxrwxrwx   0 david     (1000) david     (1000)     1023 2019-11-22 00:08:23.000000 ynab-api-1.0.0/test/test_account.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1161 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_accounts_api.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1097 2019-11-22 00:08:23.000000 ynab-api-1.0.0/test/test_accounts_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1131 2019-11-22 00:08:23.000000 ynab-api-1.0.0/test/test_accounts_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1089 2019-11-22 00:08:23.000000 ynab-api-1.0.0/test/test_account_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1123 2019-11-22 00:08:23.000000 ynab-api-1.0.0/test/test_account_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1312 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_budgets_api.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1065 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_budget_detail.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1109 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_budget_detail_all_of.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1131 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_budget_detail_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1165 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_budget_detail_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1081 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_budget_settings.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1147 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_budget_settings_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1181 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_budget_settings_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1073 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_budget_summary.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1139 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_budget_summary_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1173 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_budget_summary_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1065 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_bulk_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1099 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_bulk_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1133 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_bulk_response_data_bulk.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1097 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_bulk_transactions.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1548 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_categories_api.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1113 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_categories_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1147 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_categories_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1031 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_category.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1073 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_category_group.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1189 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_category_group_with_categories.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1233 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_category_group_with_categories_all_of.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1097 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_category_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1131 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_category_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1081 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_currency_format.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1049 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_date_format.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1064 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_deprecated_api.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1057 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_error_detail.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1073 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_error_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1105 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_hybrid_transaction.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1179 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_hybrid_transactions_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1213 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_hybrid_transactions_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1149 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_hybrid_transaction_all_of.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1168 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_months_api.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1057 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_month_detail.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1101 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_month_detail_all_of.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1123 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_month_detail_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1157 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_month_detail_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1147 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_month_summaries_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1181 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_month_summaries_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1065 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_month_summary.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1007 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_payee.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1138 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_payees_api.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1081 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_payees_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1115 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_payees_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1073 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_payee_location.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1421 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_payee_locations_api.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1147 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_payee_locations_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1181 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_payee_locations_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1139 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_payee_location_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1173 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_payee_location_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1073 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_payee_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1107 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_payee_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1131 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_save_category_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1165 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_save_category_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1107 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_save_month_category.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1165 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_save_month_category_wrapper.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1089 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_save_transaction.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1163 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_save_transactions_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1197 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_save_transactions_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1155 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_save_transactions_wrapper.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1147 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_save_transaction_wrapper.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1155 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_scheduled_sub_transaction.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1326 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_scheduled_transactions_api.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1203 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_scheduled_transactions_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1237 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_scheduled_transactions_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1179 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_scheduled_transaction_detail.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1223 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_scheduled_transaction_detail_all_of.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1195 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_scheduled_transaction_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1229 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_scheduled_transaction_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1187 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_scheduled_transaction_summary.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1081 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_sub_transaction.py
--rwxrwxrwx   0 david     (1000) david     (1000)     2247 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_transactions_api.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1129 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_transactions_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1163 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_transactions_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1105 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_transaction_detail.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1149 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_transaction_detail_all_of.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1121 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_transaction_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1155 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_transaction_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1113 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_transaction_summary.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1105 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_update_transaction.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1171 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_update_transactions_wrapper.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1149 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_update_transaction_all_of.py
--rwxrwxrwx   0 david     (1000) david     (1000)      999 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_user.py
--rwxrwxrwx   0 david     (1000) david     (1000)      981 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_user_api.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1065 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_user_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     1099 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/test_user_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)        0 2019-11-22 00:08:24.000000 ynab-api-1.0.0/test/__init__.py
-drwxrwxrwx   0 david     (1000) david     (1000)        0 2019-11-22 00:28:14.000000 ynab-api-1.0.0/ynab_api/
-drwxrwxrwx   0 david     (1000) david     (1000)        0 2019-11-22 00:28:14.000000 ynab-api-1.0.0/ynab_api/api/
--rwxrwxrwx   0 david     (1000) david     (1000)    13089 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/api/accounts_api.py
--rwxrwxrwx   0 david     (1000) david     (1000)    16907 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/api/budgets_api.py
--rwxrwxrwx   0 david     (1000) david     (1000)    28821 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/api/categories_api.py
--rwxrwxrwx   0 david     (1000) david     (1000)     7547 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/api/deprecated_api.py
--rwxrwxrwx   0 david     (1000) david     (1000)    13308 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/api/months_api.py
--rwxrwxrwx   0 david     (1000) david     (1000)    12987 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/api/payees_api.py
--rwxrwxrwx   0 david     (1000) david     (1000)    19068 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/api/payee_locations_api.py
--rwxrwxrwx   0 david     (1000) david     (1000)    13784 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/api/scheduled_transactions_api.py
--rwxrwxrwx   0 david     (1000) david     (1000)    59073 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/api/transactions_api.py
--rwxrwxrwx   0 david     (1000) david     (1000)     5216 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/api/user_api.py
--rwxrwxrwx   0 david     (1000) david     (1000)      625 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/api/__init__.py
--rwxrwxrwx   0 david     (1000) david     (1000)    25572 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/api_client.py
--rwxrwxrwx   0 david     (1000) david     (1000)    10709 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/configuration.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3965 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/exceptions.py
-drwxrwxrwx   0 david     (1000) david     (1000)        0 2019-11-22 00:28:14.000000 ynab-api-1.0.0/ynab_api/models/
--rwxrwxrwx   0 david     (1000) david     (1000)    13513 2019-11-22 00:08:23.000000 ynab-api-1.0.0/ynab_api/models/account.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3667 2019-11-22 00:08:23.000000 ynab-api-1.0.0/ynab_api/models/accounts_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     4877 2019-11-22 00:08:23.000000 ynab-api-1.0.0/ynab_api/models/accounts_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3656 2019-11-22 00:08:23.000000 ynab-api-1.0.0/ynab_api/models/account_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3715 2019-11-22 00:08:23.000000 ynab-api-1.0.0/ynab_api/models/account_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)    16652 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/budget_detail.py
--rwxrwxrwx   0 david     (1000) david     (1000)    11230 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/budget_detail_all_of.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3711 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/budget_detail_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     4880 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/budget_detail_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     4771 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/budget_settings.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3733 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/budget_settings_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3813 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/budget_settings_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     8527 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/budget_summary.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3722 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/budget_summary_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     4658 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/budget_summary_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3623 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/bulk_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3667 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/bulk_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     5550 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/bulk_response_data_bulk.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3838 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/bulk_transactions.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3689 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/categories_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     5108 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/categories_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)    16962 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/category.py
--rwxrwxrwx   0 david     (1000) david     (1000)     6278 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/category_group.py
--rwxrwxrwx   0 david     (1000) david     (1000)     7792 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/category_group_with_categories.py
--rwxrwxrwx   0 david     (1000) david     (1000)     4187 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/category_group_with_categories_all_of.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3667 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/category_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3747 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/category_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)    10396 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/currency_format.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3610 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/date_format.py
--rwxrwxrwx   0 david     (1000) david     (1000)     5030 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/error_detail.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3637 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/error_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)    23043 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/hybrid_transaction.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3777 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/hybrid_transactions_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3956 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/hybrid_transactions_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     7954 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/hybrid_transaction_all_of.py
--rwxrwxrwx   0 david     (1000) david     (1000)    11273 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/month_detail.py
--rwxrwxrwx   0 david     (1000) david     (1000)     4065 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/month_detail_all_of.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3700 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/month_detail_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3717 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/month_detail_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3733 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/month_summaries_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     4922 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/month_summaries_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)    10133 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/month_summary.py
--rwxrwxrwx   0 david     (1000) david     (1000)     6233 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/payee.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3645 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/payees_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     4805 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/payees_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     7109 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/payee_location.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3733 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/payee_locations_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3975 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/payee_locations_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3722 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/payee_location_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3928 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/payee_location_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3634 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/payee_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3651 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/payee_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3711 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/save_category_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     4910 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/save_category_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3826 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/save_month_category.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3806 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/save_month_category_wrapper.py
--rwxrwxrwx   0 david     (1000) david     (1000)    17221 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/save_transaction.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3755 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/save_transactions_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     8409 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/save_transactions_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     4529 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/save_transactions_wrapper.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3847 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/save_transaction_wrapper.py
--rwxrwxrwx   0 david     (1000) david     (1000)    10165 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/scheduled_sub_transaction.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3810 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/scheduled_transactions_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     5384 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/scheduled_transactions_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)    18549 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/scheduled_transaction_detail.py
--rwxrwxrwx   0 david     (1000) david     (1000)     6780 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/scheduled_transaction_detail_all_of.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3799 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/scheduled_transaction_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     4170 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/scheduled_transaction_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)    14830 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/scheduled_transaction_summary.py
--rwxrwxrwx   0 david     (1000) david     (1000)     9551 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/sub_transaction.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3711 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/transactions_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     5039 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/transactions_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)    21662 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/transaction_detail.py
--rwxrwxrwx   0 david     (1000) david     (1000)     6553 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/transaction_detail_all_of.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3700 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/transaction_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3861 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/transaction_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)    18146 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/transaction_summary.py
--rwxrwxrwx   0 david     (1000) david     (1000)    18026 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/update_transaction.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3916 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/update_transactions_wrapper.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3622 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/update_transaction_all_of.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3478 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/user.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3623 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/user_response.py
--rwxrwxrwx   0 david     (1000) david     (1000)     3619 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/user_response_data.py
--rwxrwxrwx   0 david     (1000) david     (1000)     6410 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/models/__init__.py
--rwxrwxrwx   0 david     (1000) david     (1000)    12668 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/rest.py
--rwxrwxrwx   0 david     (1000) david     (1000)     7342 2019-11-22 00:08:24.000000 ynab-api-1.0.0/ynab_api/__init__.py
-drwxrwxrwx   0 david     (1000) david     (1000)        0 2019-11-22 00:28:14.000000 ynab-api-1.0.0/ynab_api.egg-info/
--rwxrwxrwx   0 david     (1000) david     (1000)        1 2019-11-22 00:28:13.000000 ynab-api-1.0.0/ynab_api.egg-info/dependency_links.txt
--rwxrwxrwx   0 david     (1000) david     (1000)    14530 2019-11-22 00:28:13.000000 ynab-api-1.0.0/ynab_api.egg-info/PKG-INFO
--rwxrwxrwx   0 david     (1000) david     (1000)       48 2019-11-22 00:28:13.000000 ynab-api-1.0.0/ynab_api.egg-info/requires.txt
--rwxrwxrwx   0 david     (1000) david     (1000)     7321 2019-11-22 00:28:14.000000 ynab-api-1.0.0/ynab_api.egg-info/SOURCES.txt
--rwxrwxrwx   0 david     (1000) david     (1000)       14 2019-11-22 00:28:13.000000 ynab-api-1.0.0/ynab_api.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 16:51:09.379814 ynab-api-2.0.0/
+-rw-rw-r--   0 david     (1000) david     (1000)      525 2023-07-03 16:51:09.379814 ynab-api-2.0.0/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)    13661 2023-07-03 16:46:53.000000 ynab-api-2.0.0/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)       69 2023-07-03 16:51:09.379814 ynab-api-2.0.0/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)     1448 2023-07-03 16:46:53.000000 ynab-api-2.0.0/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 16:51:09.367814 ynab-api-2.0.0/test/
+-rw-rw-r--   0 david     (1000) david     (1000)      897 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_account.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1079 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_account_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1058 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_account_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1182 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_accounts_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1090 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_accounts_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1065 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_accounts_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2365 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_budget_detail.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1996 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_budget_detail_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1136 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_budget_detail_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1115 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_budget_detail_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1138 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_budget_settings.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1158 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_budget_settings_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1137 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_budget_settings_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1205 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_budget_summary.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1147 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_budget_summary_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1126 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_budget_summary_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1189 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_budgets_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1046 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_bulk_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1092 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_bulk_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)      991 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_bulk_response_data_bulk.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1069 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_bulk_transactions.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1422 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_categories_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1112 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_categories_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1162 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_categories_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)      904 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_category.py
+-rw-rw-r--   0 david     (1000) david     (1000)      940 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_category_group.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1398 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_category_group_with_categories.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1156 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_category_group_with_categories_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1090 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_category_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1069 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_category_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)      947 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_currency_format.py
+-rw-rw-r--   0 david     (1000) david     (1000)      919 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_date_format.py
+-rw-rw-r--   0 david     (1000) david     (1000)      938 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_deprecated_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)      926 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_error_detail.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1032 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_error_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1225 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_hybrid_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1005 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_hybrid_transaction_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1202 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_hybrid_transactions_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1177 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_hybrid_transactions_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1213 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_month_detail.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1042 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_month_detail_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1125 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_month_detail_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1104 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_month_detail_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1158 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_month_summaries_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1129 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_month_summaries_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)      933 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_month_summary.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1046 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_months_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)      883 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payee.py
+-rw-rw-r--   0 david     (1000) david     (1000)      940 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payee_location.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1147 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payee_location_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1126 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payee_location_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1290 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payee_locations_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1158 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payee_locations_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1133 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payee_locations_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1057 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payee_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1036 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payee_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1016 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payees_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1068 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payees_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1043 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_payees_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)      926 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_account.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1068 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_account_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1136 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_category_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1098 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_category_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)      969 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_month_category.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1136 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_month_category_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)      976 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_sub_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1075 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1112 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_transaction_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1180 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_transactions_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1163 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_transactions_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1119 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_save_transactions_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1011 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_scheduled_sub_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1503 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_scheduled_transaction_detail.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1210 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_scheduled_transaction_detail_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1225 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_scheduled_transaction_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1228 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_scheduled_transaction_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1039 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_scheduled_transaction_summary.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1188 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_scheduled_transactions_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1236 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_scheduled_transactions_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1235 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_scheduled_transactions_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)      947 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_sub_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1328 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_transaction_detail.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1109 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_transaction_detail_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1123 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_transaction_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1127 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_transaction_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)      975 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_transaction_summary.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2273 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_transactions_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1202 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_transactions_import_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1061 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_transactions_import_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1134 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_transactions_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1134 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_transactions_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1333 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_update_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1005 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_update_transaction_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1141 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_update_transactions_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)      876 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_user.py
+-rw-rw-r--   0 david     (1000) david     (1000)      861 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_user_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1046 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_user_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1025 2023-07-03 16:46:01.000000 ynab-api-2.0.0/test/test_user_response_data.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 16:51:09.367814 ynab-api-2.0.0/ynab_api/
+-rw-rw-r--   0 david     (1000) david     (1000)      897 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 16:51:09.367814 ynab-api-2.0.0/ynab_api/api/
+-rw-rw-r--   0 david     (1000) david     (1000)      213 2023-07-03 16:46:01.000000 ynab-api-2.0.0/ynab_api/api/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    14003 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/api/accounts_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)    14518 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/api/budgets_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)    20333 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/api/categories_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5668 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/api/deprecated_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11493 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/api/months_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)    14006 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/api/payee_locations_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11258 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/api/payees_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10380 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/api/scheduled_transactions_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)    46788 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/api/transactions_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4953 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/api/user_api.py
+-rw-rw-r--   0 david     (1000) david     (1000)    37468 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/api_client.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 16:51:09.367814 ynab-api-2.0.0/ynab_api/apis/
+-rw-rw-r--   0 david     (1000) david     (1000)      952 2023-07-03 16:46:01.000000 ynab-api-2.0.0/ynab_api/apis/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    17225 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/configuration.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5314 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/exceptions.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 16:51:09.379814 ynab-api-2.0.0/ynab_api/model/
+-rw-rw-r--   0 david     (1000) david     (1000)      348 2023-07-03 16:46:01.000000 ynab-api-2.0.0/ynab_api/model/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    16686 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/account.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11651 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/account_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11610 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/account_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11661 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/accounts_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12053 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/accounts_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    19151 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/budget_detail.py
+-rw-rw-r--   0 david     (1000) david     (1000)    15032 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/budget_detail_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11702 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/budget_detail_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12073 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/budget_detail_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12161 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/budget_settings.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11722 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/budget_settings_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11692 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/budget_settings_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13786 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/budget_summary.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11712 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/budget_summary_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11936 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/budget_summary_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11621 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/bulk_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11662 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/bulk_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12417 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/bulk_response_data_bulk.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11719 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/bulk_transactions.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11681 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/categories_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12279 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/categories_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    18876 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/category.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12380 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/category_group.py
+-rw-rw-r--   0 david     (1000) david     (1000)    14954 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/category_group_with_categories.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11935 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/category_group_with_categories_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11661 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/category_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11631 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/category_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13725 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/currency_format.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11413 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/date_format.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11803 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/error_detail.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11599 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/error_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    20383 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/hybrid_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12976 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/hybrid_transaction_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11767 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/hybrid_transactions_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11775 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/hybrid_transactions_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    16149 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/month_detail.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11893 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/month_detail_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11692 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/month_detail_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11629 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/month_detail_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11722 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/month_summaries_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12085 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/month_summaries_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13983 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/month_summary.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12397 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/payee.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12601 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/payee_location.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11712 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/payee_location_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11748 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/payee_location_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11722 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/payee_locations_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11795 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/payee_locations_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11631 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/payee_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11568 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/payee_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11641 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/payees_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12011 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/payees_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12338 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_account.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11636 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_account_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11702 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_category_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12066 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_category_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11530 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_month_category.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11708 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_month_category_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13410 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_sub_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)    19841 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11720 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_transaction_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11742 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_transactions_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13485 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_transactions_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11900 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/save_transactions_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13697 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/scheduled_sub_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)    18477 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/scheduled_transaction_detail.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12720 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/scheduled_transaction_detail_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11787 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/scheduled_transaction_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11977 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/scheduled_transaction_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    15597 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/scheduled_transaction_summary.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11797 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/scheduled_transactions_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12393 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/scheduled_transactions_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    14331 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/sub_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)    19873 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/transaction_detail.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12609 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/transaction_detail_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11691 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/transaction_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11737 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/transaction_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    17120 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/transaction_summary.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11767 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/transactions_import_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11701 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/transactions_import_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11701 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/transactions_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12180 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/transactions_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    21912 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/update_transaction.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11405 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/update_transaction_all_of.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11760 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/update_transactions_wrapper.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11351 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/user.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11621 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/user_response.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11547 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model/user_response_data.py
+-rw-rw-r--   0 david     (1000) david     (1000)    83377 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/model_utils.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 16:51:09.379814 ynab-api-2.0.0/ynab_api/models/
+-rw-rw-r--   0 david     (1000) david     (1000)     6525 2023-07-03 16:46:01.000000 ynab-api-2.0.0/ynab_api/models/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13847 2023-07-03 16:46:53.000000 ynab-api-2.0.0/ynab_api/rest.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-03 16:51:09.367814 ynab-api-2.0.0/ynab_api.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)      525 2023-07-03 16:51:09.000000 ynab-api-2.0.0/ynab_api.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     7689 2023-07-03 16:51:09.000000 ynab-api-2.0.0/ynab_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-07-03 16:51:09.000000 ynab-api-2.0.0/ynab_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       32 2023-07-03 16:51:09.000000 ynab-api-2.0.0/ynab_api.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        9 2023-07-03 16:51:09.000000 ynab-api-2.0.0/ynab_api.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ynab-api-1.0.0/PKG-INFO` & `ynab-api-2.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,234 +1,275 @@
-Metadata-Version: 2.1
-Name: ynab-api
-Version: 1.0.0
-Summary: YNAB API Endpoint
-Home-page: https://github.com/dmlerner/ynab-api
-Author: David Lerner
-Author-email: dmlerner@gmail.com
-License: MIT
-Download-URL: https://github.com/dmlerner/ynab-api/archive/v1.0.tar.gz
-Description: # ynab-api
-        Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com
-        
-        This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
-        
-        - API version: 1.0.0
-        - Package version: 1.0.0
-        - Build package: org.openapitools.codegen.languages.PythonClientCodegen
-        
-        ## Requirements.
-        
-        Python 2.7 and 3.4+
-        
-        ## Installation & Usage
-        ### pip install
-        
-        If the python package is hosted on a repository, you can install directly using:
-        
-        ```sh
-        pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
-        ```
-        (you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
-        
-        Then import the package:
-        ```python
-        import ynab_api 
-        ```
-        
-        ### Setuptools
-        
-        Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
-        
-        ```sh
-        python setup.py install --user
-        ```
-        (or `sudo python setup.py install` to install the package for all users)
-        
-        Then import the package:
-        ```python
-        import ynab_api
-        ```
-        
-        ## Getting Started
-        
-        Please follow the [installation procedure](#installation--usage) and then run the following:
-        
-        ```python
-        from __future__ import print_function
-        import time
-        import ynab_api
-        from ynab_api.rest import ApiException
-        from pprint import pprint
-        
-        configuration = ynab_api.Configuration()
-        # Configure API key authorization: bearer
-        configuration.api_key['Authorization'] = 'YOUR_API_KEY'
-        # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
-        # configuration.api_key_prefix['Authorization'] = 'Bearer'
-        
-        # Defining host is optional and default to https://api.youneedabudget.com/v1
-        configuration.host = "https://api.youneedabudget.com/v1"
-        # Create an instance of the API class
-        api_instance = ynab_api.AccountsApi(ynab_api.ApiClient(configuration))
-        budget_id = 'budget_id_example' # str | The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget)
-        account_id = 'account_id_example' # str | The id of the account
-        
-        try:
-            # Single account
-            api_response = api_instance.get_account_by_id(budget_id, account_id)
-            pprint(api_response)
-        except ApiException as e:
-            print("Exception when calling AccountsApi->get_account_by_id: %s\n" % e)
-        
-        ```
-        
-        ## Documentation for API Endpoints
-        
-        All URIs are relative to *https://api.youneedabudget.com/v1*
-        
-        Class | Method | HTTP request | Description
-        ------------ | ------------- | ------------- | -------------
-        *AccountsApi* | [**get_account_by_id**](docs/AccountsApi.md#get_account_by_id) | **GET** /budgets/{budget_id}/accounts/{account_id} | Single account
-        *AccountsApi* | [**get_accounts**](docs/AccountsApi.md#get_accounts) | **GET** /budgets/{budget_id}/accounts | Account list
-        *BudgetsApi* | [**get_budget_by_id**](docs/BudgetsApi.md#get_budget_by_id) | **GET** /budgets/{budget_id} | Single budget
-        *BudgetsApi* | [**get_budget_settings_by_id**](docs/BudgetsApi.md#get_budget_settings_by_id) | **GET** /budgets/{budget_id}/settings | Budget Settings
-        *BudgetsApi* | [**get_budgets**](docs/BudgetsApi.md#get_budgets) | **GET** /budgets | List budgets
-        *CategoriesApi* | [**get_categories**](docs/CategoriesApi.md#get_categories) | **GET** /budgets/{budget_id}/categories | List categories
-        *CategoriesApi* | [**get_category_by_id**](docs/CategoriesApi.md#get_category_by_id) | **GET** /budgets/{budget_id}/categories/{category_id} | Single category
-        *CategoriesApi* | [**get_month_category_by_id**](docs/CategoriesApi.md#get_month_category_by_id) | **GET** /budgets/{budget_id}/months/{month}/categories/{category_id} | Single category for a specific budget month
-        *CategoriesApi* | [**update_month_category**](docs/CategoriesApi.md#update_month_category) | **PATCH** /budgets/{budget_id}/months/{month}/categories/{category_id} | Update a category for a specific month
-        *DeprecatedApi* | [**bulk_create_transactions**](docs/DeprecatedApi.md#bulk_create_transactions) | **POST** /budgets/{budget_id}/transactions/bulk | Bulk create transactions
-        *MonthsApi* | [**get_budget_month**](docs/MonthsApi.md#get_budget_month) | **GET** /budgets/{budget_id}/months/{month} | Single budget month
-        *MonthsApi* | [**get_budget_months**](docs/MonthsApi.md#get_budget_months) | **GET** /budgets/{budget_id}/months | List budget months
-        *PayeeLocationsApi* | [**get_payee_location_by_id**](docs/PayeeLocationsApi.md#get_payee_location_by_id) | **GET** /budgets/{budget_id}/payee_locations/{payee_location_id} | Single payee location
-        *PayeeLocationsApi* | [**get_payee_locations**](docs/PayeeLocationsApi.md#get_payee_locations) | **GET** /budgets/{budget_id}/payee_locations | List payee locations
-        *PayeeLocationsApi* | [**get_payee_locations_by_payee**](docs/PayeeLocationsApi.md#get_payee_locations_by_payee) | **GET** /budgets/{budget_id}/payees/{payee_id}/payee_locations | List locations for a payee
-        *PayeesApi* | [**get_payee_by_id**](docs/PayeesApi.md#get_payee_by_id) | **GET** /budgets/{budget_id}/payees/{payee_id} | Single payee
-        *PayeesApi* | [**get_payees**](docs/PayeesApi.md#get_payees) | **GET** /budgets/{budget_id}/payees | List payees
-        *ScheduledTransactionsApi* | [**get_scheduled_transaction_by_id**](docs/ScheduledTransactionsApi.md#get_scheduled_transaction_by_id) | **GET** /budgets/{budget_id}/scheduled_transactions/{scheduled_transaction_id} | Single scheduled transaction
-        *ScheduledTransactionsApi* | [**get_scheduled_transactions**](docs/ScheduledTransactionsApi.md#get_scheduled_transactions) | **GET** /budgets/{budget_id}/scheduled_transactions | List scheduled transactions
-        *TransactionsApi* | [**create_transaction**](docs/TransactionsApi.md#create_transaction) | **POST** /budgets/{budget_id}/transactions | Create a single transaction or multiple transactions
-        *TransactionsApi* | [**get_transaction_by_id**](docs/TransactionsApi.md#get_transaction_by_id) | **GET** /budgets/{budget_id}/transactions/{transaction_id} | Single transaction
-        *TransactionsApi* | [**get_transactions**](docs/TransactionsApi.md#get_transactions) | **GET** /budgets/{budget_id}/transactions | List transactions
-        *TransactionsApi* | [**get_transactions_by_account**](docs/TransactionsApi.md#get_transactions_by_account) | **GET** /budgets/{budget_id}/accounts/{account_id}/transactions | List account transactions
-        *TransactionsApi* | [**get_transactions_by_category**](docs/TransactionsApi.md#get_transactions_by_category) | **GET** /budgets/{budget_id}/categories/{category_id}/transactions | List category transactions
-        *TransactionsApi* | [**get_transactions_by_payee**](docs/TransactionsApi.md#get_transactions_by_payee) | **GET** /budgets/{budget_id}/payees/{payee_id}/transactions | List payee transactions
-        *TransactionsApi* | [**update_transaction**](docs/TransactionsApi.md#update_transaction) | **PUT** /budgets/{budget_id}/transactions/{transaction_id} | Updates an existing transaction
-        *TransactionsApi* | [**update_transactions**](docs/TransactionsApi.md#update_transactions) | **PATCH** /budgets/{budget_id}/transactions | Update multiple transactions
-        *UserApi* | [**get_user**](docs/UserApi.md#get_user) | **GET** /user | User info
-        
-        
-        ## Documentation For Models
-        
-         - [Account](docs/Account.md)
-         - [AccountResponse](docs/AccountResponse.md)
-         - [AccountResponseData](docs/AccountResponseData.md)
-         - [AccountsResponse](docs/AccountsResponse.md)
-         - [AccountsResponseData](docs/AccountsResponseData.md)
-         - [BudgetDetail](docs/BudgetDetail.md)
-         - [BudgetDetailAllOf](docs/BudgetDetailAllOf.md)
-         - [BudgetDetailResponse](docs/BudgetDetailResponse.md)
-         - [BudgetDetailResponseData](docs/BudgetDetailResponseData.md)
-         - [BudgetSettings](docs/BudgetSettings.md)
-         - [BudgetSettingsResponse](docs/BudgetSettingsResponse.md)
-         - [BudgetSettingsResponseData](docs/BudgetSettingsResponseData.md)
-         - [BudgetSummary](docs/BudgetSummary.md)
-         - [BudgetSummaryResponse](docs/BudgetSummaryResponse.md)
-         - [BudgetSummaryResponseData](docs/BudgetSummaryResponseData.md)
-         - [BulkResponse](docs/BulkResponse.md)
-         - [BulkResponseData](docs/BulkResponseData.md)
-         - [BulkResponseDataBulk](docs/BulkResponseDataBulk.md)
-         - [BulkTransactions](docs/BulkTransactions.md)
-         - [CategoriesResponse](docs/CategoriesResponse.md)
-         - [CategoriesResponseData](docs/CategoriesResponseData.md)
-         - [Category](docs/Category.md)
-         - [CategoryGroup](docs/CategoryGroup.md)
-         - [CategoryGroupWithCategories](docs/CategoryGroupWithCategories.md)
-         - [CategoryGroupWithCategoriesAllOf](docs/CategoryGroupWithCategoriesAllOf.md)
-         - [CategoryResponse](docs/CategoryResponse.md)
-         - [CategoryResponseData](docs/CategoryResponseData.md)
-         - [CurrencyFormat](docs/CurrencyFormat.md)
-         - [DateFormat](docs/DateFormat.md)
-         - [ErrorDetail](docs/ErrorDetail.md)
-         - [ErrorResponse](docs/ErrorResponse.md)
-         - [HybridTransaction](docs/HybridTransaction.md)
-         - [HybridTransactionAllOf](docs/HybridTransactionAllOf.md)
-         - [HybridTransactionsResponse](docs/HybridTransactionsResponse.md)
-         - [HybridTransactionsResponseData](docs/HybridTransactionsResponseData.md)
-         - [MonthDetail](docs/MonthDetail.md)
-         - [MonthDetailAllOf](docs/MonthDetailAllOf.md)
-         - [MonthDetailResponse](docs/MonthDetailResponse.md)
-         - [MonthDetailResponseData](docs/MonthDetailResponseData.md)
-         - [MonthSummariesResponse](docs/MonthSummariesResponse.md)
-         - [MonthSummariesResponseData](docs/MonthSummariesResponseData.md)
-         - [MonthSummary](docs/MonthSummary.md)
-         - [Payee](docs/Payee.md)
-         - [PayeeLocation](docs/PayeeLocation.md)
-         - [PayeeLocationResponse](docs/PayeeLocationResponse.md)
-         - [PayeeLocationResponseData](docs/PayeeLocationResponseData.md)
-         - [PayeeLocationsResponse](docs/PayeeLocationsResponse.md)
-         - [PayeeLocationsResponseData](docs/PayeeLocationsResponseData.md)
-         - [PayeeResponse](docs/PayeeResponse.md)
-         - [PayeeResponseData](docs/PayeeResponseData.md)
-         - [PayeesResponse](docs/PayeesResponse.md)
-         - [PayeesResponseData](docs/PayeesResponseData.md)
-         - [SaveCategoryResponse](docs/SaveCategoryResponse.md)
-         - [SaveCategoryResponseData](docs/SaveCategoryResponseData.md)
-         - [SaveMonthCategory](docs/SaveMonthCategory.md)
-         - [SaveMonthCategoryWrapper](docs/SaveMonthCategoryWrapper.md)
-         - [SaveTransaction](docs/SaveTransaction.md)
-         - [SaveTransactionWrapper](docs/SaveTransactionWrapper.md)
-         - [SaveTransactionsResponse](docs/SaveTransactionsResponse.md)
-         - [SaveTransactionsResponseData](docs/SaveTransactionsResponseData.md)
-         - [SaveTransactionsWrapper](docs/SaveTransactionsWrapper.md)
-         - [ScheduledSubTransaction](docs/ScheduledSubTransaction.md)
-         - [ScheduledTransactionDetail](docs/ScheduledTransactionDetail.md)
-         - [ScheduledTransactionDetailAllOf](docs/ScheduledTransactionDetailAllOf.md)
-         - [ScheduledTransactionResponse](docs/ScheduledTransactionResponse.md)
-         - [ScheduledTransactionResponseData](docs/ScheduledTransactionResponseData.md)
-         - [ScheduledTransactionSummary](docs/ScheduledTransactionSummary.md)
-         - [ScheduledTransactionsResponse](docs/ScheduledTransactionsResponse.md)
-         - [ScheduledTransactionsResponseData](docs/ScheduledTransactionsResponseData.md)
-         - [SubTransaction](docs/SubTransaction.md)
-         - [TransactionDetail](docs/TransactionDetail.md)
-         - [TransactionDetailAllOf](docs/TransactionDetailAllOf.md)
-         - [TransactionResponse](docs/TransactionResponse.md)
-         - [TransactionResponseData](docs/TransactionResponseData.md)
-         - [TransactionSummary](docs/TransactionSummary.md)
-         - [TransactionsResponse](docs/TransactionsResponse.md)
-         - [TransactionsResponseData](docs/TransactionsResponseData.md)
-         - [UpdateTransaction](docs/UpdateTransaction.md)
-         - [UpdateTransactionAllOf](docs/UpdateTransactionAllOf.md)
-         - [UpdateTransactionsWrapper](docs/UpdateTransactionsWrapper.md)
-         - [User](docs/User.md)
-         - [UserResponse](docs/UserResponse.md)
-         - [UserResponseData](docs/UserResponseData.md)
-        
-        
-        ## Documentation For Authorization
-        
-        
-        ## bearer
-        
-        - **Type**: API key
-        - **API key parameter name**: Authorization
-        - **Location**: HTTP header
-        
-        
-        ## Author
-        
-        
-        
-        
-        
-Keywords: YNAB
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Description-Content-Type: text/markdown
+# ynab-api
+
+Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com
+
+This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
+
+- API version: 1.0.0
+- Package version: 1.0.0
+- Build package: org.openapitools.codegen.languages.PythonClientCodegen
+
+## Requirements.
+
+Python >= 3.6
+
+## Installation & Usage
+
+### pip install
+
+```sh
+pip install git+https://github.com/dmlerner/ynab-api.git
+```
+
+NOTE: If you get issues about nullability or things being not set, consider installed the "nullfix" branch:
+
+```sh
+pip install git+https://github.com/dmlerner/ynab-api.git@nullfix
+```
+
+(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/dmlerner/ynab-api.git`)
+
+Then import the package:
+
+```python
+import ynab_api
+```
+
+NOTE: the pip package `ynab_api` is an old, non-working version of this.
+I am working to get it updated, but am locked out of that account.
+
+### Setuptools
+
+Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
+
+```sh
+python setup.py install --user
+```
+
+(or `sudo python setup.py install` to install the package for all users)
+
+Then import the package:
+
+```python
+import ynab_api
+```
+
+## Getting Started
+
+Please follow the [installation procedure](#installation--usage) and then run the following:
+
+```
+python ynabdemo.py
+```
+
+## Sample usage (ynabdemo.py)
+
+```python
+import json
+import ynab_api
+from pprint import pprint
+from ynab_api.api import accounts_api
+'''
+secrets.json should be manually generated as:
+
+{
+   "budget_id":"xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx"
+   "api_key":"xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
+}
+
+To get an api_key:
+Sign in to the YNAB web app
+and go to the "Account Settings" page
+and then to the "Developer Settings" page.
+Under the "Personal Access Tokens" section,
+click "New Token", enter your password
+and click "Generate" to get an access token.
+
+To get your budget_id:
+Sign in to the YNAB web app and go the budget of interest.
+Copy YOUR_BUDGET_ID from the url:
+https://app.youneedabudget.com/YOUR_BUDGET_ID/budget
+
+Or, populate the fields directly in your code.
+'''
+
+with open('secrets.json') as f:
+    secrets = json.load(f)
+budget_id = secrets['budget_id']
+api_key = secrets['api_key']
+
+configuration = ynab_api.Configuration(
+    host="https://api.youneedabudget.com/v1")
+configuration.api_key['bearer'] = api_key
+configuration.api_key_prefix['bearer'] = 'Bearer'
+
+with ynab_api.ApiClient(configuration) as api_client:
+    api_instance = accounts_api.AccountsApi(api_client)
+
+    try:
+        api_response = api_instance.get_accounts(budget_id)
+        pprint(api_response)
+    except ynab_api.ApiException as e:
+        print("Exception: %s\n" % e)
+```
+
+## Documentation for API Endpoints
+
+All URIs are relative to *https://api.youneedabudget.com/v1*
+
+Class | Method | HTTP request | Description
+------------ | ------------- | ------------- | -------------
+*AccountsApi* | [**create_account**](docs/AccountsApi.md#create_account) | **POST** /budgets/{budget_id}/accounts | Create a new account
+*AccountsApi* | [**get_account_by_id**](docs/AccountsApi.md#get_account_by_id) | **GET** /budgets/{budget_id}/accounts/{account_id} | Single account
+*AccountsApi* | [**get_accounts**](docs/AccountsApi.md#get_accounts) | **GET** /budgets/{budget_id}/accounts | Account list
+*BudgetsApi* | [**get_budget_by_id**](docs/BudgetsApi.md#get_budget_by_id) | **GET** /budgets/{budget_id} | Single budget
+*BudgetsApi* | [**get_budget_settings_by_id**](docs/BudgetsApi.md#get_budget_settings_by_id) | **GET** /budgets/{budget_id}/settings | Budget Settings
+*BudgetsApi* | [**get_budgets**](docs/BudgetsApi.md#get_budgets) | **GET** /budgets | List budgets
+*CategoriesApi* | [**get_categories**](docs/CategoriesApi.md#get_categories) | **GET** /budgets/{budget_id}/categories | List categories
+*CategoriesApi* | [**get_category_by_id**](docs/CategoriesApi.md#get_category_by_id) | **GET** /budgets/{budget_id}/categories/{category_id} | Single category
+*CategoriesApi* | [**get_month_category_by_id**](docs/CategoriesApi.md#get_month_category_by_id) | **GET** /budgets/{budget_id}/months/{month}/categories/{category_id} | Single category for a specific budget month
+*CategoriesApi* | [**update_month_category**](docs/CategoriesApi.md#update_month_category) | **PATCH** /budgets/{budget_id}/months/{month}/categories/{category_id} | Update a category for a specific month
+*DeprecatedApi* | [**bulk_create_transactions**](docs/DeprecatedApi.md#bulk_create_transactions) | **POST** /budgets/{budget_id}/transactions/bulk | Bulk create transactions
+*MonthsApi* | [**get_budget_month**](docs/MonthsApi.md#get_budget_month) | **GET** /budgets/{budget_id}/months/{month} | Single budget month
+*MonthsApi* | [**get_budget_months**](docs/MonthsApi.md#get_budget_months) | **GET** /budgets/{budget_id}/months | List budget months
+*PayeeLocationsApi* | [**get_payee_location_by_id**](docs/PayeeLocationsApi.md#get_payee_location_by_id) | **GET** /budgets/{budget_id}/payee_locations/{payee_location_id} | Single payee location
+*PayeeLocationsApi* | [**get_payee_locations**](docs/PayeeLocationsApi.md#get_payee_locations) | **GET** /budgets/{budget_id}/payee_locations | List payee locations
+*PayeeLocationsApi* | [**get_payee_locations_by_payee**](docs/PayeeLocationsApi.md#get_payee_locations_by_payee) | **GET** /budgets/{budget_id}/payees/{payee_id}/payee_locations | List locations for a payee
+*PayeesApi* | [**get_payee_by_id**](docs/PayeesApi.md#get_payee_by_id) | **GET** /budgets/{budget_id}/payees/{payee_id} | Single payee
+*PayeesApi* | [**get_payees**](docs/PayeesApi.md#get_payees) | **GET** /budgets/{budget_id}/payees | List payees
+*ScheduledTransactionsApi* | [**get_scheduled_transaction_by_id**](docs/ScheduledTransactionsApi.md#get_scheduled_transaction_by_id) | **GET** /budgets/{budget_id}/scheduled_transactions/{scheduled_transaction_id} | Single scheduled transaction
+*ScheduledTransactionsApi* | [**get_scheduled_transactions**](docs/ScheduledTransactionsApi.md#get_scheduled_transactions) | **GET** /budgets/{budget_id}/scheduled_transactions | List scheduled transactions
+*TransactionsApi* | [**create_transaction**](docs/TransactionsApi.md#create_transaction) | **POST** /budgets/{budget_id}/transactions | Create a single transaction or multiple transactions
+*TransactionsApi* | [**get_transaction_by_id**](docs/TransactionsApi.md#get_transaction_by_id) | **GET** /budgets/{budget_id}/transactions/{transaction_id} | Single transaction
+*TransactionsApi* | [**get_transactions**](docs/TransactionsApi.md#get_transactions) | **GET** /budgets/{budget_id}/transactions | List transactions
+*TransactionsApi* | [**get_transactions_by_account**](docs/TransactionsApi.md#get_transactions_by_account) | **GET** /budgets/{budget_id}/accounts/{account_id}/transactions | List account transactions
+*TransactionsApi* | [**get_transactions_by_category**](docs/TransactionsApi.md#get_transactions_by_category) | **GET** /budgets/{budget_id}/categories/{category_id}/transactions | List category transactions
+*TransactionsApi* | [**get_transactions_by_payee**](docs/TransactionsApi.md#get_transactions_by_payee) | **GET** /budgets/{budget_id}/payees/{payee_id}/transactions | List payee transactions
+*TransactionsApi* | [**import_transactions**](docs/TransactionsApi.md#import_transactions) | **POST** /budgets/{budget_id}/transactions/import | Import transactions
+*TransactionsApi* | [**update_transaction**](docs/TransactionsApi.md#update_transaction) | **PUT** /budgets/{budget_id}/transactions/{transaction_id} | Updates an existing transaction
+*TransactionsApi* | [**update_transactions**](docs/TransactionsApi.md#update_transactions) | **PATCH** /budgets/{budget_id}/transactions | Update multiple transactions
+*UserApi* | [**get_user**](docs/UserApi.md#get_user) | **GET** /user | User info
+
+## Documentation For Models
+
+- [Account](docs/Account.md)
+- [AccountResponse](docs/AccountResponse.md)
+- [AccountResponseData](docs/AccountResponseData.md)
+- [AccountsResponse](docs/AccountsResponse.md)
+- [AccountsResponseData](docs/AccountsResponseData.md)
+- [BudgetDetail](docs/BudgetDetail.md)
+- [BudgetDetailAllOf](docs/BudgetDetailAllOf.md)
+- [BudgetDetailResponse](docs/BudgetDetailResponse.md)
+- [BudgetDetailResponseData](docs/BudgetDetailResponseData.md)
+- [BudgetSettings](docs/BudgetSettings.md)
+- [BudgetSettingsResponse](docs/BudgetSettingsResponse.md)
+- [BudgetSettingsResponseData](docs/BudgetSettingsResponseData.md)
+- [BudgetSummary](docs/BudgetSummary.md)
+- [BudgetSummaryResponse](docs/BudgetSummaryResponse.md)
+- [BudgetSummaryResponseData](docs/BudgetSummaryResponseData.md)
+- [BulkResponse](docs/BulkResponse.md)
+- [BulkResponseData](docs/BulkResponseData.md)
+- [BulkResponseDataBulk](docs/BulkResponseDataBulk.md)
+- [BulkTransactions](docs/BulkTransactions.md)
+- [CategoriesResponse](docs/CategoriesResponse.md)
+- [CategoriesResponseData](docs/CategoriesResponseData.md)
+- [Category](docs/Category.md)
+- [CategoryGroup](docs/CategoryGroup.md)
+- [CategoryGroupWithCategories](docs/CategoryGroupWithCategories.md)
+- [CategoryGroupWithCategoriesAllOf](docs/CategoryGroupWithCategoriesAllOf.md)
+- [CategoryResponse](docs/CategoryResponse.md)
+- [CategoryResponseData](docs/CategoryResponseData.md)
+- [CurrencyFormat](docs/CurrencyFormat.md)
+- [DateFormat](docs/DateFormat.md)
+- [ErrorDetail](docs/ErrorDetail.md)
+- [ErrorResponse](docs/ErrorResponse.md)
+- [HybridTransaction](docs/HybridTransaction.md)
+- [HybridTransactionAllOf](docs/HybridTransactionAllOf.md)
+- [HybridTransactionsResponse](docs/HybridTransactionsResponse.md)
+- [HybridTransactionsResponseData](docs/HybridTransactionsResponseData.md)
+- [MonthDetail](docs/MonthDetail.md)
+- [MonthDetailAllOf](docs/MonthDetailAllOf.md)
+- [MonthDetailResponse](docs/MonthDetailResponse.md)
+- [MonthDetailResponseData](docs/MonthDetailResponseData.md)
+- [MonthSummariesResponse](docs/MonthSummariesResponse.md)
+- [MonthSummariesResponseData](docs/MonthSummariesResponseData.md)
+- [MonthSummary](docs/MonthSummary.md)
+- [Payee](docs/Payee.md)
+- [PayeeLocation](docs/PayeeLocation.md)
+- [PayeeLocationResponse](docs/PayeeLocationResponse.md)
+- [PayeeLocationResponseData](docs/PayeeLocationResponseData.md)
+- [PayeeLocationsResponse](docs/PayeeLocationsResponse.md)
+- [PayeeLocationsResponseData](docs/PayeeLocationsResponseData.md)
+- [PayeeResponse](docs/PayeeResponse.md)
+- [PayeeResponseData](docs/PayeeResponseData.md)
+- [PayeesResponse](docs/PayeesResponse.md)
+- [PayeesResponseData](docs/PayeesResponseData.md)
+- [SaveAccount](docs/SaveAccount.md)
+- [SaveAccountWrapper](docs/SaveAccountWrapper.md)
+- [SaveCategoryResponse](docs/SaveCategoryResponse.md)
+- [SaveCategoryResponseData](docs/SaveCategoryResponseData.md)
+- [SaveMonthCategory](docs/SaveMonthCategory.md)
+- [SaveMonthCategoryWrapper](docs/SaveMonthCategoryWrapper.md)
+- [SaveSubTransaction](docs/SaveSubTransaction.md)
+- [SaveTransaction](docs/SaveTransaction.md)
+- [SaveTransactionWrapper](docs/SaveTransactionWrapper.md)
+- [SaveTransactionsResponse](docs/SaveTransactionsResponse.md)
+- [SaveTransactionsResponseData](docs/SaveTransactionsResponseData.md)
+- [SaveTransactionsWrapper](docs/SaveTransactionsWrapper.md)
+- [ScheduledSubTransaction](docs/ScheduledSubTransaction.md)
+- [ScheduledTransactionDetail](docs/ScheduledTransactionDetail.md)
+- [ScheduledTransactionDetailAllOf](docs/ScheduledTransactionDetailAllOf.md)
+- [ScheduledTransactionResponse](docs/ScheduledTransactionResponse.md)
+- [ScheduledTransactionResponseData](docs/ScheduledTransactionResponseData.md)
+- [ScheduledTransactionSummary](docs/ScheduledTransactionSummary.md)
+- [ScheduledTransactionsResponse](docs/ScheduledTransactionsResponse.md)
+- [ScheduledTransactionsResponseData](docs/ScheduledTransactionsResponseData.md)
+- [SubTransaction](docs/SubTransaction.md)
+- [TransactionDetail](docs/TransactionDetail.md)
+- [TransactionDetailAllOf](docs/TransactionDetailAllOf.md)
+- [TransactionResponse](docs/TransactionResponse.md)
+- [TransactionResponseData](docs/TransactionResponseData.md)
+- [TransactionSummary](docs/TransactionSummary.md)
+- [TransactionsImportResponse](docs/TransactionsImportResponse.md)
+- [TransactionsImportResponseData](docs/TransactionsImportResponseData.md)
+- [TransactionsResponse](docs/TransactionsResponse.md)
+- [TransactionsResponseData](docs/TransactionsResponseData.md)
+- [UpdateTransaction](docs/UpdateTransaction.md)
+- [UpdateTransactionAllOf](docs/UpdateTransactionAllOf.md)
+- [UpdateTransactionsWrapper](docs/UpdateTransactionsWrapper.md)
+- [User](docs/User.md)
+- [UserResponse](docs/UserResponse.md)
+- [UserResponseData](docs/UserResponseData.md)
+
+## Documentation For Authorization
+
+## bearer
+
+- **Type**: API key
+- **API key parameter name**: Authorization
+- **Location**: HTTP header
+
+## Author
+
+David Lerner
+
+## Notes for Large OpenAPI documents
+
+If the OpenAPI document is large, imports in ynab_api.apis and ynab_api.models may fail with a
+RecursionError indicating the maximum recursion limit has been exceeded. In that case, there are a couple of solutions:
+
+Solution 1:
+Use specific imports for apis and models like:
+
+- `from ynab_api.api.default_api import DefaultApi`
+- `from ynab_api.model.pet import Pet`
+
+Solution 2:
+Before importing the package, adjust the maximum recursion limit as shown below:
+
+```
+import sys
+sys.setrecursionlimit(1500)
+import ynab_api
+from ynab_api.apis import *
+from ynab_api.models import *
+```
```

### Comparing `ynab-api-1.0.0/test/test_account.py` & `ynab-api-2.0.0/test/test_save_account_wrapper.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.account import Account  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.save_account import SaveAccount
 
+globals()['SaveAccount'] = SaveAccount
+from ynab_api.model.save_account_wrapper import SaveAccountWrapper
 
-class TestAccount(unittest.TestCase):
-    """Account unit test stubs"""
 
+class TestSaveAccountWrapper(unittest.TestCase):
+    """SaveAccountWrapper unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAccount(self):
-        """Test Account"""
+    def testSaveAccountWrapper(self):
+        """Test SaveAccountWrapper"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.account.Account()  # noqa: E501
+        # model = SaveAccountWrapper()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_accounts_api.py` & `ynab-api-2.0.0/test/test_user_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,33 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
 import unittest
 
 import ynab_api
-from ynab_api.api.accounts_api import AccountsApi  # noqa: E501
-from ynab_api.rest import ApiException
-
+from ynab_api.api.user_api import UserApi  # noqa: E501
 
-class TestAccountsApi(unittest.TestCase):
-    """AccountsApi unit test stubs"""
 
+class TestUserApi(unittest.TestCase):
+    """UserApi unit test stubs"""
     def setUp(self):
-        self.api = ynab_api.api.accounts_api.AccountsApi()  # noqa: E501
+        self.api = UserApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_get_account_by_id(self):
-        """Test case for get_account_by_id
-
-        Single account  # noqa: E501
-        """
-        pass
-
-    def test_get_accounts(self):
-        """Test case for get_accounts
+    def test_get_user(self):
+        """Test case for get_user
 
-        Account list  # noqa: E501
+        User info  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_accounts_response.py` & `ynab-api-2.0.0/test/test_bulk_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.accounts_response import AccountsResponse  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.bulk_response_data import BulkResponseData
 
+globals()['BulkResponseData'] = BulkResponseData
+from ynab_api.model.bulk_response import BulkResponse
 
-class TestAccountsResponse(unittest.TestCase):
-    """AccountsResponse unit test stubs"""
 
+class TestBulkResponse(unittest.TestCase):
+    """BulkResponse unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAccountsResponse(self):
-        """Test AccountsResponse"""
+    def testBulkResponse(self):
+        """Test BulkResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.accounts_response.AccountsResponse()  # noqa: E501
+        # model = BulkResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_accounts_response_data.py` & `ynab-api-2.0.0/test/test_accounts_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.accounts_response_data import AccountsResponseData  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.accounts_response_data import AccountsResponseData
 
+globals()['AccountsResponseData'] = AccountsResponseData
+from ynab_api.model.accounts_response import AccountsResponse
 
-class TestAccountsResponseData(unittest.TestCase):
-    """AccountsResponseData unit test stubs"""
 
+class TestAccountsResponse(unittest.TestCase):
+    """AccountsResponse unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAccountsResponseData(self):
-        """Test AccountsResponseData"""
+    def testAccountsResponse(self):
+        """Test AccountsResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.accounts_response_data.AccountsResponseData()  # noqa: E501
+        # model = AccountsResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_account_response.py` & `ynab-api-2.0.0/test/test_save_category_response_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.account_response import AccountResponse  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.category import Category
 
+globals()['Category'] = Category
+from ynab_api.model.save_category_response_data import SaveCategoryResponseData
 
-class TestAccountResponse(unittest.TestCase):
-    """AccountResponse unit test stubs"""
 
+class TestSaveCategoryResponseData(unittest.TestCase):
+    """SaveCategoryResponseData unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAccountResponse(self):
-        """Test AccountResponse"""
+    def testSaveCategoryResponseData(self):
+        """Test SaveCategoryResponseData"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.account_response.AccountResponse()  # noqa: E501
+        # model = SaveCategoryResponseData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_account_response_data.py` & `ynab-api-2.0.0/test/test_user_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.account_response_data import AccountResponseData  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.user_response_data import UserResponseData
 
+globals()['UserResponseData'] = UserResponseData
+from ynab_api.model.user_response import UserResponse
 
-class TestAccountResponseData(unittest.TestCase):
-    """AccountResponseData unit test stubs"""
 
+class TestUserResponse(unittest.TestCase):
+    """UserResponse unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAccountResponseData(self):
-        """Test AccountResponseData"""
+    def testUserResponse(self):
+        """Test UserResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.account_response_data.AccountResponseData()  # noqa: E501
+        # model = UserResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_budgets_api.py` & `ynab-api-2.0.0/test/test_months_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,40 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
 import unittest
 
 import ynab_api
-from ynab_api.api.budgets_api import BudgetsApi  # noqa: E501
-from ynab_api.rest import ApiException
-
+from ynab_api.api.months_api import MonthsApi  # noqa: E501
 
-class TestBudgetsApi(unittest.TestCase):
-    """BudgetsApi unit test stubs"""
 
+class TestMonthsApi(unittest.TestCase):
+    """MonthsApi unit test stubs"""
     def setUp(self):
-        self.api = ynab_api.api.budgets_api.BudgetsApi()  # noqa: E501
+        self.api = MonthsApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_get_budget_by_id(self):
-        """Test case for get_budget_by_id
-
-        Single budget  # noqa: E501
-        """
-        pass
-
-    def test_get_budget_settings_by_id(self):
-        """Test case for get_budget_settings_by_id
+    def test_get_budget_month(self):
+        """Test case for get_budget_month
 
-        Budget Settings  # noqa: E501
+        Single budget month  # noqa: E501
         """
         pass
 
-    def test_get_budgets(self):
-        """Test case for get_budgets
+    def test_get_budget_months(self):
+        """Test case for get_budget_months
 
-        List budgets  # noqa: E501
+        List budget months  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_budget_detail.py` & `ynab-api-2.0.0/test/test_date_format.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.budget_detail import BudgetDetail  # noqa: E501
-from ynab_api.rest import ApiException
-
+from ynab_api.model.date_format import DateFormat
 
-class TestBudgetDetail(unittest.TestCase):
-    """BudgetDetail unit test stubs"""
 
+class TestDateFormat(unittest.TestCase):
+    """DateFormat unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testBudgetDetail(self):
-        """Test BudgetDetail"""
+    def testDateFormat(self):
+        """Test DateFormat"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.budget_detail.BudgetDetail()  # noqa: E501
+        # model = DateFormat()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_budget_detail_all_of.py` & `ynab-api-2.0.0/test/test_user_response_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.budget_detail_all_of import BudgetDetailAllOf  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.user import User
 
+globals()['User'] = User
+from ynab_api.model.user_response_data import UserResponseData
 
-class TestBudgetDetailAllOf(unittest.TestCase):
-    """BudgetDetailAllOf unit test stubs"""
 
+class TestUserResponseData(unittest.TestCase):
+    """UserResponseData unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testBudgetDetailAllOf(self):
-        """Test BudgetDetailAllOf"""
+    def testUserResponseData(self):
+        """Test UserResponseData"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.budget_detail_all_of.BudgetDetailAllOf()  # noqa: E501
+        # model = UserResponseData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_budget_detail_response.py` & `ynab-api-2.0.0/test/test_budget_detail_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.budget_detail_response import BudgetDetailResponse  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.budget_detail_response_data import BudgetDetailResponseData
+
+globals()['BudgetDetailResponseData'] = BudgetDetailResponseData
+from ynab_api.model.budget_detail_response import BudgetDetailResponse
 
 
 class TestBudgetDetailResponse(unittest.TestCase):
     """BudgetDetailResponse unit test stubs"""
-
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testBudgetDetailResponse(self):
         """Test BudgetDetailResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.budget_detail_response.BudgetDetailResponse()  # noqa: E501
+        # model = BudgetDetailResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_budget_detail_response_data.py` & `ynab-api-2.0.0/test/test_budget_detail_response_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.budget_detail_response_data import BudgetDetailResponseData  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.budget_detail import BudgetDetail
+
+globals()['BudgetDetail'] = BudgetDetail
+from ynab_api.model.budget_detail_response_data import BudgetDetailResponseData
 
 
 class TestBudgetDetailResponseData(unittest.TestCase):
     """BudgetDetailResponseData unit test stubs"""
-
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testBudgetDetailResponseData(self):
         """Test BudgetDetailResponseData"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.budget_detail_response_data.BudgetDetailResponseData()  # noqa: E501
+        # model = BudgetDetailResponseData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_budget_settings.py` & `ynab-api-2.0.0/test/test_budget_settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.budget_settings import BudgetSettings  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.currency_format import CurrencyFormat
+from ynab_api.model.date_format import DateFormat
+
+globals()['CurrencyFormat'] = CurrencyFormat
+globals()['DateFormat'] = DateFormat
+from ynab_api.model.budget_settings import BudgetSettings
 
 
 class TestBudgetSettings(unittest.TestCase):
     """BudgetSettings unit test stubs"""
-
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testBudgetSettings(self):
         """Test BudgetSettings"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.budget_settings.BudgetSettings()  # noqa: E501
+        # model = BudgetSettings()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_budget_settings_response.py` & `ynab-api-2.0.0/test/test_payees_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.budget_settings_response import BudgetSettingsResponse  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.payees_response_data import PayeesResponseData
 
+globals()['PayeesResponseData'] = PayeesResponseData
+from ynab_api.model.payees_response import PayeesResponse
 
-class TestBudgetSettingsResponse(unittest.TestCase):
-    """BudgetSettingsResponse unit test stubs"""
 
+class TestPayeesResponse(unittest.TestCase):
+    """PayeesResponse unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testBudgetSettingsResponse(self):
-        """Test BudgetSettingsResponse"""
+    def testPayeesResponse(self):
+        """Test PayeesResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.budget_settings_response.BudgetSettingsResponse()  # noqa: E501
+        # model = PayeesResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_budget_settings_response_data.py` & `ynab-api-2.0.0/test/test_budget_settings_response_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.budget_settings_response_data import BudgetSettingsResponseData  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.budget_settings import BudgetSettings
+
+globals()['BudgetSettings'] = BudgetSettings
+from ynab_api.model.budget_settings_response_data import BudgetSettingsResponseData
 
 
 class TestBudgetSettingsResponseData(unittest.TestCase):
     """BudgetSettingsResponseData unit test stubs"""
-
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testBudgetSettingsResponseData(self):
         """Test BudgetSettingsResponseData"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.budget_settings_response_data.BudgetSettingsResponseData()  # noqa: E501
+        # model = BudgetSettingsResponseData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_budget_summary.py` & `ynab-api-2.0.0/test/test_user.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.budget_summary import BudgetSummary  # noqa: E501
-from ynab_api.rest import ApiException
-
+from ynab_api.model.user import User
 
-class TestBudgetSummary(unittest.TestCase):
-    """BudgetSummary unit test stubs"""
 
+class TestUser(unittest.TestCase):
+    """User unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testBudgetSummary(self):
-        """Test BudgetSummary"""
+    def testUser(self):
+        """Test User"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.budget_summary.BudgetSummary()  # noqa: E501
+        # model = User()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_budget_summary_response.py` & `ynab-api-2.0.0/test/test_budget_summary_response_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.budget_summary_response import BudgetSummaryResponse  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.budget_summary import BudgetSummary
 
+globals()['BudgetSummary'] = BudgetSummary
+from ynab_api.model.budget_summary_response_data import BudgetSummaryResponseData
 
-class TestBudgetSummaryResponse(unittest.TestCase):
-    """BudgetSummaryResponse unit test stubs"""
 
+class TestBudgetSummaryResponseData(unittest.TestCase):
+    """BudgetSummaryResponseData unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testBudgetSummaryResponse(self):
-        """Test BudgetSummaryResponse"""
+    def testBudgetSummaryResponseData(self):
+        """Test BudgetSummaryResponseData"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.budget_summary_response.BudgetSummaryResponse()  # noqa: E501
+        # model = BudgetSummaryResponseData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_budget_summary_response_data.py` & `ynab-api-2.0.0/test/test_payee_locations_response_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.budget_summary_response_data import BudgetSummaryResponseData  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.payee_location import PayeeLocation
 
+globals()['PayeeLocation'] = PayeeLocation
+from ynab_api.model.payee_locations_response_data import PayeeLocationsResponseData
 
-class TestBudgetSummaryResponseData(unittest.TestCase):
-    """BudgetSummaryResponseData unit test stubs"""
 
+class TestPayeeLocationsResponseData(unittest.TestCase):
+    """PayeeLocationsResponseData unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testBudgetSummaryResponseData(self):
-        """Test BudgetSummaryResponseData"""
+    def testPayeeLocationsResponseData(self):
+        """Test PayeeLocationsResponseData"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.budget_summary_response_data.BudgetSummaryResponseData()  # noqa: E501
+        # model = PayeeLocationsResponseData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_bulk_response_data.py` & `ynab-api-2.0.0/test/test_account_response_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.bulk_response_data import BulkResponseData  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.account import Account
 
+globals()['Account'] = Account
+from ynab_api.model.account_response_data import AccountResponseData
 
-class TestBulkResponseData(unittest.TestCase):
-    """BulkResponseData unit test stubs"""
 
+class TestAccountResponseData(unittest.TestCase):
+    """AccountResponseData unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testBulkResponseData(self):
-        """Test BulkResponseData"""
+    def testAccountResponseData(self):
+        """Test AccountResponseData"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.bulk_response_data.BulkResponseData()  # noqa: E501
+        # model = AccountResponseData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_bulk_response_data_bulk.py` & `ynab-api-2.0.0/test/test_transactions_response_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.bulk_response_data_bulk import BulkResponseDataBulk  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.transaction_detail import TransactionDetail
 
+globals()['TransactionDetail'] = TransactionDetail
+from ynab_api.model.transactions_response_data import TransactionsResponseData
 
-class TestBulkResponseDataBulk(unittest.TestCase):
-    """BulkResponseDataBulk unit test stubs"""
 
+class TestTransactionsResponseData(unittest.TestCase):
+    """TransactionsResponseData unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testBulkResponseDataBulk(self):
-        """Test BulkResponseDataBulk"""
+    def testTransactionsResponseData(self):
+        """Test TransactionsResponseData"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.bulk_response_data_bulk.BulkResponseDataBulk()  # noqa: E501
+        # model = TransactionsResponseData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_bulk_transactions.py` & `ynab-api-2.0.0/test/test_sub_transaction.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.bulk_transactions import BulkTransactions  # noqa: E501
-from ynab_api.rest import ApiException
-
+from ynab_api.model.sub_transaction import SubTransaction
 
-class TestBulkTransactions(unittest.TestCase):
-    """BulkTransactions unit test stubs"""
 
+class TestSubTransaction(unittest.TestCase):
+    """SubTransaction unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testBulkTransactions(self):
-        """Test BulkTransactions"""
+    def testSubTransaction(self):
+        """Test SubTransaction"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.bulk_transactions.BulkTransactions()  # noqa: E501
+        # model = SubTransaction()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_categories_api.py` & `ynab-api-2.0.0/test/test_categories_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,26 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
 import unittest
 
 import ynab_api
 from ynab_api.api.categories_api import CategoriesApi  # noqa: E501
-from ynab_api.rest import ApiException
 
 
 class TestCategoriesApi(unittest.TestCase):
     """CategoriesApi unit test stubs"""
-
     def setUp(self):
-        self.api = ynab_api.api.categories_api.CategoriesApi()  # noqa: E501
+        self.api = CategoriesApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_get_categories(self):
         """Test case for get_categories
```

### Comparing `ynab-api-1.0.0/test/test_categories_response.py` & `ynab-api-2.0.0/test/test_save_month_category.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.categories_response import CategoriesResponse  # noqa: E501
-from ynab_api.rest import ApiException
-
+from ynab_api.model.save_month_category import SaveMonthCategory
 
-class TestCategoriesResponse(unittest.TestCase):
-    """CategoriesResponse unit test stubs"""
 
+class TestSaveMonthCategory(unittest.TestCase):
+    """SaveMonthCategory unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCategoriesResponse(self):
-        """Test CategoriesResponse"""
+    def testSaveMonthCategory(self):
+        """Test SaveMonthCategory"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.categories_response.CategoriesResponse()  # noqa: E501
+        # model = SaveMonthCategory()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_categories_response_data.py` & `ynab-api-2.0.0/test/test_payees_response_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.categories_response_data import CategoriesResponseData  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.payee import Payee
 
+globals()['Payee'] = Payee
+from ynab_api.model.payees_response_data import PayeesResponseData
 
-class TestCategoriesResponseData(unittest.TestCase):
-    """CategoriesResponseData unit test stubs"""
 
+class TestPayeesResponseData(unittest.TestCase):
+    """PayeesResponseData unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCategoriesResponseData(self):
-        """Test CategoriesResponseData"""
+    def testPayeesResponseData(self):
+        """Test PayeesResponseData"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.categories_response_data.CategoriesResponseData()  # noqa: E501
+        # model = PayeesResponseData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_category.py` & `ynab-api-2.0.0/test/test_deprecated_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
 import unittest
 
 import ynab_api
-from ynab_api.models.category import Category  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.api.deprecated_api import DeprecatedApi  # noqa: E501
 
 
-class TestCategory(unittest.TestCase):
-    """Category unit test stubs"""
-
+class TestDeprecatedApi(unittest.TestCase):
+    """DeprecatedApi unit test stubs"""
     def setUp(self):
-        pass
+        self.api = DeprecatedApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testCategory(self):
-        """Test Category"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.category.Category()  # noqa: E501
+    def test_bulk_create_transactions(self):
+        """Test case for bulk_create_transactions
+
+        Bulk create transactions  # noqa: E501
+        """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_category_group.py` & `ynab-api-2.0.0/test/test_category_group.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.category_group import CategoryGroup  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.category_group import CategoryGroup
 
 
 class TestCategoryGroup(unittest.TestCase):
     """CategoryGroup unit test stubs"""
-
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testCategoryGroup(self):
         """Test CategoryGroup"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.category_group.CategoryGroup()  # noqa: E501
+        # model = CategoryGroup()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_category_group_with_categories.py` & `ynab-api-2.0.0/test/test_categories_response_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.category_group_with_categories import CategoryGroupWithCategories  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.category_group_with_categories import CategoryGroupWithCategories
 
+globals()['CategoryGroupWithCategories'] = CategoryGroupWithCategories
+from ynab_api.model.categories_response_data import CategoriesResponseData
 
-class TestCategoryGroupWithCategories(unittest.TestCase):
-    """CategoryGroupWithCategories unit test stubs"""
 
+class TestCategoriesResponseData(unittest.TestCase):
+    """CategoriesResponseData unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCategoryGroupWithCategories(self):
-        """Test CategoryGroupWithCategories"""
+    def testCategoriesResponseData(self):
+        """Test CategoriesResponseData"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.category_group_with_categories.CategoryGroupWithCategories()  # noqa: E501
+        # model = CategoriesResponseData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_category_group_with_categories_all_of.py` & `ynab-api-2.0.0/test/test_category_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.category_group_with_categories_all_of import CategoryGroupWithCategoriesAllOf  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.category_response_data import CategoryResponseData
 
+globals()['CategoryResponseData'] = CategoryResponseData
+from ynab_api.model.category_response import CategoryResponse
 
-class TestCategoryGroupWithCategoriesAllOf(unittest.TestCase):
-    """CategoryGroupWithCategoriesAllOf unit test stubs"""
 
+class TestCategoryResponse(unittest.TestCase):
+    """CategoryResponse unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCategoryGroupWithCategoriesAllOf(self):
-        """Test CategoryGroupWithCategoriesAllOf"""
+    def testCategoryResponse(self):
+        """Test CategoryResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.category_group_with_categories_all_of.CategoryGroupWithCategoriesAllOf()  # noqa: E501
+        # model = CategoryResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_category_response.py` & `ynab-api-2.0.0/test/test_category.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.category_response import CategoryResponse  # noqa: E501
-from ynab_api.rest import ApiException
-
+from ynab_api.model.category import Category
 
-class TestCategoryResponse(unittest.TestCase):
-    """CategoryResponse unit test stubs"""
 
+class TestCategory(unittest.TestCase):
+    """Category unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCategoryResponse(self):
-        """Test CategoryResponse"""
+    def testCategory(self):
+        """Test Category"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.category_response.CategoryResponse()  # noqa: E501
+        # model = Category()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_category_response_data.py` & `ynab-api-2.0.0/test/test_transactions_import_response_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.category_response_data import CategoryResponseData  # noqa: E501
-from ynab_api.rest import ApiException
-
+from ynab_api.model.transactions_import_response_data import TransactionsImportResponseData
 
-class TestCategoryResponseData(unittest.TestCase):
-    """CategoryResponseData unit test stubs"""
 
+class TestTransactionsImportResponseData(unittest.TestCase):
+    """TransactionsImportResponseData unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCategoryResponseData(self):
-        """Test CategoryResponseData"""
+    def testTransactionsImportResponseData(self):
+        """Test TransactionsImportResponseData"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.category_response_data.CategoryResponseData()  # noqa: E501
+        # model = TransactionsImportResponseData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_currency_format.py` & `ynab-api-2.0.0/test/test_budget_summary.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.currency_format import CurrencyFormat  # noqa: E501
-from ynab_api.rest import ApiException
-
+from ynab_api.model.account import Account
+from ynab_api.model.currency_format import CurrencyFormat
+from ynab_api.model.date_format import DateFormat
+
+globals()['Account'] = Account
+globals()['CurrencyFormat'] = CurrencyFormat
+globals()['DateFormat'] = DateFormat
+from ynab_api.model.budget_summary import BudgetSummary
 
-class TestCurrencyFormat(unittest.TestCase):
-    """CurrencyFormat unit test stubs"""
 
+class TestBudgetSummary(unittest.TestCase):
+    """BudgetSummary unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCurrencyFormat(self):
-        """Test CurrencyFormat"""
+    def testBudgetSummary(self):
+        """Test BudgetSummary"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.currency_format.CurrencyFormat()  # noqa: E501
+        # model = BudgetSummary()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_date_format.py` & `ynab-api-2.0.0/test/test_save_account.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.date_format import DateFormat  # noqa: E501
-from ynab_api.rest import ApiException
-
+from ynab_api.model.save_account import SaveAccount
 
-class TestDateFormat(unittest.TestCase):
-    """DateFormat unit test stubs"""
 
+class TestSaveAccount(unittest.TestCase):
+    """SaveAccount unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDateFormat(self):
-        """Test DateFormat"""
+    def testSaveAccount(self):
+        """Test SaveAccount"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.date_format.DateFormat()  # noqa: E501
+        # model = SaveAccount()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_deprecated_api.py` & `ynab-api-2.0.0/test/test_transaction_response_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.api.deprecated_api import DeprecatedApi  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.transaction_detail import TransactionDetail
 
+globals()['TransactionDetail'] = TransactionDetail
+from ynab_api.model.transaction_response_data import TransactionResponseData
 
-class TestDeprecatedApi(unittest.TestCase):
-    """DeprecatedApi unit test stubs"""
 
+class TestTransactionResponseData(unittest.TestCase):
+    """TransactionResponseData unit test stubs"""
     def setUp(self):
-        self.api = ynab_api.api.deprecated_api.DeprecatedApi()  # noqa: E501
+        pass
 
     def tearDown(self):
         pass
 
-    def test_bulk_create_transactions(self):
-        """Test case for bulk_create_transactions
-
-        Bulk create transactions  # noqa: E501
-        """
+    def testTransactionResponseData(self):
+        """Test TransactionResponseData"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = TransactionResponseData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_error_detail.py` & `ynab-api-2.0.0/test/test_payee_location.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.error_detail import ErrorDetail  # noqa: E501
-from ynab_api.rest import ApiException
-
+from ynab_api.model.payee_location import PayeeLocation
 
-class TestErrorDetail(unittest.TestCase):
-    """ErrorDetail unit test stubs"""
 
+class TestPayeeLocation(unittest.TestCase):
+    """PayeeLocation unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testErrorDetail(self):
-        """Test ErrorDetail"""
+    def testPayeeLocation(self):
+        """Test PayeeLocation"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.error_detail.ErrorDetail()  # noqa: E501
+        # model = PayeeLocation()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_hybrid_transaction.py` & `ynab-api-2.0.0/test/test_bulk_transactions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.hybrid_transaction import HybridTransaction  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.save_transaction import SaveTransaction
 
+globals()['SaveTransaction'] = SaveTransaction
+from ynab_api.model.bulk_transactions import BulkTransactions
 
-class TestHybridTransaction(unittest.TestCase):
-    """HybridTransaction unit test stubs"""
 
+class TestBulkTransactions(unittest.TestCase):
+    """BulkTransactions unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testHybridTransaction(self):
-        """Test HybridTransaction"""
+    def testBulkTransactions(self):
+        """Test BulkTransactions"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.hybrid_transaction.HybridTransaction()  # noqa: E501
+        # model = BulkTransactions()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_hybrid_transactions_response.py` & `ynab-api-2.0.0/test/test_hybrid_transactions_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.hybrid_transactions_response import HybridTransactionsResponse  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.hybrid_transactions_response_data import HybridTransactionsResponseData
+
+globals()['HybridTransactionsResponseData'] = HybridTransactionsResponseData
+from ynab_api.model.hybrid_transactions_response import HybridTransactionsResponse
 
 
 class TestHybridTransactionsResponse(unittest.TestCase):
     """HybridTransactionsResponse unit test stubs"""
-
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testHybridTransactionsResponse(self):
         """Test HybridTransactionsResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.hybrid_transactions_response.HybridTransactionsResponse()  # noqa: E501
+        # model = HybridTransactionsResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_hybrid_transactions_response_data.py` & `ynab-api-2.0.0/test/test_transactions_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.hybrid_transactions_response_data import HybridTransactionsResponseData  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.transactions_response_data import TransactionsResponseData
 
+globals()['TransactionsResponseData'] = TransactionsResponseData
+from ynab_api.model.transactions_response import TransactionsResponse
 
-class TestHybridTransactionsResponseData(unittest.TestCase):
-    """HybridTransactionsResponseData unit test stubs"""
 
+class TestTransactionsResponse(unittest.TestCase):
+    """TransactionsResponse unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testHybridTransactionsResponseData(self):
-        """Test HybridTransactionsResponseData"""
+    def testTransactionsResponse(self):
+        """Test TransactionsResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.hybrid_transactions_response_data.HybridTransactionsResponseData()  # noqa: E501
+        # model = TransactionsResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_hybrid_transaction_all_of.py` & `ynab-api-2.0.0/test/test_transaction_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.hybrid_transaction_all_of import HybridTransactionAllOf  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.transaction_response_data import TransactionResponseData
 
+globals()['TransactionResponseData'] = TransactionResponseData
+from ynab_api.model.transaction_response import TransactionResponse
 
-class TestHybridTransactionAllOf(unittest.TestCase):
-    """HybridTransactionAllOf unit test stubs"""
 
+class TestTransactionResponse(unittest.TestCase):
+    """TransactionResponse unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testHybridTransactionAllOf(self):
-        """Test HybridTransactionAllOf"""
+    def testTransactionResponse(self):
+        """Test TransactionResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.hybrid_transaction_all_of.HybridTransactionAllOf()  # noqa: E501
+        # model = TransactionResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_months_api.py` & `ynab-api-2.0.0/test/test_month_summaries_response_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.api.months_api import MonthsApi  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.month_summary import MonthSummary
 
+globals()['MonthSummary'] = MonthSummary
+from ynab_api.model.month_summaries_response_data import MonthSummariesResponseData
 
-class TestMonthsApi(unittest.TestCase):
-    """MonthsApi unit test stubs"""
 
+class TestMonthSummariesResponseData(unittest.TestCase):
+    """MonthSummariesResponseData unit test stubs"""
     def setUp(self):
-        self.api = ynab_api.api.months_api.MonthsApi()  # noqa: E501
-
-    def tearDown(self):
         pass
 
-    def test_get_budget_month(self):
-        """Test case for get_budget_month
-
-        Single budget month  # noqa: E501
-        """
+    def tearDown(self):
         pass
 
-    def test_get_budget_months(self):
-        """Test case for get_budget_months
-
-        List budget months  # noqa: E501
-        """
+    def testMonthSummariesResponseData(self):
+        """Test MonthSummariesResponseData"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = MonthSummariesResponseData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_month_detail_all_of.py` & `ynab-api-2.0.0/test/test_month_detail.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.month_detail_all_of import MonthDetailAllOf  # noqa: E501
-from ynab_api.rest import ApiException
-
+from ynab_api.model.category import Category
+from ynab_api.model.month_detail_all_of import MonthDetailAllOf
+from ynab_api.model.month_summary import MonthSummary
+
+globals()['Category'] = Category
+globals()['MonthDetailAllOf'] = MonthDetailAllOf
+globals()['MonthSummary'] = MonthSummary
+from ynab_api.model.month_detail import MonthDetail
 
-class TestMonthDetailAllOf(unittest.TestCase):
-    """MonthDetailAllOf unit test stubs"""
 
+class TestMonthDetail(unittest.TestCase):
+    """MonthDetail unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMonthDetailAllOf(self):
-        """Test MonthDetailAllOf"""
+    def testMonthDetail(self):
+        """Test MonthDetail"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.month_detail_all_of.MonthDetailAllOf()  # noqa: E501
+        # model = MonthDetail()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_month_detail_response.py` & `ynab-api-2.0.0/test/test_month_detail_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.month_detail_response import MonthDetailResponse  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.month_detail_response_data import MonthDetailResponseData
+
+globals()['MonthDetailResponseData'] = MonthDetailResponseData
+from ynab_api.model.month_detail_response import MonthDetailResponse
 
 
 class TestMonthDetailResponse(unittest.TestCase):
     """MonthDetailResponse unit test stubs"""
-
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testMonthDetailResponse(self):
         """Test MonthDetailResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.month_detail_response.MonthDetailResponse()  # noqa: E501
+        # model = MonthDetailResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_month_detail_response_data.py` & `ynab-api-2.0.0/test/test_transactions_import_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.month_detail_response_data import MonthDetailResponseData  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.transactions_import_response_data import TransactionsImportResponseData
 
+globals()['TransactionsImportResponseData'] = TransactionsImportResponseData
+from ynab_api.model.transactions_import_response import TransactionsImportResponse
 
-class TestMonthDetailResponseData(unittest.TestCase):
-    """MonthDetailResponseData unit test stubs"""
 
+class TestTransactionsImportResponse(unittest.TestCase):
+    """TransactionsImportResponse unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMonthDetailResponseData(self):
-        """Test MonthDetailResponseData"""
+    def testTransactionsImportResponse(self):
+        """Test TransactionsImportResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.month_detail_response_data.MonthDetailResponseData()  # noqa: E501
+        # model = TransactionsImportResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_month_summaries_response.py` & `ynab-api-2.0.0/test/test_month_summaries_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.month_summaries_response import MonthSummariesResponse  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.month_summaries_response_data import MonthSummariesResponseData
+
+globals()['MonthSummariesResponseData'] = MonthSummariesResponseData
+from ynab_api.model.month_summaries_response import MonthSummariesResponse
 
 
 class TestMonthSummariesResponse(unittest.TestCase):
     """MonthSummariesResponse unit test stubs"""
-
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testMonthSummariesResponse(self):
         """Test MonthSummariesResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.month_summaries_response.MonthSummariesResponse()  # noqa: E501
+        # model = MonthSummariesResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_month_summaries_response_data.py` & `ynab-api-2.0.0/test/test_payee_location_response_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.month_summaries_response_data import MonthSummariesResponseData  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.payee_location import PayeeLocation
 
+globals()['PayeeLocation'] = PayeeLocation
+from ynab_api.model.payee_location_response_data import PayeeLocationResponseData
 
-class TestMonthSummariesResponseData(unittest.TestCase):
-    """MonthSummariesResponseData unit test stubs"""
 
+class TestPayeeLocationResponseData(unittest.TestCase):
+    """PayeeLocationResponseData unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMonthSummariesResponseData(self):
-        """Test MonthSummariesResponseData"""
+    def testPayeeLocationResponseData(self):
+        """Test PayeeLocationResponseData"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.month_summaries_response_data.MonthSummariesResponseData()  # noqa: E501
+        # model = PayeeLocationResponseData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_month_summary.py` & `ynab-api-2.0.0/test/test_accounts_response_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.month_summary import MonthSummary  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.account import Account
 
+globals()['Account'] = Account
+from ynab_api.model.accounts_response_data import AccountsResponseData
 
-class TestMonthSummary(unittest.TestCase):
-    """MonthSummary unit test stubs"""
 
+class TestAccountsResponseData(unittest.TestCase):
+    """AccountsResponseData unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMonthSummary(self):
-        """Test MonthSummary"""
+    def testAccountsResponseData(self):
+        """Test AccountsResponseData"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.month_summary.MonthSummary()  # noqa: E501
+        # model = AccountsResponseData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_payee.py` & `ynab-api-2.0.0/test/test_scheduled_sub_transaction.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.payee import Payee  # noqa: E501
-from ynab_api.rest import ApiException
-
+from ynab_api.model.scheduled_sub_transaction import ScheduledSubTransaction
 
-class TestPayee(unittest.TestCase):
-    """Payee unit test stubs"""
 
+class TestScheduledSubTransaction(unittest.TestCase):
+    """ScheduledSubTransaction unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPayee(self):
-        """Test Payee"""
+    def testScheduledSubTransaction(self):
+        """Test ScheduledSubTransaction"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.payee.Payee()  # noqa: E501
+        # model = ScheduledSubTransaction()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_payees_api.py` & `ynab-api-2.0.0/test/test_payees_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,26 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
 import unittest
 
 import ynab_api
 from ynab_api.api.payees_api import PayeesApi  # noqa: E501
-from ynab_api.rest import ApiException
 
 
 class TestPayeesApi(unittest.TestCase):
     """PayeesApi unit test stubs"""
-
     def setUp(self):
-        self.api = ynab_api.api.payees_api.PayeesApi()  # noqa: E501
+        self.api = PayeesApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_get_payee_by_id(self):
         """Test case for get_payee_by_id
```

### Comparing `ynab-api-1.0.0/test/test_payees_response.py` & `ynab-api-2.0.0/test/test_payee_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.payees_response import PayeesResponse  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.payee_response_data import PayeeResponseData
 
+globals()['PayeeResponseData'] = PayeeResponseData
+from ynab_api.model.payee_response import PayeeResponse
 
-class TestPayeesResponse(unittest.TestCase):
-    """PayeesResponse unit test stubs"""
 
+class TestPayeeResponse(unittest.TestCase):
+    """PayeeResponse unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPayeesResponse(self):
-        """Test PayeesResponse"""
+    def testPayeeResponse(self):
+        """Test PayeeResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.payees_response.PayeesResponse()  # noqa: E501
+        # model = PayeeResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_payees_response_data.py` & `ynab-api-2.0.0/test/test_payee_response_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.payees_response_data import PayeesResponseData  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.payee import Payee
 
+globals()['Payee'] = Payee
+from ynab_api.model.payee_response_data import PayeeResponseData
 
-class TestPayeesResponseData(unittest.TestCase):
-    """PayeesResponseData unit test stubs"""
 
+class TestPayeeResponseData(unittest.TestCase):
+    """PayeeResponseData unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPayeesResponseData(self):
-        """Test PayeesResponseData"""
+    def testPayeeResponseData(self):
+        """Test PayeeResponseData"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.payees_response_data.PayeesResponseData()  # noqa: E501
+        # model = PayeeResponseData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_payee_locations_api.py` & `ynab-api-2.0.0/test/test_payee_locations_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,26 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
 import unittest
 
 import ynab_api
 from ynab_api.api.payee_locations_api import PayeeLocationsApi  # noqa: E501
-from ynab_api.rest import ApiException
 
 
 class TestPayeeLocationsApi(unittest.TestCase):
     """PayeeLocationsApi unit test stubs"""
-
     def setUp(self):
-        self.api = ynab_api.api.payee_locations_api.PayeeLocationsApi()  # noqa: E501
+        self.api = PayeeLocationsApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_get_payee_location_by_id(self):
         """Test case for get_payee_location_by_id
```

### Comparing `ynab-api-1.0.0/test/test_payee_locations_response.py` & `ynab-api-2.0.0/test/test_scheduled_transaction_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.payee_locations_response import PayeeLocationsResponse  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.scheduled_transaction_response_data import ScheduledTransactionResponseData
 
+globals(
+)['ScheduledTransactionResponseData'] = ScheduledTransactionResponseData
+from ynab_api.model.scheduled_transaction_response import ScheduledTransactionResponse
 
-class TestPayeeLocationsResponse(unittest.TestCase):
-    """PayeeLocationsResponse unit test stubs"""
 
+class TestScheduledTransactionResponse(unittest.TestCase):
+    """ScheduledTransactionResponse unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPayeeLocationsResponse(self):
-        """Test PayeeLocationsResponse"""
+    def testScheduledTransactionResponse(self):
+        """Test ScheduledTransactionResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.payee_locations_response.PayeeLocationsResponse()  # noqa: E501
+        # model = ScheduledTransactionResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_payee_locations_response_data.py` & `ynab-api-2.0.0/test/test_scheduled_transactions_response_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.payee_locations_response_data import PayeeLocationsResponseData  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.scheduled_transaction_detail import ScheduledTransactionDetail
 
+globals()['ScheduledTransactionDetail'] = ScheduledTransactionDetail
+from ynab_api.model.scheduled_transactions_response_data import ScheduledTransactionsResponseData
 
-class TestPayeeLocationsResponseData(unittest.TestCase):
-    """PayeeLocationsResponseData unit test stubs"""
 
+class TestScheduledTransactionsResponseData(unittest.TestCase):
+    """ScheduledTransactionsResponseData unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPayeeLocationsResponseData(self):
-        """Test PayeeLocationsResponseData"""
+    def testScheduledTransactionsResponseData(self):
+        """Test ScheduledTransactionsResponseData"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.payee_locations_response_data.PayeeLocationsResponseData()  # noqa: E501
+        # model = ScheduledTransactionsResponseData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_payee_location_response.py` & `ynab-api-2.0.0/test/test_payee_location_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.payee_location_response import PayeeLocationResponse  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.payee_location_response_data import PayeeLocationResponseData
+
+globals()['PayeeLocationResponseData'] = PayeeLocationResponseData
+from ynab_api.model.payee_location_response import PayeeLocationResponse
 
 
 class TestPayeeLocationResponse(unittest.TestCase):
     """PayeeLocationResponse unit test stubs"""
-
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testPayeeLocationResponse(self):
         """Test PayeeLocationResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.payee_location_response.PayeeLocationResponse()  # noqa: E501
+        # model = PayeeLocationResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_payee_response.py` & `ynab-api-2.0.0/test/test_payee.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.payee_response import PayeeResponse  # noqa: E501
-from ynab_api.rest import ApiException
-
+from ynab_api.model.payee import Payee
 
-class TestPayeeResponse(unittest.TestCase):
-    """PayeeResponse unit test stubs"""
 
+class TestPayee(unittest.TestCase):
+    """Payee unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPayeeResponse(self):
-        """Test PayeeResponse"""
+    def testPayee(self):
+        """Test Payee"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.payee_response.PayeeResponse()  # noqa: E501
+        # model = Payee()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_payee_response_data.py` & `ynab-api-2.0.0/test/test_account_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.payee_response_data import PayeeResponseData  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.account_response_data import AccountResponseData
 
+globals()['AccountResponseData'] = AccountResponseData
+from ynab_api.model.account_response import AccountResponse
 
-class TestPayeeResponseData(unittest.TestCase):
-    """PayeeResponseData unit test stubs"""
 
+class TestAccountResponse(unittest.TestCase):
+    """AccountResponse unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPayeeResponseData(self):
-        """Test PayeeResponseData"""
+    def testAccountResponse(self):
+        """Test AccountResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.payee_response_data.PayeeResponseData()  # noqa: E501
+        # model = AccountResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_save_transaction.py` & `ynab-api-2.0.0/test/test_save_sub_transaction.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.save_transaction import SaveTransaction  # noqa: E501
-from ynab_api.rest import ApiException
-
+from ynab_api.model.save_sub_transaction import SaveSubTransaction
 
-class TestSaveTransaction(unittest.TestCase):
-    """SaveTransaction unit test stubs"""
 
+class TestSaveSubTransaction(unittest.TestCase):
+    """SaveSubTransaction unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSaveTransaction(self):
-        """Test SaveTransaction"""
+    def testSaveSubTransaction(self):
+        """Test SaveSubTransaction"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.save_transaction.SaveTransaction()  # noqa: E501
+        # model = SaveSubTransaction()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_save_transactions_response.py` & `ynab-api-2.0.0/test/test_save_transactions_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.save_transactions_response import SaveTransactionsResponse  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.save_transactions_response_data import SaveTransactionsResponseData
+
+globals()['SaveTransactionsResponseData'] = SaveTransactionsResponseData
+from ynab_api.model.save_transactions_response import SaveTransactionsResponse
 
 
 class TestSaveTransactionsResponse(unittest.TestCase):
     """SaveTransactionsResponse unit test stubs"""
-
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testSaveTransactionsResponse(self):
         """Test SaveTransactionsResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.save_transactions_response.SaveTransactionsResponse()  # noqa: E501
+        # model = SaveTransactionsResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_save_transactions_response_data.py` & `ynab-api-2.0.0/test/test_save_transactions_response_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.save_transactions_response_data import SaveTransactionsResponseData  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.transaction_detail import TransactionDetail
+
+globals()['TransactionDetail'] = TransactionDetail
+from ynab_api.model.save_transactions_response_data import SaveTransactionsResponseData
 
 
 class TestSaveTransactionsResponseData(unittest.TestCase):
     """SaveTransactionsResponseData unit test stubs"""
-
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testSaveTransactionsResponseData(self):
         """Test SaveTransactionsResponseData"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.save_transactions_response_data.SaveTransactionsResponseData()  # noqa: E501
+        # model = SaveTransactionsResponseData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_save_transaction_wrapper.py` & `ynab-api-2.0.0/test/test_save_transaction.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.save_transaction_wrapper import SaveTransactionWrapper  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.save_sub_transaction import SaveSubTransaction
 
+globals()['SaveSubTransaction'] = SaveSubTransaction
+from ynab_api.model.save_transaction import SaveTransaction
 
-class TestSaveTransactionWrapper(unittest.TestCase):
-    """SaveTransactionWrapper unit test stubs"""
 
+class TestSaveTransaction(unittest.TestCase):
+    """SaveTransaction unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSaveTransactionWrapper(self):
-        """Test SaveTransactionWrapper"""
+    def testSaveTransaction(self):
+        """Test SaveTransaction"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.save_transaction_wrapper.SaveTransactionWrapper()  # noqa: E501
+        # model = SaveTransaction()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_scheduled_sub_transaction.py` & `ynab-api-2.0.0/test/test_scheduled_transaction_response_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.scheduled_sub_transaction import ScheduledSubTransaction  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.scheduled_transaction_detail import ScheduledTransactionDetail
 
+globals()['ScheduledTransactionDetail'] = ScheduledTransactionDetail
+from ynab_api.model.scheduled_transaction_response_data import ScheduledTransactionResponseData
 
-class TestScheduledSubTransaction(unittest.TestCase):
-    """ScheduledSubTransaction unit test stubs"""
 
+class TestScheduledTransactionResponseData(unittest.TestCase):
+    """ScheduledTransactionResponseData unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScheduledSubTransaction(self):
-        """Test ScheduledSubTransaction"""
+    def testScheduledTransactionResponseData(self):
+        """Test ScheduledTransactionResponseData"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.scheduled_sub_transaction.ScheduledSubTransaction()  # noqa: E501
+        # model = ScheduledTransactionResponseData()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_scheduled_transactions_api.py` & `ynab-api-2.0.0/test/test_scheduled_transactions_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,26 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
 import unittest
 
 import ynab_api
 from ynab_api.api.scheduled_transactions_api import ScheduledTransactionsApi  # noqa: E501
-from ynab_api.rest import ApiException
 
 
 class TestScheduledTransactionsApi(unittest.TestCase):
     """ScheduledTransactionsApi unit test stubs"""
-
     def setUp(self):
-        self.api = ynab_api.api.scheduled_transactions_api.ScheduledTransactionsApi()  # noqa: E501
+        self.api = ScheduledTransactionsApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_get_scheduled_transaction_by_id(self):
         """Test case for get_scheduled_transaction_by_id
```

### Comparing `ynab-api-1.0.0/test/test_scheduled_transactions_response.py` & `ynab-api-2.0.0/test/test_scheduled_transactions_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.scheduled_transactions_response import ScheduledTransactionsResponse  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.scheduled_transactions_response_data import ScheduledTransactionsResponseData
+
+globals(
+)['ScheduledTransactionsResponseData'] = ScheduledTransactionsResponseData
+from ynab_api.model.scheduled_transactions_response import ScheduledTransactionsResponse
 
 
 class TestScheduledTransactionsResponse(unittest.TestCase):
     """ScheduledTransactionsResponse unit test stubs"""
-
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testScheduledTransactionsResponse(self):
         """Test ScheduledTransactionsResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.scheduled_transactions_response.ScheduledTransactionsResponse()  # noqa: E501
+        # model = ScheduledTransactionsResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_scheduled_transactions_response_data.py` & `ynab-api-2.0.0/test/test_scheduled_transaction_summary.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.scheduled_transactions_response_data import ScheduledTransactionsResponseData  # noqa: E501
-from ynab_api.rest import ApiException
-
+from ynab_api.model.scheduled_transaction_summary import ScheduledTransactionSummary
 
-class TestScheduledTransactionsResponseData(unittest.TestCase):
-    """ScheduledTransactionsResponseData unit test stubs"""
 
+class TestScheduledTransactionSummary(unittest.TestCase):
+    """ScheduledTransactionSummary unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScheduledTransactionsResponseData(self):
-        """Test ScheduledTransactionsResponseData"""
+    def testScheduledTransactionSummary(self):
+        """Test ScheduledTransactionSummary"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.scheduled_transactions_response_data.ScheduledTransactionsResponseData()  # noqa: E501
+        # model = ScheduledTransactionSummary()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_scheduled_transaction_detail.py` & `ynab-api-2.0.0/test/test_update_transaction.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.scheduled_transaction_detail import ScheduledTransactionDetail  # noqa: E501
-from ynab_api.rest import ApiException
-
+from ynab_api.model.save_sub_transaction import SaveSubTransaction
+from ynab_api.model.save_transaction import SaveTransaction
+from ynab_api.model.update_transaction_all_of import UpdateTransactionAllOf
+
+globals()['SaveSubTransaction'] = SaveSubTransaction
+globals()['SaveTransaction'] = SaveTransaction
+globals()['UpdateTransactionAllOf'] = UpdateTransactionAllOf
+from ynab_api.model.update_transaction import UpdateTransaction
 
-class TestScheduledTransactionDetail(unittest.TestCase):
-    """ScheduledTransactionDetail unit test stubs"""
 
+class TestUpdateTransaction(unittest.TestCase):
+    """UpdateTransaction unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScheduledTransactionDetail(self):
-        """Test ScheduledTransactionDetail"""
+    def testUpdateTransaction(self):
+        """Test UpdateTransaction"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.scheduled_transaction_detail.ScheduledTransactionDetail()  # noqa: E501
+        # model = UpdateTransaction()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_scheduled_transaction_detail_all_of.py` & `ynab-api-2.0.0/test/test_scheduled_transaction_detail_all_of.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.scheduled_transaction_detail_all_of import ScheduledTransactionDetailAllOf  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.scheduled_sub_transaction import ScheduledSubTransaction
+
+globals()['ScheduledSubTransaction'] = ScheduledSubTransaction
+from ynab_api.model.scheduled_transaction_detail_all_of import ScheduledTransactionDetailAllOf
 
 
 class TestScheduledTransactionDetailAllOf(unittest.TestCase):
     """ScheduledTransactionDetailAllOf unit test stubs"""
-
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testScheduledTransactionDetailAllOf(self):
         """Test ScheduledTransactionDetailAllOf"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.scheduled_transaction_detail_all_of.ScheduledTransactionDetailAllOf()  # noqa: E501
+        # model = ScheduledTransactionDetailAllOf()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_sub_transaction.py` & `ynab-api-2.0.0/test/test_error_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.sub_transaction import SubTransaction  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.error_detail import ErrorDetail
 
+globals()['ErrorDetail'] = ErrorDetail
+from ynab_api.model.error_response import ErrorResponse
 
-class TestSubTransaction(unittest.TestCase):
-    """SubTransaction unit test stubs"""
 
+class TestErrorResponse(unittest.TestCase):
+    """ErrorResponse unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSubTransaction(self):
-        """Test SubTransaction"""
+    def testErrorResponse(self):
+        """Test ErrorResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.sub_transaction.SubTransaction()  # noqa: E501
+        # model = ErrorResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_transactions_api.py` & `ynab-api-2.0.0/test/test_transactions_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,26 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
 import unittest
 
 import ynab_api
 from ynab_api.api.transactions_api import TransactionsApi  # noqa: E501
-from ynab_api.rest import ApiException
 
 
 class TestTransactionsApi(unittest.TestCase):
     """TransactionsApi unit test stubs"""
-
     def setUp(self):
-        self.api = ynab_api.api.transactions_api.TransactionsApi()  # noqa: E501
+        self.api = TransactionsApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
     def test_create_transaction(self):
         """Test case for create_transaction
 
@@ -66,14 +59,21 @@
     def test_get_transactions_by_payee(self):
         """Test case for get_transactions_by_payee
 
         List payee transactions  # noqa: E501
         """
         pass
 
+    def test_import_transactions(self):
+        """Test case for import_transactions
+
+        Import transactions  # noqa: E501
+        """
+        pass
+
     def test_update_transaction(self):
         """Test case for update_transaction
 
         Updates an existing transaction  # noqa: E501
         """
         pass
```

### Comparing `ynab-api-1.0.0/test/test_transactions_response.py` & `ynab-api-2.0.0/test/test_update_transactions_wrapper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.transactions_response import TransactionsResponse  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.update_transaction import UpdateTransaction
 
+globals()['UpdateTransaction'] = UpdateTransaction
+from ynab_api.model.update_transactions_wrapper import UpdateTransactionsWrapper
 
-class TestTransactionsResponse(unittest.TestCase):
-    """TransactionsResponse unit test stubs"""
 
+class TestUpdateTransactionsWrapper(unittest.TestCase):
+    """UpdateTransactionsWrapper unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTransactionsResponse(self):
-        """Test TransactionsResponse"""
+    def testUpdateTransactionsWrapper(self):
+        """Test UpdateTransactionsWrapper"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.transactions_response.TransactionsResponse()  # noqa: E501
+        # model = UpdateTransactionsWrapper()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_transactions_response_data.py` & `ynab-api-2.0.0/test/test_save_transactions_wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.transactions_response_data import TransactionsResponseData  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.save_transaction import SaveTransaction
 
+globals()['SaveTransaction'] = SaveTransaction
+from ynab_api.model.save_transactions_wrapper import SaveTransactionsWrapper
 
-class TestTransactionsResponseData(unittest.TestCase):
-    """TransactionsResponseData unit test stubs"""
 
+class TestSaveTransactionsWrapper(unittest.TestCase):
+    """SaveTransactionsWrapper unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTransactionsResponseData(self):
-        """Test TransactionsResponseData"""
+    def testSaveTransactionsWrapper(self):
+        """Test SaveTransactionsWrapper"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.transactions_response_data.TransactionsResponseData()  # noqa: E501
+        # model = SaveTransactionsWrapper()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_transaction_detail_all_of.py` & `ynab-api-2.0.0/test/test_transaction_detail_all_of.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.transaction_detail_all_of import TransactionDetailAllOf  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.sub_transaction import SubTransaction
+
+globals()['SubTransaction'] = SubTransaction
+from ynab_api.model.transaction_detail_all_of import TransactionDetailAllOf
 
 
 class TestTransactionDetailAllOf(unittest.TestCase):
     """TransactionDetailAllOf unit test stubs"""
-
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def testTransactionDetailAllOf(self):
         """Test TransactionDetailAllOf"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.transaction_detail_all_of.TransactionDetailAllOf()  # noqa: E501
+        # model = TransactionDetailAllOf()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_transaction_response.py` & `ynab-api-2.0.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 2.0.0
     Generated by: https://openapi-generator.tech
 """
 
+from setuptools import setup, find_packages  # noqa: H301
 
-from __future__ import absolute_import
-
-import unittest
-
-import ynab_api
-from ynab_api.models.transaction_response import TransactionResponse  # noqa: E501
-from ynab_api.rest import ApiException
-
-
-class TestTransactionResponse(unittest.TestCase):
-    """TransactionResponse unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def testTransactionResponse(self):
-        """Test TransactionResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.transaction_response.TransactionResponse()  # noqa: E501
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+NAME = "ynab-api"
+VERSION = "2.0.0"
+# To install the library, run the following
+#
+# python setup.py install
+#
+# prerequisite: setuptools
+# http://pypi.python.org/pypi/setuptools
+
+REQUIRES = [
+    "urllib3 >= 1.25.3",
+    "python-dateutil",
+]
+
+setup(name=NAME,
+      version=VERSION,
+      description="YNAB API Endpoints",
+      author="David Lerner",
+      author_email="dmlerner@gmail.com",
+      url="",
+      keywords=["OpenAPI", "OpenAPI-Generator", "YNAB API Endpoints"],
+      python_requires=">=3.6",
+      install_requires=REQUIRES,
+      packages=find_packages(exclude=["test", "tests"]),
+      include_package_data=True,
+      long_description="""\
+    Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
+    """)
```

### Comparing `ynab-api-1.0.0/test/test_transaction_response_data.py` & `ynab-api-2.0.0/test/test_payee_locations_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.transaction_response_data import TransactionResponseData  # noqa: E501
-from ynab_api.rest import ApiException
+from ynab_api.model.payee_locations_response_data import PayeeLocationsResponseData
 
+globals()['PayeeLocationsResponseData'] = PayeeLocationsResponseData
+from ynab_api.model.payee_locations_response import PayeeLocationsResponse
 
-class TestTransactionResponseData(unittest.TestCase):
-    """TransactionResponseData unit test stubs"""
 
+class TestPayeeLocationsResponse(unittest.TestCase):
+    """PayeeLocationsResponse unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTransactionResponseData(self):
-        """Test TransactionResponseData"""
+    def testPayeeLocationsResponse(self):
+        """Test PayeeLocationsResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.transaction_response_data.TransactionResponseData()  # noqa: E501
+        # model = PayeeLocationsResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_update_transaction.py` & `ynab-api-2.0.0/test/test_update_transaction_all_of.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.update_transaction import UpdateTransaction  # noqa: E501
-from ynab_api.rest import ApiException
-
+from ynab_api.model.update_transaction_all_of import UpdateTransactionAllOf
 
-class TestUpdateTransaction(unittest.TestCase):
-    """UpdateTransaction unit test stubs"""
 
+class TestUpdateTransactionAllOf(unittest.TestCase):
+    """UpdateTransactionAllOf unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUpdateTransaction(self):
-        """Test UpdateTransaction"""
+    def testUpdateTransactionAllOf(self):
+        """Test UpdateTransactionAllOf"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.update_transaction.UpdateTransaction()  # noqa: E501
+        # model = UpdateTransactionAllOf()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_update_transaction_all_of.py` & `ynab-api-2.0.0/test/test_transaction_summary.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.update_transaction_all_of import UpdateTransactionAllOf  # noqa: E501
-from ynab_api.rest import ApiException
-
+from ynab_api.model.transaction_summary import TransactionSummary
 
-class TestUpdateTransactionAllOf(unittest.TestCase):
-    """UpdateTransactionAllOf unit test stubs"""
 
+class TestTransactionSummary(unittest.TestCase):
+    """TransactionSummary unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUpdateTransactionAllOf(self):
-        """Test UpdateTransactionAllOf"""
+    def testTransactionSummary(self):
+        """Test TransactionSummary"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.update_transaction_all_of.UpdateTransactionAllOf()  # noqa: E501
+        # model = TransactionSummary()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/test/test_user_response_data.py` & `ynab-api-2.0.0/test/test_account.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
+import sys
 import unittest
 
 import ynab_api
-from ynab_api.models.user_response_data import UserResponseData  # noqa: E501
-from ynab_api.rest import ApiException
-
+from ynab_api.model.account import Account
 
-class TestUserResponseData(unittest.TestCase):
-    """UserResponseData unit test stubs"""
 
+class TestAccount(unittest.TestCase):
+    """Account unit test stubs"""
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUserResponseData(self):
-        """Test UserResponseData"""
+    def testAccount(self):
+        """Test Account"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ynab_api.models.user_response_data.UserResponseData()  # noqa: E501
+        # model = Account()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ynab-api-1.0.0/ynab_api/configuration.py` & `ynab-api-2.0.0/ynab_api/configuration.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,162 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
-import six
-from six.moves import http_client as httplib
+from http import client as http_client
+from ynab_api.exceptions import ApiValueError
 
+JSON_SCHEMA_VALIDATION_KEYWORDS = {
+    'multipleOf', 'maximum', 'exclusiveMaximum', 'minimum', 'exclusiveMinimum',
+    'maxLength', 'minLength', 'pattern', 'maxItems', 'minItems'
+}
 
-class TypeWithDefault(type):
-    def __init__(cls, name, bases, dct):
-        super(TypeWithDefault, cls).__init__(name, bases, dct)
-        cls._default = None
-
-    def __call__(cls, **kwargs):
-        if cls._default is None:
-            cls._default = type.__call__(cls, **kwargs)
-        return copy.copy(cls._default)
 
-    def set_default(cls, default):
-        cls._default = copy.copy(default)
-
-
-class Configuration(six.with_metaclass(TypeWithDefault, object)):
+class Configuration(object):
     """NOTE: This class is auto generated by OpenAPI Generator
 
     Ref: https://openapi-generator.tech
     Do not edit the class manually.
 
     :param host: Base url
-    :param api_key: Dict to store API key(s)
+    :param api_key: Dict to store API key(s).
+      Each entry in the dict specifies an API key.
+      The dict key is the name of the security scheme in the OAS specification.
+      The dict value is the API key secret.
     :param api_key_prefix: Dict to store API prefix (e.g. Bearer)
+      The dict key is the name of the security scheme in the OAS specification.
+      The dict value is an API key prefix when generating the auth data.
     :param username: Username for HTTP basic authentication
     :param password: Password for HTTP basic authentication
+    :param discard_unknown_keys: Boolean value indicating whether to discard
+      unknown properties. A server may send a response that includes additional
+      properties that are not known by the client in the following scenarios:
+      1. The OpenAPI document is incomplete, i.e. it does not match the server
+         implementation.
+      2. The client was generated using an older version of the OpenAPI document
+         and the server has been upgraded since then.
+      If a schema in the OpenAPI document defines the additionalProperties attribute,
+      then all undeclared properties received by the server are injected into the
+      additional properties map. In that case, there are undeclared properties, and
+      nothing to discard.
+    :param disabled_client_side_validations (string): Comma-separated list of
+      JSON schema validation keywords to disable JSON schema structural validation
+      rules. The following keywords may be specified: multipleOf, maximum,
+      exclusiveMaximum, minimum, exclusiveMinimum, maxLength, minLength, pattern,
+      maxItems, minItems.
+      By default, the validation is performed for data generated locally by the client
+      and data received from the server, independent of any validation performed by
+      the server side. If the input data does not satisfy the JSON schema validation
+      rules specified in the OpenAPI document, an exception is raised.
+      If disabled_client_side_validations is set, structural validation is
+      disabled. This can be useful to troubleshoot data validation problem, such as
+      when the OpenAPI document validation rules do not match the actual API data
+      received by the server.
+    :param server_index: Index to servers configuration.
+    :param server_variables: Mapping with string values to replace variables in
+      templated server configuration. The validation of enums is performed for
+      variables with defined enum values before.
+    :param server_operation_index: Mapping from operation ID to an index to server
+      configuration.
+    :param server_operation_variables: Mapping from operation ID to a mapping with
+      string values to replace variables in templated server configuration.
+      The validation of enums is performed for variables with defined enum values before.
+    :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
+      in PEM format
+
+    :Example:
+
+    API Key Authentication Example.
+    Given the following security scheme in the OpenAPI specification:
+      components:
+        securitySchemes:
+          cookieAuth:         # name for the security scheme
+            type: apiKey
+            in: cookie
+            name: JSESSIONID  # cookie name
+
+    You can programmatically set the cookie:
+
+conf = ynab_api.Configuration(
+    api_key={'cookieAuth': 'abc123'}
+    api_key_prefix={'cookieAuth': 'JSESSIONID'}
+)
+
+    The following cookie will be added to the HTTP request:
+       Cookie: JSESSIONID abc123
     """
 
-    def __init__(self, host="https://api.youneedabudget.com/v1",
-                 api_key={}, api_key_prefix={},
-                 username="", password=""):
+    _default = None
+
+    def __init__(
+        self,
+        host=None,
+        api_key=None,
+        api_key_prefix=None,
+        access_token=None,
+        username=None,
+        password=None,
+        discard_unknown_keys=False,
+        disabled_client_side_validations="",
+        server_index=None,
+        server_variables=None,
+        server_operation_index=None,
+        server_operation_variables=None,
+        ssl_ca_cert=None,
+    ):
         """Constructor
         """
-        self.host = host
+        self._base_path = "https://api.youneedabudget.com/v1" if host is None else host
         """Default Base url
         """
+        self.server_index = 0 if server_index is None and host is None else server_index
+        self.server_operation_index = server_operation_index or {}
+        """Default server index
+        """
+        self.server_variables = server_variables or {}
+        self.server_operation_variables = server_operation_variables or {}
+        """Default server variables
+        """
         self.temp_folder_path = None
         """Temp file folder for downloading files
         """
         # Authentication Settings
-        self.api_key = api_key
+        self.access_token = access_token
+        self.api_key = {}
+        if api_key:
+            self.api_key = api_key
         """dict to store API key(s)
         """
-        self.api_key_prefix = api_key_prefix
+        self.api_key_prefix = {}
+        if api_key_prefix:
+            self.api_key_prefix = api_key_prefix
         """dict to store API prefix (e.g. Bearer)
         """
         self.refresh_api_key_hook = None
         """function hook to refresh API key if expired
         """
         self.username = username
         """Username for HTTP basic authentication
         """
         self.password = password
         """Password for HTTP basic authentication
         """
+        self.discard_unknown_keys = discard_unknown_keys
+        self.disabled_client_side_validations = disabled_client_side_validations
         self.logger = {}
         """Logging Settings
         """
         self.logger["package_logger"] = logging.getLogger("ynab_api")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
@@ -98,15 +175,15 @@
         """
 
         self.verify_ssl = True
         """SSL/TLS verification
            Set this to false to skip verifying SSL certificate when calling API
            from https server.
         """
-        self.ssl_ca_cert = None
+        self.ssl_ca_cert = ssl_ca_cert
         """Set this to customize the certificate file to verify the peer.
         """
         self.cert_file = None
         """client certificate file
         """
         self.key_file = None
         """client key file
@@ -131,17 +208,68 @@
         """
         self.safe_chars_for_path_param = ''
         """Safe chars for path_param
         """
         self.retries = None
         """Adding retries to override urllib3 default value 3
         """
-        # Disable client side validation
+        # Enable client side validation
         self.client_side_validation = True
 
+        # Options to pass down to the underlying urllib3 socket
+        self.socket_options = None
+
+    def __deepcopy__(self, memo):
+        cls = self.__class__
+        result = cls.__new__(cls)
+        memo[id(self)] = result
+        for k, v in self.__dict__.items():
+            if k not in ('logger', 'logger_file_handler'):
+                setattr(result, k, copy.deepcopy(v, memo))
+        # shallow copy of loggers
+        result.logger = copy.copy(self.logger)
+        # use setters to configure loggers
+        result.logger_file = self.logger_file
+        result.debug = self.debug
+        return result
+
+    def __setattr__(self, name, value):
+        object.__setattr__(self, name, value)
+        if name == 'disabled_client_side_validations':
+            s = set(filter(None, value.split(',')))
+            for v in s:
+                if v not in JSON_SCHEMA_VALIDATION_KEYWORDS:
+                    raise ApiValueError("Invalid keyword: '{0}''".format(v))
+            self._disabled_client_side_validations = s
+
+    @classmethod
+    def set_default(cls, default):
+        """Set default instance of configuration.
+
+        It stores default configuration, which can be
+        returned by get_default_copy method.
+
+        :param default: object of Configuration
+        """
+        cls._default = copy.deepcopy(default)
+
+    @classmethod
+    def get_default_copy(cls):
+        """Return new instance of configuration.
+
+        This method returns newly created, based on default constructor,
+        object of Configuration class or returns a copy of default
+        configuration passed by the set_default method.
+
+        :return: The configuration object.
+        """
+        if cls._default is not None:
+            return copy.deepcopy(cls._default)
+        return Configuration()
+
     @property
     def logger_file(self):
         """The logger file.
 
         If the logger_file is None, then add stream handler and remove file
         handler. Otherwise, add file handler and remove stream handler.
 
@@ -162,15 +290,15 @@
         """
         self.__logger_file = value
         if self.__logger_file:
             # If set logging file,
             # then add file handler and remove stream handler.
             self.logger_file_handler = logging.FileHandler(self.__logger_file)
             self.logger_file_handler.setFormatter(self.logger_formatter)
-            for _, logger in six.iteritems(self.logger):
+            for _, logger in self.logger.items():
                 logger.addHandler(self.logger_file_handler)
 
     @property
     def debug(self):
         """Debug status
 
         :param value: The debug status, True or False.
@@ -184,25 +312,25 @@
 
         :param value: The debug status, True or False.
         :type: bool
         """
         self.__debug = value
         if self.__debug:
             # if debug status is True, turn on debug logging
-            for _, logger in six.iteritems(self.logger):
+            for _, logger in self.logger.items():
                 logger.setLevel(logging.DEBUG)
-            # turn on httplib debug
-            httplib.HTTPConnection.debuglevel = 1
+            # turn on http_client debug
+            http_client.HTTPConnection.debuglevel = 1
         else:
             # if debug status is False, turn off debug logging,
             # setting log level to default `logging.WARNING`
-            for _, logger in six.iteritems(self.logger):
+            for _, logger in self.logger.items():
                 logger.setLevel(logging.WARNING)
-            # turn off httplib debug
-            httplib.HTTPConnection.debuglevel = 0
+            # turn off http_client debug
+            http_client.HTTPConnection.debuglevel = 0
 
     @property
     def logger_format(self):
         """The logger format.
 
         The logger_formatter will be updated when sets logger_format.
 
@@ -219,53 +347,61 @@
 
         :param value: The format string.
         :type: str
         """
         self.__logger_format = value
         self.logger_formatter = logging.Formatter(self.__logger_format)
 
-    def get_api_key_with_prefix(self, identifier):
+    def get_api_key_with_prefix(self, identifier, alias=None):
         """Gets API key (with prefix if set).
 
         :param identifier: The identifier of apiKey.
+        :param alias: The alternative identifier of apiKey.
         :return: The token for api key authentication.
         """
         if self.refresh_api_key_hook is not None:
             self.refresh_api_key_hook(self)
-        key = self.api_key.get(identifier)
+        key = self.api_key.get(
+            identifier,
+            self.api_key.get(alias) if alias is not None else None)
         if key:
             prefix = self.api_key_prefix.get(identifier)
             if prefix:
                 return "%s %s" % (prefix, key)
             else:
                 return key
 
     def get_basic_auth_token(self):
         """Gets HTTP basic authentication header (string).
 
         :return: The token for basic HTTP authentication.
         """
-        return urllib3.util.make_headers(
-            basic_auth=self.username + ':' + self.password
-        ).get('authorization')
+        username = ""
+        if self.username is not None:
+            username = self.username
+        password = ""
+        if self.password is not None:
+            password = self.password
+        return urllib3.util.make_headers(basic_auth=username + ':' +
+                                         password).get('authorization')
 
     def auth_settings(self):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
-        return {
-            'bearer':
-                {
-                    'type': 'api_key',
-                    'in': 'header',
-                    'key': 'Authorization',
-                    'value': self.get_api_key_with_prefix('Authorization')
-                },
-        }
+        auth = {}
+        if 'bearer' in self.api_key:
+            auth['bearer'] = {
+                'type': 'api_key',
+                'in': 'header',
+                'key': 'Authorization',
+                'value': self.get_api_key_with_prefix('bearer', ),
+            }
+        return auth
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
@@ -276,52 +412,62 @@
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
-        return [
-            {
-                'url': "https://api.youneedabudget.com/v1",
-                'description': "No description provided",
-            }
-        ]
+        return [{
+            'url': "https://api.youneedabudget.com/v1",
+            'description': "No description provided",
+        }]
 
-    def get_host_from_settings(self, index, variables={}):
+    def get_host_from_settings(self, index, variables=None, servers=None):
         """Gets host URL based on the index and variables
         :param index: array index of the host settings
         :param variables: hash of variable and the corresponding value
+        :param servers: an array of host settings or None
         :return: URL based on host settings
         """
+        if index is None:
+            return self._base_path
 
-        servers = self.get_host_settings()
+        variables = {} if variables is None else variables
+        servers = self.get_host_settings() if servers is None else servers
 
-        # check array index out of bound
-        if index < 0 or index >= len(servers):
+        try:
+            server = servers[index]
+        except IndexError:
             raise ValueError(
-                "Invalid index {} when selecting the host settings. Must be less than {}"  # noqa: E501
-                .format(index, len(servers)))
+                "Invalid index {0} when selecting the host settings. "
+                "Must be less than {1}".format(index, len(servers)))
 
-        server = servers[index]
         url = server['url']
 
-        # go through variable and assign a value
-        for variable_name in server['variables']:
-            if variable_name in variables:
-                if variables[variable_name] in server['variables'][
-                        variable_name]['enum_values']:
-                    url = url.replace("{" + variable_name + "}",
-                                      variables[variable_name])
-                else:
-                    raise ValueError(
-                        "The variable `{}` in the host URL has invalid value {}. Must be {}."  # noqa: E501
-                        .format(
-                            variable_name, variables[variable_name],
-                            server['variables'][variable_name]['enum_values']))
-            else:
-                # use default value
-                url = url.replace(
-                    "{" + variable_name + "}",
-                    server['variables'][variable_name]['default_value'])
+        # go through variables and replace placeholders
+        for variable_name, variable in server.get('variables', {}).items():
+            used_value = variables.get(variable_name,
+                                       variable['default_value'])
+
+            if 'enum_values' in variable \
+                    and used_value not in variable['enum_values']:
+                raise ValueError(
+                    "The variable `{0}` in the host URL has invalid value "
+                    "{1}. Must be {2}.".format(variable_name,
+                                               variables[variable_name],
+                                               variable['enum_values']))
+
+            url = url.replace("{" + variable_name + "}", used_value)
 
         return url
+
+    @property
+    def host(self):
+        """Return generated host."""
+        return self.get_host_from_settings(self.server_index,
+                                           variables=self.server_variables)
+
+    @host.setter
+    def host(self, value):
+        """Fix base path."""
+        self._base_path = value
+        self.server_index = None
```

### Comparing `ynab-api-1.0.0/ynab_api/exceptions.py` & `ynab-api-2.0.0/ynab_api/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
-import six
-
-
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
 
 
 class ApiTypeError(OpenApiException, TypeError):
-    def __init__(self, msg, path_to_item=None, valid_classes=None,
+    def __init__(self,
+                 msg,
+                 path_to_item=None,
+                 valid_classes=None,
                  key_type=None):
         """ Raises an exception for TypeErrors
 
         Args:
             msg (str): the exception message
 
         Keyword Args:
@@ -60,14 +58,33 @@
         self.path_to_item = path_to_item
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiValueError, self).__init__(full_msg)
 
 
+class ApiAttributeError(OpenApiException, AttributeError):
+    def __init__(self, msg, path_to_item=None):
+        """
+        Raised when an attribute reference or assignment fails.
+
+        Args:
+            msg (str): the exception message
+
+        Keyword Args:
+            path_to_item (None/list) the path to the exception in the
+                received_data dict
+        """
+        self.path_to_item = path_to_item
+        full_msg = msg
+        if path_to_item:
+            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
+        super(ApiAttributeError, self).__init__(full_msg)
+
+
 class ApiKeyError(OpenApiException, KeyError):
     def __init__(self, msg, path_to_item=None):
         """
         Args:
             msg (str): the exception message
 
         Keyword Args:
@@ -78,15 +95,14 @@
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiKeyError, self).__init__(full_msg)
 
 
 class ApiException(OpenApiException):
-
     def __init__(self, status=None, reason=None, http_resp=None):
         if http_resp:
             self.status = http_resp.status
             self.reason = http_resp.reason
             self.body = http_resp.data
             self.headers = http_resp.getheaders()
         else:
@@ -105,16 +121,36 @@
 
         if self.body:
             error_message += "HTTP response body: {0}\n".format(self.body)
 
         return error_message
 
 
+class NotFoundException(ApiException):
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(NotFoundException, self).__init__(status, reason, http_resp)
+
+
+class UnauthorizedException(ApiException):
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(UnauthorizedException, self).__init__(status, reason, http_resp)
+
+
+class ForbiddenException(ApiException):
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(ForbiddenException, self).__init__(status, reason, http_resp)
+
+
+class ServiceException(ApiException):
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(ServiceException, self).__init__(status, reason, http_resp)
+
+
 def render_path(path_to_item):
     """Returns a string representation of a path"""
     result = ""
     for pth in path_to_item:
-        if isinstance(pth, six.integer_types):
+        if isinstance(pth, int):
             result += "[{0}]".format(pth)
         else:
             result += "['{0}']".format(pth)
     return result
```

### Comparing `ynab-api-1.0.0/ynab_api/models/save_transaction.py` & `ynab-api-2.0.0/ynab_api/model/budget_detail.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,422 +1,401 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import pprint
 import re  # noqa: F401
+import sys  # noqa: F401
 
-import six
+from ynab_api.model_utils import (  # noqa: F401
+    ApiTypeError, ModelComposed, ModelNormal, ModelSimple, cached_property,
+    change_keys_js_to_python, convert_js_args_to_python_args, date, datetime,
+    file_type, none_type, validate_get_composed_info,
+)
+from ..model_utils import OpenApiModel
+from ynab_api.exceptions import ApiAttributeError
+
+
+def lazy_import():
+    from ynab_api.model.account import Account
+    from ynab_api.model.budget_detail_all_of import BudgetDetailAllOf
+    from ynab_api.model.budget_summary import BudgetSummary
+    from ynab_api.model.category import Category
+    from ynab_api.model.category_group import CategoryGroup
+    from ynab_api.model.currency_format import CurrencyFormat
+    from ynab_api.model.date_format import DateFormat
+    from ynab_api.model.month_detail import MonthDetail
+    from ynab_api.model.payee import Payee
+    from ynab_api.model.payee_location import PayeeLocation
+    from ynab_api.model.scheduled_sub_transaction import ScheduledSubTransaction
+    from ynab_api.model.scheduled_transaction_summary import ScheduledTransactionSummary
+    from ynab_api.model.sub_transaction import SubTransaction
+    from ynab_api.model.transaction_summary import TransactionSummary
+    globals()['Account'] = Account
+    globals()['BudgetDetailAllOf'] = BudgetDetailAllOf
+    globals()['BudgetSummary'] = BudgetSummary
+    globals()['Category'] = Category
+    globals()['CategoryGroup'] = CategoryGroup
+    globals()['CurrencyFormat'] = CurrencyFormat
+    globals()['DateFormat'] = DateFormat
+    globals()['MonthDetail'] = MonthDetail
+    globals()['Payee'] = Payee
+    globals()['PayeeLocation'] = PayeeLocation
+    globals()['ScheduledSubTransaction'] = ScheduledSubTransaction
+    globals()['ScheduledTransactionSummary'] = ScheduledTransactionSummary
+    globals()['SubTransaction'] = SubTransaction
+    globals()['TransactionSummary'] = TransactionSummary
 
-from ynab_api.configuration import Configuration
 
-
-class SaveTransaction(object):
+class BudgetDetail(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
-    """
 
-    """
     Attributes:
-      openapi_types (dict): The key is attribute name
-                            and the value is attribute type.
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
-                            and the value is json key in definition.
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
     """
-    openapi_types = {
-        'account_id': 'str',
-        'date': 'date',
-        'amount': 'int',
-        'payee_id': 'str',
-        'payee_name': 'str',
-        'category_id': 'str',
-        'memo': 'str',
-        'cleared': 'str',
-        'approved': 'bool',
-        'flag_color': 'str',
-        'import_id': 'str'
-    }
-
-    attribute_map = {
-        'account_id': 'account_id',
-        'date': 'date',
-        'amount': 'amount',
-        'payee_id': 'payee_id',
-        'payee_name': 'payee_name',
-        'category_id': 'category_id',
-        'memo': 'memo',
-        'cleared': 'cleared',
-        'approved': 'approved',
-        'flag_color': 'flag_color',
-        'import_id': 'import_id'
-    }
-
-    def __init__(self, account_id=None, date=None, amount=None, payee_id=None, payee_name=None, category_id=None, memo=None, cleared=None, approved=None, flag_color=None, import_id=None, local_vars_configuration=None):  # noqa: E501
-        """SaveTransaction - a model defined in OpenAPI"""  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration()
-        self.local_vars_configuration = local_vars_configuration
-
-        self._account_id = None
-        self._date = None
-        self._amount = None
-        self._payee_id = None
-        self._payee_name = None
-        self._category_id = None
-        self._memo = None
-        self._cleared = None
-        self._approved = None
-        self._flag_color = None
-        self._import_id = None
-        self.discriminator = None
-
-        self.account_id = account_id
-        self.date = date
-        self.amount = amount
-        if payee_id is not None:
-            self.payee_id = payee_id
-        if payee_name is not None:
-            self.payee_name = payee_name
-        if category_id is not None:
-            self.category_id = category_id
-        if memo is not None:
-            self.memo = memo
-        if cleared is not None:
-            self.cleared = cleared
-        if approved is not None:
-            self.approved = approved
-        if flag_color is not None:
-            self.flag_color = flag_color
-        if import_id is not None:
-            self.import_id = import_id
-
-    @property
-    def account_id(self):
-        """Gets the account_id of this SaveTransaction.  # noqa: E501
-
-
-        :return: The account_id of this SaveTransaction.  # noqa: E501
-        :rtype: str
-        """
-        return self._account_id
 
-    @account_id.setter
-    def account_id(self, account_id):
-        """Sets the account_id of this SaveTransaction.
+    allowed_values = {}
 
+    validations = {}
 
-        :param account_id: The account_id of this SaveTransaction.  # noqa: E501
-        :type: str
+    @cached_property
+    def additional_properties_type():
         """
-        if self.local_vars_configuration.client_side_validation and account_id is None:  # noqa: E501
-            raise ValueError("Invalid value for `account_id`, must not be `None`")  # noqa: E501
-
-        self._account_id = account_id
-
-    @property
-    def date(self):
-        """Gets the date of this SaveTransaction.  # noqa: E501
-
-        The transaction date in ISO format (e.g. 2016-12-01).  Future dates (scheduled transactions) are not permitted.  Split transaction dates cannot be changed and if a different date is supplied it will be ignored.  # noqa: E501
-
-        :return: The date of this SaveTransaction.  # noqa: E501
-        :rtype: date
-        """
-        return self._date
-
-    @date.setter
-    def date(self, date):
-        """Sets the date of this SaveTransaction.
-
-        The transaction date in ISO format (e.g. 2016-12-01).  Future dates (scheduled transactions) are not permitted.  Split transaction dates cannot be changed and if a different date is supplied it will be ignored.  # noqa: E501
-
-        :param date: The date of this SaveTransaction.  # noqa: E501
-        :type: date
-        """
-        if self.local_vars_configuration.client_side_validation and date is None:  # noqa: E501
-            raise ValueError("Invalid value for `date`, must not be `None`")  # noqa: E501
-
-        self._date = date
-
-    @property
-    def amount(self):
-        """Gets the amount of this SaveTransaction.  # noqa: E501
-
-        The transaction amount in milliunits format.  Split transaction amounts cannot be changed and if a different amount is supplied it will be ignored.  # noqa: E501
-
-        :return: The amount of this SaveTransaction.  # noqa: E501
-        :rtype: int
-        """
-        return self._amount
-
-    @amount.setter
-    def amount(self, amount):
-        """Sets the amount of this SaveTransaction.
-
-        The transaction amount in milliunits format.  Split transaction amounts cannot be changed and if a different amount is supplied it will be ignored.  # noqa: E501
-
-        :param amount: The amount of this SaveTransaction.  # noqa: E501
-        :type: int
-        """
-        if self.local_vars_configuration.client_side_validation and amount is None:  # noqa: E501
-            raise ValueError("Invalid value for `amount`, must not be `None`")  # noqa: E501
-
-        self._amount = amount
-
-    @property
-    def payee_id(self):
-        """Gets the payee_id of this SaveTransaction.  # noqa: E501
-
-        The payee for the transaction.  To create a transfer between two accounts, use the account transfer payee pointing to the target account.  Account transfer payees are specified as tranfer_payee_id on the account resource.  # noqa: E501
-
-        :return: The payee_id of this SaveTransaction.  # noqa: E501
-        :rtype: str
-        """
-        return self._payee_id
-
-    @payee_id.setter
-    def payee_id(self, payee_id):
-        """Sets the payee_id of this SaveTransaction.
-
-        The payee for the transaction.  To create a transfer between two accounts, use the account transfer payee pointing to the target account.  Account transfer payees are specified as tranfer_payee_id on the account resource.  # noqa: E501
-
-        :param payee_id: The payee_id of this SaveTransaction.  # noqa: E501
-        :type: str
-        """
-
-        self._payee_id = payee_id
-
-    @property
-    def payee_name(self):
-        """Gets the payee_name of this SaveTransaction.  # noqa: E501
-
-        The payee name.  If a payee_name value is provided and payee_id has a null value, the payee_name value will be used to resolve the payee by either (1) a matching payee rename rule (only if import_id is also specified) or (2) a payee with the same name or (3) creation of a new payee.  # noqa: E501
-
-        :return: The payee_name of this SaveTransaction.  # noqa: E501
-        :rtype: str
-        """
-        return self._payee_name
-
-    @payee_name.setter
-    def payee_name(self, payee_name):
-        """Sets the payee_name of this SaveTransaction.
-
-        The payee name.  If a payee_name value is provided and payee_id has a null value, the payee_name value will be used to resolve the payee by either (1) a matching payee rename rule (only if import_id is also specified) or (2) a payee with the same name or (3) creation of a new payee.  # noqa: E501
-
-        :param payee_name: The payee_name of this SaveTransaction.  # noqa: E501
-        :type: str
-        """
-        if (self.local_vars_configuration.client_side_validation and
-                payee_name is not None and len(payee_name) > 50):
-            raise ValueError("Invalid value for `payee_name`, length must be less than or equal to `50`")  # noqa: E501
-
-        self._payee_name = payee_name
-
-    @property
-    def category_id(self):
-        """Gets the category_id of this SaveTransaction.  # noqa: E501
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        lazy_import()
+        return (
+            bool,
+            date,
+            datetime,
+            dict,
+            float,
+            int,
+            list,
+            str,
+            none_type,
+        )  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        lazy_import()
+        return {
+            'id': (str, ),  # noqa: E501
+            'name': (str, ),  # noqa: E501
+            'last_modified_on': (datetime, ),  # noqa: E501
+            'first_month': (date, ),  # noqa: E501
+            'last_month': (date, ),  # noqa: E501
+            'date_format': (DateFormat, ),  # noqa: E501
+            'currency_format': (CurrencyFormat, ),  # noqa: E501
+            'accounts': ([Account], ),  # noqa: E501
+            'payees': ([Payee], ),  # noqa: E501
+            'payee_locations': ([PayeeLocation], ),  # noqa: E501
+            'category_groups': ([CategoryGroup], ),  # noqa: E501
+            'categories': ([Category], ),  # noqa: E501
+            'months': ([MonthDetail], ),  # noqa: E501
+            'transactions': ([TransactionSummary], ),  # noqa: E501
+            'subtransactions': ([SubTransaction], ),  # noqa: E501
+            'scheduled_transactions':
+            ([ScheduledTransactionSummary], ),  # noqa: E501
+            'scheduled_subtransactions':
+            ([ScheduledSubTransaction], ),  # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
 
-        The category for the transaction.  Split and Credit Card Payment categories are not permitted and will be ignored if supplied.  If an existing transaction has a Split category it cannot be changed.  # noqa: E501
-
-        :return: The category_id of this SaveTransaction.  # noqa: E501
-        :rtype: str
-        """
-        return self._category_id
-
-    @category_id.setter
-    def category_id(self, category_id):
-        """Sets the category_id of this SaveTransaction.
-
-        The category for the transaction.  Split and Credit Card Payment categories are not permitted and will be ignored if supplied.  If an existing transaction has a Split category it cannot be changed.  # noqa: E501
-
-        :param category_id: The category_id of this SaveTransaction.  # noqa: E501
-        :type: str
-        """
-
-        self._category_id = category_id
-
-    @property
-    def memo(self):
-        """Gets the memo of this SaveTransaction.  # noqa: E501
-
-
-        :return: The memo of this SaveTransaction.  # noqa: E501
-        :rtype: str
-        """
-        return self._memo
-
-    @memo.setter
-    def memo(self, memo):
-        """Sets the memo of this SaveTransaction.
-
-
-        :param memo: The memo of this SaveTransaction.  # noqa: E501
-        :type: str
-        """
-        if (self.local_vars_configuration.client_side_validation and
-                memo is not None and len(memo) > 200):
-            raise ValueError("Invalid value for `memo`, length must be less than or equal to `200`")  # noqa: E501
-
-        self._memo = memo
-
-    @property
-    def cleared(self):
-        """Gets the cleared of this SaveTransaction.  # noqa: E501
-
-        The cleared status of the transaction  # noqa: E501
-
-        :return: The cleared of this SaveTransaction.  # noqa: E501
-        :rtype: str
-        """
-        return self._cleared
-
-    @cleared.setter
-    def cleared(self, cleared):
-        """Sets the cleared of this SaveTransaction.
+    attribute_map = {
+        'id': 'id',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'last_modified_on': 'last_modified_on',  # noqa: E501
+        'first_month': 'first_month',  # noqa: E501
+        'last_month': 'last_month',  # noqa: E501
+        'date_format': 'date_format',  # noqa: E501
+        'currency_format': 'currency_format',  # noqa: E501
+        'accounts': 'accounts',  # noqa: E501
+        'payees': 'payees',  # noqa: E501
+        'payee_locations': 'payee_locations',  # noqa: E501
+        'category_groups': 'category_groups',  # noqa: E501
+        'categories': 'categories',  # noqa: E501
+        'months': 'months',  # noqa: E501
+        'transactions': 'transactions',  # noqa: E501
+        'subtransactions': 'subtransactions',  # noqa: E501
+        'scheduled_transactions': 'scheduled_transactions',  # noqa: E501
+        'scheduled_subtransactions': 'scheduled_subtransactions',  # noqa: E501
+    }
 
-        The cleared status of the transaction  # noqa: E501
+    read_only_vars = {}
 
-        :param cleared: The cleared of this SaveTransaction.  # noqa: E501
-        :type: str
-        """
-        allowed_values = ["cleared", "uncleared", "reconciled"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and cleared not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `cleared` ({0}), must be one of {1}"  # noqa: E501
-                .format(cleared, allowed_values)
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """BudgetDetail - a model defined in OpenAPI
+
+        Keyword Args:
+            id (str):
+            name (str):
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            last_modified_on (datetime): The last time any changes were made to the budget from either a web or mobile client. [optional]  # noqa: E501
+            first_month (date): The earliest budget month. [optional]  # noqa: E501
+            last_month (date): The latest budget month. [optional]  # noqa: E501
+            date_format (DateFormat): [optional]  # noqa: E501
+            currency_format (CurrencyFormat): [optional]  # noqa: E501
+            accounts ([Account]): [optional]  # noqa: E501
+            payees ([Payee]): [optional]  # noqa: E501
+            payee_locations ([PayeeLocation]): [optional]  # noqa: E501
+            category_groups ([CategoryGroup]): [optional]  # noqa: E501
+            categories ([Category]): [optional]  # noqa: E501
+            months ([MonthDetail]): [optional]  # noqa: E501
+            transactions ([TransactionSummary]): [optional]  # noqa: E501
+            subtransactions ([SubTransaction]): [optional]  # noqa: E501
+            scheduled_transactions ([ScheduledTransactionSummary]): [optional]  # noqa: E501
+            scheduled_subtransactions ([ScheduledSubTransaction]): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            raise ApiTypeError(
+                "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments."
+                % (
+                    args,
+                    self.__class__.__name__,
+                ),
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__, ),
             )
 
-        self._cleared = cleared
-
-    @property
-    def approved(self):
-        """Gets the approved of this SaveTransaction.  # noqa: E501
-
-        Whether or not the transaction is approved.  If not supplied, transaction will be unapproved by default.  # noqa: E501
-
-        :return: The approved of this SaveTransaction.  # noqa: E501
-        :rtype: bool
-        """
-        return self._approved
-
-    @approved.setter
-    def approved(self, approved):
-        """Sets the approved of this SaveTransaction.
-
-        Whether or not the transaction is approved.  If not supplied, transaction will be unapproved by default.  # noqa: E501
-
-        :param approved: The approved of this SaveTransaction.  # noqa: E501
-        :type: bool
-        """
-
-        self._approved = approved
-
-    @property
-    def flag_color(self):
-        """Gets the flag_color of this SaveTransaction.  # noqa: E501
-
-        The transaction flag  # noqa: E501
-
-        :return: The flag_color of this SaveTransaction.  # noqa: E501
-        :rtype: str
-        """
-        return self._flag_color
-
-    @flag_color.setter
-    def flag_color(self, flag_color):
-        """Sets the flag_color of this SaveTransaction.
-
-        The transaction flag  # noqa: E501
-
-        :param flag_color: The flag_color of this SaveTransaction.  # noqa: E501
-        :type: str
-        """
-        allowed_values = ["red", "orange", "yellow", "green", "blue", "purple"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and flag_color not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `flag_color` ({0}), must be one of {1}"  # noqa: E501
-                .format(flag_color, allowed_values)
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (
+            self.__class__, )
+
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
+        for var_name, var_value in kwargs.items():
+            if var_name in discarded_args and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self._additional_properties_model_instances:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+        '_composed_instances',
+        '_var_name_to_model_instances',
+        '_additional_properties_model_instances',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """BudgetDetail - a model defined in OpenAPI
+
+        Keyword Args:
+            id (str):
+            name (str):
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            last_modified_on (datetime): The last time any changes were made to the budget from either a web or mobile client. [optional]  # noqa: E501
+            first_month (date): The earliest budget month. [optional]  # noqa: E501
+            last_month (date): The latest budget month. [optional]  # noqa: E501
+            date_format (DateFormat): [optional]  # noqa: E501
+            currency_format (CurrencyFormat): [optional]  # noqa: E501
+            accounts ([Account]): [optional]  # noqa: E501
+            payees ([Payee]): [optional]  # noqa: E501
+            payee_locations ([PayeeLocation]): [optional]  # noqa: E501
+            category_groups ([CategoryGroup]): [optional]  # noqa: E501
+            categories ([Category]): [optional]  # noqa: E501
+            months ([MonthDetail]): [optional]  # noqa: E501
+            transactions ([TransactionSummary]): [optional]  # noqa: E501
+            subtransactions ([SubTransaction]): [optional]  # noqa: E501
+            scheduled_transactions ([ScheduledTransactionSummary]): [optional]  # noqa: E501
+            scheduled_subtransactions ([ScheduledSubTransaction]): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            raise ApiTypeError(
+                "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments."
+                % (
+                    args,
+                    self.__class__.__name__,
+                ),
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__, ),
             )
 
-        self._flag_color = flag_color
-
-    @property
-    def import_id(self):
-        """Gets the import_id of this SaveTransaction.  # noqa: E501
-
-        If specified, the new transaction will be assigned this import_id and considered \"imported\".  We will also attempt to match this imported transaction to an existing \"user-entered\" transation on the same account, with the same amount, and with a date +/-10 days from the imported transaction date.<br><br>Transactions imported through File Based Import or Direct Import (not through the API) are assigned an import_id in the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'. For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.  Using a consistent format will prevent duplicates through Direct Import and File Based Import.<br><br>If import_id is omitted or specified as null, the transaction will be treated as a \"user-entered\" transaction. As such, it will be eligible to be matched against transactions later being imported (via DI, FBI, or API).  # noqa: E501
-
-        :return: The import_id of this SaveTransaction.  # noqa: E501
-        :rtype: str
-        """
-        return self._import_id
-
-    @import_id.setter
-    def import_id(self, import_id):
-        """Sets the import_id of this SaveTransaction.
-
-        If specified, the new transaction will be assigned this import_id and considered \"imported\".  We will also attempt to match this imported transaction to an existing \"user-entered\" transation on the same account, with the same amount, and with a date +/-10 days from the imported transaction date.<br><br>Transactions imported through File Based Import or Direct Import (not through the API) are assigned an import_id in the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'. For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.  Using a consistent format will prevent duplicates through Direct Import and File Based Import.<br><br>If import_id is omitted or specified as null, the transaction will be treated as a \"user-entered\" transaction. As such, it will be eligible to be matched against transactions later being imported (via DI, FBI, or API).  # noqa: E501
-
-        :param import_id: The import_id of this SaveTransaction.  # noqa: E501
-        :type: str
-        """
-        if (self.local_vars_configuration.client_side_validation and
-                import_id is not None and len(import_id) > 36):
-            raise ValueError("Invalid value for `import_id`, length must be less than or equal to `36`")  # noqa: E501
-
-        self._import_id = import_id
-
-    def to_dict(self):
-        """Returns the model properties as a dict"""
-        result = {}
-
-        for attr, _ in six.iteritems(self.openapi_types):
-            value = getattr(self, attr)
-            if isinstance(value, list):
-                result[attr] = list(map(
-                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
-                    value
-                ))
-            elif hasattr(value, "to_dict"):
-                result[attr] = value.to_dict()
-            elif isinstance(value, dict):
-                result[attr] = dict(map(
-                    lambda item: (item[0], item[1].to_dict())
-                    if hasattr(item[1], "to_dict") else item,
-                    value.items()
-                ))
-            else:
-                result[attr] = value
-
-        return result
-
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return pprint.pformat(self.to_dict())
-
-    def __repr__(self):
-        """For `print` and `pprint`"""
-        return self.to_str()
-
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, SaveTransaction):
-            return False
-
-        return self.to_dict() == other.to_dict()
-
-    def __ne__(self, other):
-        """Returns true if both objects are not equal"""
-        if not isinstance(other, SaveTransaction):
-            return True
-
-        return self.to_dict() != other.to_dict()
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (
+            self.__class__, )
+
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
+        for var_name, var_value in kwargs.items():
+            if var_name in discarded_args and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self._additional_properties_model_instances:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(
+                    f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                    f"class with read only attributes.")
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
+                BudgetDetailAllOf,
+                BudgetSummary,
+            ],
+            'oneOf': [],
+        }
```

### Comparing `ynab-api-1.0.0/ynab_api/rest.py` & `ynab-api-2.0.0/ynab_api/rest.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,31 @@
-# coding: utf-8
-
 """
     YNAB API Endpoints
 
     Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
 import io
 import json
 import logging
 import re
 import ssl
+from urllib.parse import urlencode
 
-import certifi
-# python 2 and python 3 compatibility library
-import six
-from six.moves.urllib.parse import urlencode
 import urllib3
 
-from ynab_api.exceptions import ApiException, ApiValueError
-
+from ynab_api.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
 
 logger = logging.getLogger(__name__)
 
 
 class RESTResponse(io.IOBase):
-
     def __init__(self, resp):
         self.urllib3_response = resp
         self.status = resp.status
         self.reason = resp.reason
         self.data = resp.data
 
     def getheaders(self):
@@ -44,74 +34,74 @@
 
     def getheader(self, name, default=None):
         """Returns a given response header."""
         return self.urllib3_response.getheader(name, default)
 
 
 class RESTClientObject(object):
-
     def __init__(self, configuration, pools_size=4, maxsize=None):
         # urllib3.PoolManager will pass all kw parameters to connectionpool
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/poolmanager.py#L75  # noqa: E501
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/connectionpool.py#L680  # noqa: E501
         # maxsize is the number of requests to host that are allowed in parallel  # noqa: E501
         # Custom SSL certificates and client certificates: http://urllib3.readthedocs.io/en/latest/advanced-usage.html  # noqa: E501
 
         # cert_reqs
         if configuration.verify_ssl:
             cert_reqs = ssl.CERT_REQUIRED
         else:
             cert_reqs = ssl.CERT_NONE
 
-        # ca_certs
-        if configuration.ssl_ca_cert:
-            ca_certs = configuration.ssl_ca_cert
-        else:
-            # if not set certificate file, use Mozilla's root certificates.
-            ca_certs = certifi.where()
-
         addition_pool_args = {}
         if configuration.assert_hostname is not None:
-            addition_pool_args['assert_hostname'] = configuration.assert_hostname  # noqa: E501
+            addition_pool_args[
+                'assert_hostname'] = configuration.assert_hostname  # noqa: E501
 
         if configuration.retries is not None:
             addition_pool_args['retries'] = configuration.retries
 
+        if configuration.socket_options is not None:
+            addition_pool_args['socket_options'] = configuration.socket_options
+
         if maxsize is None:
             if configuration.connection_pool_maxsize is not None:
                 maxsize = configuration.connection_pool_maxsize
             else:
                 maxsize = 4
 
         # https pool manager
         if configuration.proxy:
             self.pool_manager = urllib3.ProxyManager(
                 num_pools=pools_size,
                 maxsize=maxsize,
                 cert_reqs=cert_reqs,
-                ca_certs=ca_certs,
+                ca_certs=configuration.ssl_ca_cert,
                 cert_file=configuration.cert_file,
                 key_file=configuration.key_file,
                 proxy_url=configuration.proxy,
                 proxy_headers=configuration.proxy_headers,
-                **addition_pool_args
-            )
+                **addition_pool_args)
         else:
             self.pool_manager = urllib3.PoolManager(
                 num_pools=pools_size,
                 maxsize=maxsize,
                 cert_reqs=cert_reqs,
-                ca_certs=ca_certs,
+                ca_certs=configuration.ssl_ca_cert,
                 cert_file=configuration.cert_file,
                 key_file=configuration.key_file,
-                **addition_pool_args
-            )
+                **addition_pool_args)
 
-    def request(self, method, url, query_params=None, headers=None,
-                body=None, post_params=None, _preload_content=True,
+    def request(self,
+                method,
+                url,
+                query_params=None,
+                headers=None,
+                body=None,
+                post_params=None,
+                _preload_content=True,
                 _request_timeout=None):
         """Perform requests.
 
         :param method: http request method
         :param url: http request url
         :param query_params: query parameters in the url
         :param headers: http request headers
@@ -124,173 +114,231 @@
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         """
         method = method.upper()
-        assert method in ['GET', 'HEAD', 'DELETE', 'POST', 'PUT',
-                          'PATCH', 'OPTIONS']
+        assert method in [
+            'GET', 'HEAD', 'DELETE', 'POST', 'PUT', 'PATCH', 'OPTIONS'
+        ]
 
         if post_params and body:
             raise ApiValueError(
-                "body parameter cannot be used with post_params parameter."
-            )
+                "body parameter cannot be used with post_params parameter.")
 
         post_params = post_params or {}
         headers = headers or {}
 
         timeout = None
         if _request_timeout:
-            if isinstance(_request_timeout, (int, ) if six.PY3 else (int, long)):  # noqa: E501,F821
+            if isinstance(_request_timeout, (int, float)):  # noqa: E501,F821
                 timeout = urllib3.Timeout(total=_request_timeout)
-            elif (isinstance(_request_timeout, tuple) and
-                  len(_request_timeout) == 2):
-                timeout = urllib3.Timeout(
-                    connect=_request_timeout[0], read=_request_timeout[1])
-
-        if 'Content-Type' not in headers:
-            headers['Content-Type'] = 'application/json'
+            elif (isinstance(_request_timeout, tuple)
+                  and len(_request_timeout) == 2):
+                timeout = urllib3.Timeout(connect=_request_timeout[0],
+                                          read=_request_timeout[1])
 
         try:
             # For `POST`, `PUT`, `PATCH`, `OPTIONS`, `DELETE`
             if method in ['POST', 'PUT', 'PATCH', 'OPTIONS', 'DELETE']:
+                # Only set a default Content-Type for POST, PUT, PATCH and OPTIONS requests
+                if (method != 'DELETE') and ('Content-Type' not in headers):
+                    headers['Content-Type'] = 'application/json'
                 if query_params:
                     url += '?' + urlencode(query_params)
-                if re.search('json', headers['Content-Type'], re.IGNORECASE):
+                if ('Content-Type' not in headers) or (re.search(
+                        'json', headers['Content-Type'], re.IGNORECASE)):
                     request_body = None
                     if body is not None:
                         request_body = json.dumps(body)
                     r = self.pool_manager.request(
-                        method, url,
+                        method,
+                        url,
                         body=request_body,
                         preload_content=_preload_content,
                         timeout=timeout,
                         headers=headers)
-                elif headers['Content-Type'] == 'application/x-www-form-urlencoded':  # noqa: E501
+                elif headers[
+                        'Content-Type'] == 'application/x-www-form-urlencoded':  # noqa: E501
                     r = self.pool_manager.request(
-                        method, url,
+                        method,
+                        url,
                         fields=post_params,
                         encode_multipart=False,
                         preload_content=_preload_content,
                         timeout=timeout,
                         headers=headers)
                 elif headers['Content-Type'] == 'multipart/form-data':
                     # must del headers['Content-Type'], or the correct
                     # Content-Type which generated by urllib3 will be
                     # overwritten.
                     del headers['Content-Type']
                     r = self.pool_manager.request(
-                        method, url,
+                        method,
+                        url,
                         fields=post_params,
                         encode_multipart=True,
                         preload_content=_preload_content,
                         timeout=timeout,
                         headers=headers)
                 # Pass a `string` parameter directly in the body to support
                 # other content types than Json when `body` argument is
                 # provided in serialized form
                 elif isinstance(body, str) or isinstance(body, bytes):
                     request_body = body
                     r = self.pool_manager.request(
-                        method, url,
+                        method,
+                        url,
                         body=request_body,
                         preload_content=_preload_content,
                         timeout=timeout,
                         headers=headers)
                 else:
                     # Cannot generate the request from given parameters
                     msg = """Cannot prepare a request message for provided
                              arguments. Please check that your arguments match
                              declared content type."""
                     raise ApiException(status=0, reason=msg)
             # For `GET`, `HEAD`
             else:
-                r = self.pool_manager.request(method, url,
+                r = self.pool_manager.request(method,
+                                              url,
                                               fields=query_params,
                                               preload_content=_preload_content,
                                               timeout=timeout,
                                               headers=headers)
         except urllib3.exceptions.SSLError as e:
             msg = "{0}\n{1}".format(type(e).__name__, str(e))
             raise ApiException(status=0, reason=msg)
 
         if _preload_content:
             r = RESTResponse(r)
 
-            # In the python 3, the response.data is bytes.
-            # we need to decode it to string.
-            if six.PY3:
-                r.data = r.data.decode('utf8')
-
             # log response body
             logger.debug("response body: %s", r.data)
 
         if not 200 <= r.status <= 299:
+            if r.status == 401:
+                raise UnauthorizedException(http_resp=r)
+
+            if r.status == 403:
+                raise ForbiddenException(http_resp=r)
+
+            if r.status == 404:
+                raise NotFoundException(http_resp=r)
+
+            if 500 <= r.status <= 599:
+                raise ServiceException(http_resp=r)
+
             raise ApiException(http_resp=r)
 
         return r
 
-    def GET(self, url, headers=None, query_params=None, _preload_content=True,
+    def GET(self,
+            url,
+            headers=None,
+            query_params=None,
+            _preload_content=True,
             _request_timeout=None):
-        return self.request("GET", url,
+        return self.request("GET",
+                            url,
                             headers=headers,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             query_params=query_params)
 
-    def HEAD(self, url, headers=None, query_params=None, _preload_content=True,
+    def HEAD(self,
+             url,
+             headers=None,
+             query_params=None,
+             _preload_content=True,
              _request_timeout=None):
-        return self.request("HEAD", url,
+        return self.request("HEAD",
+                            url,
                             headers=headers,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             query_params=query_params)
 
-    def OPTIONS(self, url, headers=None, query_params=None, post_params=None,
-                body=None, _preload_content=True, _request_timeout=None):
-        return self.request("OPTIONS", url,
+    def OPTIONS(self,
+                url,
+                headers=None,
+                query_params=None,
+                post_params=None,
+                body=None,
+                _preload_content=True,
+                _request_timeout=None):
+        return self.request("OPTIONS",
+                            url,
                             headers=headers,
                             query_params=query_params,
                             post_params=post_params,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             body=body)
 
-    def DELETE(self, url, headers=None, query_params=None, body=None,
-               _preload_content=True, _request_timeout=None):
-        return self.request("DELETE", url,
+    def DELETE(self,
+               url,
+               headers=None,
+               query_params=None,
+               body=None,
+               _preload_content=True,
+               _request_timeout=None):
+        return self.request("DELETE",
+                            url,
                             headers=headers,
                             query_params=query_params,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             body=body)
 
-    def POST(self, url, headers=None, query_params=None, post_params=None,
-             body=None, _preload_content=True, _request_timeout=None):
-        return self.request("POST", url,
+    def POST(self,
+             url,
+             headers=None,
+             query_params=None,
+             post_params=None,
+             body=None,
+             _preload_content=True,
+             _request_timeout=None):
+        return self.request("POST",
+                            url,
                             headers=headers,
                             query_params=query_params,
                             post_params=post_params,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             body=body)
 
-    def PUT(self, url, headers=None, query_params=None, post_params=None,
-            body=None, _preload_content=True, _request_timeout=None):
-        return self.request("PUT", url,
+    def PUT(self,
+            url,
+            headers=None,
+            query_params=None,
+            post_params=None,
+            body=None,
+            _preload_content=True,
+            _request_timeout=None):
+        return self.request("PUT",
+                            url,
                             headers=headers,
                             query_params=query_params,
                             post_params=post_params,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             body=body)
 
-    def PATCH(self, url, headers=None, query_params=None, post_params=None,
-              body=None, _preload_content=True, _request_timeout=None):
-        return self.request("PATCH", url,
+    def PATCH(self,
+              url,
+              headers=None,
+              query_params=None,
+              post_params=None,
+              body=None,
+              _preload_content=True,
+              _request_timeout=None):
+        return self.request("PATCH",
+                            url,
                             headers=headers,
                             query_params=query_params,
                             post_params=post_params,
                             _preload_content=_preload_content,
                             _request_timeout=_request_timeout,
                             body=body)
```

### Comparing `ynab-api-1.0.0/ynab_api/__init__.py` & `ynab-api-2.0.0/ynab_api/models/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,123 +1,99 @@
-# coding: utf-8
-
 # flake8: noqa
 
-"""
-    YNAB API Endpoints
-
-    Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com  # noqa: E501
-
-    The version of the OpenAPI document: 1.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-from __future__ import absolute_import
-
-__version__ = "1.0.0"
-
-# import apis into sdk package
-from ynab_api.api.accounts_api import AccountsApi
-from ynab_api.api.budgets_api import BudgetsApi
-from ynab_api.api.categories_api import CategoriesApi
-from ynab_api.api.deprecated_api import DeprecatedApi
-from ynab_api.api.months_api import MonthsApi
-from ynab_api.api.payee_locations_api import PayeeLocationsApi
-from ynab_api.api.payees_api import PayeesApi
-from ynab_api.api.scheduled_transactions_api import ScheduledTransactionsApi
-from ynab_api.api.transactions_api import TransactionsApi
-from ynab_api.api.user_api import UserApi
-
-# import ApiClient
-from ynab_api.api_client import ApiClient
-from ynab_api.configuration import Configuration
-from ynab_api.exceptions import OpenApiException
-from ynab_api.exceptions import ApiTypeError
-from ynab_api.exceptions import ApiValueError
-from ynab_api.exceptions import ApiKeyError
-from ynab_api.exceptions import ApiException
-# import models into sdk package
-from ynab_api.models.account import Account
-from ynab_api.models.account_response import AccountResponse
-from ynab_api.models.account_response_data import AccountResponseData
-from ynab_api.models.accounts_response import AccountsResponse
-from ynab_api.models.accounts_response_data import AccountsResponseData
-from ynab_api.models.budget_detail import BudgetDetail
-from ynab_api.models.budget_detail_all_of import BudgetDetailAllOf
-from ynab_api.models.budget_detail_response import BudgetDetailResponse
-from ynab_api.models.budget_detail_response_data import BudgetDetailResponseData
-from ynab_api.models.budget_settings import BudgetSettings
-from ynab_api.models.budget_settings_response import BudgetSettingsResponse
-from ynab_api.models.budget_settings_response_data import BudgetSettingsResponseData
-from ynab_api.models.budget_summary import BudgetSummary
-from ynab_api.models.budget_summary_response import BudgetSummaryResponse
-from ynab_api.models.budget_summary_response_data import BudgetSummaryResponseData
-from ynab_api.models.bulk_response import BulkResponse
-from ynab_api.models.bulk_response_data import BulkResponseData
-from ynab_api.models.bulk_response_data_bulk import BulkResponseDataBulk
-from ynab_api.models.bulk_transactions import BulkTransactions
-from ynab_api.models.categories_response import CategoriesResponse
-from ynab_api.models.categories_response_data import CategoriesResponseData
-from ynab_api.models.category import Category
-from ynab_api.models.category_group import CategoryGroup
-from ynab_api.models.category_group_with_categories import CategoryGroupWithCategories
-from ynab_api.models.category_group_with_categories_all_of import CategoryGroupWithCategoriesAllOf
-from ynab_api.models.category_response import CategoryResponse
-from ynab_api.models.category_response_data import CategoryResponseData
-from ynab_api.models.currency_format import CurrencyFormat
-from ynab_api.models.date_format import DateFormat
-from ynab_api.models.error_detail import ErrorDetail
-from ynab_api.models.error_response import ErrorResponse
-from ynab_api.models.hybrid_transaction import HybridTransaction
-from ynab_api.models.hybrid_transaction_all_of import HybridTransactionAllOf
-from ynab_api.models.hybrid_transactions_response import HybridTransactionsResponse
-from ynab_api.models.hybrid_transactions_response_data import HybridTransactionsResponseData
-from ynab_api.models.month_detail import MonthDetail
-from ynab_api.models.month_detail_all_of import MonthDetailAllOf
-from ynab_api.models.month_detail_response import MonthDetailResponse
-from ynab_api.models.month_detail_response_data import MonthDetailResponseData
-from ynab_api.models.month_summaries_response import MonthSummariesResponse
-from ynab_api.models.month_summaries_response_data import MonthSummariesResponseData
-from ynab_api.models.month_summary import MonthSummary
-from ynab_api.models.payee import Payee
-from ynab_api.models.payee_location import PayeeLocation
-from ynab_api.models.payee_location_response import PayeeLocationResponse
-from ynab_api.models.payee_location_response_data import PayeeLocationResponseData
-from ynab_api.models.payee_locations_response import PayeeLocationsResponse
-from ynab_api.models.payee_locations_response_data import PayeeLocationsResponseData
-from ynab_api.models.payee_response import PayeeResponse
-from ynab_api.models.payee_response_data import PayeeResponseData
-from ynab_api.models.payees_response import PayeesResponse
-from ynab_api.models.payees_response_data import PayeesResponseData
-from ynab_api.models.save_category_response import SaveCategoryResponse
-from ynab_api.models.save_category_response_data import SaveCategoryResponseData
-from ynab_api.models.save_month_category import SaveMonthCategory
-from ynab_api.models.save_month_category_wrapper import SaveMonthCategoryWrapper
-from ynab_api.models.save_transaction import SaveTransaction
-from ynab_api.models.save_transaction_wrapper import SaveTransactionWrapper
-from ynab_api.models.save_transactions_response import SaveTransactionsResponse
-from ynab_api.models.save_transactions_response_data import SaveTransactionsResponseData
-from ynab_api.models.save_transactions_wrapper import SaveTransactionsWrapper
-from ynab_api.models.scheduled_sub_transaction import ScheduledSubTransaction
-from ynab_api.models.scheduled_transaction_detail import ScheduledTransactionDetail
-from ynab_api.models.scheduled_transaction_detail_all_of import ScheduledTransactionDetailAllOf
-from ynab_api.models.scheduled_transaction_response import ScheduledTransactionResponse
-from ynab_api.models.scheduled_transaction_response_data import ScheduledTransactionResponseData
-from ynab_api.models.scheduled_transaction_summary import ScheduledTransactionSummary
-from ynab_api.models.scheduled_transactions_response import ScheduledTransactionsResponse
-from ynab_api.models.scheduled_transactions_response_data import ScheduledTransactionsResponseData
-from ynab_api.models.sub_transaction import SubTransaction
-from ynab_api.models.transaction_detail import TransactionDetail
-from ynab_api.models.transaction_detail_all_of import TransactionDetailAllOf
-from ynab_api.models.transaction_response import TransactionResponse
-from ynab_api.models.transaction_response_data import TransactionResponseData
-from ynab_api.models.transaction_summary import TransactionSummary
-from ynab_api.models.transactions_response import TransactionsResponse
-from ynab_api.models.transactions_response_data import TransactionsResponseData
-from ynab_api.models.update_transaction import UpdateTransaction
-from ynab_api.models.update_transaction_all_of import UpdateTransactionAllOf
-from ynab_api.models.update_transactions_wrapper import UpdateTransactionsWrapper
-from ynab_api.models.user import User
-from ynab_api.models.user_response import UserResponse
-from ynab_api.models.user_response_data import UserResponseData
-
+# import all models into this package
+# if you have many models here with many references from one model to another this may
+# raise a RecursionError
+# to avoid this, import only the models that you directly need like:
+# from from ynab_api.model.pet import Pet
+# or import this package, but before doing it, use:
+# import sys
+# sys.setrecursionlimit(n)
+
+from ynab_api.model.account import Account
+from ynab_api.model.account_response import AccountResponse
+from ynab_api.model.account_response_data import AccountResponseData
+from ynab_api.model.accounts_response import AccountsResponse
+from ynab_api.model.accounts_response_data import AccountsResponseData
+from ynab_api.model.budget_detail import BudgetDetail
+from ynab_api.model.budget_detail_all_of import BudgetDetailAllOf
+from ynab_api.model.budget_detail_response import BudgetDetailResponse
+from ynab_api.model.budget_detail_response_data import BudgetDetailResponseData
+from ynab_api.model.budget_settings import BudgetSettings
+from ynab_api.model.budget_settings_response import BudgetSettingsResponse
+from ynab_api.model.budget_settings_response_data import BudgetSettingsResponseData
+from ynab_api.model.budget_summary import BudgetSummary
+from ynab_api.model.budget_summary_response import BudgetSummaryResponse
+from ynab_api.model.budget_summary_response_data import BudgetSummaryResponseData
+from ynab_api.model.bulk_response import BulkResponse
+from ynab_api.model.bulk_response_data import BulkResponseData
+from ynab_api.model.bulk_response_data_bulk import BulkResponseDataBulk
+from ynab_api.model.bulk_transactions import BulkTransactions
+from ynab_api.model.categories_response import CategoriesResponse
+from ynab_api.model.categories_response_data import CategoriesResponseData
+from ynab_api.model.category import Category
+from ynab_api.model.category_group import CategoryGroup
+from ynab_api.model.category_group_with_categories import CategoryGroupWithCategories
+from ynab_api.model.category_group_with_categories_all_of import CategoryGroupWithCategoriesAllOf
+from ynab_api.model.category_response import CategoryResponse
+from ynab_api.model.category_response_data import CategoryResponseData
+from ynab_api.model.currency_format import CurrencyFormat
+from ynab_api.model.date_format import DateFormat
+from ynab_api.model.error_detail import ErrorDetail
+from ynab_api.model.error_response import ErrorResponse
+from ynab_api.model.hybrid_transaction import HybridTransaction
+from ynab_api.model.hybrid_transaction_all_of import HybridTransactionAllOf
+from ynab_api.model.hybrid_transactions_response import HybridTransactionsResponse
+from ynab_api.model.hybrid_transactions_response_data import HybridTransactionsResponseData
+from ynab_api.model.month_detail import MonthDetail
+from ynab_api.model.month_detail_all_of import MonthDetailAllOf
+from ynab_api.model.month_detail_response import MonthDetailResponse
+from ynab_api.model.month_detail_response_data import MonthDetailResponseData
+from ynab_api.model.month_summaries_response import MonthSummariesResponse
+from ynab_api.model.month_summaries_response_data import MonthSummariesResponseData
+from ynab_api.model.month_summary import MonthSummary
+from ynab_api.model.payee import Payee
+from ynab_api.model.payee_location import PayeeLocation
+from ynab_api.model.payee_location_response import PayeeLocationResponse
+from ynab_api.model.payee_location_response_data import PayeeLocationResponseData
+from ynab_api.model.payee_locations_response import PayeeLocationsResponse
+from ynab_api.model.payee_locations_response_data import PayeeLocationsResponseData
+from ynab_api.model.payee_response import PayeeResponse
+from ynab_api.model.payee_response_data import PayeeResponseData
+from ynab_api.model.payees_response import PayeesResponse
+from ynab_api.model.payees_response_data import PayeesResponseData
+from ynab_api.model.save_account import SaveAccount
+from ynab_api.model.save_account_wrapper import SaveAccountWrapper
+from ynab_api.model.save_category_response import SaveCategoryResponse
+from ynab_api.model.save_category_response_data import SaveCategoryResponseData
+from ynab_api.model.save_month_category import SaveMonthCategory
+from ynab_api.model.save_month_category_wrapper import SaveMonthCategoryWrapper
+from ynab_api.model.save_sub_transaction import SaveSubTransaction
+from ynab_api.model.save_transaction import SaveTransaction
+from ynab_api.model.save_transaction_wrapper import SaveTransactionWrapper
+from ynab_api.model.save_transactions_response import SaveTransactionsResponse
+from ynab_api.model.save_transactions_response_data import SaveTransactionsResponseData
+from ynab_api.model.save_transactions_wrapper import SaveTransactionsWrapper
+from ynab_api.model.scheduled_sub_transaction import ScheduledSubTransaction
+from ynab_api.model.scheduled_transaction_detail import ScheduledTransactionDetail
+from ynab_api.model.scheduled_transaction_detail_all_of import ScheduledTransactionDetailAllOf
+from ynab_api.model.scheduled_transaction_response import ScheduledTransactionResponse
+from ynab_api.model.scheduled_transaction_response_data import ScheduledTransactionResponseData
+from ynab_api.model.scheduled_transaction_summary import ScheduledTransactionSummary
+from ynab_api.model.scheduled_transactions_response import ScheduledTransactionsResponse
+from ynab_api.model.scheduled_transactions_response_data import ScheduledTransactionsResponseData
+from ynab_api.model.sub_transaction import SubTransaction
+from ynab_api.model.transaction_detail import TransactionDetail
+from ynab_api.model.transaction_detail_all_of import TransactionDetailAllOf
+from ynab_api.model.transaction_response import TransactionResponse
+from ynab_api.model.transaction_response_data import TransactionResponseData
+from ynab_api.model.transaction_summary import TransactionSummary
+from ynab_api.model.transactions_import_response import TransactionsImportResponse
+from ynab_api.model.transactions_import_response_data import TransactionsImportResponseData
+from ynab_api.model.transactions_response import TransactionsResponse
+from ynab_api.model.transactions_response_data import TransactionsResponseData
+from ynab_api.model.update_transaction import UpdateTransaction
+from ynab_api.model.update_transaction_all_of import UpdateTransactionAllOf
+from ynab_api.model.update_transactions_wrapper import UpdateTransactionsWrapper
+from ynab_api.model.user import User
+from ynab_api.model.user_response import UserResponse
+from ynab_api.model.user_response_data import UserResponseData
```

### Comparing `ynab-api-1.0.0/ynab_api.egg-info/SOURCES.txt` & `ynab-api-2.0.0/ynab_api.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 README.md
 setup.cfg
 setup.py
-test/__init__.py
 test/test_account.py
 test/test_account_response.py
 test/test_account_response_data.py
 test/test_accounts_api.py
 test/test_accounts_response.py
 test/test_accounts_response_data.py
 test/test_budget_detail.py
@@ -57,18 +56,21 @@
 test/test_payee_locations_response.py
 test/test_payee_locations_response_data.py
 test/test_payee_response.py
 test/test_payee_response_data.py
 test/test_payees_api.py
 test/test_payees_response.py
 test/test_payees_response_data.py
+test/test_save_account.py
+test/test_save_account_wrapper.py
 test/test_save_category_response.py
 test/test_save_category_response_data.py
 test/test_save_month_category.py
 test/test_save_month_category_wrapper.py
+test/test_save_sub_transaction.py
 test/test_save_transaction.py
 test/test_save_transaction_wrapper.py
 test/test_save_transactions_response.py
 test/test_save_transactions_response_data.py
 test/test_save_transactions_wrapper.py
 test/test_scheduled_sub_transaction.py
 test/test_scheduled_transaction_detail.py
@@ -82,27 +84,30 @@
 test/test_sub_transaction.py
 test/test_transaction_detail.py
 test/test_transaction_detail_all_of.py
 test/test_transaction_response.py
 test/test_transaction_response_data.py
 test/test_transaction_summary.py
 test/test_transactions_api.py
+test/test_transactions_import_response.py
+test/test_transactions_import_response_data.py
 test/test_transactions_response.py
 test/test_transactions_response_data.py
 test/test_update_transaction.py
 test/test_update_transaction_all_of.py
 test/test_update_transactions_wrapper.py
 test/test_user.py
 test/test_user_api.py
 test/test_user_response.py
 test/test_user_response_data.py
 ynab_api/__init__.py
 ynab_api/api_client.py
 ynab_api/configuration.py
 ynab_api/exceptions.py
+ynab_api/model_utils.py
 ynab_api/rest.py
 ynab_api.egg-info/PKG-INFO
 ynab_api.egg-info/SOURCES.txt
 ynab_api.egg-info/dependency_links.txt
 ynab_api.egg-info/requires.txt
 ynab_api.egg-info/top_level.txt
 ynab_api/api/__init__.py
@@ -112,91 +117,98 @@
 ynab_api/api/deprecated_api.py
 ynab_api/api/months_api.py
 ynab_api/api/payee_locations_api.py
 ynab_api/api/payees_api.py
 ynab_api/api/scheduled_transactions_api.py
 ynab_api/api/transactions_api.py
 ynab_api/api/user_api.py
-ynab_api/models/__init__.py
-ynab_api/models/account.py
-ynab_api/models/account_response.py
-ynab_api/models/account_response_data.py
-ynab_api/models/accounts_response.py
-ynab_api/models/accounts_response_data.py
-ynab_api/models/budget_detail.py
-ynab_api/models/budget_detail_all_of.py
-ynab_api/models/budget_detail_response.py
-ynab_api/models/budget_detail_response_data.py
-ynab_api/models/budget_settings.py
-ynab_api/models/budget_settings_response.py
-ynab_api/models/budget_settings_response_data.py
-ynab_api/models/budget_summary.py
-ynab_api/models/budget_summary_response.py
-ynab_api/models/budget_summary_response_data.py
-ynab_api/models/bulk_response.py
-ynab_api/models/bulk_response_data.py
-ynab_api/models/bulk_response_data_bulk.py
-ynab_api/models/bulk_transactions.py
-ynab_api/models/categories_response.py
-ynab_api/models/categories_response_data.py
-ynab_api/models/category.py
-ynab_api/models/category_group.py
-ynab_api/models/category_group_with_categories.py
-ynab_api/models/category_group_with_categories_all_of.py
-ynab_api/models/category_response.py
-ynab_api/models/category_response_data.py
-ynab_api/models/currency_format.py
-ynab_api/models/date_format.py
-ynab_api/models/error_detail.py
-ynab_api/models/error_response.py
-ynab_api/models/hybrid_transaction.py
-ynab_api/models/hybrid_transaction_all_of.py
-ynab_api/models/hybrid_transactions_response.py
-ynab_api/models/hybrid_transactions_response_data.py
-ynab_api/models/month_detail.py
-ynab_api/models/month_detail_all_of.py
-ynab_api/models/month_detail_response.py
-ynab_api/models/month_detail_response_data.py
-ynab_api/models/month_summaries_response.py
-ynab_api/models/month_summaries_response_data.py
-ynab_api/models/month_summary.py
-ynab_api/models/payee.py
-ynab_api/models/payee_location.py
-ynab_api/models/payee_location_response.py
-ynab_api/models/payee_location_response_data.py
-ynab_api/models/payee_locations_response.py
-ynab_api/models/payee_locations_response_data.py
-ynab_api/models/payee_response.py
-ynab_api/models/payee_response_data.py
-ynab_api/models/payees_response.py
-ynab_api/models/payees_response_data.py
-ynab_api/models/save_category_response.py
-ynab_api/models/save_category_response_data.py
-ynab_api/models/save_month_category.py
-ynab_api/models/save_month_category_wrapper.py
-ynab_api/models/save_transaction.py
-ynab_api/models/save_transaction_wrapper.py
-ynab_api/models/save_transactions_response.py
-ynab_api/models/save_transactions_response_data.py
-ynab_api/models/save_transactions_wrapper.py
-ynab_api/models/scheduled_sub_transaction.py
-ynab_api/models/scheduled_transaction_detail.py
-ynab_api/models/scheduled_transaction_detail_all_of.py
-ynab_api/models/scheduled_transaction_response.py
-ynab_api/models/scheduled_transaction_response_data.py
-ynab_api/models/scheduled_transaction_summary.py
-ynab_api/models/scheduled_transactions_response.py
-ynab_api/models/scheduled_transactions_response_data.py
-ynab_api/models/sub_transaction.py
-ynab_api/models/transaction_detail.py
-ynab_api/models/transaction_detail_all_of.py
-ynab_api/models/transaction_response.py
-ynab_api/models/transaction_response_data.py
-ynab_api/models/transaction_summary.py
-ynab_api/models/transactions_response.py
-ynab_api/models/transactions_response_data.py
-ynab_api/models/update_transaction.py
-ynab_api/models/update_transaction_all_of.py
-ynab_api/models/update_transactions_wrapper.py
-ynab_api/models/user.py
-ynab_api/models/user_response.py
-ynab_api/models/user_response_data.py
+ynab_api/apis/__init__.py
+ynab_api/model/__init__.py
+ynab_api/model/account.py
+ynab_api/model/account_response.py
+ynab_api/model/account_response_data.py
+ynab_api/model/accounts_response.py
+ynab_api/model/accounts_response_data.py
+ynab_api/model/budget_detail.py
+ynab_api/model/budget_detail_all_of.py
+ynab_api/model/budget_detail_response.py
+ynab_api/model/budget_detail_response_data.py
+ynab_api/model/budget_settings.py
+ynab_api/model/budget_settings_response.py
+ynab_api/model/budget_settings_response_data.py
+ynab_api/model/budget_summary.py
+ynab_api/model/budget_summary_response.py
+ynab_api/model/budget_summary_response_data.py
+ynab_api/model/bulk_response.py
+ynab_api/model/bulk_response_data.py
+ynab_api/model/bulk_response_data_bulk.py
+ynab_api/model/bulk_transactions.py
+ynab_api/model/categories_response.py
+ynab_api/model/categories_response_data.py
+ynab_api/model/category.py
+ynab_api/model/category_group.py
+ynab_api/model/category_group_with_categories.py
+ynab_api/model/category_group_with_categories_all_of.py
+ynab_api/model/category_response.py
+ynab_api/model/category_response_data.py
+ynab_api/model/currency_format.py
+ynab_api/model/date_format.py
+ynab_api/model/error_detail.py
+ynab_api/model/error_response.py
+ynab_api/model/hybrid_transaction.py
+ynab_api/model/hybrid_transaction_all_of.py
+ynab_api/model/hybrid_transactions_response.py
+ynab_api/model/hybrid_transactions_response_data.py
+ynab_api/model/month_detail.py
+ynab_api/model/month_detail_all_of.py
+ynab_api/model/month_detail_response.py
+ynab_api/model/month_detail_response_data.py
+ynab_api/model/month_summaries_response.py
+ynab_api/model/month_summaries_response_data.py
+ynab_api/model/month_summary.py
+ynab_api/model/payee.py
+ynab_api/model/payee_location.py
+ynab_api/model/payee_location_response.py
+ynab_api/model/payee_location_response_data.py
+ynab_api/model/payee_locations_response.py
+ynab_api/model/payee_locations_response_data.py
+ynab_api/model/payee_response.py
+ynab_api/model/payee_response_data.py
+ynab_api/model/payees_response.py
+ynab_api/model/payees_response_data.py
+ynab_api/model/save_account.py
+ynab_api/model/save_account_wrapper.py
+ynab_api/model/save_category_response.py
+ynab_api/model/save_category_response_data.py
+ynab_api/model/save_month_category.py
+ynab_api/model/save_month_category_wrapper.py
+ynab_api/model/save_sub_transaction.py
+ynab_api/model/save_transaction.py
+ynab_api/model/save_transaction_wrapper.py
+ynab_api/model/save_transactions_response.py
+ynab_api/model/save_transactions_response_data.py
+ynab_api/model/save_transactions_wrapper.py
+ynab_api/model/scheduled_sub_transaction.py
+ynab_api/model/scheduled_transaction_detail.py
+ynab_api/model/scheduled_transaction_detail_all_of.py
+ynab_api/model/scheduled_transaction_response.py
+ynab_api/model/scheduled_transaction_response_data.py
+ynab_api/model/scheduled_transaction_summary.py
+ynab_api/model/scheduled_transactions_response.py
+ynab_api/model/scheduled_transactions_response_data.py
+ynab_api/model/sub_transaction.py
+ynab_api/model/transaction_detail.py
+ynab_api/model/transaction_detail_all_of.py
+ynab_api/model/transaction_response.py
+ynab_api/model/transaction_response_data.py
+ynab_api/model/transaction_summary.py
+ynab_api/model/transactions_import_response.py
+ynab_api/model/transactions_import_response_data.py
+ynab_api/model/transactions_response.py
+ynab_api/model/transactions_response_data.py
+ynab_api/model/update_transaction.py
+ynab_api/model/update_transaction_all_of.py
+ynab_api/model/update_transactions_wrapper.py
+ynab_api/model/user.py
+ynab_api/model/user_response.py
+ynab_api/model/user_response_data.py
+ynab_api/models/__init__.py
```

