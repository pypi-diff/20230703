# Comparing `tmp/feedancy-0.0.5.tar.gz` & `tmp/feedancy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedancy-0.0.5.tar", max compression
+gzip compressed data, was "feedancy-0.0.6.tar", max compression
```

## Comparing `feedancy-0.0.5.tar` & `feedancy-0.0.6.tar`

### file list

```diff
@@ -1,125 +1,3 @@
--rw-r--r--   0        0        0      203 2023-06-30 14:22:35.814360 feedancy-0.0.5/feedancy/MANIFEST.in
--rw-r--r--   0        0        0      615 2023-06-30 14:22:35.810361 feedancy-0.0.5/feedancy/README.md
--rw-r--r--   0        0        0      126 2023-06-30 14:22:35.806361 feedancy-0.0.5/feedancy/feedancy/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 14:22:35.746363 feedancy-0.0.5/feedancy/feedancy/apis/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 14:22:35.746363 feedancy-0.0.5/feedancy/feedancy/apis/api/__init__.py
--rw-r--r--   0        0        0    13072 2023-06-30 14:22:35.750363 feedancy-0.0.5/feedancy/feedancy/apis/api/api.py
--rw-r--r--   0        0        0      763 2023-06-30 14:22:35.762363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_activitysphere_create.py
--rw-r--r--   0        0        0      820 2023-06-30 14:22:35.762363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_activitysphere_destroy.py
--rw-r--r--   0        0        0      762 2023-06-30 14:22:35.762363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_activitysphere_retrieve.py
--rw-r--r--   0        0        0      817 2023-06-30 14:22:35.762363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py
--rw-r--r--   0        0        0      817 2023-06-30 14:22:35.762363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_activitysphere_update.py
--rw-r--r--   0        0        0      753 2023-06-30 14:22:35.762363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_city_create.py
--rw-r--r--   0        0        0      810 2023-06-30 14:22:35.766363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_city_destroy.py
--rw-r--r--   0        0        0      752 2023-06-30 14:22:35.762363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_city_retrieve.py
--rw-r--r--   0        0        0      807 2023-06-30 14:22:35.762363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_city_retrieve_2.py
--rw-r--r--   0        0        0      807 2023-06-30 14:22:35.766363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_city_update.py
--rw-r--r--   0        0        0      756 2023-06-30 14:22:35.766363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_company_create.py
--rw-r--r--   0        0        0      813 2023-06-30 14:22:35.766363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_company_destroy.py
--rw-r--r--   0        0        0      755 2023-06-30 14:22:35.766363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_company_retrieve.py
--rw-r--r--   0        0        0      810 2023-06-30 14:22:35.766363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_company_retrieve_2.py
--rw-r--r--   0        0        0      810 2023-06-30 14:22:35.766363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_company_update.py
--rw-r--r--   0        0        0      760 2023-06-30 14:22:35.766363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_companycity_create.py
--rw-r--r--   0        0        0      817 2023-06-30 14:22:35.766363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_companycity_destroy.py
--rw-r--r--   0        0        0      759 2023-06-30 14:22:35.766363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_companycity_retrieve.py
--rw-r--r--   0        0        0      814 2023-06-30 14:22:35.766363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_companycity_retrieve_2.py
--rw-r--r--   0        0        0      814 2023-06-30 14:22:35.766363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_companycity_update.py
--rw-r--r--   0        0        0      756 2023-06-30 14:22:35.766363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_contact_create.py
--rw-r--r--   0        0        0      813 2023-06-30 14:22:35.766363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_contact_destroy.py
--rw-r--r--   0        0        0      755 2023-06-30 14:22:35.766363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_contact_retrieve.py
--rw-r--r--   0        0        0      810 2023-06-30 14:22:35.766363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_contact_retrieve_2.py
--rw-r--r--   0        0        0      810 2023-06-30 14:22:35.766363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_contact_update.py
--rw-r--r--   0        0        0      756 2023-06-30 14:22:35.766363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_country_create.py
--rw-r--r--   0        0        0      813 2023-06-30 14:22:35.770362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_country_destroy.py
--rw-r--r--   0        0        0      755 2023-06-30 14:22:35.766363 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_country_retrieve.py
--rw-r--r--   0        0        0      810 2023-06-30 14:22:35.770362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_country_retrieve_2.py
--rw-r--r--   0        0        0      810 2023-06-30 14:22:35.770362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_country_update.py
--rw-r--r--   0        0        0      757 2023-06-30 14:22:35.770362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_currency_create.py
--rw-r--r--   0        0        0      814 2023-06-30 14:22:35.770362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_currency_destroy.py
--rw-r--r--   0        0        0      756 2023-06-30 14:22:35.770362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_currency_retrieve.py
--rw-r--r--   0        0        0      811 2023-06-30 14:22:35.770362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_currency_retrieve_2.py
--rw-r--r--   0        0        0      811 2023-06-30 14:22:35.770362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_currency_update.py
--rw-r--r--   0        0        0      759 2023-06-30 14:22:35.770362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_internship_create.py
--rw-r--r--   0        0        0     1941 2023-06-30 14:22:35.778362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_internship_destroy.py
--rw-r--r--   0        0        0      758 2023-06-30 14:22:35.770362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_internship_retrieve.py
--rw-r--r--   0        0        0     1938 2023-06-30 14:22:35.774362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_internship_retrieve_2.py
--rw-r--r--   0        0        0     1976 2023-06-30 14:22:35.774362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_internship_update.py
--rw-r--r--   0        0        0      763 2023-06-30 14:22:35.778362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_internshipcity_create.py
--rw-r--r--   0        0        0      820 2023-06-30 14:22:35.778362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_internshipcity_destroy.py
--rw-r--r--   0        0        0      762 2023-06-30 14:22:35.778362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_internshipcity_retrieve.py
--rw-r--r--   0        0        0      817 2023-06-30 14:22:35.778362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_internshipcity_retrieve_2.py
--rw-r--r--   0        0        0      817 2023-06-30 14:22:35.778362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_internshipcity_update.py
--rw-r--r--   0        0        0      766 2023-06-30 14:22:35.778362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_internshipcontact_create.py
--rw-r--r--   0        0        0      823 2023-06-30 14:22:35.782362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_internshipcontact_destroy.py
--rw-r--r--   0        0        0      765 2023-06-30 14:22:35.778362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_internshipcontact_retrieve.py
--rw-r--r--   0        0        0      820 2023-06-30 14:22:35.782362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py
--rw-r--r--   0        0        0      820 2023-06-30 14:22:35.782362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_internshipcontact_update.py
--rw-r--r--   0        0        0      764 2023-06-30 14:22:35.782362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_internshipskill_create.py
--rw-r--r--   0        0        0      821 2023-06-30 14:22:35.782362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_internshipskill_destroy.py
--rw-r--r--   0        0        0      763 2023-06-30 14:22:35.782362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_internshipskill_retrieve.py
--rw-r--r--   0        0        0      818 2023-06-30 14:22:35.782362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py
--rw-r--r--   0        0        0      818 2023-06-30 14:22:35.782362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_internshipskill_update.py
--rw-r--r--   0        0        0      757 2023-06-30 14:22:35.782362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_jobmixin_create.py
--rw-r--r--   0        0        0      814 2023-06-30 14:22:35.782362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_jobmixin_destroy.py
--rw-r--r--   0        0        0      756 2023-06-30 14:22:35.782362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_jobmixin_retrieve.py
--rw-r--r--   0        0        0      811 2023-06-30 14:22:35.782362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py
--rw-r--r--   0        0        0      811 2023-06-30 14:22:35.782362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_jobmixin_update.py
--rw-r--r--   0        0        0      755 2023-06-30 14:22:35.786362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_region_create.py
--rw-r--r--   0        0        0      812 2023-06-30 14:22:35.786362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_region_destroy.py
--rw-r--r--   0        0        0      754 2023-06-30 14:22:35.782362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_region_retrieve.py
--rw-r--r--   0        0        0      809 2023-06-30 14:22:35.786362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_region_retrieve_2.py
--rw-r--r--   0        0        0      809 2023-06-30 14:22:35.786362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_region_update.py
--rw-r--r--   0        0        0      755 2023-06-30 14:22:35.786362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_salary_create.py
--rw-r--r--   0        0        0      812 2023-06-30 14:22:35.786362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_salary_destroy.py
--rw-r--r--   0        0        0      754 2023-06-30 14:22:35.786362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_salary_retrieve.py
--rw-r--r--   0        0        0      809 2023-06-30 14:22:35.786362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_salary_retrieve_2.py
--rw-r--r--   0        0        0      809 2023-06-30 14:22:35.786362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_salary_update.py
--rw-r--r--   0        0        0      770 2023-06-30 14:22:35.786362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_create.py
--rw-r--r--   0        0        0      827 2023-06-30 14:22:35.786362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py
--rw-r--r--   0        0        0      769 2023-06-30 14:22:35.786362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py
--rw-r--r--   0        0        0      824 2023-06-30 14:22:35.786362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py
--rw-r--r--   0        0        0      824 2023-06-30 14:22:35.786362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_update.py
--rw-r--r--   0        0        0      763 2023-06-30 14:22:35.786362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_searchkeywords_create.py
--rw-r--r--   0        0        0      820 2023-06-30 14:22:35.790362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_searchkeywords_destroy.py
--rw-r--r--   0        0        0      762 2023-06-30 14:22:35.786362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_searchkeywords_retrieve.py
--rw-r--r--   0        0        0      817 2023-06-30 14:22:35.786362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py
--rw-r--r--   0        0        0      817 2023-06-30 14:22:35.786362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_searchkeywords_update.py
--rw-r--r--   0        0        0      754 2023-06-30 14:22:35.790362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_skill_create.py
--rw-r--r--   0        0        0      811 2023-06-30 14:22:35.790362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_skill_destroy.py
--rw-r--r--   0        0        0      753 2023-06-30 14:22:35.790362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_skill_retrieve.py
--rw-r--r--   0        0        0      808 2023-06-30 14:22:35.790362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_skill_retrieve_2.py
--rw-r--r--   0        0        0      808 2023-06-30 14:22:35.790362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_skill_update.py
--rw-r--r--   0        0        0      755 2023-06-30 14:22:35.790362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_source_create.py
--rw-r--r--   0        0        0      812 2023-06-30 14:22:35.790362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_source_destroy.py
--rw-r--r--   0        0        0      754 2023-06-30 14:22:35.790362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_source_retrieve.py
--rw-r--r--   0        0        0      809 2023-06-30 14:22:35.790362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_source_retrieve_2.py
--rw-r--r--   0        0        0      809 2023-06-30 14:22:35.790362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_source_update.py
--rw-r--r--   0        0        0      761 2023-06-30 14:22:35.790362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_stopkeywords_create.py
--rw-r--r--   0        0        0      818 2023-06-30 14:22:35.790362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_stopkeywords_destroy.py
--rw-r--r--   0        0        0      760 2023-06-30 14:22:35.790362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_stopkeywords_retrieve.py
--rw-r--r--   0        0        0      815 2023-06-30 14:22:35.790362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py
--rw-r--r--   0        0        0      815 2023-06-30 14:22:35.790362 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_stopkeywords_update.py
--rw-r--r--   0        0        0     2046 2023-06-30 14:22:35.794361 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_vacancy_create.py
--rw-r--r--   0        0        0     2068 2023-06-30 14:22:35.798361 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_vacancy_destroy.py
--rw-r--r--   0        0        0     3236 2023-06-30 14:22:35.794361 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_vacancy_list.py
--rw-r--r--   0        0        0     2065 2023-06-30 14:22:35.798361 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_vacancy_retrieve.py
--rw-r--r--   0        0        0     2100 2023-06-30 14:22:35.798361 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_vacancy_update.py
--rw-r--r--   0        0        0      760 2023-06-30 14:22:35.802361 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_vacancycity_create.py
--rw-r--r--   0        0        0      817 2023-06-30 14:22:35.802361 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_vacancycity_destroy.py
--rw-r--r--   0        0        0      759 2023-06-30 14:22:35.802361 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_vacancycity_retrieve.py
--rw-r--r--   0        0        0      814 2023-06-30 14:22:35.802361 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_vacancycity_retrieve_2.py
--rw-r--r--   0        0        0      814 2023-06-30 14:22:35.802361 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_vacancycity_update.py
--rw-r--r--   0        0        0      763 2023-06-30 14:22:35.802361 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_vacancycontact_create.py
--rw-r--r--   0        0        0      820 2023-06-30 14:22:35.802361 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_vacancycontact_destroy.py
--rw-r--r--   0        0        0      762 2023-06-30 14:22:35.802361 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_vacancycontact_retrieve.py
--rw-r--r--   0        0        0      817 2023-06-30 14:22:35.802361 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py
--rw-r--r--   0        0        0      817 2023-06-30 14:22:35.802361 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_vacancycontact_update.py
--rw-r--r--   0        0        0      761 2023-06-30 14:22:35.802361 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_vacancyskill_create.py
--rw-r--r--   0        0        0      818 2023-06-30 14:22:35.802361 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_vacancyskill_destroy.py
--rw-r--r--   0        0        0      760 2023-06-30 14:22:35.802361 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_vacancyskill_retrieve.py
--rw-r--r--   0        0        0      815 2023-06-30 14:22:35.802361 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_vacancyskill_retrieve_2.py
--rw-r--r--   0        0        0      815 2023-06-30 14:22:35.802361 feedancy-0.0.5/feedancy/feedancy/apis/api/api_v1_vacancyskill_update.py
--rw-r--r--   0        0        0      658 2023-06-30 14:22:35.806361 feedancy-0.0.5/feedancy/feedancy/client.py
--rw-r--r--   0        0        0     1000 2023-06-30 14:22:35.814360 feedancy-0.0.5/feedancy/setup.py
--rw-r--r--   0        0        0      996 2023-06-30 14:44:56.836432 feedancy-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1474 1970-01-01 00:00:00.000000 feedancy-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      657 2023-07-03 17:16:29.011425 feedancy-0.0.6/feedancy-client/README.md
+-rw-r--r--   0        0        0     1014 2023-07-03 17:31:07.310148 feedancy-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 feedancy-0.0.6/PKG-INFO
```

### Comparing `feedancy-0.0.5/feedancy/README.md` & `feedancy-0.0.6/feedancy-client/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# feedancy
+# feedancy-client
 
 The client is provided with async and sync adapters.
 
 To install the async version with all its dependencies use:
 ```bash
-pip install feedancy[asyncio]
+pip install feedancy-client[asyncio]
 ```
 
 To install the sync version with all its dependencies use:
 ```bash
-pip install feedancy[sync]
+pip install feedancy-client[sync]
 ```
 
 To install both versions with all their dependencies use:
 ```bash
-pip install feedancy[asyncio,sync]
+pip install feedancy-client[asyncio,sync]
 ```
 
 ## Client instantiation example
 
 ```python
 
-from feedancy import new_client, Configuration
-from feedancy.lib.adapter.requests import RequestsAdapter
+from feedancy_client import new_client, Configuration
+from feedancy_client.lib.adapter.requests import RequestsAdapter
 
 client = new_client(RequestsAdapter(), Configuration(host="<your openapi server URL>"))
 ```
