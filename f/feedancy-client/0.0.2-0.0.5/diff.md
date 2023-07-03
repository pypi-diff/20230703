# Comparing `tmp/feedancy_client-0.0.2.tar.gz` & `tmp/feedancy_client-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedancy_client-0.0.2.tar", max compression
+gzip compressed data, was "feedancy_client-0.0.5.tar", max compression
```

## Comparing `feedancy_client-0.0.2.tar` & `feedancy_client-0.0.5.tar`

### file list

```diff
@@ -1,167 +1,125 @@
--rw-r--r--   0        0        0      657 2023-07-03 14:15:11.864272 feedancy_client-0.0.2/feedancy-client/README.md
--rw-r--r--   0        0        0      133 2023-07-03 14:15:11.856272 feedancy_client-0.0.2/feedancy-client/feedancy_client/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.856272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.776270 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/activitysphere/__init__.py
--rw-r--r--   0        0        0      910 2023-07-03 14:15:11.792271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/activitysphere/activitysphere_create.py
--rw-r--r--   0        0        0      834 2023-07-03 14:15:11.792271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/activitysphere/activitysphere_destroy.py
--rw-r--r--   0        0        0      867 2023-07-03 14:15:11.792271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/activitysphere/activitysphere_retrieve.py
--rw-r--r--   0        0        0      922 2023-07-03 14:15:11.792271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/activitysphere/activitysphere_retrieve_2.py
--rw-r--r--   0        0        0      964 2023-07-03 14:15:11.792271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/activitysphere/activitysphere_update.py
--rw-r--r--   0        0        0      631 2023-07-03 14:15:11.780270 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/activitysphere/api.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.792271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/city/__init__.py
--rw-r--r--   0        0        0      471 2023-07-03 14:15:11.792271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/city/api.py
--rw-r--r--   0        0        0      877 2023-07-03 14:15:11.796271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/city/city_create.py
--rw-r--r--   0        0        0      824 2023-07-03 14:15:11.796271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/city/city_destroy.py
--rw-r--r--   0        0        0      844 2023-07-03 14:15:11.792271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/city/city_retrieve.py
--rw-r--r--   0        0        0      899 2023-07-03 14:15:11.796271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/city/city_retrieve_2.py
--rw-r--r--   0        0        0      931 2023-07-03 14:15:11.796271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/city/city_update.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.796271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/company/__init__.py
--rw-r--r--   0        0        0      519 2023-07-03 14:15:11.796271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/company/api.py
--rw-r--r--   0        0        0     1272 2023-07-03 14:15:11.796271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/company/company_create.py
--rw-r--r--   0        0        0      827 2023-07-03 14:15:11.800271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/company/company_destroy.py
--rw-r--r--   0        0        0     1236 2023-07-03 14:15:11.796271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/company/company_retrieve.py
--rw-r--r--   0        0        0     1291 2023-07-03 14:15:11.796271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/company/company_retrieve_2.py
--rw-r--r--   0        0        0     1326 2023-07-03 14:15:11.800271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/company/company_update.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.800271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/companycity/__init__.py
--rw-r--r--   0        0        0      583 2023-07-03 14:15:11.800271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/companycity/api.py
--rw-r--r--   0        0        0      913 2023-07-03 14:15:11.800271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/companycity/companycity_create.py
--rw-r--r--   0        0        0      831 2023-07-03 14:15:11.800271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/companycity/companycity_destroy.py
--rw-r--r--   0        0        0      873 2023-07-03 14:15:11.800271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/companycity/companycity_retrieve.py
--rw-r--r--   0        0        0      928 2023-07-03 14:15:11.800271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/companycity/companycity_retrieve_2.py
--rw-r--r--   0        0        0      967 2023-07-03 14:15:11.800271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/companycity/companycity_update.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.800271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/contact/__init__.py
--rw-r--r--   0        0        0      519 2023-07-03 14:15:11.800271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/contact/api.py
--rw-r--r--   0        0        0      949 2023-07-03 14:15:11.800271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/contact/contact_create.py
--rw-r--r--   0        0        0      827 2023-07-03 14:15:11.804271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/contact/contact_destroy.py
--rw-r--r--   0        0        0      913 2023-07-03 14:15:11.800271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/contact/contact_retrieve.py
--rw-r--r--   0        0        0      968 2023-07-03 14:15:11.804271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/contact/contact_retrieve_2.py
--rw-r--r--   0        0        0     1003 2023-07-03 14:15:11.804271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/contact/contact_update.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.804271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/country/__init__.py
--rw-r--r--   0        0        0      519 2023-07-03 14:15:11.804271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/country/api.py
--rw-r--r--   0        0        0      890 2023-07-03 14:15:11.804271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/country/country_create.py
--rw-r--r--   0        0        0      827 2023-07-03 14:15:11.804271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/country/country_destroy.py
--rw-r--r--   0        0        0      854 2023-07-03 14:15:11.804271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/country/country_retrieve.py
--rw-r--r--   0        0        0      909 2023-07-03 14:15:11.804271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/country/country_retrieve_2.py
--rw-r--r--   0        0        0      944 2023-07-03 14:15:11.804271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/country/country_update.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.804271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/currency/__init__.py
--rw-r--r--   0        0        0      535 2023-07-03 14:15:11.804271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/currency/api.py
--rw-r--r--   0        0        0      895 2023-07-03 14:15:11.804271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/currency/currency_create.py
--rw-r--r--   0        0        0      828 2023-07-03 14:15:11.808271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/currency/currency_destroy.py
--rw-r--r--   0        0        0      858 2023-07-03 14:15:11.804271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/currency/currency_retrieve.py
--rw-r--r--   0        0        0      913 2023-07-03 14:15:11.808271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/currency/currency_retrieve_2.py
--rw-r--r--   0        0        0      949 2023-07-03 14:15:11.808271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/currency/currency_update.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.808271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internship/__init__.py
--rw-r--r--   0        0        0      567 2023-07-03 14:15:11.808271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internship/api.py
--rw-r--r--   0        0        0     1936 2023-07-03 14:15:11.808271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internship/internship_create.py
--rw-r--r--   0        0        0     1955 2023-07-03 14:15:11.812271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internship/internship_destroy.py
--rw-r--r--   0        0        0     1897 2023-07-03 14:15:11.808271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internship/internship_retrieve.py
--rw-r--r--   0        0        0     1952 2023-07-03 14:15:11.812271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internship/internship_retrieve_2.py
--rw-r--r--   0        0        0     1990 2023-07-03 14:15:11.812271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internship/internship_update.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.812271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipcity/__init__.py
--rw-r--r--   0        0        0      631 2023-07-03 14:15:11.812271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipcity/api.py
--rw-r--r--   0        0        0      931 2023-07-03 14:15:11.816271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipcity/internshipcity_create.py
--rw-r--r--   0        0        0      834 2023-07-03 14:15:11.816271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipcity/internshipcity_destroy.py
--rw-r--r--   0        0        0      888 2023-07-03 14:15:11.816271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipcity/internshipcity_retrieve.py
--rw-r--r--   0        0        0      943 2023-07-03 14:15:11.816271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipcity/internshipcity_retrieve_2.py
--rw-r--r--   0        0        0      985 2023-07-03 14:15:11.816271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipcity/internshipcity_update.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.816271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipcontact/__init__.py
--rw-r--r--   0        0        0      679 2023-07-03 14:15:11.816271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipcontact/api.py
--rw-r--r--   0        0        0      949 2023-07-03 14:15:11.816271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipcontact/internshipcontact_create.py
--rw-r--r--   0        0        0      837 2023-07-03 14:15:11.816271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipcontact/internshipcontact_destroy.py
--rw-r--r--   0        0        0      903 2023-07-03 14:15:11.816271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipcontact/internshipcontact_retrieve.py
--rw-r--r--   0        0        0      958 2023-07-03 14:15:11.816271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipcontact/internshipcontact_retrieve_2.py
--rw-r--r--   0        0        0     1003 2023-07-03 14:15:11.816271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipcontact/internshipcontact_update.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.816271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipskill/__init__.py
--rw-r--r--   0        0        0      647 2023-07-03 14:15:11.820271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipskill/api.py
--rw-r--r--   0        0        0      937 2023-07-03 14:15:11.820271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipskill/internshipskill_create.py
--rw-r--r--   0        0        0      835 2023-07-03 14:15:11.820271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipskill/internshipskill_destroy.py
--rw-r--r--   0        0        0      893 2023-07-03 14:15:11.820271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipskill/internshipskill_retrieve.py
--rw-r--r--   0        0        0      948 2023-07-03 14:15:11.820271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipskill/internshipskill_retrieve_2.py
--rw-r--r--   0        0        0      991 2023-07-03 14:15:11.820271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipskill/internshipskill_update.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.820271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/jobmixin/__init__.py
--rw-r--r--   0        0        0      535 2023-07-03 14:15:11.820271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/jobmixin/api.py
--rw-r--r--   0        0        0     1641 2023-07-03 14:15:11.824271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/jobmixin/jobmixin_create.py
--rw-r--r--   0        0        0      828 2023-07-03 14:15:11.824271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/jobmixin/jobmixin_destroy.py
--rw-r--r--   0        0        0     1604 2023-07-03 14:15:11.820271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/jobmixin/jobmixin_retrieve.py
--rw-r--r--   0        0        0     1659 2023-07-03 14:15:11.824271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/jobmixin/jobmixin_retrieve_2.py
--rw-r--r--   0        0        0     1695 2023-07-03 14:15:11.824271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/jobmixin/jobmixin_update.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.824271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/region/__init__.py
--rw-r--r--   0        0        0      503 2023-07-03 14:15:11.824271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/region/api.py
--rw-r--r--   0        0        0      888 2023-07-03 14:15:11.828271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/region/region_create.py
--rw-r--r--   0        0        0      826 2023-07-03 14:15:11.828271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/region/region_destroy.py
--rw-r--r--   0        0        0      853 2023-07-03 14:15:11.828271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/region/region_retrieve.py
--rw-r--r--   0        0        0      908 2023-07-03 14:15:11.828271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/region/region_retrieve_2.py
--rw-r--r--   0        0        0      942 2023-07-03 14:15:11.828271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/region/region_update.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.828271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/salary/__init__.py
--rw-r--r--   0        0        0      503 2023-07-03 14:15:11.828271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/salary/api.py
--rw-r--r--   0        0        0     1002 2023-07-03 14:15:11.828271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/salary/salary_create.py
--rw-r--r--   0        0        0      826 2023-07-03 14:15:11.832272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/salary/salary_destroy.py
--rw-r--r--   0        0        0      967 2023-07-03 14:15:11.828271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/salary/salary_retrieve.py
--rw-r--r--   0        0        0     1022 2023-07-03 14:15:11.828271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/salary/salary_retrieve_2.py
--rw-r--r--   0        0        0     1056 2023-07-03 14:15:11.828271 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/salary/salary_update.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.832272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchandstopkeywords/__init__.py
--rw-r--r--   0        0        0      743 2023-07-03 14:15:11.832272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchandstopkeywords/api.py
--rw-r--r--   0        0        0      980 2023-07-03 14:15:11.832272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchandstopkeywords/searchandstopkeywords_create.py
--rw-r--r--   0        0        0      841 2023-07-03 14:15:11.832272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchandstopkeywords/searchandstopkeywords_destroy.py
--rw-r--r--   0        0        0      930 2023-07-03 14:15:11.832272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchandstopkeywords/searchandstopkeywords_retrieve.py
--rw-r--r--   0        0        0      985 2023-07-03 14:15:11.832272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchandstopkeywords/searchandstopkeywords_retrieve_2.py
--rw-r--r--   0        0        0     1034 2023-07-03 14:15:11.832272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchandstopkeywords/searchandstopkeywords_update.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.832272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchkeywords/__init__.py
--rw-r--r--   0        0        0      631 2023-07-03 14:15:11.832272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchkeywords/api.py
--rw-r--r--   0        0        0      910 2023-07-03 14:15:11.832272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchkeywords/searchkeywords_create.py
--rw-r--r--   0        0        0      834 2023-07-03 14:15:11.832272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchkeywords/searchkeywords_destroy.py
--rw-r--r--   0        0        0      904 2023-07-03 14:15:11.832272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchkeywords/searchkeywords_retrieve.py
--rw-r--r--   0        0        0      959 2023-07-03 14:15:11.832272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchkeywords/searchkeywords_retrieve_2.py
--rw-r--r--   0        0        0      964 2023-07-03 14:15:11.832272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchkeywords/searchkeywords_update.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.832272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/skill/__init__.py
--rw-r--r--   0        0        0      487 2023-07-03 14:15:11.836272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/skill/api.py
--rw-r--r--   0        0        0      865 2023-07-03 14:15:11.836272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/skill/skill_create.py
--rw-r--r--   0        0        0      825 2023-07-03 14:15:11.836272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/skill/skill_destroy.py
--rw-r--r--   0        0        0      831 2023-07-03 14:15:11.836272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/skill/skill_retrieve.py
--rw-r--r--   0        0        0      886 2023-07-03 14:15:11.836272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/skill/skill_retrieve_2.py
--rw-r--r--   0        0        0      919 2023-07-03 14:15:11.836272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/skill/skill_update.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.836272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/source/__init__.py
--rw-r--r--   0        0        0      503 2023-07-03 14:15:11.836272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/source/api.py
--rw-r--r--   0        0        0      870 2023-07-03 14:15:11.840272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/source/source_create.py
--rw-r--r--   0        0        0      826 2023-07-03 14:15:11.840272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/source/source_destroy.py
--rw-r--r--   0        0        0      835 2023-07-03 14:15:11.840272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/source/source_retrieve.py
--rw-r--r--   0        0        0      890 2023-07-03 14:15:11.840272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/source/source_retrieve_2.py
--rw-r--r--   0        0        0      924 2023-07-03 14:15:11.840272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/source/source_update.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.840272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/stopkeywords/__init__.py
--rw-r--r--   0        0        0      599 2023-07-03 14:15:11.840272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/stopkeywords/api.py
--rw-r--r--   0        0        0      900 2023-07-03 14:15:11.840272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/stopkeywords/stopkeywords_create.py
--rw-r--r--   0        0        0      832 2023-07-03 14:15:11.844272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/stopkeywords/stopkeywords_destroy.py
--rw-r--r--   0        0        0      859 2023-07-03 14:15:11.840272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/stopkeywords/stopkeywords_retrieve.py
--rw-r--r--   0        0        0      914 2023-07-03 14:15:11.840272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/stopkeywords/stopkeywords_retrieve_2.py
--rw-r--r--   0        0        0      954 2023-07-03 14:15:11.844272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/stopkeywords/stopkeywords_update.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.844272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancy/__init__.py
--rw-r--r--   0        0        0      501 2023-07-03 14:15:11.844272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancy/api.py
--rw-r--r--   0        0        0     2060 2023-07-03 14:15:11.848272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancy/vacancy_create.py
--rw-r--r--   0        0        0     2082 2023-07-03 14:15:11.852272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancy/vacancy_destroy.py
--rw-r--r--   0        0        0     3250 2023-07-03 14:15:11.844272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancy/vacancy_list.py
--rw-r--r--   0        0        0     2079 2023-07-03 14:15:11.848272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancy/vacancy_retrieve.py
--rw-r--r--   0        0        0     2114 2023-07-03 14:15:11.848272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancy/vacancy_update.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.852272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancycity/__init__.py
--rw-r--r--   0        0        0      583 2023-07-03 14:15:11.852272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancycity/api.py
--rw-r--r--   0        0        0      913 2023-07-03 14:15:11.852272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancycity/vacancycity_create.py
--rw-r--r--   0        0        0      831 2023-07-03 14:15:11.852272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancycity/vacancycity_destroy.py
--rw-r--r--   0        0        0      873 2023-07-03 14:15:11.852272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancycity/vacancycity_retrieve.py
--rw-r--r--   0        0        0      928 2023-07-03 14:15:11.852272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancycity/vacancycity_retrieve_2.py
--rw-r--r--   0        0        0      967 2023-07-03 14:15:11.852272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancycity/vacancycity_update.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.852272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancycontact/__init__.py
--rw-r--r--   0        0        0      631 2023-07-03 14:15:11.852272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancycontact/api.py
--rw-r--r--   0        0        0      931 2023-07-03 14:15:11.852272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancycontact/vacancycontact_create.py
--rw-r--r--   0        0        0      834 2023-07-03 14:15:11.856272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancycontact/vacancycontact_destroy.py
--rw-r--r--   0        0        0      888 2023-07-03 14:15:11.852272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancycontact/vacancycontact_retrieve.py
--rw-r--r--   0        0        0      943 2023-07-03 14:15:11.852272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancycontact/vacancycontact_retrieve_2.py
--rw-r--r--   0        0        0      985 2023-07-03 14:15:11.852272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancycontact/vacancycontact_update.py
--rw-r--r--   0        0        0        0 2023-07-03 14:15:11.856272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancyskill/__init__.py
--rw-r--r--   0        0        0      599 2023-07-03 14:15:11.856272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancyskill/api.py
--rw-r--r--   0        0        0      919 2023-07-03 14:15:11.856272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancyskill/vacancyskill_create.py
--rw-r--r--   0        0        0      832 2023-07-03 14:15:11.856272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancyskill/vacancyskill_destroy.py
--rw-r--r--   0        0        0      878 2023-07-03 14:15:11.856272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancyskill/vacancyskill_retrieve.py
--rw-r--r--   0        0        0      933 2023-07-03 14:15:11.856272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancyskill/vacancyskill_retrieve_2.py
--rw-r--r--   0        0        0      973 2023-07-03 14:15:11.856272 feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancyskill/vacancyskill_update.py
--rw-r--r--   0        0        0     3925 2023-07-03 14:15:11.860272 feedancy_client-0.0.2/feedancy-client/feedancy_client/client.py
--rw-r--r--   0        0        0     1057 2023-07-03 14:14:38.067469 feedancy_client-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1268 1970-01-01 00:00:00.000000 feedancy_client-0.0.2/PKG-INFO
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

