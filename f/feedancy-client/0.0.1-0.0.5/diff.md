# Comparing `tmp/feedancy_client-0.0.1.tar.gz` & `tmp/feedancy_client-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedancy_client-0.0.1.tar", max compression
+gzip compressed data, was "feedancy_client-0.0.5.tar", max compression
```

## Comparing `feedancy_client-0.0.1.tar` & `feedancy_client-0.0.5.tar`

### file list

```diff
@@ -1,123 +1,125 @@
--rw-r--r--   0        0        0      657 2023-07-03 13:41:07.205539 feedancy_client-0.0.1/feedancy-client/README.md
--rw-r--r--   0        0        0      133 2023-07-03 13:41:07.197539 feedancy_client-0.0.1/feedancy-client/feedancy_client/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 13:41:07.121537 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 13:41:07.121537 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/__init__.py
--rw-r--r--   0        0        0    13079 2023-07-03 13:41:07.129537 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api.py
--rw-r--r--   0        0        0      784 2023-07-03 13:41:07.145538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_create.py
--rw-r--r--   0        0        0      841 2023-07-03 13:41:07.145538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_destroy.py
--rw-r--r--   0        0        0      783 2023-07-03 13:41:07.145538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_retrieve.py
--rw-r--r--   0        0        0      838 2023-07-03 13:41:07.145538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_retrieve_2.py
--rw-r--r--   0        0        0      838 2023-07-03 13:41:07.145538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_update.py
--rw-r--r--   0        0        0      774 2023-07-03 13:41:07.145538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_city_create.py
--rw-r--r--   0        0        0      831 2023-07-03 13:41:07.145538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_city_destroy.py
--rw-r--r--   0        0        0      773 2023-07-03 13:41:07.145538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_city_retrieve.py
--rw-r--r--   0        0        0      828 2023-07-03 13:41:07.145538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_city_retrieve_2.py
--rw-r--r--   0        0        0      828 2023-07-03 13:41:07.145538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_city_update.py
--rw-r--r--   0        0        0      777 2023-07-03 13:41:07.145538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_company_create.py
--rw-r--r--   0        0        0      834 2023-07-03 13:41:07.149538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_company_destroy.py
--rw-r--r--   0        0        0      776 2023-07-03 13:41:07.145538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_company_retrieve.py
--rw-r--r--   0        0        0      831 2023-07-03 13:41:07.145538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_company_retrieve_2.py
--rw-r--r--   0        0        0      831 2023-07-03 13:41:07.145538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_company_update.py
--rw-r--r--   0        0        0      781 2023-07-03 13:41:07.149538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_companycity_create.py
--rw-r--r--   0        0        0      838 2023-07-03 13:41:07.149538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_companycity_destroy.py
--rw-r--r--   0        0        0      780 2023-07-03 13:41:07.149538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_companycity_retrieve.py
--rw-r--r--   0        0        0      835 2023-07-03 13:41:07.149538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_companycity_retrieve_2.py
--rw-r--r--   0        0        0      835 2023-07-03 13:41:07.149538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_companycity_update.py
--rw-r--r--   0        0        0      777 2023-07-03 13:41:07.149538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_contact_create.py
--rw-r--r--   0        0        0      834 2023-07-03 13:41:07.149538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_contact_destroy.py
--rw-r--r--   0        0        0      776 2023-07-03 13:41:07.149538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_contact_retrieve.py
--rw-r--r--   0        0        0      831 2023-07-03 13:41:07.149538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_contact_retrieve_2.py
--rw-r--r--   0        0        0      831 2023-07-03 13:41:07.149538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_contact_update.py
--rw-r--r--   0        0        0      777 2023-07-03 13:41:07.149538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_country_create.py
--rw-r--r--   0        0        0      834 2023-07-03 13:41:07.149538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_country_destroy.py
--rw-r--r--   0        0        0      776 2023-07-03 13:41:07.149538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_country_retrieve.py
--rw-r--r--   0        0        0      831 2023-07-03 13:41:07.149538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_country_retrieve_2.py
--rw-r--r--   0        0        0      831 2023-07-03 13:41:07.149538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_country_update.py
--rw-r--r--   0        0        0      778 2023-07-03 13:41:07.153538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_currency_create.py
--rw-r--r--   0        0        0      835 2023-07-03 13:41:07.153538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_currency_destroy.py
--rw-r--r--   0        0        0      777 2023-07-03 13:41:07.153538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_currency_retrieve.py
--rw-r--r--   0        0        0      832 2023-07-03 13:41:07.153538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_currency_retrieve_2.py
--rw-r--r--   0        0        0      832 2023-07-03 13:41:07.153538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_currency_update.py
--rw-r--r--   0        0        0      780 2023-07-03 13:41:07.153538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internship_create.py
--rw-r--r--   0        0        0     1962 2023-07-03 13:41:07.165538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internship_destroy.py
--rw-r--r--   0        0        0      779 2023-07-03 13:41:07.153538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internship_retrieve.py
--rw-r--r--   0        0        0     1959 2023-07-03 13:41:07.157538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internship_retrieve_2.py
--rw-r--r--   0        0        0     1997 2023-07-03 13:41:07.161538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internship_update.py
--rw-r--r--   0        0        0      784 2023-07-03 13:41:07.165538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_create.py
--rw-r--r--   0        0        0      841 2023-07-03 13:41:07.169538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_destroy.py
--rw-r--r--   0        0        0      783 2023-07-03 13:41:07.165538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_retrieve.py
--rw-r--r--   0        0        0      838 2023-07-03 13:41:07.165538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_retrieve_2.py
--rw-r--r--   0        0        0      838 2023-07-03 13:41:07.169538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_update.py
--rw-r--r--   0        0        0      787 2023-07-03 13:41:07.169538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_create.py
--rw-r--r--   0        0        0      844 2023-07-03 13:41:07.169538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_destroy.py
--rw-r--r--   0        0        0      786 2023-07-03 13:41:07.169538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_retrieve.py
--rw-r--r--   0        0        0      841 2023-07-03 13:41:07.169538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_retrieve_2.py
--rw-r--r--   0        0        0      841 2023-07-03 13:41:07.169538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_update.py
--rw-r--r--   0        0        0      785 2023-07-03 13:41:07.169538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_create.py
--rw-r--r--   0        0        0      842 2023-07-03 13:41:07.169538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_destroy.py
--rw-r--r--   0        0        0      784 2023-07-03 13:41:07.169538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_retrieve.py
--rw-r--r--   0        0        0      839 2023-07-03 13:41:07.169538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_retrieve_2.py
--rw-r--r--   0        0        0      839 2023-07-03 13:41:07.169538 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_update.py
--rw-r--r--   0        0        0      778 2023-07-03 13:41:07.173539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_create.py
--rw-r--r--   0        0        0      835 2023-07-03 13:41:07.173539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_destroy.py
--rw-r--r--   0        0        0      777 2023-07-03 13:41:07.173539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_retrieve.py
--rw-r--r--   0        0        0      832 2023-07-03 13:41:07.173539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_retrieve_2.py
--rw-r--r--   0        0        0      832 2023-07-03 13:41:07.173539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_update.py
--rw-r--r--   0        0        0      776 2023-07-03 13:41:07.173539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_region_create.py
--rw-r--r--   0        0        0      833 2023-07-03 13:41:07.173539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_region_destroy.py
--rw-r--r--   0        0        0      775 2023-07-03 13:41:07.173539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_region_retrieve.py
--rw-r--r--   0        0        0      830 2023-07-03 13:41:07.173539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_region_retrieve_2.py
--rw-r--r--   0        0        0      830 2023-07-03 13:41:07.173539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_region_update.py
--rw-r--r--   0        0        0      776 2023-07-03 13:41:07.173539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_salary_create.py
--rw-r--r--   0        0        0      833 2023-07-03 13:41:07.173539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_salary_destroy.py
--rw-r--r--   0        0        0      775 2023-07-03 13:41:07.173539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_salary_retrieve.py
--rw-r--r--   0        0        0      830 2023-07-03 13:41:07.173539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_salary_retrieve_2.py
--rw-r--r--   0        0        0      830 2023-07-03 13:41:07.173539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_salary_update.py
--rw-r--r--   0        0        0      791 2023-07-03 13:41:07.177539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_create.py
--rw-r--r--   0        0        0      848 2023-07-03 13:41:07.177539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_destroy.py
--rw-r--r--   0        0        0      790 2023-07-03 13:41:07.177539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_retrieve.py
--rw-r--r--   0        0        0      845 2023-07-03 13:41:07.177539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_retrieve_2.py
--rw-r--r--   0        0        0      845 2023-07-03 13:41:07.177539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_update.py
--rw-r--r--   0        0        0      784 2023-07-03 13:41:07.177539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_create.py
--rw-r--r--   0        0        0      841 2023-07-03 13:41:07.177539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_destroy.py
--rw-r--r--   0        0        0      783 2023-07-03 13:41:07.177539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_retrieve.py
--rw-r--r--   0        0        0      838 2023-07-03 13:41:07.177539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_retrieve_2.py
--rw-r--r--   0        0        0      838 2023-07-03 13:41:07.177539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_update.py
--rw-r--r--   0        0        0      775 2023-07-03 13:41:07.177539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_skill_create.py
--rw-r--r--   0        0        0      832 2023-07-03 13:41:07.177539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_skill_destroy.py
--rw-r--r--   0        0        0      774 2023-07-03 13:41:07.177539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_skill_retrieve.py
--rw-r--r--   0        0        0      829 2023-07-03 13:41:07.177539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_skill_retrieve_2.py
--rw-r--r--   0        0        0      829 2023-07-03 13:41:07.177539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_skill_update.py
--rw-r--r--   0        0        0      776 2023-07-03 13:41:07.177539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_source_create.py
--rw-r--r--   0        0        0      833 2023-07-03 13:41:07.181539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_source_destroy.py
--rw-r--r--   0        0        0      775 2023-07-03 13:41:07.177539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_source_retrieve.py
--rw-r--r--   0        0        0      830 2023-07-03 13:41:07.177539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_source_retrieve_2.py
--rw-r--r--   0        0        0      830 2023-07-03 13:41:07.181539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_source_update.py
--rw-r--r--   0        0        0      782 2023-07-03 13:41:07.181539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_create.py
--rw-r--r--   0        0        0      839 2023-07-03 13:41:07.181539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_destroy.py
--rw-r--r--   0        0        0      781 2023-07-03 13:41:07.181539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_retrieve.py
--rw-r--r--   0        0        0      836 2023-07-03 13:41:07.181539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_retrieve_2.py
--rw-r--r--   0        0        0      836 2023-07-03 13:41:07.181539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_update.py
--rw-r--r--   0        0        0     2067 2023-07-03 13:41:07.185539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_create.py
--rw-r--r--   0        0        0     2089 2023-07-03 13:41:07.193539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_destroy.py
--rw-r--r--   0        0        0     3257 2023-07-03 13:41:07.181539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_list.py
--rw-r--r--   0        0        0     2086 2023-07-03 13:41:07.185539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_retrieve.py
--rw-r--r--   0        0        0     2121 2023-07-03 13:41:07.189539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_update.py
--rw-r--r--   0        0        0      781 2023-07-03 13:41:07.193539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_create.py
--rw-r--r--   0        0        0      838 2023-07-03 13:41:07.193539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_destroy.py
--rw-r--r--   0        0        0      780 2023-07-03 13:41:07.193539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_retrieve.py
--rw-r--r--   0        0        0      835 2023-07-03 13:41:07.193539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_retrieve_2.py
--rw-r--r--   0        0        0      835 2023-07-03 13:41:07.193539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_update.py
--rw-r--r--   0        0        0      784 2023-07-03 13:41:07.193539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_create.py
--rw-r--r--   0        0        0      841 2023-07-03 13:41:07.193539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_destroy.py
--rw-r--r--   0        0        0      783 2023-07-03 13:41:07.193539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_retrieve.py
--rw-r--r--   0        0        0      838 2023-07-03 13:41:07.193539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_retrieve_2.py
--rw-r--r--   0        0        0      838 2023-07-03 13:41:07.193539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_update.py
--rw-r--r--   0        0        0      782 2023-07-03 13:41:07.197539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_create.py
--rw-r--r--   0        0        0      839 2023-07-03 13:41:07.197539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_destroy.py
--rw-r--r--   0        0        0      781 2023-07-03 13:41:07.193539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_retrieve.py
--rw-r--r--   0        0        0      836 2023-07-03 13:41:07.197539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_retrieve_2.py
--rw-r--r--   0        0        0      836 2023-07-03 13:41:07.197539 feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_update.py
--rw-r--r--   0        0        0      679 2023-07-03 13:41:07.201539 feedancy_client-0.0.1/feedancy-client/feedancy_client/client.py
--rw-r--r--   0        0        0     1031 2023-07-03 13:46:06.977676 feedancy_client-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1495 1970-01-01 00:00:00.000000 feedancy_client-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      210 2023-07-03 13:41:07.205539 feedancy_client-0.0.5/feedancy-client/MANIFEST.in
+-rw-r--r--   0        0        0      657 2023-07-03 13:41:07.205539 feedancy_client-0.0.5/feedancy-client/README.md
+-rw-r--r--   0        0        0      133 2023-07-03 13:41:07.197539 feedancy_client-0.0.5/feedancy-client/feedancy_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 13:41:07.121537 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 13:41:07.121537 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/__init__.py
+-rw-r--r--   0        0        0    13079 2023-07-03 13:41:07.129537 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api.py
+-rw-r--r--   0        0        0      784 2023-07-03 13:41:07.145538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_create.py
+-rw-r--r--   0        0        0      841 2023-07-03 13:41:07.145538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_destroy.py
+-rw-r--r--   0        0        0      783 2023-07-03 13:41:07.145538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_retrieve.py
+-rw-r--r--   0        0        0      838 2023-07-03 13:41:07.145538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_retrieve_2.py
+-rw-r--r--   0        0        0      838 2023-07-03 13:41:07.145538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_update.py
+-rw-r--r--   0        0        0      774 2023-07-03 13:41:07.145538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_city_create.py
+-rw-r--r--   0        0        0      831 2023-07-03 13:41:07.145538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_city_destroy.py
+-rw-r--r--   0        0        0      773 2023-07-03 13:41:07.145538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_city_retrieve.py
+-rw-r--r--   0        0        0      828 2023-07-03 13:41:07.145538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_city_retrieve_2.py
+-rw-r--r--   0        0        0      828 2023-07-03 13:41:07.145538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_city_update.py
+-rw-r--r--   0        0        0      777 2023-07-03 13:41:07.145538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_company_create.py
+-rw-r--r--   0        0        0      834 2023-07-03 13:41:07.149538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_company_destroy.py
+-rw-r--r--   0        0        0      776 2023-07-03 13:41:07.145538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_company_retrieve.py
+-rw-r--r--   0        0        0      831 2023-07-03 13:41:07.145538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_company_retrieve_2.py
+-rw-r--r--   0        0        0      831 2023-07-03 13:41:07.145538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_company_update.py
+-rw-r--r--   0        0        0      781 2023-07-03 13:41:07.149538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_companycity_create.py
+-rw-r--r--   0        0        0      838 2023-07-03 13:41:07.149538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_companycity_destroy.py
+-rw-r--r--   0        0        0      780 2023-07-03 13:41:07.149538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_companycity_retrieve.py
+-rw-r--r--   0        0        0      835 2023-07-03 13:41:07.149538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_companycity_retrieve_2.py
+-rw-r--r--   0        0        0      835 2023-07-03 13:41:07.149538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_companycity_update.py
+-rw-r--r--   0        0        0      777 2023-07-03 13:41:07.149538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_contact_create.py
+-rw-r--r--   0        0        0      834 2023-07-03 13:41:07.149538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_contact_destroy.py
+-rw-r--r--   0        0        0      776 2023-07-03 13:41:07.149538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_contact_retrieve.py
+-rw-r--r--   0        0        0      831 2023-07-03 13:41:07.149538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_contact_retrieve_2.py
+-rw-r--r--   0        0        0      831 2023-07-03 13:41:07.149538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_contact_update.py
+-rw-r--r--   0        0        0      777 2023-07-03 13:41:07.149538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_country_create.py
+-rw-r--r--   0        0        0      834 2023-07-03 13:41:07.149538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_country_destroy.py
+-rw-r--r--   0        0        0      776 2023-07-03 13:41:07.149538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_country_retrieve.py
+-rw-r--r--   0        0        0      831 2023-07-03 13:41:07.149538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_country_retrieve_2.py
+-rw-r--r--   0        0        0      831 2023-07-03 13:41:07.149538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_country_update.py
+-rw-r--r--   0        0        0      778 2023-07-03 13:41:07.153538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_currency_create.py
+-rw-r--r--   0        0        0      835 2023-07-03 13:41:07.153538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_currency_destroy.py
+-rw-r--r--   0        0        0      777 2023-07-03 13:41:07.153538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_currency_retrieve.py
+-rw-r--r--   0        0        0      832 2023-07-03 13:41:07.153538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_currency_retrieve_2.py
+-rw-r--r--   0        0        0      832 2023-07-03 13:41:07.153538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_currency_update.py
+-rw-r--r--   0        0        0      780 2023-07-03 13:41:07.153538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internship_create.py
+-rw-r--r--   0        0        0     1962 2023-07-03 13:41:07.165538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internship_destroy.py
+-rw-r--r--   0        0        0      779 2023-07-03 13:41:07.153538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internship_retrieve.py
+-rw-r--r--   0        0        0     1959 2023-07-03 13:41:07.157538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internship_retrieve_2.py
+-rw-r--r--   0        0        0     1997 2023-07-03 13:41:07.161538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internship_update.py
+-rw-r--r--   0        0        0      784 2023-07-03 13:41:07.165538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_create.py
+-rw-r--r--   0        0        0      841 2023-07-03 13:41:07.169538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_destroy.py
+-rw-r--r--   0        0        0      783 2023-07-03 13:41:07.165538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_retrieve.py
+-rw-r--r--   0        0        0      838 2023-07-03 13:41:07.165538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_retrieve_2.py
+-rw-r--r--   0        0        0      838 2023-07-03 13:41:07.169538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_update.py
+-rw-r--r--   0        0        0      787 2023-07-03 13:41:07.169538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_create.py
+-rw-r--r--   0        0        0      844 2023-07-03 13:41:07.169538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_destroy.py
+-rw-r--r--   0        0        0      786 2023-07-03 13:41:07.169538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_retrieve.py
+-rw-r--r--   0        0        0      841 2023-07-03 13:41:07.169538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_retrieve_2.py
+-rw-r--r--   0        0        0      841 2023-07-03 13:41:07.169538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_update.py
+-rw-r--r--   0        0        0      785 2023-07-03 13:41:07.169538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_create.py
+-rw-r--r--   0        0        0      842 2023-07-03 13:41:07.169538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_destroy.py
+-rw-r--r--   0        0        0      784 2023-07-03 13:41:07.169538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_retrieve.py
+-rw-r--r--   0        0        0      839 2023-07-03 13:41:07.169538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_retrieve_2.py
+-rw-r--r--   0        0        0      839 2023-07-03 13:41:07.169538 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_update.py
+-rw-r--r--   0        0        0      778 2023-07-03 13:41:07.173539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_create.py
+-rw-r--r--   0        0        0      835 2023-07-03 13:41:07.173539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_destroy.py
+-rw-r--r--   0        0        0      777 2023-07-03 13:41:07.173539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_retrieve.py
+-rw-r--r--   0        0        0      832 2023-07-03 13:41:07.173539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_retrieve_2.py
+-rw-r--r--   0        0        0      832 2023-07-03 13:41:07.173539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_update.py
+-rw-r--r--   0        0        0      776 2023-07-03 13:41:07.173539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_region_create.py
+-rw-r--r--   0        0        0      833 2023-07-03 13:41:07.173539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_region_destroy.py
+-rw-r--r--   0        0        0      775 2023-07-03 13:41:07.173539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_region_retrieve.py
+-rw-r--r--   0        0        0      830 2023-07-03 13:41:07.173539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_region_retrieve_2.py
+-rw-r--r--   0        0        0      830 2023-07-03 13:41:07.173539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_region_update.py
+-rw-r--r--   0        0        0      776 2023-07-03 13:41:07.173539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_salary_create.py
+-rw-r--r--   0        0        0      833 2023-07-03 13:41:07.173539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_salary_destroy.py
+-rw-r--r--   0        0        0      775 2023-07-03 13:41:07.173539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_salary_retrieve.py
+-rw-r--r--   0        0        0      830 2023-07-03 13:41:07.173539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_salary_retrieve_2.py
+-rw-r--r--   0        0        0      830 2023-07-03 13:41:07.173539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_salary_update.py
+-rw-r--r--   0        0        0      791 2023-07-03 13:41:07.177539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_create.py
+-rw-r--r--   0        0        0      848 2023-07-03 13:41:07.177539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_destroy.py
+-rw-r--r--   0        0        0      790 2023-07-03 13:41:07.177539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_retrieve.py
+-rw-r--r--   0        0        0      845 2023-07-03 13:41:07.177539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_retrieve_2.py
+-rw-r--r--   0        0        0      845 2023-07-03 13:41:07.177539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_update.py
+-rw-r--r--   0        0        0      784 2023-07-03 13:41:07.177539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_create.py
+-rw-r--r--   0        0        0      841 2023-07-03 13:41:07.177539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_destroy.py
+-rw-r--r--   0        0        0      783 2023-07-03 13:41:07.177539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_retrieve.py
+-rw-r--r--   0        0        0      838 2023-07-03 13:41:07.177539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_retrieve_2.py
+-rw-r--r--   0        0        0      838 2023-07-03 13:41:07.177539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_update.py
+-rw-r--r--   0        0        0      775 2023-07-03 13:41:07.177539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_skill_create.py
+-rw-r--r--   0        0        0      832 2023-07-03 13:41:07.177539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_skill_destroy.py
+-rw-r--r--   0        0        0      774 2023-07-03 13:41:07.177539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_skill_retrieve.py
+-rw-r--r--   0        0        0      829 2023-07-03 13:41:07.177539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_skill_retrieve_2.py
+-rw-r--r--   0        0        0      829 2023-07-03 13:41:07.177539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_skill_update.py
+-rw-r--r--   0        0        0      776 2023-07-03 13:41:07.177539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_source_create.py
+-rw-r--r--   0        0        0      833 2023-07-03 13:41:07.181539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_source_destroy.py
+-rw-r--r--   0        0        0      775 2023-07-03 13:41:07.177539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_source_retrieve.py
+-rw-r--r--   0        0        0      830 2023-07-03 13:41:07.177539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_source_retrieve_2.py
+-rw-r--r--   0        0        0      830 2023-07-03 13:41:07.181539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_source_update.py
+-rw-r--r--   0        0        0      782 2023-07-03 13:41:07.181539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_create.py
+-rw-r--r--   0        0        0      839 2023-07-03 13:41:07.181539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_destroy.py
+-rw-r--r--   0        0        0      781 2023-07-03 13:41:07.181539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_retrieve.py
+-rw-r--r--   0        0        0      836 2023-07-03 13:41:07.181539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_retrieve_2.py
+-rw-r--r--   0        0        0      836 2023-07-03 13:41:07.181539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_update.py
+-rw-r--r--   0        0        0     2067 2023-07-03 13:41:07.185539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_create.py
+-rw-r--r--   0        0        0     2089 2023-07-03 13:41:07.193539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_destroy.py
+-rw-r--r--   0        0        0     3257 2023-07-03 13:41:07.181539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_list.py
+-rw-r--r--   0        0        0     2086 2023-07-03 13:41:07.185539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_retrieve.py
+-rw-r--r--   0        0        0     2121 2023-07-03 13:41:07.189539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_update.py
+-rw-r--r--   0        0        0      781 2023-07-03 13:41:07.193539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_create.py
+-rw-r--r--   0        0        0      838 2023-07-03 13:41:07.193539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_destroy.py
+-rw-r--r--   0        0        0      780 2023-07-03 13:41:07.193539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_retrieve.py
+-rw-r--r--   0        0        0      835 2023-07-03 13:41:07.193539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_retrieve_2.py
+-rw-r--r--   0        0        0      835 2023-07-03 13:41:07.193539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_update.py
+-rw-r--r--   0        0        0      784 2023-07-03 13:41:07.193539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_create.py
+-rw-r--r--   0        0        0      841 2023-07-03 13:41:07.193539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_destroy.py
+-rw-r--r--   0        0        0      783 2023-07-03 13:41:07.193539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_retrieve.py
+-rw-r--r--   0        0        0      838 2023-07-03 13:41:07.193539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_retrieve_2.py
+-rw-r--r--   0        0        0      838 2023-07-03 13:41:07.193539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_update.py
+-rw-r--r--   0        0        0      782 2023-07-03 13:41:07.197539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_create.py
+-rw-r--r--   0        0        0      839 2023-07-03 13:41:07.197539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_destroy.py
+-rw-r--r--   0        0        0      781 2023-07-03 13:41:07.193539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_retrieve.py
+-rw-r--r--   0        0        0      836 2023-07-03 13:41:07.197539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_retrieve_2.py
+-rw-r--r--   0        0        0      836 2023-07-03 13:41:07.197539 feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_update.py
+-rw-r--r--   0        0        0      679 2023-07-03 13:41:07.201539 feedancy_client-0.0.5/feedancy-client/feedancy_client/client.py
+-rw-r--r--   0        0        0     1014 2023-07-03 13:41:07.205539 feedancy_client-0.0.5/feedancy-client/setup.py
+-rw-r--r--   0        0        0     1015 2023-07-03 13:42:28.607811 feedancy_client-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1495 1970-01-01 00:00:00.000000 feedancy_client-0.0.5/PKG-INFO
```

### Comparing `feedancy_client-0.0.1/feedancy-client/README.md` & `feedancy_client-0.0.5/feedancy-client/README.md`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_create.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_update.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_city_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_city_create.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_city_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_city_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_city_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_city_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_city_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_city_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_city_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_city_update.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_company_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_company_create.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_company_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_company_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_company_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_company_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_company_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_company_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_company_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_company_update.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_companycity_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_companycity_create.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_companycity_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_companycity_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_companycity_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_companycity_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_companycity_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_companycity_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_companycity_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_companycity_update.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_contact_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_contact_create.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_contact_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_contact_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_contact_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_contact_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_contact_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_contact_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_contact_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_contact_update.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_country_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_country_create.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_country_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_country_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_country_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_country_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_country_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_country_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_country_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_country_update.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_currency_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_currency_create.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_currency_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_currency_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_currency_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_currency_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_currency_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_currency_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_currency_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_currency_update.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internship_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internship_create.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internship_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internship_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internship_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internship_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internship_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internship_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internship_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internship_update.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_create.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_update.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_create.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_update.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_create.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_update.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_create.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_update.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_region_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_region_create.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_region_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_region_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_region_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_region_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_region_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_region_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_region_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_region_update.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_salary_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_salary_create.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_salary_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_salary_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_salary_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_salary_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_salary_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_salary_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_salary_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_salary_update.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_create.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_update.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_create.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_update.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_skill_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_skill_create.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_skill_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_skill_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_skill_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_skill_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_skill_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_skill_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_skill_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_skill_update.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_source_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_source_create.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_source_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_source_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_source_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_source_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_source_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_source_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_source_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_source_update.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_create.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_update.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_create.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_list.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_list.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_update.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_create.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_update.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_create.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_update.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_create.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_update.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/feedancy-client/feedancy_client/client.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/client.py`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.1/pyproject.toml` & `feedancy_client-0.0.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -15,25 +15,25 @@
   | build
   | dist
 )/
 '''
 
 [tool.poetry]
 name = "feedancy-client"
-version = "0.0.1"
+version = "0.0.5"
 description = "сервис по сбору вакансий"
 authors = [
     "Alexey Ostanin <aostaninn@gmal.com>",
     "Stanislav Losev <stanislav_losev@protonmail.com>",
     "Tatiana Zimina <tratatatanya@gmail.com>"
 ]
 license = "MIT"
 readme = "./feedancy-client/README.md"
 packages = [
-    { include = './feedancy-client/feedancy_client' }
+    { include = './feedancy-client' }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 djangorestframework = ">=3.14.0"
 #Django = ">=4"
 gunicorn = ">=20.1.0"
```

### Comparing `feedancy_client-0.0.1/PKG-INFO` & `feedancy_client-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedancy-client
-Version: 0.0.1
+Version: 0.0.5
 Summary: сервис по сбору вакансий
 License: MIT
 Author: Alexey Ostanin
 Author-email: aostaninn@gmal.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