```

### Comparing `feedancy-0.0.5/pyproject.toml` & `feedancy-0.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -15,36 +15,36 @@
   | build
   | dist
 )/
 '''
 
 [tool.poetry]
 name = "feedancy"
-version = "0.0.5"
+version = "0.0.6"
 description = "сервис по сбору вакансий"
 authors = [
     "Alexey Ostanin <aostaninn@gmal.com>",
     "Stanislav Losev <stanislav_losev@protonmail.com>",
     "Tatiana Zimina <tratatatanya@gmail.com>"
 ]
 license = "MIT"
-readme = "./feedancy/README.md"
-#packages = [
-#    { include = './feedancy' }
-#]
+readme = "./feedancy-client/README.md"
+packages = [
+    { include = 'feedancy/feedancy' }
+]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-djangorestframework = ">=3.14.0"
-Django = ">=4"
-gunicorn = ">=20.1.0"
-psycopg2-binary = ">=2.9.6"
-Pillow = ">=9.5.0"
-django-filter = ">=23.2"
-pydantic = ">=1.10.8"
+#djangorestframework = ">=3.14.0"
+#Django = ">=4"
+#gunicorn = ">=20.1.0"
+#psycopg2-binary = ">=2.9.6"
+#Pillow = ">=9.5.0"
+#django-filter = ">=23.2"
+#pydantic = ">=1.10.8"
 requests = ">=2.31"
 bs4 = ">=0.0.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `feedancy-0.0.5/PKG-INFO` & `feedancy-0.0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,46 @@
 Metadata-Version: 2.1
 Name: feedancy
-Version: 0.0.5
+Version: 0.0.6
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
-Requires-Dist: Django (>=4)
-Requires-Dist: Pillow (>=9.5.0)
 Requires-Dist: bs4 (>=0.0.1)
-Requires-Dist: django-filter (>=23.2)
-Requires-Dist: djangorestframework (>=3.14.0)
-Requires-Dist: gunicorn (>=20.1.0)
-Requires-Dist: psycopg2-binary (>=2.9.6)
-Requires-Dist: pydantic (>=1.10.8)
 Requires-Dist: requests (>=2.31)
 Description-Content-Type: text/markdown
 
-# feedancy
+# feedancy-client
 
 The client is provided with async and sync adapters.
 
 To install the async version with all its dependencies use:
 ```bash
-pip install feedancy[asyncio]
+pip install feedancy-client[asyncio]
 ```
 
 To install the sync version with all its dependencies use:
 ```bash
-pip install feedancy[sync]
+pip install feedancy-client[sync]
 ```
 
 To install both versions with all their dependencies use:
 ```bash
-pip install feedancy[asyncio,sync]
+pip install feedancy-client[asyncio,sync]
 ```
 
 ## Client instantiation example
 
 ```python
 
-from feedancy import new_client, Configuration
-from feedancy.lib.adapter.requests import RequestsAdapter
+from feedancy_client import new_client, Configuration
+from feedancy_client.lib.adapter.requests import RequestsAdapter
 
 client = new_client(RequestsAdapter(), Configuration(host="<your openapi server URL>"))
 ```
```