### Comparing `feedancy_client-0.0.2/feedancy-client/README.md` & `feedancy_client-0.0.5/feedancy-client/README.md`

 * *Files identical despite different names*

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/activitysphere/activitysphere_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_create.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,45 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class ActivitySphere(BaseModel):
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: ActivitySphere,
-
 
-) -> ActivitySphere:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="POST",
-        path="/activitysphere/".format(
+        path="/api/v1/internshipcontact/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": ActivitySphere,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/activitysphere/activitysphere_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_skill_destroy.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     
     body = None
     
 
     m = ApiRequest(
         method="DELETE",
-        path="/activitysphere/{id}/".format(
+        path="/api/v1/skill/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/activitysphere/activitysphere_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_retrieve.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,31 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class ActivitySphere(BaseModel):
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
-) -> ActivitySphere:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/activitysphere/".format(
+        path="/api/v1/activitysphere/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -37,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": ActivitySphere,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/activitysphere/activitysphere_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_destroy.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,33 +5,29 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class ActivitySphere(BaseModel):
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> ActivitySphere:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/activitysphere/{id}/".format(
+        method="DELETE",
+        path="/api/v1/activitysphere/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -39,14 +35,14 @@
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "200": {
+        "204": {
             
-                "application/json": ActivitySphere,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/activitysphere/activitysphere_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_retrieve_2.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,49 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class ActivitySphere(BaseModel):
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: ActivitySphere,
-
 
     id: str,
 
-) -> ActivitySphere:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/activitysphere/{id}/".format(
+        method="GET",
+        path="/api/v1/searchkeywords/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": ActivitySphere,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/city/city_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_salary_create.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,46 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class City(BaseModel):
-    name: str 
-    region: int 
-
 def make_request(self: BaseApi,
 
-    __request__: City,
-
 
-) -> City:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="POST",
-        path="/city/".format(
+        path="/api/v1/salary/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": City,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/city/city_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_retrieve.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,41 +8,37 @@
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
 def make_request(self: BaseApi,
 
 
-    id: str,
-
 ) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="DELETE",
-        path="/city/{id}/".format(
-            
-                id=id,
+        method="GET",
+        path="/api/v1/vacancycity/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "204": {
+        "200": {
             
                 "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/city/city_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_retrieve_2.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class City(BaseModel):
-    id: int 
-    name: str 
-    region: int 
-
 def make_request(self: BaseApi,
 
 
-) -> City:
+    id: str,
+
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/city/".format(
+        path="/api/v1/jobmixin/{id}/".format(
+            
+                id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": City,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/city/city_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_skill_create.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,36 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class City(BaseModel):
-    id: int 
-    name: str 
-    region: int 
-
 def make_request(self: BaseApi,
 
 
-    id: str,
-
-) -> City:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/city/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/skill/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -42,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": City,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/city/city_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_destroy.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,50 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class City(BaseModel):
-    name: str 
-    region: int 
-
 def make_request(self: BaseApi,
 
-    __request__: City,
-
 
     id: str,
 
-) -> City:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/city/{id}/".format(
+        method="DELETE",
+        path="/api/v1/jobmixin/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "200": {
+        "204": {
             
-                "application/json": City,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/company/company_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internship_update.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,38 +5,53 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Company(BaseModel):
-    description: typing.Optional[typing.Union[str, None]]  = None
-    is_accredited: typing.Optional[typing.Union[bool, None]]  = None
-    link: typing.Optional[typing.Union[str, None]]  = None
-    logo: typing.Optional[typing.Union[str, None]]  = None
+class Internship(BaseModel):
+    company: typing.Optional[typing.Union[int, None]]  = None
+    duration: typing.Optional[typing.Union[int, None]]  = None
+    external_id: str 
+    has_employment: typing.Optional[typing.Union[bool, None]]  = None
+    has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
+    has_test_task: typing.Optional[typing.Union[bool, None]]  = None
+    is_paid: typing.Optional[typing.Union[bool, None]]  = None
+    link: str 
     name: str 
-    size: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
-    sphere: typing.Optional[typing.Union[int, None]]  = None
+    publicated_at: typing.Optional[typing.Union[datetime.datetime, None]]  = None
+    raw_description: typing.Optional[typing.Union[str, None]]  = None
+    recruitment_end_date: typing.Optional[typing.Union[datetime.datetime, None]]  = None
+    requirement: typing.Optional[typing.Union[str, None]]  = None
+    responsibility: typing.Optional[typing.Union[str, None]]  = None
+    salary: typing.Optional[typing.Union[int, None]]  = None
+    source: int 
+    test_task_link: typing.Optional[typing.Union[str, None]]  = None
+    work_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
 
 def make_request(self: BaseApi,
 
-    __request__: Company,
+    __request__: Internship,
 
 
-) -> Company:
+    id: str,
+
+) -> Internship:
     
 
     
     body = __request__
     
 
     m = ApiRequest(
-        method="POST",
-        path="/company/".format(
+        method="PUT",
+        path="/api/v1/internship/{id}/".format(
+            
+                id=id,
             
         ),
         content_type="application/json",
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -44,12 +59,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Company,
+                "application/json": Internship,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/company/company_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_create.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,41 +8,37 @@
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
 def make_request(self: BaseApi,
 
 
-    id: str,
-
 ) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="DELETE",
-        path="/company/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/vacancycity/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "204": {
+        "200": {
             
                 "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/company/company_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internship_retrieve_2.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,37 +5,52 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Company(BaseModel):
-    description: typing.Optional[typing.Union[str, None]]  = None
+class Internship(BaseModel):
+    company: typing.Optional[typing.Union[int, None]]  = None
+    duration: typing.Optional[typing.Union[int, None]]  = None
+    external_id: str 
+    has_employment: typing.Optional[typing.Union[bool, None]]  = None
+    has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
+    has_test_task: typing.Optional[typing.Union[bool, None]]  = None
     id: int 
-    is_accredited: typing.Optional[typing.Union[bool, None]]  = None
-    link: typing.Optional[typing.Union[str, None]]  = None
-    logo: typing.Optional[typing.Union[str, None]]  = None
+    is_paid: typing.Optional[typing.Union[bool, None]]  = None
+    link: str 
     name: str 
-    size: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
-    sphere: typing.Optional[typing.Union[int, None]]  = None
+    publicated_at: typing.Optional[typing.Union[datetime.datetime, None]]  = None
+    raw_description: typing.Optional[typing.Union[str, None]]  = None
+    recruitment_end_date: typing.Optional[typing.Union[datetime.datetime, None]]  = None
+    requirement: typing.Optional[typing.Union[str, None]]  = None
+    responsibility: typing.Optional[typing.Union[str, None]]  = None
+    salary: typing.Optional[typing.Union[int, None]]  = None
+    source: int 
+    test_task_link: typing.Optional[typing.Union[str, None]]  = None
+    work_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
 
 def make_request(self: BaseApi,
 
 
-) -> Company:
+    id: str,
+
+) -> Internship:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/company/".format(
+        path="/api/v1/internship/{id}/".format(
+            
+                id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -43,12 +58,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Company,
+                "application/json": Internship,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/company/company_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internship_destroy.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,39 +5,50 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Company(BaseModel):
-    description: typing.Optional[typing.Union[str, None]]  = None
+class Internship(BaseModel):
+    company: typing.Optional[typing.Union[int, None]]  = None
+    duration: typing.Optional[typing.Union[int, None]]  = None
+    external_id: str 
+    has_employment: typing.Optional[typing.Union[bool, None]]  = None
+    has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
+    has_test_task: typing.Optional[typing.Union[bool, None]]  = None
     id: int 
-    is_accredited: typing.Optional[typing.Union[bool, None]]  = None
-    link: typing.Optional[typing.Union[str, None]]  = None
-    logo: typing.Optional[typing.Union[str, None]]  = None
+    is_paid: typing.Optional[typing.Union[bool, None]]  = None
+    link: str 
     name: str 
-    size: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
-    sphere: typing.Optional[typing.Union[int, None]]  = None
+    publicated_at: typing.Optional[typing.Union[datetime.datetime, None]]  = None
+    raw_description: typing.Optional[typing.Union[str, None]]  = None
+    recruitment_end_date: typing.Optional[typing.Union[datetime.datetime, None]]  = None
+    requirement: typing.Optional[typing.Union[str, None]]  = None
+    responsibility: typing.Optional[typing.Union[str, None]]  = None
+    salary: typing.Optional[typing.Union[int, None]]  = None
+    source: int 
+    test_task_link: typing.Optional[typing.Union[str, None]]  = None
+    work_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
 
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> Company:
+) -> Internship:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/company/{id}/".format(
+        method="DELETE",
+        path="/api/v1/internship/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -47,12 +58,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Company,
+                "application/json": Internship,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/company/company_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_create.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,55 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Company(BaseModel):
-    description: typing.Optional[typing.Union[str, None]]  = None
-    is_accredited: typing.Optional[typing.Union[bool, None]]  = None
-    link: typing.Optional[typing.Union[str, None]]  = None
-    logo: typing.Optional[typing.Union[str, None]]  = None
-    name: str 
-    size: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
-    sphere: typing.Optional[typing.Union[int, None]]  = None
-
 def make_request(self: BaseApi,
 
-    __request__: Company,
-
 
-    id: str,
-
-) -> Company:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/company/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/jobmixin/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Company,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/companycity/companycity_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_retrieve.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,46 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class CompanyCity(BaseModel):
-    city: int 
-    company: int 
-
 def make_request(self: BaseApi,
 
-    __request__: CompanyCity,
-
 
-) -> CompanyCity:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/companycity/".format(
+        method="GET",
+        path="/api/v1/jobmixin/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": CompanyCity,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/companycity/companycity_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_create.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,41 +8,37 @@
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
 def make_request(self: BaseApi,
 
 
-    id: str,
-
 ) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="DELETE",
-        path="/companycity/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/searchandstopkeywords/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "204": {
+        "200": {
             
                 "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/companycity/companycity_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_company_destroy.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,45 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class CompanyCity(BaseModel):
-    city: int 
-    company: int 
-    id: int 
-
 def make_request(self: BaseApi,
 
 
-) -> CompanyCity:
+    id: str,
+
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/companycity/".format(
+        method="DELETE",
+        path="/api/v1/company/{id}/".format(
+            
+                id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "200": {
+        "204": {
             
-                "application/json": CompanyCity,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/companycity/companycity_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_companycity_retrieve_2.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,34 +5,29 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class CompanyCity(BaseModel):
-    city: int 
-    company: int 
-    id: int 
-
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> CompanyCity:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/companycity/{id}/".format(
+        path="/api/v1/companycity/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -42,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": CompanyCity,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/companycity/companycity_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_skill_retrieve_2.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,50 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class CompanyCity(BaseModel):
-    city: int 
-    company: int 
-
 def make_request(self: BaseApi,
 
-    __request__: CompanyCity,
-
 
     id: str,
 
-) -> CompanyCity:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/companycity/{id}/".format(
+        method="GET",
+        path="/api/v1/skill/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": CompanyCity,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/contact/contact_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_companycity_destroy.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,47 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Contact(BaseModel):
-    data: str 
-    name: typing.Optional[typing.Union[str, None]]  = None
-    type: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Contact,
 
+    id: str,
 
-) -> Contact:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/contact/".format(
+        method="DELETE",
+        path="/api/v1/companycity/{id}/".format(
+            
+                id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "200": {
+        "204": {
             
-                "application/json": Contact,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/contact/contact_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_retrieve.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,41 +8,37 @@
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
 def make_request(self: BaseApi,
 
 
-    id: str,
-
 ) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="DELETE",
-        path="/contact/{id}/".format(
-            
-                id=id,
+        method="GET",
+        path="/api/v1/internshipcontact/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "204": {
+        "200": {
             
                 "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/contact/contact_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_destroy.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,46 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Contact(BaseModel):
-    data: str 
-    id: int 
-    name: typing.Optional[typing.Union[str, None]]  = None
-    type: str 
-
 def make_request(self: BaseApi,
 
 
-) -> Contact:
+    id: str,
+
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/contact/".format(
+        method="DELETE",
+        path="/api/v1/searchkeywords/{id}/".format(
+            
+                id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "200": {
+        "204": {
             
-                "application/json": Contact,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/contact/contact_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_destroy.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,35 +5,29 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Contact(BaseModel):
-    data: str 
-    id: int 
-    name: typing.Optional[typing.Union[str, None]]  = None
-    type: str 
-
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> Contact:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/contact/{id}/".format(
+        method="DELETE",
+        path="/api/v1/searchandstopkeywords/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -41,14 +35,14 @@
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "200": {
+        "204": {
             
-                "application/json": Contact,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/contact/contact_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_destroy.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,51 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Contact(BaseModel):
-    data: str 
-    name: typing.Optional[typing.Union[str, None]]  = None
-    type: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Contact,
-
 
     id: str,
 
-) -> Contact:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/contact/{id}/".format(
+        method="DELETE",
+        path="/api/v1/internshipcity/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "200": {
+        "204": {
             
-                "application/json": Contact,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/country/country_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_retrieve_2.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,46 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Country(BaseModel):
-    code: str 
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Country,
 
+    id: str,
 
-) -> Country:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/country/".format(
+        method="GET",
+        path="/api/v1/stopkeywords/{id}/".format(
+            
+                id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Country,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/country/country_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_destroy.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     
     body = None
     
 
     m = ApiRequest(
         method="DELETE",
-        path="/country/{id}/".format(
+        path="/api/v1/stopkeywords/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/country/country_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_region_retrieve_2.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Country(BaseModel):
-    code: str 
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
-) -> Country:
+    id: str,
+
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/country/".format(
+        path="/api/v1/region/{id}/".format(
+            
+                id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Country,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/country/country_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_retrieve_2.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,34 +5,29 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Country(BaseModel):
-    code: str 
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> Country:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/country/{id}/".format(
+        path="/api/v1/activitysphere/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -42,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Country,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/country/country_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_region_create.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,50 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Country(BaseModel):
-    code: str 
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Country,
-
 
-    id: str,
-
-) -> Country:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/country/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/region/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Country,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/currency/currency_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_retrieve_2.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,46 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Currency(BaseModel):
-    code: str 
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Currency,
 
+    id: str,
 
-) -> Currency:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/currency/".format(
+        method="GET",
+        path="/api/v1/vacancycity/{id}/".format(
+            
+                id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Currency,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/currency/currency_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_retrieve.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,41 +8,37 @@
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
 def make_request(self: BaseApi,
 
 
-    id: str,
-
 ) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="DELETE",
-        path="/currency/{id}/".format(
-            
-                id=id,
+        method="GET",
+        path="/api/v1/internshipcity/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "204": {
+        "200": {
             
                 "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/currency/currency_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_currency_retrieve_2.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,34 +5,29 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Currency(BaseModel):
-    code: str 
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> Currency:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/currency/{id}/".format(
+        path="/api/v1/currency/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -42,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Currency,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/currency/currency_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_region_destroy.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,50 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Currency(BaseModel):
-    code: str 
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Currency,
-
 
     id: str,
 
-) -> Currency:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/currency/{id}/".format(
+        method="DELETE",
+        path="/api/v1/region/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "200": {
+        "204": {
             
-                "application/json": Currency,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internship/internship_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_retrieve.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,62 +5,66 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Internship(BaseModel):
+class Vacancy(BaseModel):
     company: typing.Optional[typing.Union[int, None]]  = None
-    duration: typing.Optional[typing.Union[int, None]]  = None
+    contract_type: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
+    employment_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
+    experience: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     external_id: str 
-    has_employment: typing.Optional[typing.Union[bool, None]]  = None
+    has_insurance: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
-    is_paid: typing.Optional[typing.Union[bool, None]]  = None
+    id: int 
+    is_relocation_required: typing.Optional[typing.Union[bool, None]]  = None
     link: str 
     name: str 
     publicated_at: typing.Optional[typing.Union[datetime.datetime, None]]  = None
     raw_description: typing.Optional[typing.Union[str, None]]  = None
-    recruitment_end_date: typing.Optional[typing.Union[datetime.datetime, None]]  = None
     requirement: typing.Optional[typing.Union[str, None]]  = None
     responsibility: typing.Optional[typing.Union[str, None]]  = None
     salary: typing.Optional[typing.Union[int, None]]  = None
     source: int 
     test_task_link: typing.Optional[typing.Union[str, None]]  = None
     work_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
 
 def make_request(self: BaseApi,
 
-    __request__: Internship,
 
+    id: str,
 
-) -> Internship:
+) -> Vacancy:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/internship/".format(
+        method="GET",
+        path="/api/v1/vacancy/{id}/".format(
+            
+                id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Internship,
+                "application/json": Vacancy,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internship/internship_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_create.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,65 +5,63 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Internship(BaseModel):
+class Vacancy(BaseModel):
     company: typing.Optional[typing.Union[int, None]]  = None
-    duration: typing.Optional[typing.Union[int, None]]  = None
+    contract_type: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
+    employment_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
+    experience: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     external_id: str 
-    has_employment: typing.Optional[typing.Union[bool, None]]  = None
+    has_insurance: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
-    id: int 
-    is_paid: typing.Optional[typing.Union[bool, None]]  = None
+    is_relocation_required: typing.Optional[typing.Union[bool, None]]  = None
     link: str 
     name: str 
     publicated_at: typing.Optional[typing.Union[datetime.datetime, None]]  = None
     raw_description: typing.Optional[typing.Union[str, None]]  = None
-    recruitment_end_date: typing.Optional[typing.Union[datetime.datetime, None]]  = None
     requirement: typing.Optional[typing.Union[str, None]]  = None
     responsibility: typing.Optional[typing.Union[str, None]]  = None
     salary: typing.Optional[typing.Union[int, None]]  = None
     source: int 
     test_task_link: typing.Optional[typing.Union[str, None]]  = None
     work_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
 
 def make_request(self: BaseApi,
 
+    __request__: Vacancy,
 
-    id: str,
 
-) -> Internship:
+) -> Vacancy:
     
 
     
-    body = None
+    body = __request__
     
 
     m = ApiRequest(
-        method="DELETE",
-        path="/internship/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/vacancy/".format(
             
         ),
-        content_type=None,
+        content_type="application/json",
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Internship,
+                "application/json": Vacancy,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internship/internship_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_destroy.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,48 +5,53 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Internship(BaseModel):
+class Vacancy(BaseModel):
     company: typing.Optional[typing.Union[int, None]]  = None
-    duration: typing.Optional[typing.Union[int, None]]  = None
+    contract_type: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
+    employment_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
+    experience: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     external_id: str 
-    has_employment: typing.Optional[typing.Union[bool, None]]  = None
+    has_insurance: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
     id: int 
-    is_paid: typing.Optional[typing.Union[bool, None]]  = None
+    is_relocation_required: typing.Optional[typing.Union[bool, None]]  = None
     link: str 
     name: str 
     publicated_at: typing.Optional[typing.Union[datetime.datetime, None]]  = None
     raw_description: typing.Optional[typing.Union[str, None]]  = None
-    recruitment_end_date: typing.Optional[typing.Union[datetime.datetime, None]]  = None
     requirement: typing.Optional[typing.Union[str, None]]  = None
     responsibility: typing.Optional[typing.Union[str, None]]  = None
     salary: typing.Optional[typing.Union[int, None]]  = None
     source: int 
     test_task_link: typing.Optional[typing.Union[str, None]]  = None
     work_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
 
 def make_request(self: BaseApi,
 
 
-) -> Internship:
+    id: str,
+
+) -> Vacancy:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/internship/".format(
+        method="DELETE",
+        path="/api/v1/vacancy/{id}/".format(
+            
+                id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -54,12 +59,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Internship,
+                "application/json": Vacancy,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internship/internship_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_update.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,65 +5,67 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Internship(BaseModel):
+class Vacancy(BaseModel):
     company: typing.Optional[typing.Union[int, None]]  = None
-    duration: typing.Optional[typing.Union[int, None]]  = None
+    contract_type: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
+    employment_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
+    experience: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     external_id: str 
-    has_employment: typing.Optional[typing.Union[bool, None]]  = None
+    has_insurance: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
-    id: int 
-    is_paid: typing.Optional[typing.Union[bool, None]]  = None
+    is_relocation_required: typing.Optional[typing.Union[bool, None]]  = None
     link: str 
     name: str 
     publicated_at: typing.Optional[typing.Union[datetime.datetime, None]]  = None
     raw_description: typing.Optional[typing.Union[str, None]]  = None
-    recruitment_end_date: typing.Optional[typing.Union[datetime.datetime, None]]  = None
     requirement: typing.Optional[typing.Union[str, None]]  = None
     responsibility: typing.Optional[typing.Union[str, None]]  = None
     salary: typing.Optional[typing.Union[int, None]]  = None
     source: int 
     test_task_link: typing.Optional[typing.Union[str, None]]  = None
     work_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
 
 def make_request(self: BaseApi,
 
+    __request__: Vacancy,
+
 
     id: str,
 
-) -> Internship:
+) -> Vacancy:
     
 
     
-    body = None
+    body = __request__
     
 
     m = ApiRequest(
-        method="GET",
-        path="/internship/{id}/".format(
+        method="PUT",
+        path="/api/v1/vacancy/{id}/".format(
             
                 id=id,
             
         ),
-        content_type=None,
+        content_type="application/json",
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Internship,
+                "application/json": Vacancy,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipcity/internshipcity_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internship_create.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,46 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class InternshipCity(BaseModel):
-    city: int 
-    internship: int 
-
 def make_request(self: BaseApi,
 
-    __request__: InternshipCity,
-
 
-) -> InternshipCity:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="POST",
-        path="/internshipcity/".format(
+        path="/api/v1/internship/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipCity,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipcity/internshipcity_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_city_destroy.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     
     body = None
     
 
     m = ApiRequest(
         method="DELETE",
-        path="/internshipcity/{id}/".format(
+        path="/api/v1/city/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipcity/internshipcity_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_create.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,32 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class InternshipCity(BaseModel):
-    city: int 
-    id: int 
-    internship: int 
-
 def make_request(self: BaseApi,
 
 
-) -> InternshipCity:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/internshipcity/".format(
+        method="POST",
+        path="/api/v1/internshipskill/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipCity,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipcity/internshipcity_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_destroy.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,34 +5,29 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class InternshipCity(BaseModel):
-    city: int 
-    id: int 
-    internship: int 
-
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> InternshipCity:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/internshipcity/{id}/".format(
+        method="DELETE",
+        path="/api/v1/internshipskill/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -40,14 +35,14 @@
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "200": {
+        "204": {
             
-                "application/json": InternshipCity,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipcity/internshipcity_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_currency_destroy.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,50 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class InternshipCity(BaseModel):
-    city: int 
-    internship: int 
-
 def make_request(self: BaseApi,
 
-    __request__: InternshipCity,
-
 
     id: str,
 
-) -> InternshipCity:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/internshipcity/{id}/".format(
+        method="DELETE",
+        path="/api/v1/currency/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "200": {
+        "204": {
             
-                "application/json": InternshipCity,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipcontact/internshipcontact_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,46 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class InternshipContact(BaseModel):
-    contact: int 
-    internship: int 
-
 def make_request(self: BaseApi,
 
-    __request__: InternshipContact,
 
+    id: str,
 
-) -> InternshipContact:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/internshipcontact/".format(
+        method="PUT",
+        path="/api/v1/internshipskill/{id}/".format(
+            
+                id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipContact,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipcontact/internshipcontact_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_destroy.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     
     body = None
     
 
     m = ApiRequest(
         method="DELETE",
-        path="/internshipcontact/{id}/".format(
+        path="/api/v1/internshipcontact/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipcontact/internshipcontact_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_retrieve.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,32 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class InternshipContact(BaseModel):
-    contact: int 
-    id: int 
-    internship: int 
-
 def make_request(self: BaseApi,
 
 
-) -> InternshipContact:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/internshipcontact/".format(
+        path="/api/v1/internshipskill/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipContact,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipcontact/internshipcontact_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internship_retrieve.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,36 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class InternshipContact(BaseModel):
-    contact: int 
-    id: int 
-    internship: int 
-
 def make_request(self: BaseApi,
 
 
-    id: str,
-
-) -> InternshipContact:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/internshipcontact/{id}/".format(
-            
-                id=id,
+        path="/api/v1/internship/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -42,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipContact,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipskill/internshipskill_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_create.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,46 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class InternshipSkill(BaseModel):
-    internship: int 
-    skill: int 
-
 def make_request(self: BaseApi,
 
-    __request__: InternshipSkill,
-
 
-) -> InternshipSkill:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="POST",
-        path="/internshipskill/".format(
+        path="/api/v1/internshipcity/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipSkill,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipskill/internshipskill_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_skill_update.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="DELETE",
-        path="/internshipskill/{id}/".format(
+        method="PUT",
+        path="/api/v1/skill/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -35,14 +35,14 @@
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "204": {
+        "200": {
             
                 "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipskill/internshipskill_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_update.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class InternshipSkill(BaseModel):
-    id: int 
-    internship: int 
-    skill: int 
-
 def make_request(self: BaseApi,
 
 
-) -> InternshipSkill:
+    id: str,
+
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/internshipskill/".format(
+        method="PUT",
+        path="/api/v1/internshipcontact/{id}/".format(
+            
+                id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipSkill,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipskill/internshipskill_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_source_create.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,36 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class InternshipSkill(BaseModel):
-    id: int 
-    internship: int 
-    skill: int 
-
 def make_request(self: BaseApi,
 
 
-    id: str,
-
-) -> InternshipSkill:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/internshipskill/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/source/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -42,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipSkill,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/internshipskill/internshipskill_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_update.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,50 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class InternshipSkill(BaseModel):
-    internship: int 
-    skill: int 
-
 def make_request(self: BaseApi,
 
-    __request__: InternshipSkill,
-
 
     id: str,
 
-) -> InternshipSkill:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="PUT",
-        path="/internshipskill/{id}/".format(
+        path="/api/v1/internshipcity/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipSkill,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/jobmixin/jobmixin_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancy_list.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,58 +5,108 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class JobMixin(BaseModel):
+class Vacancy(BaseModel):
     company: typing.Optional[typing.Union[int, None]]  = None
+    contract_type: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
+    employment_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
+    experience: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     external_id: str 
+    has_insurance: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
+    id: int 
+    is_relocation_required: typing.Optional[typing.Union[bool, None]]  = None
     link: str 
     name: str 
     publicated_at: typing.Optional[typing.Union[datetime.datetime, None]]  = None
     raw_description: typing.Optional[typing.Union[str, None]]  = None
     requirement: typing.Optional[typing.Union[str, None]]  = None
     responsibility: typing.Optional[typing.Union[str, None]]  = None
     salary: typing.Optional[typing.Union[int, None]]  = None
     source: int 
     test_task_link: typing.Optional[typing.Union[str, None]]  = None
     work_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
 
+class PaginatedVacancyList(BaseModel):
+    count: typing.Optional[int]  = None
+    next: typing.Optional[typing.Union[str, None]]  = None
+    previous: typing.Optional[typing.Union[str, None]]  = None
+    results: typing.Optional[typing.List[Vacancy]]  = None
+
 def make_request(self: BaseApi,
 
-    __request__: JobMixin,
 
+    activity_sphere: str = ...,
+
+    company_size: str = ...,
+
+    employment_format: str = ...,
+
+    has_insurance: bool = ...,
+
+    is_accredited: bool = ...,
+
+    is_relocation_required: bool = ...,
+
+    page: int = ...,
+
+    relocation_is_required: bool = ...,
+
+    search: str = ...,
+
+    work_format: str = ...,
 
-) -> JobMixin:
+) -> PaginatedVacancyList:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/jobmixin/".format(
+        method="GET",
+        path="/api/v1/vacancy/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
+                "activity_sphere": activity_sphere,
+            
+                "company_size": company_size,
+            
+                "employment_format": employment_format,
+            
+                "has_insurance": has_insurance,
+            
+                "is_accredited": is_accredited,
+            
+                "is_relocation_required": is_relocation_required,
+            
+                "page": page,
+            
+                "relocation_is_required": relocation_is_required,
+            
+                "search": search,
+            
+                "work_format": work_format,
+            
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": JobMixin,
+                "application/json": PaginatedVacancyList,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/jobmixin/jobmixin_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_create.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,41 +8,37 @@
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
 def make_request(self: BaseApi,
 
 
-    id: str,
-
 ) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="DELETE",
-        path="/jobmixin/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/vacancyskill/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "204": {
+        "200": {
             
                 "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/region/region_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_region_retrieve.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,46 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Region(BaseModel):
-    country: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Region,
-
 
-) -> Region:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/region/".format(
+        method="GET",
+        path="/api/v1/region/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Region,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/region/region_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_activitysphere_create.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,41 +8,37 @@
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
 def make_request(self: BaseApi,
 
 
-    id: str,
-
 ) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="DELETE",
-        path="/region/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/activitysphere/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "204": {
+        "200": {
             
                 "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/region/region_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_salary_retrieve.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,32 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Region(BaseModel):
-    country: int 
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
-) -> Region:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/region/".format(
+        path="/api/v1/salary/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Region,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/region/region_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_skill_retrieve.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,36 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Region(BaseModel):
-    country: int 
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
-    id: str,
-
-) -> Region:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/region/{id}/".format(
-            
-                id=id,
+        path="/api/v1/skill/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -42,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Region,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/region/region_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_retrieve_2.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,50 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Region(BaseModel):
-    country: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Region,
-
 
     id: str,
 
-) -> Region:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/region/{id}/".format(
+        method="GET",
+        path="/api/v1/searchandstopkeywords/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Region,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/salary/salary_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_region_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,47 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Salary(BaseModel):
-    currency: int 
-    max_value: typing.Optional[typing.Union[int, None]]  = None
-    min_value: typing.Optional[typing.Union[int, None]]  = None
-
 def make_request(self: BaseApi,
 
-    __request__: Salary,
 
+    id: str,
 
-) -> Salary:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/salary/".format(
+        method="PUT",
+        path="/api/v1/region/{id}/".format(
+            
+                id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Salary,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/salary/salary_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_retrieve.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,41 +8,37 @@
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
 def make_request(self: BaseApi,
 
 
-    id: str,
-
 ) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="DELETE",
-        path="/salary/{id}/".format(
-            
-                id=id,
+        method="GET",
+        path="/api/v1/vacancyskill/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "204": {
+        "200": {
             
                 "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/salary/salary_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_retrieve_2.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,33 +5,31 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Salary(BaseModel):
-    currency: int 
-    id: int 
-    max_value: typing.Optional[typing.Union[int, None]]  = None
-    min_value: typing.Optional[typing.Union[int, None]]  = None
-
 def make_request(self: BaseApi,
 
 
-) -> Salary:
+    id: str,
+
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/salary/".format(
+        path="/api/v1/vacancycontact/{id}/".format(
+            
+                id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -39,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Salary,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/salary/salary_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipskill_retrieve_2.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,35 +5,29 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Salary(BaseModel):
-    currency: int 
-    id: int 
-    max_value: typing.Optional[typing.Union[int, None]]  = None
-    min_value: typing.Optional[typing.Union[int, None]]  = None
-
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> Salary:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/salary/{id}/".format(
+        path="/api/v1/internshipskill/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -43,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Salary,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/salary/salary_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_country_destroy.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,51 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Salary(BaseModel):
-    currency: int 
-    max_value: typing.Optional[typing.Union[int, None]]  = None
-    min_value: typing.Optional[typing.Union[int, None]]  = None
-
 def make_request(self: BaseApi,
 
-    __request__: Salary,
-
 
     id: str,
 
-) -> Salary:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/salary/{id}/".format(
+        method="DELETE",
+        path="/api/v1/country/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "200": {
+        "204": {
             
-                "application/json": Salary,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchandstopkeywords/searchandstopkeywords_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_company_create.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,46 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class SearchAndStopKeywords(BaseModel):
-    search_keywords: int 
-    stop_keywords: int 
-
 def make_request(self: BaseApi,
 
-    __request__: SearchAndStopKeywords,
-
 
-) -> SearchAndStopKeywords:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="POST",
-        path="/searchandstopkeywords/".format(
+        path="/api/v1/company/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": SearchAndStopKeywords,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchandstopkeywords/searchandstopkeywords_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_contact_retrieve_2.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="DELETE",
-        path="/searchandstopkeywords/{id}/".format(
+        method="GET",
+        path="/api/v1/contact/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -35,14 +35,14 @@
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "204": {
+        "200": {
             
                 "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchandstopkeywords/searchandstopkeywords_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_create.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,32 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class SearchAndStopKeywords(BaseModel):
-    id: int 
-    search_keywords: int 
-    stop_keywords: int 
-
 def make_request(self: BaseApi,
 
 
-) -> SearchAndStopKeywords:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/searchandstopkeywords/".format(
+        method="POST",
+        path="/api/v1/stopkeywords/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": SearchAndStopKeywords,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchandstopkeywords/searchandstopkeywords_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_create.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,36 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class SearchAndStopKeywords(BaseModel):
-    id: int 
-    search_keywords: int 
-    stop_keywords: int 
-
 def make_request(self: BaseApi,
 
 
-    id: str,
-
-) -> SearchAndStopKeywords:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/searchandstopkeywords/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/searchkeywords/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -42,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": SearchAndStopKeywords,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchandstopkeywords/searchandstopkeywords_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_country_retrieve_2.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,50 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class SearchAndStopKeywords(BaseModel):
-    search_keywords: int 
-    stop_keywords: int 
-
 def make_request(self: BaseApi,
 
-    __request__: SearchAndStopKeywords,
-
 
     id: str,
 
-) -> SearchAndStopKeywords:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/searchandstopkeywords/{id}/".format(
+        method="GET",
+        path="/api/v1/country/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": SearchAndStopKeywords,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchkeywords/searchkeywords_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_retrieve.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,45 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class SearchKeywords(BaseModel):
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: SearchKeywords,
-
 
-) -> SearchKeywords:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/searchkeywords/".format(
+        method="GET",
+        path="/api/v1/searchkeywords/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": SearchKeywords,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchkeywords/searchkeywords_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_create.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,41 +8,37 @@
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
 def make_request(self: BaseApi,
 
 
-    id: str,
-
 ) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="DELETE",
-        path="/searchkeywords/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/vacancycontact/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "204": {
+        "200": {
             
                 "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchkeywords/searchkeywords_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_retrieve.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,32 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class SearchKeywords(BaseModel):
-    id: int 
-    name: str 
-    stop_keywords: typing.List[int] 
-
 def make_request(self: BaseApi,
 
 
-) -> SearchKeywords:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/searchkeywords/".format(
+        path="/api/v1/vacancycontact/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": SearchKeywords,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchkeywords/searchkeywords_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_destroy.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,34 +5,29 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class SearchKeywords(BaseModel):
-    id: int 
-    name: str 
-    stop_keywords: typing.List[int] 
-
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> SearchKeywords:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/searchkeywords/{id}/".format(
+        method="DELETE",
+        path="/api/v1/vacancycity/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -40,14 +35,14 @@
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "200": {
+        "204": {
             
-                "application/json": SearchKeywords,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/searchkeywords/searchkeywords_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycity_update.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,49 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class SearchKeywords(BaseModel):
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: SearchKeywords,
-
 
     id: str,
 
-) -> SearchKeywords:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="PUT",
-        path="/searchkeywords/{id}/".format(
+        path="/api/v1/vacancycity/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": SearchKeywords,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/skill/skill_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_country_create.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,45 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Skill(BaseModel):
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Skill,
-
 
-) -> Skill:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="POST",
-        path="/skill/".format(
+        path="/api/v1/country/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Skill,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/skill/skill_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_destroy.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     
     body = None
     
 
     m = ApiRequest(
         method="DELETE",
-        path="/skill/{id}/".format(
+        path="/api/v1/vacancyskill/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/skill/skill_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcity_retrieve_2.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Skill(BaseModel):
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
-) -> Skill:
+    id: str,
+
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/skill/".format(
+        path="/api/v1/internshipcity/{id}/".format(
+            
+                id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -37,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Skill,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/skill/skill_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_update.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,33 +5,29 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Skill(BaseModel):
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> Skill:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/skill/{id}/".format(
+        method="PUT",
+        path="/api/v1/vacancyskill/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -41,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Skill,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/skill/skill_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_country_retrieve.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,49 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Skill(BaseModel):
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Skill,
-
 
-    id: str,
-
-) -> Skill:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/skill/{id}/".format(
-            
-                id=id,
+        method="GET",
+        path="/api/v1/country/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Skill,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/source/source_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_contact_create.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,45 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Source(BaseModel):
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Source,
-
 
-) -> Source:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="POST",
-        path="/source/".format(
+        path="/api/v1/contact/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Source,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/source/source_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_source_destroy.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     
     body = None
     
 
     m = ApiRequest(
         method="DELETE",
-        path="/source/{id}/".format(
+        path="/api/v1/source/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/source/source_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_source_retrieve.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,31 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Source(BaseModel):
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
-) -> Source:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/source/".format(
+        path="/api/v1/source/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -37,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Source,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/source/source_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_source_retrieve_2.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,33 +5,29 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Source(BaseModel):
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> Source:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/source/{id}/".format(
+        path="/api/v1/source/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -41,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Source,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/source/source_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_stopkeywords_retrieve.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,49 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class Source(BaseModel):
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Source,
-
 
-    id: str,
-
-) -> Source:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/source/{id}/".format(
-            
-                id=id,
+        method="GET",
+        path="/api/v1/stopkeywords/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Source,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/stopkeywords/stopkeywords_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_retrieve.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,41 +8,37 @@
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
 def make_request(self: BaseApi,
 
 
-    id: str,
-
 ) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="DELETE",
-        path="/stopkeywords/{id}/".format(
-            
-                id=id,
+        method="GET",
+        path="/api/v1/searchandstopkeywords/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "204": {
+        "200": {
             
                 "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/stopkeywords/stopkeywords_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_company_retrieve_2.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class StopKeywords(BaseModel):
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
-) -> StopKeywords:
+    id: str,
+
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/stopkeywords/".format(
+        path="/api/v1/company/{id}/".format(
+            
+                id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -37,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": StopKeywords,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/stopkeywords/stopkeywords_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_city_retrieve_2.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,33 +5,29 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class StopKeywords(BaseModel):
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> StopKeywords:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/stopkeywords/{id}/".format(
+        path="/api/v1/city/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -41,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": StopKeywords,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/stopkeywords/stopkeywords_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_contact_retrieve.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,49 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class StopKeywords(BaseModel):
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: StopKeywords,
-
 
-    id: str,
-
-) -> StopKeywords:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/stopkeywords/{id}/".format(
-            
-                id=id,
+        method="GET",
+        path="/api/v1/contact/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": StopKeywords,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancycity/vacancycity_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_update.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,46 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class VacancyCity(BaseModel):
-    city: int 
-    vacancy: int 
-
 def make_request(self: BaseApi,
 
-    __request__: VacancyCity,
 
+    id: str,
 
-) -> VacancyCity:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/vacancycity/".format(
+        method="PUT",
+        path="/api/v1/vacancycontact/{id}/".format(
+            
+                id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": VacancyCity,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancycity/vacancycity_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_salary_destroy.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     
     body = None
     
 
     m = ApiRequest(
         method="DELETE",
-        path="/vacancycity/{id}/".format(
+        path="/api/v1/salary/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancycity/vacancycity_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_jobmixin_update.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,34 +5,29 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class VacancyCity(BaseModel):
-    city: int 
-    id: int 
-    vacancy: int 
-
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> VacancyCity:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/vacancycity/{id}/".format(
+        method="PUT",
+        path="/api/v1/jobmixin/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -42,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": VacancyCity,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancycity/vacancycity_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancycontact_destroy.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,50 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class VacancyCity(BaseModel):
-    city: int 
-    vacancy: int 
-
 def make_request(self: BaseApi,
 
-    __request__: VacancyCity,
-
 
     id: str,
 
-) -> VacancyCity:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/vacancycity/{id}/".format(
+        method="DELETE",
+        path="/api/v1/vacancycontact/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "200": {
+        "204": {
             
-                "application/json": VacancyCity,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancycontact/vacancycontact_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_contact_destroy.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     
     body = None
     
 
     m = ApiRequest(
         method="DELETE",
-        path="/vacancycontact/{id}/".format(
+        path="/api/v1/contact/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancycontact/vacancycontact_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_contact_update.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class VacancyContact(BaseModel):
-    contact: int 
-    id: int 
-    vacancy: int 
-
 def make_request(self: BaseApi,
 
 
-) -> VacancyContact:
+    id: str,
+
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/vacancycontact/".format(
+        method="PUT",
+        path="/api/v1/contact/{id}/".format(
+            
+                id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": VacancyContact,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancycontact/vacancycontact_retrieve_2.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_internshipcontact_retrieve_2.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,34 +5,29 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class VacancyContact(BaseModel):
-    contact: int 
-    id: int 
-    vacancy: int 
-
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> VacancyContact:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/vacancycontact/{id}/".format(
+        path="/api/v1/internshipcontact/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -42,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": VacancyContact,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancycontact/vacancycontact_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchandstopkeywords_update.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,50 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class VacancyContact(BaseModel):
-    contact: int 
-    vacancy: int 
-
 def make_request(self: BaseApi,
 
-    __request__: VacancyContact,
-
 
     id: str,
 
-) -> VacancyContact:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="PUT",
-        path="/vacancycontact/{id}/".format(
+        path="/api/v1/searchandstopkeywords/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": VacancyContact,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancyskill/vacancyskill_create.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_searchkeywords_update.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,46 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class VacancySkill(BaseModel):
-    skill: int 
-    vacancy: int 
-
 def make_request(self: BaseApi,
 
-    __request__: VacancySkill,
 
+    id: str,
 
-) -> VacancySkill:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/vacancyskill/".format(
+        method="PUT",
+        path="/api/v1/searchkeywords/{id}/".format(
+            
+                id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": VacancySkill,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancyskill/vacancyskill_destroy.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_vacancyskill_retrieve_2.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="DELETE",
-        path="/vacancyskill/{id}/".format(
+        method="GET",
+        path="/api/v1/vacancyskill/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -35,14 +35,14 @@
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "204": {
+        "200": {
             
                 "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancyskill/vacancyskill_retrieve.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_source_update.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class VacancySkill(BaseModel):
-    id: int 
-    skill: int 
-    vacancy: int 
-
 def make_request(self: BaseApi,
 
 
-) -> VacancySkill:
+    id: str,
+
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/vacancyskill/".format(
+        method="PUT",
+        path="/api/v1/source/{id}/".format(
+            
+                id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": VacancySkill,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/feedancy-client/feedancy_client/apis/vacancyskill/vacancyskill_update.py` & `feedancy_client-0.0.5/feedancy-client/feedancy_client/apis/api/api_v1_city_update.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,50 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy_client.lib.base import BaseApi
 from feedancy_client.lib.request import ApiRequest
 from feedancy_client.lib import json
-class VacancySkill(BaseModel):
-    skill: int 
-    vacancy: int 
-
 def make_request(self: BaseApi,
 
-    __request__: VacancySkill,
-
 
     id: str,
 
-) -> VacancySkill:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="PUT",
-        path="/vacancyskill/{id}/".format(
+        path="/api/v1/city/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": VacancySkill,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy_client-0.0.2/pyproject.toml` & `feedancy_client-0.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -10,42 +10,41 @@
   | \.mypy_cache
   | \.tox
   | \.venv
   | _build
   | buck-out
   | build
   | dist
-  | feedancy-client
 )/
 '''
 
 [tool.poetry]
 name = "feedancy-client"
-version = "0.0.2"
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
-#djangorestframework = ">=3.14.0"
+djangorestframework = ">=3.14.0"
 #Django = ">=4"
-#gunicorn = ">=20.1.0"
-#psycopg2-binary = ">=2.9.6"
-#Pillow = ">=9.5.0"
-#django-filter = ">=23.2"
-#pydantic = ">=1.10.8"
+gunicorn = ">=20.1.0"
+psycopg2-binary = ">=2.9.6"
+Pillow = ">=9.5.0"
+django-filter = ">=23.2"
+pydantic = ">=1.10.8"
 requests = ">=2.31"
 bs4 = ">=0.0.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `feedancy_client-0.0.2/PKG-INFO` & `feedancy_client-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 Metadata-Version: 2.1
 Name: feedancy-client
-Version: 0.0.2
+Version: 0.0.5
 Summary: сервис по сбору вакансий
 License: MIT
 Author: Alexey Ostanin
 Author-email: aostaninn@gmal.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Pillow (>=9.5.0)
 Requires-Dist: bs4 (>=0.0.1)
+Requires-Dist: django-filter (>=23.2)
+Requires-Dist: djangorestframework (>=3.14.0)
+Requires-Dist: gunicorn (>=20.1.0)
+Requires-Dist: psycopg2-binary (>=2.9.6)
+Requires-Dist: pydantic (>=1.10.8)
 Requires-Dist: requests (>=2.31)
 Description-Content-Type: text/markdown
 
 # feedancy-client
 
 The client is provided with async and sync adapters.
```

