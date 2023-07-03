# Comparing `tmp/candidhealth-0.3.0.tar.gz` & `tmp/candidhealth-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "candidhealth-0.3.0.tar", max compression
+gzip compressed data, was "candidhealth-0.4.0.tar", max compression
```

## Comparing `candidhealth-0.3.0.tar` & `candidhealth-0.4.0.tar`

### file list

```diff
@@ -1,273 +1,270 @@
--rw-r--r--   0        0        0      257 2023-06-20 17:26:29.356214 candidhealth-0.3.0/README.md
--rw-r--r--   0        0        0      373 2023-06-20 17:26:29.356214 candidhealth-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5791 2023-06-20 17:26:29.356214 candidhealth-0.3.0/src/candid/__init__.py
--rw-r--r--   0        0        0     3166 2023-06-20 17:26:29.356214 candidhealth-0.3.0/src/candid/candid_api_client.py
--rw-r--r--   0        0        0     2511 2023-06-20 17:26:29.356214 candidhealth-0.3.0/src/candid/client.py
--rw-r--r--   0        0        0      348 2023-06-20 17:26:29.356214 candidhealth-0.3.0/src/candid/core/__init__.py
--rw-r--r--   0        0        0      426 2023-06-20 17:26:29.356214 candidhealth-0.3.0/src/candid/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-06-20 17:26:29.356214 candidhealth-0.3.0/src/candid/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-06-20 17:26:29.356214 candidhealth-0.3.0/src/candid/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-06-20 17:26:29.356214 candidhealth-0.3.0/src/candid/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      227 2023-06-20 17:26:29.356214 candidhealth-0.3.0/src/candid/environment.py
--rw-r--r--   0        0        0        0 2023-06-20 17:26:29.356214 candidhealth-0.3.0/src/candid/py.typed
--rw-r--r--   0        0        0     5939 2023-06-20 17:26:29.356214 candidhealth-0.3.0/src/candid/resources/__init__.py
--rw-r--r--   0        0        0      111 2023-06-20 17:26:29.356214 candidhealth-0.3.0/src/candid/resources/auth/__init__.py
--rw-r--r--   0        0        0      820 2023-06-20 17:26:29.356214 candidhealth-0.3.0/src/candid/resources/auth/client.py
--rw-r--r--   0        0        0      102 2023-06-20 17:26:29.356214 candidhealth-0.3.0/src/candid/resources/auth/resources/__init__.py
--rw-r--r--   0        0        0      304 2023-06-20 17:26:29.356214 candidhealth-0.3.0/src/candid/resources/auth/resources/v_2/__init__.py
--rw-r--r--   0        0        0     3502 2023-06-20 17:26:29.356214 candidhealth-0.3.0/src/candid/resources/auth/resources/v_2/client.py
--rw-r--r--   0        0        0      159 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/auth/resources/v_2/errors/__init__.py
--rw-r--r--   0        0        0      330 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/auth/resources/v_2/errors/too_many_requests_error.py
--rw-r--r--   0        0        0      333 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/auth/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0      785 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_request.py
--rw-r--r--   0        0        0      806 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_response.py
--rw-r--r--   0        0        0      765 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/auth/resources/v_2/types/too_many_requests_error_type.py
--rw-r--r--   0        0        0      191 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/billing_notes/__init__.py
--rw-r--r--   0        0        0     2831 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/billing_notes/client.py
--rw-r--r--   0        0        0      256 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/billing_notes/types/__init__.py
--rw-r--r--   0        0        0     1136 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/billing_notes/types/billing_note.py
--rw-r--r--   0        0        0      813 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/billing_notes/types/billing_note_base.py
--rw-r--r--   0        0        0      104 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/billing_notes/types/billing_note_id.py
--rw-r--r--   0        0        0      139 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/claims/__init__.py
--rw-r--r--   0        0        0      164 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/claims/types/__init__.py
--rw-r--r--   0        0        0     1151 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/claims/types/claim.py
--rw-r--r--   0        0        0     2605 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/claims/types/claim_status.py
--rw-r--r--   0        0        0     1417 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/__init__.py
--rw-r--r--   0        0        0     2104 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/__init__.py
--rw-r--r--   0        0        0       98 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/claim_id.py
--rw-r--r--   0        0        0      905 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/contact_info.py
--rw-r--r--   0        0        0       90 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/content_download_url.py
--rw-r--r--   0        0        0       76 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/date.py
--rw-r--r--   0        0        0       77 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/email.py
--rw-r--r--   0        0        0       91 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/encounter_external_id.py
--rw-r--r--   0        0        0      102 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/encounter_id.py
--rw-r--r--   0        0        0    11148 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/facility_type_code.py
--rw-r--r--   0        0        0    15447 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/insurance_type_code.py
--rw-r--r--   0        0        0       79 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/link_url.py
--rw-r--r--   0        0        0       75 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/npi.py
--rw-r--r--   0        0        0      105 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/organization_id.py
--rw-r--r--   0        0        0       81 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/page_token.py
--rw-r--r--   0        0        0       89 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/patient_external_id.py
--rw-r--r--   0        0        0     4686 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py
--rw-r--r--   0        0        0      822 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/phone_number.py
--rw-r--r--   0        0        0      620 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/phone_number_type.py
--rw-r--r--   0        0        0    79514 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/procedure_modifier.py
--rw-r--r--   0        0        0      735 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/region_national.py
--rw-r--r--   0        0        0      790 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/region_states.py
--rw-r--r--   0        0        0      633 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/regions.py
--rw-r--r--   0        0        0      864 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/resource_page.py
--rw-r--r--   0        0        0      104 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/service_line_id.py
--rw-r--r--   0        0        0      432 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/service_line_units.py
--rw-r--r--   0        0        0     5065 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/source_of_payment_code.py
--rw-r--r--   0        0        0     6264 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/state.py
--rw-r--r--   0        0        0     1037 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/street_address_base.py
--rw-r--r--   0        0        0      985 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/street_address_long_zip.py
--rw-r--r--   0        0        0     1003 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/street_address_short_zip.py
--rw-r--r--   0        0        0       83 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/commons/types/work_queue_id.py
--rw-r--r--   0        0        0      251 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/contracts/__init__.py
--rw-r--r--   0        0        0      365 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/contracts/types/__init__.py
--rw-r--r--   0        0        0      940 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/contracts/types/authorized_signatory.py
--rw-r--r--   0        0        0     1430 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/contracts/types/contract.py
--rw-r--r--   0        0        0     1517 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/contracts/types/contract_base.py
--rw-r--r--   0        0        0      101 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/contracts/types/contract_id.py
--rw-r--r--   0        0        0      986 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/contracts/types/contract_status.py
--rw-r--r--   0        0        0     1125 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/credentialing/__init__.py
--rw-r--r--   0        0        0     1472 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/credentialing/types/__init__.py
--rw-r--r--   0        0        0      886 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/credentialing/types/credentialed_encounter_status_result.py
--rw-r--r--   0        0        0      846 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/credentialing/types/credentialing_span_dates.py
--rw-r--r--   0        0        0      977 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/credentialing/types/credentialing_span_status.py
--rw-r--r--   0        0        0      809 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/credentialing/types/encounter_credentialing_status_result.py
--rw-r--r--   0        0        0      864 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/credentialing/types/non_required_credentialing_dates.py
--rw-r--r--   0        0        0     2210 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/credentialing/types/provider_credentialing_span.py
--rw-r--r--   0        0        0      958 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/credentialing/types/provider_credentialing_span_base.py
--rw-r--r--   0        0        0      118 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/credentialing/types/provider_credentialing_span_id.py
--rw-r--r--   0        0        0      827 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/credentialing/types/required_credentialing_dates.py
--rw-r--r--   0        0        0      279 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/diagnoses/__init__.py
--rw-r--r--   0        0        0      409 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/diagnoses/types/__init__.py
--rw-r--r--   0        0        0      958 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/diagnoses/types/diagnosis.py
--rw-r--r--   0        0        0     1904 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/diagnoses/types/diagnosis_create.py
--rw-r--r--   0        0        0      102 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/diagnoses/types/diagnosis_id.py
--rw-r--r--   0        0        0     1974 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/diagnoses/types/diagnosis_type_code.py
--rw-r--r--   0        0        0      903 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py
--rw-r--r--   0        0        0      111 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounter_providers/__init__.py
--rw-r--r--   0        0        0      102 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounter_providers/resources/__init__.py
--rw-r--r--   0        0        0      381 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounter_providers/resources/v_2/__init__.py
--rw-r--r--   0        0        0      516 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0     1988 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py
--rw-r--r--   0        0        0     1092 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py
--rw-r--r--   0        0        0     1260 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py
--rw-r--r--   0        0        0      101 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounter_providers/resources/v_2/types/provider_id.py
--rw-r--r--   0        0        0     1244 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py
--rw-r--r--   0        0        0     1244 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py
--rw-r--r--   0        0        0      111 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/__init__.py
--rw-r--r--   0        0        0      832 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/client.py
--rw-r--r--   0        0        0      102 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/__init__.py
--rw-r--r--   0        0        0     2694 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/__init__.py
--rw-r--r--   0        0        0    36429 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/client.py
--rw-r--r--   0        0        0      202 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/errors/__init__.py
--rw-r--r--   0        0        0      387 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/errors/encounter_external_id_uniqueness_error.py
--rw-r--r--   0        0        0     3794 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/__init__.py
--rw-r--r--   0        0        0      103 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/attachment_id.py
--rw-r--r--   0        0        0     1206 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/attributable_contracting_status_result.py
--rw-r--r--   0        0        0      944 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/base_attachment.py
--rw-r--r--   0        0        0      874 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/clinical_note.py
--rw-r--r--   0        0        0      944 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category.py
--rw-r--r--   0        0        0      894 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category_create.py
--rw-r--r--   0        0        0      659 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/coding_attribution_type.py
--rw-r--r--   0        0        0      713 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/contracting_out_of_of_network_reason.py
--rw-r--r--   0        0        0     2992 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/encounter.py
--rw-r--r--   0        0        0      920 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/encounter_attachment.py
--rw-r--r--   0        0        0      388 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/encounter_attachment_type.py
--rw-r--r--   0        0        0     4498 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/encounter_base.py
--rw-r--r--   0        0        0      889 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/encounter_external_id_uniqueness_error_type.py
--rw-r--r--   0        0        0      885 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/encounter_page.py
--rw-r--r--   0        0        0     1025 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/encounter_sort_options.py
--rw-r--r--   0        0        0      568 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/generate_clinical_notes_pdf_response.py
--rw-r--r--   0        0        0      855 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/in_network_contracting_status_result.py
--rw-r--r--   0        0        0      862 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up.py
--rw-r--r--   0        0        0       88 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up_id.py
--rw-r--r--   0        0        0      969 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/intake_question.py
--rw-r--r--   0        0        0       88 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/intake_question_id.py
--rw-r--r--   0        0        0      891 2023-06-20 17:26:29.360214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/intake_response_and_follow_ups.py
--rw-r--r--   0        0        0     1303 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/intervention.py
--rw-r--r--   0        0        0      865 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/intervention_category.py
--rw-r--r--   0        0        0      855 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/lab.py
--rw-r--r--   0        0        0      457 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/lab_code_type.py
--rw-r--r--   0        0        0      834 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/mark_as_not_billable_response.py
--rw-r--r--   0        0        0      953 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/medication.py
--rw-r--r--   0        0        0      880 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/network_status.py
--rw-r--r--   0        0        0     1164 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/network_status_computation_results.py
--rw-r--r--   0        0        0     2615 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/note_category.py
--rw-r--r--   0        0        0      900 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/out_of_network_contracting_status_result.py
--rw-r--r--   0        0        0     1012 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category.py
--rw-r--r--   0        0        0      885 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category_enum.py
--rw-r--r--   0        0        0       96 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/prior_authorization_number.py
--rw-r--r--   0        0        0       77 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/rx_cui.py
--rw-r--r--   0        0        0      898 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/successful_generate_clinical_notes_pdf_response.py
--rw-r--r--   0        0        0      544 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/synchronicity_type.py
--rw-r--r--   0        0        0      893 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/vitals.py
--rw-r--r--   0        0        0      143 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/era/__init__.py
--rw-r--r--   0        0        0      181 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/era/types/__init__.py
--rw-r--r--   0        0        0      817 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/era/types/era.py
--rw-r--r--   0        0        0      811 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/era/types/era_base.py
--rw-r--r--   0        0        0       96 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/era/types/era_id.py
--rw-r--r--   0        0        0      207 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/expected_network_status/__init__.py
--rw-r--r--   0        0        0     5547 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/expected_network_status/client.py
--rw-r--r--   0        0        0      270 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/expected_network_status/types/__init__.py
--rw-r--r--   0        0        0      729 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/expected_network_status/types/expected_network_status.py
--rw-r--r--   0        0        0      981 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/expected_network_status/types/expected_network_status_response.py
--rw-r--r--   0        0        0      111 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/guarantor/__init__.py
--rw-r--r--   0        0        0      830 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/guarantor/client.py
--rw-r--r--   0        0        0      102 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/guarantor/resources/__init__.py
--rw-r--r--   0        0        0      215 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/guarantor/resources/v_1/__init__.py
--rw-r--r--   0        0        0     8114 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/guarantor/resources/v_1/client.py
--rw-r--r--   0        0        0      300 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/guarantor/resources/v_1/types/__init__.py
--rw-r--r--   0        0        0      867 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/guarantor/resources/v_1/types/guarantor.py
--rw-r--r--   0        0        0     1020 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_base.py
--rw-r--r--   0        0        0      804 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_create.py
--rw-r--r--   0        0        0      102 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_id.py
--rw-r--r--   0        0        0      435 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/individual/__init__.py
--rw-r--r--   0        0        0      602 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/individual/types/__init__.py
--rw-r--r--   0        0        0      871 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/individual/types/gender.py
--rw-r--r--   0        0        0      821 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/individual/types/individual_base.py
--rw-r--r--   0        0        0      103 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/individual/types/individual_id.py
--rw-r--r--   0        0        0      861 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/individual/types/patient.py
--rw-r--r--   0        0        0     1614 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/individual/types/patient_base.py
--rw-r--r--   0        0        0      794 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/individual/types/patient_create.py
--rw-r--r--   0        0        0      972 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/individual/types/subscriber.py
--rw-r--r--   0        0        0     1200 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/individual/types/subscriber_base.py
--rw-r--r--   0        0        0      925 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/individual/types/subscriber_create.py
--rw-r--r--   0        0        0      247 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/insurance_card/__init__.py
--rw-r--r--   0        0        0      352 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/insurance_card/types/__init__.py
--rw-r--r--   0        0        0     1106 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/insurance_card/types/insurance_card.py
--rw-r--r--   0        0        0     1122 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/insurance_card/types/insurance_card_base.py
--rw-r--r--   0        0        0     1026 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/insurance_card/types/insurance_card_create.py
--rw-r--r--   0        0        0      106 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/insurance_card/types/insurance_card_id.py
--rw-r--r--   0        0        0      199 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/invoices/__init__.py
--rw-r--r--   0        0        0      276 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/invoices/types/__init__.py
--rw-r--r--   0        0        0     1397 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/invoices/types/invoice.py
--rw-r--r--   0        0        0      100 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/invoices/types/invoice_id.py
--rw-r--r--   0        0        0      849 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/invoices/types/invoice_item.py
--rw-r--r--   0        0        0      908 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/invoices/types/invoice_status.py
--rw-r--r--   0        0        0      111 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/organization_providers/__init__.py
--rw-r--r--   0        0        0      102 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/organization_providers/resources/__init__.py
--rw-r--r--   0        0        0      501 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/organization_providers/resources/v_2/__init__.py
--rw-r--r--   0        0        0      704 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/organization_providers/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0      334 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/organization_providers/resources/v_2/types/address_type.py
--rw-r--r--   0        0        0      492 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/organization_providers/resources/v_2/types/employment_status.py
--rw-r--r--   0        0        0     2857 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/organization_providers/resources/v_2/types/license_type.py
--rw-r--r--   0        0        0     1562 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider.py
--rw-r--r--   0        0        0     1062 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py
--rw-r--r--   0        0        0     2853 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_base.py
--rw-r--r--   0        0        0      113 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_id.py
--rw-r--r--   0        0        0      510 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/organization_providers/resources/v_2/types/provider_type.py
--rw-r--r--   0        0        0      111 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/patient_payments/__init__.py
--rw-r--r--   0        0        0      102 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/patient_payments/resources/__init__.py
--rw-r--r--   0        0        0      259 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/patient_payments/resources/v_3/__init__.py
--rw-r--r--   0        0        0      370 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/patient_payments/resources/v_3/types/__init__.py
--rw-r--r--   0        0        0     1682 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment.py
--rw-r--r--   0        0        0       88 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_id.py
--rw-r--r--   0        0        0     2035 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_source.py
--rw-r--r--   0        0        0     2055 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_status.py
--rw-r--r--   0        0        0      159 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/payers/__init__.py
--rw-r--r--   0        0        0     4737 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/payers/client.py
--rw-r--r--   0        0        0      205 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/payers/types/__init__.py
--rw-r--r--   0        0        0     1048 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/payers/types/payer.py
--rw-r--r--   0        0        0      865 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/payers/types/payer_page.py
--rw-r--r--   0        0        0      100 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/payers/types/payer_uuid.py
--rw-r--r--   0        0        0      251 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/service_facility/__init__.py
--rw-r--r--   0        0        0      348 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/service_facility/types/__init__.py
--rw-r--r--   0        0        0      975 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/service_facility/types/encounter_service_facility.py
--rw-r--r--   0        0        0     1574 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/service_facility/types/encounter_service_facility_base.py
--rw-r--r--   0        0        0      108 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/service_facility/types/service_facility_id.py
--rw-r--r--   0        0        0      671 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/service_lines/__init__.py
--rw-r--r--   0        0        0      978 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/service_lines/types/__init__.py
--rw-r--r--   0        0        0     6559 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/service_lines/types/denial_reason_content.py
--rw-r--r--   0        0        0     1104 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/service_lines/types/drug_identification.py
--rw-r--r--   0        0        0      996 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/service_lines/types/measurement_unit_code.py
--rw-r--r--   0        0        0     1659 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/service_lines/types/service_id_qualifier.py
--rw-r--r--   0        0        0     1144 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/service_lines/types/service_line.py
--rw-r--r--   0        0        0      960 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/service_lines/types/service_line_adjustment.py
--rw-r--r--   0        0        0      866 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/service_lines/types/service_line_base.py
--rw-r--r--   0        0        0     1899 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/service_lines/types/service_line_base_with_optionals.py
--rw-r--r--   0        0        0     1618 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/service_lines/types/service_line_create.py
--rw-r--r--   0        0        0     1099 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/service_lines/types/service_line_denial_reason.py
--rw-r--r--   0        0        0      917 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/service_lines/types/service_line_era_data.py
--rw-r--r--   0        0        0      177 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/tags/__init__.py
--rw-r--r--   0        0        0      244 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/tags/types/__init__.py
--rw-r--r--   0        0        0      799 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/tags/types/tag.py
--rw-r--r--   0        0        0     1527 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/tags/types/tag_color_enum.py
--rw-r--r--   0        0        0      861 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/tags/types/tag_create.py
--rw-r--r--   0        0        0       77 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/tags/types/tag_id.py
--rw-r--r--   0        0        0      147 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/tasks/__init__.py
--rw-r--r--   0        0        0      822 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/tasks/client.py
--rw-r--r--   0        0        0      102 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/tasks/resources/__init__.py
--rw-r--r--   0        0        0      281 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/tasks/resources/v_3/__init__.py
--rw-r--r--   0        0        0     2562 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/tasks/resources/v_3/client.py
--rw-r--r--   0        0        0      353 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/tasks/resources/v_3/types/__init__.py
--rw-r--r--   0        0        0      872 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/tasks/resources/v_3/types/task_action.py
--rw-r--r--   0        0        0      393 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/tasks/resources/v_3/types/task_action_execution_method.py
--rw-r--r--   0        0        0      808 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/tasks/resources/v_3/types/task_actions.py
--rw-r--r--   0        0        0      115 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/tasks/types/__init__.py
--rw-r--r--   0        0        0       97 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/tasks/types/task_id.py
--rw-r--r--   0        0        0      111 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/users/__init__.py
--rw-r--r--   0        0        0      102 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/users/resources/__init__.py
--rw-r--r--   0        0        0      869 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/users/resources/v_2/__init__.py
--rw-r--r--   0        0        0     1069 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/users/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0      840 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/users/resources/v_2/types/auth_zero_metadata.py
--rw-r--r--   0        0        0      766 2023-06-20 17:26:29.364214 candidhealth-0.3.0/src/candid/resources/users/resources/v_2/types/google_apps_metadata.py
--rw-r--r--   0        0        0      780 2023-06-20 17:26:29.368214 candidhealth-0.3.0/src/candid/resources/users/resources/v_2/types/human_user_metadata.py
--rw-r--r--   0        0        0     1057 2023-06-20 17:26:29.368214 candidhealth-0.3.0/src/candid/resources/users/resources/v_2/types/idp_user_metadata.py
--rw-r--r--   0        0        0      757 2023-06-20 17:26:29.368214 candidhealth-0.3.0/src/candid/resources/users/resources/v_2/types/machine_user_metadata.py
--rw-r--r--   0        0        0      765 2023-06-20 17:26:29.368214 candidhealth-0.3.0/src/candid/resources/users/resources/v_2/types/other_idp_metadata.py
--rw-r--r--   0        0        0       97 2023-06-20 17:26:29.368214 candidhealth-0.3.0/src/candid/resources/users/resources/v_2/types/user_id.py
--rw-r--r--   0        0        0      760 2023-06-20 17:26:29.368214 candidhealth-0.3.0/src/candid/resources/users/resources/v_2/types/user_metadata.py
--rw-r--r--   0        0        0     1111 2023-06-20 17:26:29.368214 candidhealth-0.3.0/src/candid/resources/users/resources/v_2/types/user_v_2.py
--rw-r--r--   0        0        0      111 2023-06-20 17:26:29.368214 candidhealth-0.3.0/src/candid/resources/work_queues/__init__.py
--rw-r--r--   0        0        0      102 2023-06-20 17:26:29.368214 candidhealth-0.3.0/src/candid/resources/work_queues/resources/__init__.py
--rw-r--r--   0        0        0      207 2023-06-20 17:26:29.368214 candidhealth-0.3.0/src/candid/resources/work_queues/resources/v_1/__init__.py
--rw-r--r--   0        0        0      281 2023-06-20 17:26:29.368214 candidhealth-0.3.0/src/candid/resources/work_queues/resources/v_1/types/__init__.py
--rw-r--r--   0        0        0     1074 2023-06-20 17:26:29.368214 candidhealth-0.3.0/src/candid/resources/work_queues/resources/v_1/types/work_queue.py
--rw-r--r--   0        0        0      893 2023-06-20 17:26:29.368214 candidhealth-0.3.0/src/candid/resources/work_queues/resources/v_1/types/work_queue_category.py
--rw-r--r--   0        0        0     1242 2023-06-20 17:26:29.368214 candidhealth-0.3.0/src/candid/resources/work_queues/resources/v_1/types/work_queue_category_type.py
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 candidhealth-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      257 2023-07-03 17:35:04.633181 candidhealth-0.4.0/README.md
+-rw-r--r--   0        0        0      373 2023-07-03 17:35:04.633181 candidhealth-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5887 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/__init__.py
+-rw-r--r--   0        0        0     3166 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/candid_api_client.py
+-rw-r--r--   0        0        0     2511 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/client.py
+-rw-r--r--   0        0        0      348 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      227 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/environment.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/py.typed
+-rw-r--r--   0        0        0     6035 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/auth/__init__.py
+-rw-r--r--   0        0        0      820 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/auth/client.py
+-rw-r--r--   0        0        0      102 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/auth/resources/__init__.py
+-rw-r--r--   0        0        0      304 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/auth/resources/v_2/__init__.py
+-rw-r--r--   0        0        0     3502 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/auth/resources/v_2/client.py
+-rw-r--r--   0        0        0      159 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/auth/resources/v_2/errors/__init__.py
+-rw-r--r--   0        0        0      330 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/auth/resources/v_2/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      333 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/auth/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0      785 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_request.py
+-rw-r--r--   0        0        0      806 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_response.py
+-rw-r--r--   0        0        0      765 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/auth/resources/v_2/types/too_many_requests_error_type.py
+-rw-r--r--   0        0        0      191 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/billing_notes/__init__.py
+-rw-r--r--   0        0        0     2831 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/billing_notes/client.py
+-rw-r--r--   0        0        0      256 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/billing_notes/types/__init__.py
+-rw-r--r--   0        0        0     1136 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/billing_notes/types/billing_note.py
+-rw-r--r--   0        0        0      813 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/billing_notes/types/billing_note_base.py
+-rw-r--r--   0        0        0      104 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/billing_notes/types/billing_note_id.py
+-rw-r--r--   0        0        0      139 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/claims/__init__.py
+-rw-r--r--   0        0        0      164 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/claims/types/__init__.py
+-rw-r--r--   0        0        0     1151 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/claims/types/claim.py
+-rw-r--r--   0        0        0     2605 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/claims/types/claim_status.py
+-rw-r--r--   0        0        0     1537 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/commons/__init__.py
+-rw-r--r--   0        0        0     2295 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0       98 2023-07-03 17:35:04.633181 candidhealth-0.4.0/src/candid/resources/commons/types/claim_id.py
+-rw-r--r--   0        0        0       90 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/content_download_url.py
+-rw-r--r--   0        0        0       76 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/date.py
+-rw-r--r--   0        0        0      822 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/date_range_optional_end.py
+-rw-r--r--   0        0        0       79 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/decimal.py
+-rw-r--r--   0        0        0       77 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/email.py
+-rw-r--r--   0        0        0      485 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/emr_payer_crosswalk.py
+-rw-r--r--   0        0        0       91 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/encounter_external_id.py
+-rw-r--r--   0        0        0      102 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/encounter_id.py
+-rw-r--r--   0        0        0    11148 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/facility_type_code.py
+-rw-r--r--   0        0        0    15447 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/insurance_type_code.py
+-rw-r--r--   0        0        0       79 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/link_url.py
+-rw-r--r--   0        0        0       75 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/npi.py
+-rw-r--r--   0        0        0      105 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/organization_id.py
+-rw-r--r--   0        0        0       81 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/page_token.py
+-rw-r--r--   0        0        0       89 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/patient_external_id.py
+-rw-r--r--   0        0        0     4686 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py
+-rw-r--r--   0        0        0      822 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/phone_number.py
+-rw-r--r--   0        0        0      620 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/phone_number_type.py
+-rw-r--r--   0        0        0    79514 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/procedure_modifier.py
+-rw-r--r--   0        0        0      735 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/region_national.py
+-rw-r--r--   0        0        0      790 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/region_states.py
+-rw-r--r--   0        0        0      633 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/regions.py
+-rw-r--r--   0        0        0      864 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/resource_page.py
+-rw-r--r--   0        0        0      104 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/service_line_id.py
+-rw-r--r--   0        0        0      432 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/service_line_units.py
+-rw-r--r--   0        0        0     5065 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/source_of_payment_code.py
+-rw-r--r--   0        0        0     6264 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/state.py
+-rw-r--r--   0        0        0     1037 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/street_address_base.py
+-rw-r--r--   0        0        0      985 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/street_address_long_zip.py
+-rw-r--r--   0        0        0     1003 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/street_address_short_zip.py
+-rw-r--r--   0        0        0       97 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/user_id.py
+-rw-r--r--   0        0        0       83 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/commons/types/work_queue_id.py
+-rw-r--r--   0        0        0      251 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/contracts/__init__.py
+-rw-r--r--   0        0        0      365 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/contracts/types/__init__.py
+-rw-r--r--   0        0        0      940 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/contracts/types/authorized_signatory.py
+-rw-r--r--   0        0        0     1430 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/contracts/types/contract.py
+-rw-r--r--   0        0        0     1517 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/contracts/types/contract_base.py
+-rw-r--r--   0        0        0      101 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/contracts/types/contract_id.py
+-rw-r--r--   0        0        0      986 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/contracts/types/contract_status.py
+-rw-r--r--   0        0        0     1125 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/credentialing/__init__.py
+-rw-r--r--   0        0        0     1472 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/credentialing/types/__init__.py
+-rw-r--r--   0        0        0      886 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/credentialing/types/credentialed_encounter_status_result.py
+-rw-r--r--   0        0        0      846 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/credentialing/types/credentialing_span_dates.py
+-rw-r--r--   0        0        0      977 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/credentialing/types/credentialing_span_status.py
+-rw-r--r--   0        0        0      809 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/credentialing/types/encounter_credentialing_status_result.py
+-rw-r--r--   0        0        0      864 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/credentialing/types/non_required_credentialing_dates.py
+-rw-r--r--   0        0        0     2210 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/credentialing/types/provider_credentialing_span.py
+-rw-r--r--   0        0        0      958 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/credentialing/types/provider_credentialing_span_base.py
+-rw-r--r--   0        0        0      118 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/credentialing/types/provider_credentialing_span_id.py
+-rw-r--r--   0        0        0      827 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/credentialing/types/required_credentialing_dates.py
+-rw-r--r--   0        0        0      279 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/diagnoses/__init__.py
+-rw-r--r--   0        0        0      409 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/diagnoses/types/__init__.py
+-rw-r--r--   0        0        0      958 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/diagnoses/types/diagnosis.py
+-rw-r--r--   0        0        0     1904 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/diagnoses/types/diagnosis_create.py
+-rw-r--r--   0        0        0      102 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/diagnoses/types/diagnosis_id.py
+-rw-r--r--   0        0        0     1974 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/diagnoses/types/diagnosis_type_code.py
+-rw-r--r--   0        0        0      903 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py
+-rw-r--r--   0        0        0      111 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/encounter_providers/__init__.py
+-rw-r--r--   0        0        0      102 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/encounter_providers/resources/__init__.py
+-rw-r--r--   0        0        0      381 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/encounter_providers/resources/v_2/__init__.py
+-rw-r--r--   0        0        0      516 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0     1988 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py
+-rw-r--r--   0        0        0     1092 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py
+-rw-r--r--   0        0        0     1260 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py
+-rw-r--r--   0        0        0      101 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/encounter_providers/resources/v_2/types/provider_id.py
+-rw-r--r--   0        0        0     1244 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py
+-rw-r--r--   0        0        0     1244 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py
+-rw-r--r--   0        0        0      111 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/encounters/__init__.py
+-rw-r--r--   0        0        0      832 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/encounters/client.py
+-rw-r--r--   0        0        0      102 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/encounters/resources/__init__.py
+-rw-r--r--   0        0        0     2994 2023-07-03 17:35:04.637181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/__init__.py
+-rw-r--r--   0        0        0    37226 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/client.py
+-rw-r--r--   0        0        0      349 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/errors/__init__.py
+-rw-r--r--   0        0        0      387 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/errors/encounter_external_id_uniqueness_error.py
+-rw-r--r--   0        0        0      416 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/errors/encounter_guarantor_missing_contact_info_error.py
+-rw-r--r--   0        0        0     4122 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/__init__.py
+-rw-r--r--   0        0        0      103 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/attachment_id.py
+-rw-r--r--   0        0        0     1206 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/attributable_contracting_status_result.py
+-rw-r--r--   0        0        0      944 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/base_attachment.py
+-rw-r--r--   0        0        0      518 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/billable_status_type.py
+-rw-r--r--   0        0        0      874 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/clinical_note.py
+-rw-r--r--   0        0        0      944 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category.py
+-rw-r--r--   0        0        0      894 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category_create.py
+-rw-r--r--   0        0        0      659 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/coding_attribution_type.py
+-rw-r--r--   0        0        0      713 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/contracting_out_of_of_network_reason.py
+-rw-r--r--   0        0        0     3101 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/encounter.py
+-rw-r--r--   0        0        0      920 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/encounter_attachment.py
+-rw-r--r--   0        0        0      388 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/encounter_attachment_type.py
+-rw-r--r--   0        0        0     4874 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/encounter_base.py
+-rw-r--r--   0        0        0      889 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/encounter_external_id_uniqueness_error_type.py
+-rw-r--r--   0        0        0      806 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/encounter_guarantor_missing_contact_info_error_type.py
+-rw-r--r--   0        0        0      885 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/encounter_page.py
+-rw-r--r--   0        0        0     1025 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/encounter_sort_options.py
+-rw-r--r--   0        0        0      568 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/generate_clinical_notes_pdf_response.py
+-rw-r--r--   0        0        0      855 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/in_network_contracting_status_result.py
+-rw-r--r--   0        0        0      862 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up.py
+-rw-r--r--   0        0        0       88 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up_id.py
+-rw-r--r--   0        0        0      969 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/intake_question.py
+-rw-r--r--   0        0        0       88 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/intake_question_id.py
+-rw-r--r--   0        0        0      891 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/intake_response_and_follow_ups.py
+-rw-r--r--   0        0        0     1303 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/intervention.py
+-rw-r--r--   0        0        0      865 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/intervention_category.py
+-rw-r--r--   0        0        0      855 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/lab.py
+-rw-r--r--   0        0        0      457 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/lab_code_type.py
+-rw-r--r--   0        0        0      834 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/mark_as_not_billable_response.py
+-rw-r--r--   0        0        0      953 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/medication.py
+-rw-r--r--   0        0        0      880 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/network_status.py
+-rw-r--r--   0        0        0     1164 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/network_status_computation_results.py
+-rw-r--r--   0        0        0     2615 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/note_category.py
+-rw-r--r--   0        0        0      900 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/out_of_network_contracting_status_result.py
+-rw-r--r--   0        0        0     1012 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category.py
+-rw-r--r--   0        0        0      885 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category_enum.py
+-rw-r--r--   0        0        0       96 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/prior_authorization_number.py
+-rw-r--r--   0        0        0      710 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/responsible_party_type.py
+-rw-r--r--   0        0        0       77 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/rx_cui.py
+-rw-r--r--   0        0        0      898 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/successful_generate_clinical_notes_pdf_response.py
+-rw-r--r--   0        0        0      544 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/synchronicity_type.py
+-rw-r--r--   0        0        0      893 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/vitals.py
+-rw-r--r--   0        0        0      143 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/era/__init__.py
+-rw-r--r--   0        0        0      181 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/era/types/__init__.py
+-rw-r--r--   0        0        0      817 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/era/types/era.py
+-rw-r--r--   0        0        0      811 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/era/types/era_base.py
+-rw-r--r--   0        0        0       96 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/era/types/era_id.py
+-rw-r--r--   0        0        0      207 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/expected_network_status/__init__.py
+-rw-r--r--   0        0        0     5547 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/expected_network_status/client.py
+-rw-r--r--   0        0        0      270 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/expected_network_status/types/__init__.py
+-rw-r--r--   0        0        0      729 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/expected_network_status/types/expected_network_status.py
+-rw-r--r--   0        0        0      981 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/expected_network_status/types/expected_network_status_response.py
+-rw-r--r--   0        0        0      111 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/guarantor/__init__.py
+-rw-r--r--   0        0        0      830 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/guarantor/client.py
+-rw-r--r--   0        0        0      102 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/guarantor/resources/__init__.py
+-rw-r--r--   0        0        0      417 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/guarantor/resources/v_1/__init__.py
+-rw-r--r--   0        0        0    10165 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/guarantor/resources/v_1/client.py
+-rw-r--r--   0        0        0      202 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/guarantor/resources/v_1/errors/__init__.py
+-rw-r--r--   0        0        0      387 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/guarantor/resources/v_1/errors/encounter_has_existing_guarantor_error.py
+-rw-r--r--   0        0        0      438 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/guarantor/resources/v_1/types/__init__.py
+-rw-r--r--   0        0        0      779 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/guarantor/resources/v_1/types/encounter_has_existing_guarantor_error_type.py
+-rw-r--r--   0        0        0     1092 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/guarantor/resources/v_1/types/guarantor.py
+-rw-r--r--   0        0        0      937 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_base.py
+-rw-r--r--   0        0        0     1206 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_create.py
+-rw-r--r--   0        0        0      102 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_id.py
+-rw-r--r--   0        0        0      435 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/individual/__init__.py
+-rw-r--r--   0        0        0      602 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/individual/types/__init__.py
+-rw-r--r--   0        0        0      871 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/individual/types/gender.py
+-rw-r--r--   0        0        0      821 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/individual/types/individual_base.py
+-rw-r--r--   0        0        0      103 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/individual/types/individual_id.py
+-rw-r--r--   0        0        0     1082 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/individual/types/patient.py
+-rw-r--r--   0        0        0     1513 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/individual/types/patient_base.py
+-rw-r--r--   0        0        0     1192 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/individual/types/patient_create.py
+-rw-r--r--   0        0        0      972 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/individual/types/subscriber.py
+-rw-r--r--   0        0        0     1200 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/individual/types/subscriber_base.py
+-rw-r--r--   0        0        0      925 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/individual/types/subscriber_create.py
+-rw-r--r--   0        0        0      247 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/insurance_card/__init__.py
+-rw-r--r--   0        0        0      352 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/insurance_card/types/__init__.py
+-rw-r--r--   0        0        0     1106 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/insurance_card/types/insurance_card.py
+-rw-r--r--   0        0        0     1203 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/insurance_card/types/insurance_card_base.py
+-rw-r--r--   0        0        0     1153 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/insurance_card/types/insurance_card_create.py
+-rw-r--r--   0        0        0      106 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/insurance_card/types/insurance_card_id.py
+-rw-r--r--   0        0        0      199 2023-07-03 17:35:04.641181 candidhealth-0.4.0/src/candid/resources/invoices/__init__.py
+-rw-r--r--   0        0        0      276 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/invoices/types/__init__.py
+-rw-r--r--   0        0        0     1397 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/invoices/types/invoice.py
+-rw-r--r--   0        0        0      100 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/invoices/types/invoice_id.py
+-rw-r--r--   0        0        0      849 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/invoices/types/invoice_item.py
+-rw-r--r--   0        0        0      908 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/invoices/types/invoice_status.py
+-rw-r--r--   0        0        0      111 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/organization_providers/__init__.py
+-rw-r--r--   0        0        0      102 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/organization_providers/resources/__init__.py
+-rw-r--r--   0        0        0      501 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/organization_providers/resources/v_2/__init__.py
+-rw-r--r--   0        0        0      704 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/organization_providers/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0      334 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/organization_providers/resources/v_2/types/address_type.py
+-rw-r--r--   0        0        0      492 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/organization_providers/resources/v_2/types/employment_status.py
+-rw-r--r--   0        0        0     4304 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/organization_providers/resources/v_2/types/license_type.py
+-rw-r--r--   0        0        0     1562 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider.py
+-rw-r--r--   0        0        0     1062 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py
+-rw-r--r--   0        0        0     2853 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_base.py
+-rw-r--r--   0        0        0      113 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_id.py
+-rw-r--r--   0        0        0      510 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/organization_providers/resources/v_2/types/provider_type.py
+-rw-r--r--   0        0        0      111 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/patient_payments/__init__.py
+-rw-r--r--   0        0        0      102 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/patient_payments/resources/__init__.py
+-rw-r--r--   0        0        0      259 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/patient_payments/resources/v_3/__init__.py
+-rw-r--r--   0        0        0      370 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/patient_payments/resources/v_3/types/__init__.py
+-rw-r--r--   0        0        0     1682 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment.py
+-rw-r--r--   0        0        0       88 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_id.py
+-rw-r--r--   0        0        0     2035 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_source.py
+-rw-r--r--   0        0        0     2055 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_status.py
+-rw-r--r--   0        0        0      159 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/payers/__init__.py
+-rw-r--r--   0        0        0     4737 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/payers/client.py
+-rw-r--r--   0        0        0      205 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/payers/types/__init__.py
+-rw-r--r--   0        0        0     1048 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/payers/types/payer.py
+-rw-r--r--   0        0        0      865 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/payers/types/payer_page.py
+-rw-r--r--   0        0        0      100 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/payers/types/payer_uuid.py
+-rw-r--r--   0        0        0      251 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/service_facility/__init__.py
+-rw-r--r--   0        0        0      348 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/service_facility/types/__init__.py
+-rw-r--r--   0        0        0      975 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/service_facility/types/encounter_service_facility.py
+-rw-r--r--   0        0        0     1574 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/service_facility/types/encounter_service_facility_base.py
+-rw-r--r--   0        0        0      108 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/service_facility/types/service_facility_id.py
+-rw-r--r--   0        0        0      671 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/service_lines/__init__.py
+-rw-r--r--   0        0        0      978 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/service_lines/types/__init__.py
+-rw-r--r--   0        0        0     6559 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/service_lines/types/denial_reason_content.py
+-rw-r--r--   0        0        0     1104 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/service_lines/types/drug_identification.py
+-rw-r--r--   0        0        0      996 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/service_lines/types/measurement_unit_code.py
+-rw-r--r--   0        0        0     1659 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/service_lines/types/service_id_qualifier.py
+-rw-r--r--   0        0        0     1826 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/service_lines/types/service_line.py
+-rw-r--r--   0        0        0      960 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/service_lines/types/service_line_adjustment.py
+-rw-r--r--   0        0        0      866 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/service_lines/types/service_line_base.py
+-rw-r--r--   0        0        0     1899 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/service_lines/types/service_line_base_with_optionals.py
+-rw-r--r--   0        0        0     1952 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/service_lines/types/service_line_create.py
+-rw-r--r--   0        0        0     1099 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/service_lines/types/service_line_denial_reason.py
+-rw-r--r--   0        0        0      917 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/service_lines/types/service_line_era_data.py
+-rw-r--r--   0        0        0      177 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/tags/__init__.py
+-rw-r--r--   0        0        0      244 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/tags/types/__init__.py
+-rw-r--r--   0        0        0      799 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/tags/types/tag.py
+-rw-r--r--   0        0        0     1527 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/tags/types/tag_color_enum.py
+-rw-r--r--   0        0        0      861 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/tags/types/tag_create.py
+-rw-r--r--   0        0        0       77 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/tags/types/tag_id.py
+-rw-r--r--   0        0        0      147 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/tasks/__init__.py
+-rw-r--r--   0        0        0      822 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/tasks/client.py
+-rw-r--r--   0        0        0      102 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/tasks/resources/__init__.py
+-rw-r--r--   0        0        0      281 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/tasks/resources/v_3/__init__.py
+-rw-r--r--   0        0        0     2562 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/tasks/resources/v_3/client.py
+-rw-r--r--   0        0        0      353 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/tasks/resources/v_3/types/__init__.py
+-rw-r--r--   0        0        0      872 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/tasks/resources/v_3/types/task_action.py
+-rw-r--r--   0        0        0      393 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/tasks/resources/v_3/types/task_action_execution_method.py
+-rw-r--r--   0        0        0      808 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/tasks/resources/v_3/types/task_actions.py
+-rw-r--r--   0        0        0      115 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/tasks/types/__init__.py
+-rw-r--r--   0        0        0       97 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/tasks/types/task_id.py
+-rw-r--r--   0        0        0      111 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/work_queues/__init__.py
+-rw-r--r--   0        0        0      102 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/work_queues/resources/__init__.py
+-rw-r--r--   0        0        0      207 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/work_queues/resources/v_1/__init__.py
+-rw-r--r--   0        0        0      281 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/work_queues/resources/v_1/types/__init__.py
+-rw-r--r--   0        0        0     1061 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/work_queues/resources/v_1/types/work_queue.py
+-rw-r--r--   0        0        0      893 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/work_queues/resources/v_1/types/work_queue_category.py
+-rw-r--r--   0        0        0     1242 2023-07-03 17:35:04.645181 candidhealth-0.4.0/src/candid/resources/work_queues/resources/v_1/types/work_queue_category_type.py
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 candidhealth-0.4.0/PKG-INFO
```

### Comparing `candidhealth-0.3.0/src/candid/__init__.py` & `candidhealth-0.4.0/src/candid/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,33 +5,35 @@
     AuthorizedSignatory,
     BillingNote,
     BillingNoteBase,
     BillingNoteId,
     Claim,
     ClaimId,
     ClaimStatus,
-    ContactInfo,
     ContentDownloadUrl,
     Contract,
     ContractBase,
     ContractId,
     ContractStatus,
     CredentialedEncounterStatusResult,
     CredentialingSpanDates,
     CredentialingSpanDates_NonRequiredDates,
     CredentialingSpanDates_RequiredDates,
     CredentialingSpanStatus,
     Date,
+    DateRangeOptionalEnd,
+    Decimal,
     DenialReasonContent,
     Diagnosis,
     DiagnosisCreate,
     DiagnosisId,
     DiagnosisTypeCode,
     DrugIdentification,
     Email,
+    EmrPayerCrosswalk,
     EncounterCredentialingStatusResult,
     EncounterCredentialingStatusResult_Credentialed,
     EncounterCredentialingStatusResult_NotCredentialed,
     EncounterExternalId,
     EncounterId,
     EncounterServiceFacility,
     EncounterServiceFacilityBase,
@@ -101,14 +103,15 @@
     SubscriberBase,
     SubscriberCreate,
     Tag,
     TagColorEnum,
     TagCreate,
     TagId,
     TaskId,
+    UserId,
     WorkQueueId,
     auth,
     billing_notes,
     claims,
     commons,
     contracts,
     credentialing,
@@ -124,46 +127,47 @@
     organization_providers,
     patient_payments,
     payers,
     service_facility,
     service_lines,
     tags,
     tasks,
-    users,
     work_queues,
 )
 
 __all__ = [
     "AuthorizedSignatory",
     "BillingNote",
     "BillingNoteBase",
     "BillingNoteId",
     "CandidApiEnvironment",
     "Claim",
     "ClaimId",
     "ClaimStatus",
-    "ContactInfo",
     "ContentDownloadUrl",
     "Contract",
     "ContractBase",
     "ContractId",
     "ContractStatus",
     "CredentialedEncounterStatusResult",
     "CredentialingSpanDates",
     "CredentialingSpanDates_NonRequiredDates",
     "CredentialingSpanDates_RequiredDates",
     "CredentialingSpanStatus",
     "Date",
+    "DateRangeOptionalEnd",
+    "Decimal",
     "DenialReasonContent",
     "Diagnosis",
     "DiagnosisCreate",
     "DiagnosisId",
     "DiagnosisTypeCode",
     "DrugIdentification",
     "Email",
+    "EmrPayerCrosswalk",
     "EncounterCredentialingStatusResult",
     "EncounterCredentialingStatusResult_Credentialed",
     "EncounterCredentialingStatusResult_NotCredentialed",
     "EncounterExternalId",
     "EncounterId",
     "EncounterServiceFacility",
     "EncounterServiceFacilityBase",
@@ -233,14 +237,15 @@
     "SubscriberBase",
     "SubscriberCreate",
     "Tag",
     "TagColorEnum",
     "TagCreate",
     "TagId",
     "TaskId",
+    "UserId",
     "WorkQueueId",
     "auth",
     "billing_notes",
     "claims",
     "commons",
     "contracts",
     "credentialing",
@@ -256,10 +261,9 @@
     "organization_providers",
     "patient_payments",
     "payers",
     "service_facility",
     "service_lines",
     "tags",
     "tasks",
-    "users",
     "work_queues",
 ]
```

### Comparing `candidhealth-0.3.0/src/candid/candid_api_client.py` & `candidhealth-0.4.0/src/candid/candid_api_client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/client.py` & `candidhealth-0.4.0/src/candid/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/core/datetime_utils.py` & `candidhealth-0.4.0/src/candid/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/core/jsonable_encoder.py` & `candidhealth-0.4.0/src/candid/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/__init__.py` & `candidhealth-0.4.0/src/candid/resources/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,25 +19,26 @@
     organization_providers,
     patient_payments,
     payers,
     service_facility,
     service_lines,
     tags,
     tasks,
-    users,
     work_queues,
 )
 from .billing_notes import BillingNote, BillingNoteBase, BillingNoteId
 from .claims import Claim, ClaimStatus
 from .commons import (
     ClaimId,
-    ContactInfo,
     ContentDownloadUrl,
     Date,
+    DateRangeOptionalEnd,
+    Decimal,
     Email,
+    EmrPayerCrosswalk,
     EncounterExternalId,
     EncounterId,
     FacilityTypeCode,
     InsuranceTypeCode,
     LinkUrl,
     Npi,
     OrganizationId,
@@ -56,14 +57,15 @@
     ServiceLineId,
     ServiceLineUnits,
     SourceOfPaymentCode,
     State,
     StreetAddressBase,
     StreetAddressLongZip,
     StreetAddressShortZip,
+    UserId,
     WorkQueueId,
 )
 from .contracts import AuthorizedSignatory, Contract, ContractBase, ContractId, ContractStatus
 from .credentialing import (
     CredentialedEncounterStatusResult,
     CredentialingSpanDates,
     CredentialingSpanDates_NonRequiredDates,
@@ -116,33 +118,35 @@
     "AuthorizedSignatory",
     "BillingNote",
     "BillingNoteBase",
     "BillingNoteId",
     "Claim",
     "ClaimId",
     "ClaimStatus",
-    "ContactInfo",
     "ContentDownloadUrl",
     "Contract",
     "ContractBase",
     "ContractId",
     "ContractStatus",
     "CredentialedEncounterStatusResult",
     "CredentialingSpanDates",
     "CredentialingSpanDates_NonRequiredDates",
     "CredentialingSpanDates_RequiredDates",
     "CredentialingSpanStatus",
     "Date",
+    "DateRangeOptionalEnd",
+    "Decimal",
     "DenialReasonContent",
     "Diagnosis",
     "DiagnosisCreate",
     "DiagnosisId",
     "DiagnosisTypeCode",
     "DrugIdentification",
     "Email",
+    "EmrPayerCrosswalk",
     "EncounterCredentialingStatusResult",
     "EncounterCredentialingStatusResult_Credentialed",
     "EncounterCredentialingStatusResult_NotCredentialed",
     "EncounterExternalId",
     "EncounterId",
     "EncounterServiceFacility",
     "EncounterServiceFacilityBase",
@@ -212,14 +216,15 @@
     "SubscriberBase",
     "SubscriberCreate",
     "Tag",
     "TagColorEnum",
     "TagCreate",
     "TagId",
     "TaskId",
+    "UserId",
     "WorkQueueId",
     "auth",
     "billing_notes",
     "claims",
     "commons",
     "contracts",
     "credentialing",
@@ -235,10 +240,9 @@
     "organization_providers",
     "patient_payments",
     "payers",
     "service_facility",
     "service_lines",
     "tags",
     "tasks",
-    "users",
     "work_queues",
 ]
```

### Comparing `candidhealth-0.3.0/src/candid/resources/auth/client.py` & `candidhealth-0.4.0/src/candid/resources/auth/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/auth/resources/v_2/client.py` & `candidhealth-0.4.0/src/candid/resources/auth/resources/v_2/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_request.py` & `candidhealth-0.4.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_request.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_response.py` & `candidhealth-0.4.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/auth/resources/v_2/types/too_many_requests_error_type.py` & `candidhealth-0.4.0/src/candid/resources/auth/resources/v_2/types/too_many_requests_error_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/billing_notes/client.py` & `candidhealth-0.4.0/src/candid/resources/billing_notes/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/billing_notes/types/billing_note.py` & `candidhealth-0.4.0/src/candid/resources/billing_notes/types/billing_note.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/billing_notes/types/billing_note_base.py` & `candidhealth-0.4.0/src/candid/resources/billing_notes/types/billing_note_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/claims/types/claim.py` & `candidhealth-0.4.0/src/candid/resources/claims/types/claim.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/claims/types/claim_status.py` & `candidhealth-0.4.0/src/candid/resources/claims/types/claim_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/commons/__init__.py` & `candidhealth-0.4.0/src/candid/resources/commons/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
     ClaimId,
-    ContactInfo,
     ContentDownloadUrl,
     Date,
+    DateRangeOptionalEnd,
+    Decimal,
     Email,
+    EmrPayerCrosswalk,
     EncounterExternalId,
     EncounterId,
     FacilityTypeCode,
     InsuranceTypeCode,
     LinkUrl,
     Npi,
     OrganizationId,
@@ -28,23 +30,26 @@
     ServiceLineId,
     ServiceLineUnits,
     SourceOfPaymentCode,
     State,
     StreetAddressBase,
     StreetAddressLongZip,
     StreetAddressShortZip,
+    UserId,
     WorkQueueId,
 )
 
 __all__ = [
     "ClaimId",
-    "ContactInfo",
     "ContentDownloadUrl",
     "Date",
+    "DateRangeOptionalEnd",
+    "Decimal",
     "Email",
+    "EmrPayerCrosswalk",
     "EncounterExternalId",
     "EncounterId",
     "FacilityTypeCode",
     "InsuranceTypeCode",
     "LinkUrl",
     "Npi",
     "OrganizationId",
@@ -63,9 +68,10 @@
     "ServiceLineId",
     "ServiceLineUnits",
     "SourceOfPaymentCode",
     "State",
     "StreetAddressBase",
     "StreetAddressLongZip",
     "StreetAddressShortZip",
+    "UserId",
     "WorkQueueId",
 ]
```

### Comparing `candidhealth-0.3.0/src/candid/resources/commons/types/__init__.py` & `candidhealth-0.4.0/src/candid/resources/commons/types/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .claim_id import ClaimId
-from .contact_info import ContactInfo
 from .content_download_url import ContentDownloadUrl
 from .date import Date
+from .date_range_optional_end import DateRangeOptionalEnd
+from .decimal import Decimal
 from .email import Email
+from .emr_payer_crosswalk import EmrPayerCrosswalk
 from .encounter_external_id import EncounterExternalId
 from .encounter_id import EncounterId
 from .facility_type_code import FacilityTypeCode
 from .insurance_type_code import InsuranceTypeCode
 from .link_url import LinkUrl
 from .npi import Npi
 from .organization_id import OrganizationId
@@ -25,22 +27,25 @@
 from .service_line_id import ServiceLineId
 from .service_line_units import ServiceLineUnits
 from .source_of_payment_code import SourceOfPaymentCode
 from .state import State
 from .street_address_base import StreetAddressBase
 from .street_address_long_zip import StreetAddressLongZip
 from .street_address_short_zip import StreetAddressShortZip
+from .user_id import UserId
 from .work_queue_id import WorkQueueId
 
 __all__ = [
     "ClaimId",
-    "ContactInfo",
     "ContentDownloadUrl",
     "Date",
+    "DateRangeOptionalEnd",
+    "Decimal",
     "Email",
+    "EmrPayerCrosswalk",
     "EncounterExternalId",
     "EncounterId",
     "FacilityTypeCode",
     "InsuranceTypeCode",
     "LinkUrl",
     "Npi",
     "OrganizationId",
@@ -59,9 +64,10 @@
     "ServiceLineId",
     "ServiceLineUnits",
     "SourceOfPaymentCode",
     "State",
     "StreetAddressBase",
     "StreetAddressLongZip",
     "StreetAddressShortZip",
+    "UserId",
     "WorkQueueId",
 ]
```

### Comparing `candidhealth-0.3.0/src/candid/resources/commons/types/contact_info.py` & `candidhealth-0.4.0/src/candid/resources/commons/types/region_national.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,24 +2,17 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .email import Email
-from .phone_number import PhoneNumber
 
 
-class ContactInfo(pydantic.BaseModel):
-    phone_numbers: typing.List[PhoneNumber]
-    phone_consent: bool
-    email: Email
-    email_consent: bool
-
+class RegionNational(pydantic.BaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `candidhealth-0.3.0/src/candid/resources/commons/types/facility_type_code.py` & `candidhealth-0.4.0/src/candid/resources/commons/types/facility_type_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/commons/types/insurance_type_code.py` & `candidhealth-0.4.0/src/candid/resources/commons/types/insurance_type_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py` & `candidhealth-0.4.0/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/commons/types/phone_number.py` & `candidhealth-0.4.0/src/candid/resources/commons/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/commons/types/phone_number_type.py` & `candidhealth-0.4.0/src/candid/resources/commons/types/phone_number_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/commons/types/procedure_modifier.py` & `candidhealth-0.4.0/src/candid/resources/commons/types/procedure_modifier.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/commons/types/region_national.py` & `candidhealth-0.4.0/src/candid/resources/credentialing/types/non_required_credentialing_dates.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from ...commons.types.date import Date
 
 
-class RegionNational(pydantic.BaseModel):
+class NonRequiredCredentialingDates(pydantic.BaseModel):
+    start_date: typing.Optional[Date]
+    end_date: typing.Optional[Date]
+
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `candidhealth-0.3.0/src/candid/resources/commons/types/region_states.py` & `candidhealth-0.4.0/src/candid/resources/commons/types/region_states.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/commons/types/regions.py` & `candidhealth-0.4.0/src/candid/resources/commons/types/regions.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/commons/types/resource_page.py` & `candidhealth-0.4.0/src/candid/resources/commons/types/resource_page.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/commons/types/source_of_payment_code.py` & `candidhealth-0.4.0/src/candid/resources/commons/types/source_of_payment_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/commons/types/state.py` & `candidhealth-0.4.0/src/candid/resources/commons/types/state.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/commons/types/street_address_base.py` & `candidhealth-0.4.0/src/candid/resources/commons/types/street_address_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/commons/types/street_address_long_zip.py` & `candidhealth-0.4.0/src/candid/resources/commons/types/street_address_long_zip.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/commons/types/street_address_short_zip.py` & `candidhealth-0.4.0/src/candid/resources/commons/types/street_address_short_zip.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/contracts/types/authorized_signatory.py` & `candidhealth-0.4.0/src/candid/resources/contracts/types/authorized_signatory.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/contracts/types/contract.py` & `candidhealth-0.4.0/src/candid/resources/contracts/types/contract.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/contracts/types/contract_base.py` & `candidhealth-0.4.0/src/candid/resources/contracts/types/contract_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/contracts/types/contract_status.py` & `candidhealth-0.4.0/src/candid/resources/contracts/types/contract_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/credentialing/__init__.py` & `candidhealth-0.4.0/src/candid/resources/credentialing/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/credentialing/types/__init__.py` & `candidhealth-0.4.0/src/candid/resources/credentialing/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/credentialing/types/credentialed_encounter_status_result.py` & `candidhealth-0.4.0/src/candid/resources/credentialing/types/credentialed_encounter_status_result.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/credentialing/types/credentialing_span_dates.py` & `candidhealth-0.4.0/src/candid/resources/credentialing/types/credentialing_span_dates.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/credentialing/types/credentialing_span_status.py` & `candidhealth-0.4.0/src/candid/resources/credentialing/types/credentialing_span_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/credentialing/types/encounter_credentialing_status_result.py` & `candidhealth-0.4.0/src/candid/resources/credentialing/types/encounter_credentialing_status_result.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/credentialing/types/non_required_credentialing_dates.py` & `candidhealth-0.4.0/src/candid/resources/service_lines/types/service_line_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.date import Date
+from ...commons.types.procedure_modifier import ProcedureModifier
 
 
-class NonRequiredCredentialingDates(pydantic.BaseModel):
-    start_date: typing.Optional[Date]
-    end_date: typing.Optional[Date]
+class ServiceLineBase(pydantic.BaseModel):
+    modifiers: typing.Optional[typing.List[ProcedureModifier]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.3.0/src/candid/resources/credentialing/types/provider_credentialing_span.py` & `candidhealth-0.4.0/src/candid/resources/credentialing/types/provider_credentialing_span.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/credentialing/types/provider_credentialing_span_base.py` & `candidhealth-0.4.0/src/candid/resources/credentialing/types/provider_credentialing_span_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/credentialing/types/required_credentialing_dates.py` & `candidhealth-0.4.0/src/candid/resources/credentialing/types/required_credentialing_dates.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/diagnoses/types/diagnosis.py` & `candidhealth-0.4.0/src/candid/resources/diagnoses/types/diagnosis.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/diagnoses/types/diagnosis_create.py` & `candidhealth-0.4.0/src/candid/resources/diagnoses/types/diagnosis_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/diagnoses/types/diagnosis_type_code.py` & `candidhealth-0.4.0/src/candid/resources/diagnoses/types/diagnosis_type_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py` & `candidhealth-0.4.0/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py` & `candidhealth-0.4.0/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py` & `candidhealth-0.4.0/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py` & `candidhealth-0.4.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py` & `candidhealth-0.4.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py` & `candidhealth-0.4.0/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py` & `candidhealth-0.4.0/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/client.py` & `candidhealth-0.4.0/src/candid/resources/encounters/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/__init__.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from .errors import EncounterExternalIdUniquenessError
+from .errors import EncounterExternalIdUniquenessError, EncounterGuarantorMissingContactInfoError
 from .types import (
     AttachmentId,
     AttributableContractingStatusResult,
     AttributableContractingStatusResult_InNetwork,
     AttributableContractingStatusResult_OutOfNetwork,
     AttributableContractingStatusResult_Unknown,
     BaseAttachment,
+    BillableStatusType,
     ClinicalNote,
     ClinicalNoteCategory,
     ClinicalNoteCategoryCreate,
     CodingAttributionType,
     ContractingOutOfOfNetworkReason,
     Encounter,
     EncounterAttachment,
     EncounterAttachmentType,
     EncounterBase,
     EncounterExternalIdUniquenessErrorType,
+    EncounterGuarantorMissingContactInfoErrorType,
     EncounterPage,
     EncounterSortOptions,
     GenerateClinicalNotesPdfResponse,
     GenerateClinicalNotesPdfResponse_Success,
     InNetworkContractingStatusResult,
     IntakeFollowUp,
     IntakeFollowUpId,
@@ -37,38 +39,42 @@
     NetworkStatus,
     NetworkStatusComputationResults,
     NoteCategory,
     OutOfNetworkContractingStatusResult,
     PatientHistoryCategory,
     PatientHistoryCategoryEnum,
     PriorAuthorizationNumber,
+    ResponsiblePartyType,
     RxCui,
     SuccessfulGenerateClinicalNotesPdfResponse,
     SynchronicityType,
     Vitals,
 )
 
 __all__ = [
     "AttachmentId",
     "AttributableContractingStatusResult",
     "AttributableContractingStatusResult_InNetwork",
     "AttributableContractingStatusResult_OutOfNetwork",
     "AttributableContractingStatusResult_Unknown",
     "BaseAttachment",
+    "BillableStatusType",
     "ClinicalNote",
     "ClinicalNoteCategory",
     "ClinicalNoteCategoryCreate",
     "CodingAttributionType",
     "ContractingOutOfOfNetworkReason",
     "Encounter",
     "EncounterAttachment",
     "EncounterAttachmentType",
     "EncounterBase",
     "EncounterExternalIdUniquenessError",
     "EncounterExternalIdUniquenessErrorType",
+    "EncounterGuarantorMissingContactInfoError",
+    "EncounterGuarantorMissingContactInfoErrorType",
     "EncounterPage",
     "EncounterSortOptions",
     "GenerateClinicalNotesPdfResponse",
     "GenerateClinicalNotesPdfResponse_Success",
     "InNetworkContractingStatusResult",
     "IntakeFollowUp",
     "IntakeFollowUpId",
@@ -84,12 +90,13 @@
     "NetworkStatus",
     "NetworkStatusComputationResults",
     "NoteCategory",
     "OutOfNetworkContractingStatusResult",
     "PatientHistoryCategory",
     "PatientHistoryCategoryEnum",
     "PriorAuthorizationNumber",
+    "ResponsiblePartyType",
     "RxCui",
     "SuccessfulGenerateClinicalNotesPdfResponse",
     "SynchronicityType",
     "Vitals",
 ]
```

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/client.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,34 +24,37 @@
 from ....commons.types.work_queue_id import WorkQueueId
 from ....diagnoses.types.diagnosis_create import DiagnosisCreate
 from ....diagnoses.types.diagnosis_id import DiagnosisId
 from ....encounter_providers.resources.v_2.types.billing_provider import BillingProvider
 from ....encounter_providers.resources.v_2.types.referring_provider import ReferringProvider
 from ....encounter_providers.resources.v_2.types.rendering_provider import RenderingProvider
 from ....guarantor.resources.v_1.types.guarantor_create import GuarantorCreate
-from ....guarantor.resources.v_1.types.guarantor_id import GuarantorId
 from ....individual.types.patient_create import PatientCreate
 from ....individual.types.subscriber_create import SubscriberCreate
 from ....service_facility.types.encounter_service_facility_base import EncounterServiceFacilityBase
 from ....service_lines.types.service_line_create import ServiceLineCreate
 from ....tags.types.tag_id import TagId
 from .errors.encounter_external_id_uniqueness_error import EncounterExternalIdUniquenessError
+from .errors.encounter_guarantor_missing_contact_info_error import EncounterGuarantorMissingContactInfoError
+from .types.billable_status_type import BillableStatusType
 from .types.clinical_note_category_create import ClinicalNoteCategoryCreate
 from .types.encounter import Encounter
 from .types.encounter_attachment import EncounterAttachment
 from .types.encounter_external_id_uniqueness_error_type import EncounterExternalIdUniquenessErrorType
+from .types.encounter_guarantor_missing_contact_info_error_type import EncounterGuarantorMissingContactInfoErrorType
 from .types.encounter_page import EncounterPage
 from .types.encounter_sort_options import EncounterSortOptions
 from .types.generate_clinical_notes_pdf_response import GenerateClinicalNotesPdfResponse
 from .types.intervention import Intervention
 from .types.mark_as_not_billable_response import MarkAsNotBillableResponse
 from .types.medication import Medication
 from .types.network_status_computation_results import NetworkStatusComputationResults
 from .types.patient_history_category import PatientHistoryCategory
 from .types.prior_authorization_number import PriorAuthorizationNumber
+from .types.responsible_party_type import ResponsiblePartyType
 from .types.synchronicity_type import SynchronicityType
 from .types.vitals import Vitals
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
@@ -72,16 +75,17 @@
         date_of_service_min: typing.Optional[Date] = None,
         date_of_service_max: typing.Optional[Date] = None,
         primary_payer_names: typing.Optional[str] = None,
         search_term: typing.Optional[str] = None,
         external_id: typing.Optional[EncounterExternalId] = None,
         diagnoses_updated_since: typing.Optional[dt.datetime] = None,
         tag_ids: typing.Union[typing.Optional[TagId], typing.List[TagId]],
-        do_not_bill: typing.Optional[bool] = None,
         work_queue_id: typing.Optional[WorkQueueId] = None,
+        billable_status: typing.Optional[BillableStatusType] = None,
+        responsible_party: typing.Optional[ResponsiblePartyType] = None,
     ) -> EncounterPage:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/encounters/v4"),
             params={
                 "limit": limit,
                 "claim_status": claim_status,
@@ -92,16 +96,17 @@
                 "primary_payer_names": primary_payer_names,
                 "search_term": search_term,
                 "external_id": external_id,
                 "diagnoses_updated_since": serialize_datetime(diagnoses_updated_since)
                 if diagnoses_updated_since is not None
                 else None,
                 "tag_ids": tag_ids,
-                "do_not_bill": do_not_bill,
                 "work_queue_id": work_queue_id,
+                "billable_status": billable_status,
+                "responsible_party": responsible_party,
             },
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
@@ -129,56 +134,57 @@
             return pydantic.parse_obj_as(Encounter, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
         self,
         *,
         patient: PatientCreate,
-        patient_is_self_guarantor: typing.Optional[bool] = OMIT,
         billing_provider: BillingProvider,
         rendering_provider: RenderingProvider,
         referring_provider: typing.Optional[ReferringProvider] = OMIT,
         service_facility: typing.Optional[EncounterServiceFacilityBase] = OMIT,
         subscriber_primary: typing.Optional[SubscriberCreate] = OMIT,
         subscriber_secondary: typing.Optional[SubscriberCreate] = OMIT,
         diagnoses: typing.List[DiagnosisCreate],
         clinical_notes: typing.Optional[typing.List[ClinicalNoteCategoryCreate]] = OMIT,
         billing_notes: typing.Optional[typing.List[BillingNoteBase]] = OMIT,
         place_of_service_code: FacilityTypeCode,
         patient_histories: typing.Optional[typing.List[PatientHistoryCategory]] = OMIT,
         service_lines: typing.Optional[typing.List[ServiceLineCreate]] = OMIT,
         guarantor: typing.Optional[GuarantorCreate] = OMIT,
-        external_id: typing.Optional[EncounterExternalId] = OMIT,
+        external_id: EncounterExternalId,
         date_of_service: Date,
         end_date_of_service: typing.Optional[Date] = OMIT,
         prior_authorization_number: typing.Optional[PriorAuthorizationNumber] = OMIT,
         patient_authorized_release: bool,
         benefits_assigned_to_provider: bool,
         provider_accepts_assignment: bool,
         appointment_type: typing.Optional[str] = OMIT,
-        do_not_bill: typing.Optional[bool] = OMIT,
         existing_medications: typing.Optional[typing.List[Medication]] = OMIT,
         vitals: typing.Optional[Vitals] = OMIT,
         interventions: typing.Optional[typing.List[Intervention]] = OMIT,
         pay_to_address: typing.Optional[StreetAddressLongZip] = OMIT,
         synchronicity: typing.Optional[SynchronicityType] = OMIT,
+        billable_status: BillableStatusType,
+        responsible_party: ResponsiblePartyType,
     ) -> Encounter:
         _request: typing.Dict[str, typing.Any] = {
             "patient": patient,
             "billing_provider": billing_provider,
             "rendering_provider": rendering_provider,
             "diagnoses": diagnoses,
             "place_of_service_code": place_of_service_code,
+            "external_id": external_id,
             "date_of_service": date_of_service,
             "patient_authorized_release": patient_authorized_release,
             "benefits_assigned_to_provider": benefits_assigned_to_provider,
             "provider_accepts_assignment": provider_accepts_assignment,
+            "billable_status": billable_status,
+            "responsible_party": responsible_party,
         }
-        if patient_is_self_guarantor is not OMIT:
-            _request["patient_is_self_guarantor"] = patient_is_self_guarantor
         if referring_provider is not OMIT:
             _request["referring_provider"] = referring_provider
         if service_facility is not OMIT:
             _request["service_facility"] = service_facility
         if subscriber_primary is not OMIT:
             _request["subscriber_primary"] = subscriber_primary
         if subscriber_secondary is not OMIT:
@@ -189,24 +195,20 @@
             _request["billing_notes"] = billing_notes
         if patient_histories is not OMIT:
             _request["patient_histories"] = patient_histories
         if service_lines is not OMIT:
             _request["service_lines"] = service_lines
         if guarantor is not OMIT:
             _request["guarantor"] = guarantor
-        if external_id is not OMIT:
-            _request["external_id"] = external_id
         if end_date_of_service is not OMIT:
             _request["end_date_of_service"] = end_date_of_service
         if prior_authorization_number is not OMIT:
             _request["prior_authorization_number"] = prior_authorization_number
         if appointment_type is not OMIT:
             _request["appointment_type"] = appointment_type
-        if do_not_bill is not OMIT:
-            _request["do_not_bill"] = do_not_bill
         if existing_medications is not OMIT:
             _request["existing_medications"] = existing_medications
         if vitals is not OMIT:
             _request["vitals"] = vitals
         if interventions is not OMIT:
             _request["interventions"] = interventions
         if pay_to_address is not OMIT:
@@ -229,29 +231,33 @@
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Encounter, _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "EncounterExternalIdUniquenessError":
                 raise EncounterExternalIdUniquenessError(
                     pydantic.parse_obj_as(EncounterExternalIdUniquenessErrorType, _response_json["content"])  # type: ignore
                 )
+            if _response_json["errorName"] == "EncounterGuarantorMissingContactInfoError":
+                raise EncounterGuarantorMissingContactInfoError(
+                    pydantic.parse_obj_as(EncounterGuarantorMissingContactInfoErrorType, _response_json["content"])  # type: ignore
+                )
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update(
         self,
         encounter_id: EncounterId,
         *,
         prior_authorization_number: typing.Optional[PriorAuthorizationNumber] = OMIT,
         external_id: typing.Optional[EncounterExternalId] = OMIT,
         date_of_service: typing.Optional[Date] = OMIT,
         diagnosis_ids: typing.Optional[typing.List[DiagnosisId]] = OMIT,
         tag_ids: typing.Optional[typing.List[TagId]] = OMIT,
         clinical_notes: typing.Optional[typing.List[ClinicalNoteCategoryCreate]] = OMIT,
         pay_to_address: typing.Optional[StreetAddressLongZip] = OMIT,
-        patient_is_self_guarantor: typing.Optional[bool] = OMIT,
-        guarantor_id: typing.Optional[GuarantorId] = OMIT,
+        billable_status: typing.Optional[BillableStatusType] = OMIT,
+        responsible_party: typing.Optional[ResponsiblePartyType] = OMIT,
         provider_accepts_assignment: typing.Optional[bool] = OMIT,
         benefits_assigned_to_provider: typing.Optional[bool] = OMIT,
         synchronicity: typing.Optional[SynchronicityType] = OMIT,
         place_of_service_code: typing.Optional[FacilityTypeCode] = OMIT,
         appointment_type: typing.Optional[str] = OMIT,
         end_date_of_service: typing.Optional[Date] = OMIT,
     ) -> Encounter:
@@ -266,18 +272,18 @@
             _request["diagnosis_ids"] = diagnosis_ids
         if tag_ids is not OMIT:
             _request["tag_ids"] = tag_ids
         if clinical_notes is not OMIT:
             _request["clinical_notes"] = clinical_notes
         if pay_to_address is not OMIT:
             _request["pay_to_address"] = pay_to_address
-        if patient_is_self_guarantor is not OMIT:
-            _request["patient_is_self_guarantor"] = patient_is_self_guarantor
-        if guarantor_id is not OMIT:
-            _request["guarantor_id"] = guarantor_id
+        if billable_status is not OMIT:
+            _request["billable_status"] = billable_status
+        if responsible_party is not OMIT:
+            _request["responsible_party"] = responsible_party
         if provider_accepts_assignment is not OMIT:
             _request["provider_accepts_assignment"] = provider_accepts_assignment
         if benefits_assigned_to_provider is not OMIT:
             _request["benefits_assigned_to_provider"] = benefits_assigned_to_provider
         if synchronicity is not OMIT:
             _request["synchronicity"] = synchronicity
         if place_of_service_code is not OMIT:
@@ -400,16 +406,17 @@
         date_of_service_min: typing.Optional[Date] = None,
         date_of_service_max: typing.Optional[Date] = None,
         primary_payer_names: typing.Optional[str] = None,
         search_term: typing.Optional[str] = None,
         external_id: typing.Optional[EncounterExternalId] = None,
         diagnoses_updated_since: typing.Optional[dt.datetime] = None,
         tag_ids: typing.Union[typing.Optional[TagId], typing.List[TagId]],
-        do_not_bill: typing.Optional[bool] = None,
         work_queue_id: typing.Optional[WorkQueueId] = None,
+        billable_status: typing.Optional[BillableStatusType] = None,
+        responsible_party: typing.Optional[ResponsiblePartyType] = None,
     ) -> EncounterPage:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", "api/encounters/v4"),
                 params={
                     "limit": limit,
@@ -421,16 +428,17 @@
                     "primary_payer_names": primary_payer_names,
                     "search_term": search_term,
                     "external_id": external_id,
                     "diagnoses_updated_since": serialize_datetime(diagnoses_updated_since)
                     if diagnoses_updated_since is not None
                     else None,
                     "tag_ids": tag_ids,
-                    "do_not_bill": do_not_bill,
                     "work_queue_id": work_queue_id,
+                    "billable_status": billable_status,
+                    "responsible_party": responsible_party,
                 },
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
@@ -459,56 +467,57 @@
             return pydantic.parse_obj_as(Encounter, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
         self,
         *,
         patient: PatientCreate,
-        patient_is_self_guarantor: typing.Optional[bool] = OMIT,
         billing_provider: BillingProvider,
         rendering_provider: RenderingProvider,
         referring_provider: typing.Optional[ReferringProvider] = OMIT,
         service_facility: typing.Optional[EncounterServiceFacilityBase] = OMIT,
         subscriber_primary: typing.Optional[SubscriberCreate] = OMIT,
         subscriber_secondary: typing.Optional[SubscriberCreate] = OMIT,
         diagnoses: typing.List[DiagnosisCreate],
         clinical_notes: typing.Optional[typing.List[ClinicalNoteCategoryCreate]] = OMIT,
         billing_notes: typing.Optional[typing.List[BillingNoteBase]] = OMIT,
         place_of_service_code: FacilityTypeCode,
         patient_histories: typing.Optional[typing.List[PatientHistoryCategory]] = OMIT,
         service_lines: typing.Optional[typing.List[ServiceLineCreate]] = OMIT,
         guarantor: typing.Optional[GuarantorCreate] = OMIT,
-        external_id: typing.Optional[EncounterExternalId] = OMIT,
+        external_id: EncounterExternalId,
         date_of_service: Date,
         end_date_of_service: typing.Optional[Date] = OMIT,
         prior_authorization_number: typing.Optional[PriorAuthorizationNumber] = OMIT,
         patient_authorized_release: bool,
         benefits_assigned_to_provider: bool,
         provider_accepts_assignment: bool,
         appointment_type: typing.Optional[str] = OMIT,
-        do_not_bill: typing.Optional[bool] = OMIT,
         existing_medications: typing.Optional[typing.List[Medication]] = OMIT,
         vitals: typing.Optional[Vitals] = OMIT,
         interventions: typing.Optional[typing.List[Intervention]] = OMIT,
         pay_to_address: typing.Optional[StreetAddressLongZip] = OMIT,
         synchronicity: typing.Optional[SynchronicityType] = OMIT,
+        billable_status: BillableStatusType,
+        responsible_party: ResponsiblePartyType,
     ) -> Encounter:
         _request: typing.Dict[str, typing.Any] = {
             "patient": patient,
             "billing_provider": billing_provider,
             "rendering_provider": rendering_provider,
             "diagnoses": diagnoses,
             "place_of_service_code": place_of_service_code,
+            "external_id": external_id,
             "date_of_service": date_of_service,
             "patient_authorized_release": patient_authorized_release,
             "benefits_assigned_to_provider": benefits_assigned_to_provider,
             "provider_accepts_assignment": provider_accepts_assignment,
+            "billable_status": billable_status,
+            "responsible_party": responsible_party,
         }
-        if patient_is_self_guarantor is not OMIT:
-            _request["patient_is_self_guarantor"] = patient_is_self_guarantor
         if referring_provider is not OMIT:
             _request["referring_provider"] = referring_provider
         if service_facility is not OMIT:
             _request["service_facility"] = service_facility
         if subscriber_primary is not OMIT:
             _request["subscriber_primary"] = subscriber_primary
         if subscriber_secondary is not OMIT:
@@ -519,24 +528,20 @@
             _request["billing_notes"] = billing_notes
         if patient_histories is not OMIT:
             _request["patient_histories"] = patient_histories
         if service_lines is not OMIT:
             _request["service_lines"] = service_lines
         if guarantor is not OMIT:
             _request["guarantor"] = guarantor
-        if external_id is not OMIT:
-            _request["external_id"] = external_id
         if end_date_of_service is not OMIT:
             _request["end_date_of_service"] = end_date_of_service
         if prior_authorization_number is not OMIT:
             _request["prior_authorization_number"] = prior_authorization_number
         if appointment_type is not OMIT:
             _request["appointment_type"] = appointment_type
-        if do_not_bill is not OMIT:
-            _request["do_not_bill"] = do_not_bill
         if existing_medications is not OMIT:
             _request["existing_medications"] = existing_medications
         if vitals is not OMIT:
             _request["vitals"] = vitals
         if interventions is not OMIT:
             _request["interventions"] = interventions
         if pay_to_address is not OMIT:
@@ -560,29 +565,33 @@
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Encounter, _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "EncounterExternalIdUniquenessError":
                 raise EncounterExternalIdUniquenessError(
                     pydantic.parse_obj_as(EncounterExternalIdUniquenessErrorType, _response_json["content"])  # type: ignore
                 )
+            if _response_json["errorName"] == "EncounterGuarantorMissingContactInfoError":
+                raise EncounterGuarantorMissingContactInfoError(
+                    pydantic.parse_obj_as(EncounterGuarantorMissingContactInfoErrorType, _response_json["content"])  # type: ignore
+                )
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update(
         self,
         encounter_id: EncounterId,
         *,
         prior_authorization_number: typing.Optional[PriorAuthorizationNumber] = OMIT,
         external_id: typing.Optional[EncounterExternalId] = OMIT,
         date_of_service: typing.Optional[Date] = OMIT,
         diagnosis_ids: typing.Optional[typing.List[DiagnosisId]] = OMIT,
         tag_ids: typing.Optional[typing.List[TagId]] = OMIT,
         clinical_notes: typing.Optional[typing.List[ClinicalNoteCategoryCreate]] = OMIT,
         pay_to_address: typing.Optional[StreetAddressLongZip] = OMIT,
-        patient_is_self_guarantor: typing.Optional[bool] = OMIT,
-        guarantor_id: typing.Optional[GuarantorId] = OMIT,
+        billable_status: typing.Optional[BillableStatusType] = OMIT,
+        responsible_party: typing.Optional[ResponsiblePartyType] = OMIT,
         provider_accepts_assignment: typing.Optional[bool] = OMIT,
         benefits_assigned_to_provider: typing.Optional[bool] = OMIT,
         synchronicity: typing.Optional[SynchronicityType] = OMIT,
         place_of_service_code: typing.Optional[FacilityTypeCode] = OMIT,
         appointment_type: typing.Optional[str] = OMIT,
         end_date_of_service: typing.Optional[Date] = OMIT,
     ) -> Encounter:
@@ -597,18 +606,18 @@
             _request["diagnosis_ids"] = diagnosis_ids
         if tag_ids is not OMIT:
             _request["tag_ids"] = tag_ids
         if clinical_notes is not OMIT:
             _request["clinical_notes"] = clinical_notes
         if pay_to_address is not OMIT:
             _request["pay_to_address"] = pay_to_address
-        if patient_is_self_guarantor is not OMIT:
-            _request["patient_is_self_guarantor"] = patient_is_self_guarantor
-        if guarantor_id is not OMIT:
-            _request["guarantor_id"] = guarantor_id
+        if billable_status is not OMIT:
+            _request["billable_status"] = billable_status
+        if responsible_party is not OMIT:
+            _request["responsible_party"] = responsible_party
         if provider_accepts_assignment is not OMIT:
             _request["provider_accepts_assignment"] = provider_accepts_assignment
         if benefits_assigned_to_provider is not OMIT:
             _request["benefits_assigned_to_provider"] = benefits_assigned_to_provider
         if synchronicity is not OMIT:
             _request["synchronicity"] = synchronicity
         if place_of_service_code is not OMIT:
```

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/__init__.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 from .attributable_contracting_status_result import (
     AttributableContractingStatusResult,
     AttributableContractingStatusResult_InNetwork,
     AttributableContractingStatusResult_OutOfNetwork,
     AttributableContractingStatusResult_Unknown,
 )
 from .base_attachment import BaseAttachment
+from .billable_status_type import BillableStatusType
 from .clinical_note import ClinicalNote
 from .clinical_note_category import ClinicalNoteCategory
 from .clinical_note_category_create import ClinicalNoteCategoryCreate
 from .coding_attribution_type import CodingAttributionType
 from .contracting_out_of_of_network_reason import ContractingOutOfOfNetworkReason
 from .encounter import Encounter
 from .encounter_attachment import EncounterAttachment
 from .encounter_attachment_type import EncounterAttachmentType
 from .encounter_base import EncounterBase
 from .encounter_external_id_uniqueness_error_type import EncounterExternalIdUniquenessErrorType
+from .encounter_guarantor_missing_contact_info_error_type import EncounterGuarantorMissingContactInfoErrorType
 from .encounter_page import EncounterPage
 from .encounter_sort_options import EncounterSortOptions
 from .generate_clinical_notes_pdf_response import (
     GenerateClinicalNotesPdfResponse,
     GenerateClinicalNotesPdfResponse_Success,
 )
 from .in_network_contracting_status_result import InNetworkContractingStatusResult
@@ -39,36 +41,39 @@
 from .network_status import NetworkStatus
 from .network_status_computation_results import NetworkStatusComputationResults
 from .note_category import NoteCategory
 from .out_of_network_contracting_status_result import OutOfNetworkContractingStatusResult
 from .patient_history_category import PatientHistoryCategory
 from .patient_history_category_enum import PatientHistoryCategoryEnum
 from .prior_authorization_number import PriorAuthorizationNumber
+from .responsible_party_type import ResponsiblePartyType
 from .rx_cui import RxCui
 from .successful_generate_clinical_notes_pdf_response import SuccessfulGenerateClinicalNotesPdfResponse
 from .synchronicity_type import SynchronicityType
 from .vitals import Vitals
 
 __all__ = [
     "AttachmentId",
     "AttributableContractingStatusResult",
     "AttributableContractingStatusResult_InNetwork",
     "AttributableContractingStatusResult_OutOfNetwork",
     "AttributableContractingStatusResult_Unknown",
     "BaseAttachment",
+    "BillableStatusType",
     "ClinicalNote",
     "ClinicalNoteCategory",
     "ClinicalNoteCategoryCreate",
     "CodingAttributionType",
     "ContractingOutOfOfNetworkReason",
     "Encounter",
     "EncounterAttachment",
     "EncounterAttachmentType",
     "EncounterBase",
     "EncounterExternalIdUniquenessErrorType",
+    "EncounterGuarantorMissingContactInfoErrorType",
     "EncounterPage",
     "EncounterSortOptions",
     "GenerateClinicalNotesPdfResponse",
     "GenerateClinicalNotesPdfResponse_Success",
     "InNetworkContractingStatusResult",
     "IntakeFollowUp",
     "IntakeFollowUpId",
@@ -84,12 +89,13 @@
     "NetworkStatus",
     "NetworkStatusComputationResults",
     "NoteCategory",
     "OutOfNetworkContractingStatusResult",
     "PatientHistoryCategory",
     "PatientHistoryCategoryEnum",
     "PriorAuthorizationNumber",
+    "ResponsiblePartyType",
     "RxCui",
     "SuccessfulGenerateClinicalNotesPdfResponse",
     "SynchronicityType",
     "Vitals",
 ]
```

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/attributable_contracting_status_result.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/attributable_contracting_status_result.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/base_attachment.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/base_attachment.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/clinical_note.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/clinical_note.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category_create.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/coding_attribution_type.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/coding_attribution_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/contracting_out_of_of_network_reason.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/contracting_out_of_of_network_reason.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/encounter.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/encounter.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .....billing_notes.types.billing_note import BillingNote
 from .....claims.types.claim import Claim
 from .....commons.types.encounter_id import EncounterId
 from .....commons.types.facility_type_code import FacilityTypeCode
 from .....commons.types.link_url import LinkUrl
 from .....diagnoses.types.diagnosis import Diagnosis
 from .....encounter_providers.resources.v_2.types.encounter_provider import EncounterProvider
+from .....guarantor.resources.v_1.types.guarantor import Guarantor
 from .....individual.types.patient import Patient
 from .....individual.types.subscriber import Subscriber
 from .....patient_payments.resources.v_3.types.patient_payment import PatientPayment
 from .....service_facility.types.encounter_service_facility import EncounterServiceFacility
 from .....tags.types.tag import Tag
 from .....work_queues.resources.v_1.types.work_queue import WorkQueue
 from .clinical_note_category import ClinicalNoteCategory
@@ -25,14 +26,15 @@
 from .patient_history_category import PatientHistoryCategory
 
 
 class Encounter(EncounterBase):
     encounter_id: EncounterId
     claims: typing.List[Claim]
     patient: Patient
+    guarantor: typing.Optional[Guarantor]
     billing_provider: EncounterProvider
     rendering_provider: EncounterProvider
     referring_provider: typing.Optional[EncounterProvider]
     service_facility: EncounterServiceFacility
     subscriber_primary: typing.Optional[Subscriber]
     subscriber_secondary: typing.Optional[Subscriber]
     url: LinkUrl = pydantic.Field(description=("URL that links directly to the claim created in Candid\n"))
```

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/encounter_attachment.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/encounter_attachment.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/encounter_base.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/encounter_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 
 import pydantic
 
 from ......core.datetime_utils import serialize_datetime
 from .....commons.types.date import Date
 from .....commons.types.encounter_external_id import EncounterExternalId
 from .....commons.types.street_address_long_zip import StreetAddressLongZip
+from .billable_status_type import BillableStatusType
 from .intervention import Intervention
 from .medication import Medication
 from .prior_authorization_number import PriorAuthorizationNumber
+from .responsible_party_type import ResponsiblePartyType
 from .synchronicity_type import SynchronicityType
 from .vitals import Vitals
 
 
 class EncounterBase(pydantic.BaseModel):
-    external_id: typing.Optional[EncounterExternalId] = pydantic.Field(
+    external_id: EncounterExternalId = pydantic.Field(
         description=(
             "A client-specified unique ID to associate with this encounter;\n"
             "for example, your internal encounter ID or a Dr. Chrono encounter ID.\n"
             "This field should not contain PHI.\n"
         )
     )
     date_of_service: Date = pydantic.Field(
@@ -63,33 +65,37 @@
             "to be made to you, not them.\n"
             "Box 27 on the CMS-1500 claim form.\n"
         )
     )
     appointment_type: typing.Optional[str] = pydantic.Field(
         description=('Human-readable description of the appointment type (ex: "Acupuncture - Headaches")\n')
     )
-    do_not_bill: typing.Optional[bool] = pydantic.Field(
-        description=(
-            "Should be set to true if Candid should not create or submit a claim but you'd\n"
-            "like us to track this encounter anyway (ex: patient is paying cash)\n"
-        )
-    )
     existing_medications: typing.Optional[typing.List[Medication]]
     vitals: typing.Optional[Vitals]
     interventions: typing.Optional[typing.List[Intervention]]
     pay_to_address: typing.Optional[StreetAddressLongZip]
     synchronicity: typing.Optional[SynchronicityType] = pydantic.Field(
         description=(
             "Whether or not this was a synchronous or asynchronous encounter.\n"
             "Asynchronous encounters occur when providers and patients communicate online using\n"
             "forms, instant messaging, or other pre-recorded digital mediums.\n"
             "Synchronous encounters occur in live, real-time settings where the patient interacts\n"
             "directly with the provider, such as over video or a phone call.\n"
         )
     )
+    billable_status: BillableStatusType = pydantic.Field(
+        description=(
+            "Defines if the Encounter is to be billed by Candid to the responsible_party.\n"
+            "Examples for when this should be set to NOT_BILLABLE include\n"
+            "if the Encounter has not occurred yet or if there is no intention of ever billing the responsible_party.\n"
+        )
+    )
+    responsible_party: ResponsiblePartyType = pydantic.Field(
+        description=("Defines the party to be billed with the initial balance owed on the claim.\n")
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/encounter_external_id_uniqueness_error_type.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/encounter_external_id_uniqueness_error_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/encounter_page.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/encounter_page.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/encounter_sort_options.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/encounter_sort_options.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/generate_clinical_notes_pdf_response.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/generate_clinical_notes_pdf_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/in_network_contracting_status_result.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/in_network_contracting_status_result.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/intake_question.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/intake_question.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/intake_response_and_follow_ups.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/intake_response_and_follow_ups.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/intervention.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/intervention.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/intervention_category.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/intervention_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/lab.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/lab.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/mark_as_not_billable_response.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/mark_as_not_billable_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/medication.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/medication.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/network_status.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/network_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/network_status_computation_results.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/network_status_computation_results.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/note_category.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/note_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/out_of_network_contracting_status_result.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/out_of_network_contracting_status_result.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category_enum.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category_enum.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/successful_generate_clinical_notes_pdf_response.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/successful_generate_clinical_notes_pdf_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/synchronicity_type.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/synchronicity_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/encounters/resources/v_4/types/vitals.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/vitals.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/era/types/era.py` & `candidhealth-0.4.0/src/candid/resources/era/types/era.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/era/types/era_base.py` & `candidhealth-0.4.0/src/candid/resources/era/types/era_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/expected_network_status/client.py` & `candidhealth-0.4.0/src/candid/resources/expected_network_status/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/expected_network_status/types/expected_network_status.py` & `candidhealth-0.4.0/src/candid/resources/expected_network_status/types/expected_network_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/expected_network_status/types/expected_network_status_response.py` & `candidhealth-0.4.0/src/candid/resources/expected_network_status/types/expected_network_status_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/guarantor/client.py` & `candidhealth-0.4.0/src/candid/resources/guarantor/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/guarantor/resources/v_1/client.py` & `candidhealth-0.4.0/src/candid/resources/guarantor/resources/v_1/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,16 +8,20 @@
 import httpx
 import pydantic
 
 from .....core.api_error import ApiError
 from .....core.jsonable_encoder import jsonable_encoder
 from .....core.remove_none_from_headers import remove_none_from_headers
 from .....environment import CandidApiEnvironment
-from ....commons.types.contact_info import ContactInfo
-from ....commons.types.street_address_long_zip import StreetAddressLongZip
+from ....commons.types.email import Email
+from ....commons.types.encounter_id import EncounterId
+from ....commons.types.phone_number import PhoneNumber
+from ....commons.types.street_address_short_zip import StreetAddressShortZip
+from .errors.encounter_has_existing_guarantor_error import EncounterHasExistingGuarantorError
+from .types.encounter_has_existing_guarantor_error_type import EncounterHasExistingGuarantorErrorType
 from .types.guarantor import Guarantor
 from .types.guarantor_create import GuarantorCreate
 from .types.guarantor_id import GuarantorId
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
@@ -25,30 +29,35 @@
 class V1Client:
     def __init__(
         self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    def create(self, *, request: GuarantorCreate) -> Guarantor:
+    def create(self, encounter_id: EncounterId, *, request: GuarantorCreate) -> Guarantor:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/guarantors/v1"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/guarantors/v1/{encounter_id}"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Guarantor, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "EncounterHasExistingGuarantorError":
+                raise EncounterHasExistingGuarantorError(
+                    pydantic.parse_obj_as(EncounterHasExistingGuarantorErrorType, _response_json["content"])  # type: ignore
+                )
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, guarantor_id: GuarantorId) -> Guarantor:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/guarantors/v1/{guarantor_id}"),
             headers=remove_none_from_headers(
@@ -67,29 +76,40 @@
     def update(
         self,
         guarantor_id: GuarantorId,
         *,
         first_name: typing.Optional[str] = OMIT,
         last_name: typing.Optional[str] = OMIT,
         external_id: typing.Optional[str] = OMIT,
-        date_of_birth: dt.date,
-        address: typing.Optional[StreetAddressLongZip] = OMIT,
-        contact_info: typing.Optional[ContactInfo] = OMIT,
+        date_of_birth: typing.Optional[dt.date] = OMIT,
+        address: typing.Optional[StreetAddressShortZip] = OMIT,
+        phone_numbers: typing.Optional[typing.List[PhoneNumber]] = OMIT,
+        phone_consent: typing.Optional[bool] = OMIT,
+        email: typing.Optional[Email] = OMIT,
+        email_consent: typing.Optional[bool] = OMIT,
     ) -> Guarantor:
-        _request: typing.Dict[str, typing.Any] = {"date_of_birth": date_of_birth}
+        _request: typing.Dict[str, typing.Any] = {}
         if first_name is not OMIT:
             _request["first_name"] = first_name
         if last_name is not OMIT:
             _request["last_name"] = last_name
         if external_id is not OMIT:
             _request["external_id"] = external_id
+        if date_of_birth is not OMIT:
+            _request["date_of_birth"] = date_of_birth
         if address is not OMIT:
             _request["address"] = address
-        if contact_info is not OMIT:
-            _request["contact_info"] = contact_info
+        if phone_numbers is not OMIT:
+            _request["phone_numbers"] = phone_numbers
+        if phone_consent is not OMIT:
+            _request["phone_consent"] = phone_consent
+        if email is not OMIT:
+            _request["email"] = email
+        if email_consent is not OMIT:
+            _request["email_consent"] = email_consent
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/guarantors/v1/{guarantor_id}"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
@@ -107,31 +127,36 @@
 class AsyncV1Client:
     def __init__(
         self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    async def create(self, *, request: GuarantorCreate) -> Guarantor:
+    async def create(self, encounter_id: EncounterId, *, request: GuarantorCreate) -> Guarantor:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "api/guarantors/v1"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"api/guarantors/v1/{encounter_id}"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Guarantor, _response_json)  # type: ignore
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "EncounterHasExistingGuarantorError":
+                raise EncounterHasExistingGuarantorError(
+                    pydantic.parse_obj_as(EncounterHasExistingGuarantorErrorType, _response_json["content"])  # type: ignore
+                )
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(self, guarantor_id: GuarantorId) -> Guarantor:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/guarantors/v1/{guarantor_id}"),
@@ -151,29 +176,40 @@
     async def update(
         self,
         guarantor_id: GuarantorId,
         *,
         first_name: typing.Optional[str] = OMIT,
         last_name: typing.Optional[str] = OMIT,
         external_id: typing.Optional[str] = OMIT,
-        date_of_birth: dt.date,
-        address: typing.Optional[StreetAddressLongZip] = OMIT,
-        contact_info: typing.Optional[ContactInfo] = OMIT,
+        date_of_birth: typing.Optional[dt.date] = OMIT,
+        address: typing.Optional[StreetAddressShortZip] = OMIT,
+        phone_numbers: typing.Optional[typing.List[PhoneNumber]] = OMIT,
+        phone_consent: typing.Optional[bool] = OMIT,
+        email: typing.Optional[Email] = OMIT,
+        email_consent: typing.Optional[bool] = OMIT,
     ) -> Guarantor:
-        _request: typing.Dict[str, typing.Any] = {"date_of_birth": date_of_birth}
+        _request: typing.Dict[str, typing.Any] = {}
         if first_name is not OMIT:
             _request["first_name"] = first_name
         if last_name is not OMIT:
             _request["last_name"] = last_name
         if external_id is not OMIT:
             _request["external_id"] = external_id
+        if date_of_birth is not OMIT:
+            _request["date_of_birth"] = date_of_birth
         if address is not OMIT:
             _request["address"] = address
-        if contact_info is not OMIT:
-            _request["contact_info"] = contact_info
+        if phone_numbers is not OMIT:
+            _request["phone_numbers"] = phone_numbers
+        if phone_consent is not OMIT:
+            _request["phone_consent"] = phone_consent
+        if email is not OMIT:
+            _request["email"] = email
+        if email_consent is not OMIT:
+            _request["email_consent"] = email_consent
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/guarantors/v1/{guarantor_id}"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
```

### Comparing `candidhealth-0.3.0/src/candid/resources/guarantor/resources/v_1/types/guarantor.py` & `candidhealth-0.4.0/src/candid/resources/payers/types/payer_page.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ......core.datetime_utils import serialize_datetime
-from .guarantor_base import GuarantorBase
-from .guarantor_id import GuarantorId
+from ....core.datetime_utils import serialize_datetime
+from ...commons.types.resource_page import ResourcePage
+from .payer import Payer
 
 
-class Guarantor(GuarantorBase):
-    guarantor_id: GuarantorId
+class PayerPage(ResourcePage):
+    items: typing.List[Payer]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.3.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_base.py` & `candidhealth-0.4.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ......core.datetime_utils import serialize_datetime
-from .....commons.types.contact_info import ContactInfo
-from .....commons.types.street_address_long_zip import StreetAddressLongZip
+from .....commons.types.street_address_short_zip import StreetAddressShortZip
 
 
 class GuarantorBase(pydantic.BaseModel):
     first_name: str
     last_name: str
     external_id: str
     date_of_birth: dt.date
-    address: StreetAddressLongZip
-    contact_info: ContactInfo
+    address: StreetAddressShortZip
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.3.0/src/candid/resources/guarantor/resources/v_1/types/guarantor_create.py` & `candidhealth-0.4.0/src/candid/resources/tags/types/tag.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ......core.datetime_utils import serialize_datetime
-from .guarantor_base import GuarantorBase
+from ....core.datetime_utils import serialize_datetime
+from .tag_create import TagCreate
 
 
-class GuarantorCreate(GuarantorBase):
+class Tag(TagCreate):
+    creator_id: str
+
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `candidhealth-0.3.0/src/candid/resources/individual/types/__init__.py` & `candidhealth-0.4.0/src/candid/resources/individual/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/individual/types/gender.py` & `candidhealth-0.4.0/src/candid/resources/individual/types/gender.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/individual/types/individual_base.py` & `candidhealth-0.4.0/src/candid/resources/individual/types/individual_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/individual/types/patient.py` & `candidhealth-0.4.0/src/candid/resources/guarantor/resources/v_1/types/encounter_has_existing_guarantor_error_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .individual_id import IndividualId
-from .patient_base import PatientBase
+import pydantic
 
+from ......core.datetime_utils import serialize_datetime
 
-class Patient(PatientBase):
-    individual_id: IndividualId
+
+class EncounterHasExistingGuarantorErrorType(pydantic.BaseModel):
+    message: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `candidhealth-0.3.0/src/candid/resources/individual/types/patient_base.py` & `candidhealth-0.4.0/src/candid/resources/individual/types/subscriber_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import pydantic
-
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.contact_info import ContactInfo
 from ...commons.types.date import Date
+from ...commons.types.patient_relationship_to_insured_code_all import PatientRelationshipToInsuredCodeAll
 from ...commons.types.street_address_short_zip import StreetAddressShortZip
 from .individual_base import IndividualBase
 
 
-class PatientBase(IndividualBase):
-    external_id: str = pydantic.Field(
-        description=(
-            "Another ID you want to associate with this patient.\n"
-            "For example, your internal patient ID or a Dr. Chrono patient ID. Box 1a on the CMS-1500 claim form\n"
-        )
-    )
-    date_of_birth: Date = pydantic.Field(
-        description=(
-            "Box 3 on the CMS-1500 claim form. The date format should be in ISO 8601 date; formatted YYYY-MM-DD (i.e. 2012-02-01)\n"
-        )
-    )
-    address: StreetAddressShortZip = pydantic.Field(description=("Box 5 on the CMS-1500 claim form.\n"))
-    contact_info: typing.Optional[ContactInfo]
+class SubscriberBase(IndividualBase):
+    patient_relationship_to_subscriber_code: PatientRelationshipToInsuredCodeAll
+    date_of_birth: typing.Optional[Date]
+    address: typing.Optional[StreetAddressShortZip]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.3.0/src/candid/resources/individual/types/patient_create.py` & `candidhealth-0.4.0/src/candid/resources/service_lines/types/service_line_denial_reason.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+import pydantic
+
 from ....core.datetime_utils import serialize_datetime
-from .patient_base import PatientBase
+from .denial_reason_content import DenialReasonContent
+
+
+class ServiceLineDenialReason(pydantic.BaseModel):
+    """
+    The reason a given service line was denied within a given time range.
+    A service line may be denied for different reasons over time, but only one reason at a time.
+    """
 
+    reason: typing.Optional[DenialReasonContent] = pydantic.Field(description=("Text of the denial reason\n"))
 
-class PatientCreate(PatientBase):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `candidhealth-0.3.0/src/candid/resources/individual/types/subscriber.py` & `candidhealth-0.4.0/src/candid/resources/individual/types/subscriber.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/individual/types/subscriber_base.py` & `candidhealth-0.4.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ...commons.types.date import Date
-from ...commons.types.patient_relationship_to_insured_code_all import PatientRelationshipToInsuredCodeAll
-from ...commons.types.street_address_short_zip import StreetAddressShortZip
-from .individual_base import IndividualBase
+import pydantic
 
+from ......core.datetime_utils import serialize_datetime
+from .....commons.types.street_address_long_zip import StreetAddressLongZip
+from .address_type import AddressType
 
-class SubscriberBase(IndividualBase):
-    patient_relationship_to_subscriber_code: PatientRelationshipToInsuredCodeAll
-    date_of_birth: typing.Optional[Date]
-    address: typing.Optional[StreetAddressShortZip]
+
+class OrganizationProviderAddress(pydantic.BaseModel):
+    address: StreetAddressLongZip = pydantic.Field(description=("The address of the provider\n"))
+    address_type: AddressType = pydantic.Field(description=("The address type of the provider\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `candidhealth-0.3.0/src/candid/resources/individual/types/subscriber_create.py` & `candidhealth-0.4.0/src/candid/resources/individual/types/subscriber_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/insurance_card/types/insurance_card.py` & `candidhealth-0.4.0/src/candid/resources/insurance_card/types/insurance_card.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/insurance_card/types/insurance_card_base.py` & `candidhealth-0.4.0/src/candid/resources/insurance_card/types/insurance_card_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from ...commons.types.insurance_type_code import InsuranceTypeCode
 from ...commons.types.source_of_payment_code import SourceOfPaymentCode
 
 
 class InsuranceCardBase(pydantic.BaseModel):
     group_number: typing.Optional[str] = pydantic.Field(description=("Box 11 on the CMS-1500 claim form.\n"))
     plan_name: typing.Optional[str] = pydantic.Field(description=("Box 11c on the CMS-1500 claim form.\n"))
     plan_type: typing.Optional[SourceOfPaymentCode]
-    insurance_type: typing.Optional[str]
+    insurance_type: typing.Optional[InsuranceTypeCode]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.3.0/src/candid/resources/insurance_card/types/insurance_card_create.py` & `candidhealth-0.4.0/src/candid/resources/commons/types/date_range_optional_end.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+import pydantic
+
 from ....core.datetime_utils import serialize_datetime
-from .insurance_card_base import InsuranceCardBase
+from .date import Date
 
 
-class InsuranceCardCreate(InsuranceCardBase):
-    member_id: str
-    payer_name: str
-    payer_id: str
-    rx_bin: typing.Optional[str]
-    rx_pcn: typing.Optional[str]
-    image_url_front: typing.Optional[str]
-    image_url_back: typing.Optional[str]
+class DateRangeOptionalEnd(pydantic.BaseModel):
+    start_date: Date
+    end_date: typing.Optional[Date]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `candidhealth-0.3.0/src/candid/resources/invoices/types/invoice.py` & `candidhealth-0.4.0/src/candid/resources/invoices/types/invoice.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/invoices/types/invoice_item.py` & `candidhealth-0.4.0/src/candid/resources/invoices/types/invoice_item.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/invoices/types/invoice_status.py` & `candidhealth-0.4.0/src/candid/resources/invoices/types/invoice_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/organization_providers/resources/v_2/types/__init__.py` & `candidhealth-0.4.0/src/candid/resources/organization_providers/resources/v_2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/organization_providers/resources/v_2/types/license_type.py` & `candidhealth-0.4.0/src/candid/resources/organization_providers/resources/v_2/types/license_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,14 +24,26 @@
     PHD = "PHD"
     PSYD = "PSYD"
     LMSW = "LMSW"
     LMHC = "LMHC"
     OTHER_MASTERS = "OTHER_MASTERS"
     BCBA = "BCBA"
     UNKNOWN = "UNKNOWN"
+    RPH = "RPH"
+    PHT = "PHT"
+    LAC = "LAC"
+    LMT = "LMT"
+    DC = "DC"
+    ND = "ND"
+    MA = "MA"
+    PT = "PT"
+    IBCLC = "IBCLC"
+    RN = "RN"
+    DPT = "DPT"
+    LCMHC = "LCMHC"
 
     def visit(
         self,
         md: typing.Callable[[], T_Result],
         np: typing.Callable[[], T_Result],
         pa: typing.Callable[[], T_Result],
         lmft: typing.Callable[[], T_Result],
@@ -48,14 +60,26 @@
         phd: typing.Callable[[], T_Result],
         psyd: typing.Callable[[], T_Result],
         lmsw: typing.Callable[[], T_Result],
         lmhc: typing.Callable[[], T_Result],
         other_masters: typing.Callable[[], T_Result],
         bcba: typing.Callable[[], T_Result],
         unknown: typing.Callable[[], T_Result],
+        rph: typing.Callable[[], T_Result],
+        pht: typing.Callable[[], T_Result],
+        lac: typing.Callable[[], T_Result],
+        lmt: typing.Callable[[], T_Result],
+        dc: typing.Callable[[], T_Result],
+        nd: typing.Callable[[], T_Result],
+        ma: typing.Callable[[], T_Result],
+        pt: typing.Callable[[], T_Result],
+        ibclc: typing.Callable[[], T_Result],
+        rn: typing.Callable[[], T_Result],
+        dpt: typing.Callable[[], T_Result],
+        lcmhc: typing.Callable[[], T_Result],
     ) -> T_Result:
         if self is LicenseType.MD:
             return md()
         if self is LicenseType.NP:
             return np()
         if self is LicenseType.PA:
             return pa()
@@ -91,7 +115,31 @@
             return lmhc()
         if self is LicenseType.OTHER_MASTERS:
             return other_masters()
         if self is LicenseType.BCBA:
             return bcba()
         if self is LicenseType.UNKNOWN:
             return unknown()
+        if self is LicenseType.RPH:
+            return rph()
+        if self is LicenseType.PHT:
+            return pht()
+        if self is LicenseType.LAC:
+            return lac()
+        if self is LicenseType.LMT:
+            return lmt()
+        if self is LicenseType.DC:
+            return dc()
+        if self is LicenseType.ND:
+            return nd()
+        if self is LicenseType.MA:
+            return ma()
+        if self is LicenseType.PT:
+            return pt()
+        if self is LicenseType.IBCLC:
+            return ibclc()
+        if self is LicenseType.RN:
+            return rn()
+        if self is LicenseType.DPT:
+            return dpt()
+        if self is LicenseType.LCMHC:
+            return lcmhc()
```

### Comparing `candidhealth-0.3.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider.py` & `candidhealth-0.4.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py` & `candidhealth-0.4.0/src/candid/resources/encounters/resources/v_4/types/encounter_guarantor_missing_contact_info_error_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,21 +2,18 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ......core.datetime_utils import serialize_datetime
-from .....commons.types.street_address_long_zip import StreetAddressLongZip
-from .address_type import AddressType
 
 
-class OrganizationProviderAddress(pydantic.BaseModel):
-    address: StreetAddressLongZip = pydantic.Field(description=("The address of the provider\n"))
-    address_type: AddressType = pydantic.Field(description=("The address type of the provider\n"))
+class EncounterGuarantorMissingContactInfoErrorType(pydantic.BaseModel):
+    missing_fields: typing.List[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.3.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_base.py` & `candidhealth-0.4.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment.py` & `candidhealth-0.4.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_source.py` & `candidhealth-0.4.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_source.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_status.py` & `candidhealth-0.4.0/src/candid/resources/patient_payments/resources/v_3/types/patient_payment_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/payers/client.py` & `candidhealth-0.4.0/src/candid/resources/payers/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/payers/types/payer.py` & `candidhealth-0.4.0/src/candid/resources/payers/types/payer.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/payers/types/payer_page.py` & `candidhealth-0.4.0/src/candid/resources/tags/types/tag_create.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+import pydantic
+
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.resource_page import ResourcePage
-from .payer import Payer
+from .tag_color_enum import TagColorEnum
+from .tag_id import TagId
 
 
-class PayerPage(ResourcePage):
-    items: typing.List[Payer]
+class TagCreate(pydantic.BaseModel):
+    tag_id: TagId
+    description: str
+    color: TagColorEnum
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `candidhealth-0.3.0/src/candid/resources/service_facility/types/encounter_service_facility.py` & `candidhealth-0.4.0/src/candid/resources/service_facility/types/encounter_service_facility.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/service_facility/types/encounter_service_facility_base.py` & `candidhealth-0.4.0/src/candid/resources/service_facility/types/encounter_service_facility_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/service_lines/__init__.py` & `candidhealth-0.4.0/src/candid/resources/service_lines/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/service_lines/types/__init__.py` & `candidhealth-0.4.0/src/candid/resources/service_lines/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/service_lines/types/denial_reason_content.py` & `candidhealth-0.4.0/src/candid/resources/service_lines/types/denial_reason_content.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/service_lines/types/drug_identification.py` & `candidhealth-0.4.0/src/candid/resources/service_lines/types/drug_identification.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/service_lines/types/measurement_unit_code.py` & `candidhealth-0.4.0/src/candid/resources/service_lines/types/measurement_unit_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/service_lines/types/service_id_qualifier.py` & `candidhealth-0.4.0/src/candid/resources/service_lines/types/service_id_qualifier.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/service_lines/types/service_line.py` & `candidhealth-0.4.0/src/candid/resources/service_lines/types/service_line.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,41 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+import pydantic
+
 from ....core.datetime_utils import serialize_datetime
 from ...commons.types.claim_id import ClaimId
+from ...commons.types.date_range_optional_end import DateRangeOptionalEnd
+from ...commons.types.decimal import Decimal
 from ...commons.types.service_line_id import ServiceLineId
 from ...commons.types.service_line_units import ServiceLineUnits
 from .service_line_base_with_optionals import ServiceLineBaseWithOptionals
 
 
 class ServiceLine(ServiceLineBaseWithOptionals):
     service_line_id: ServiceLineId
     procedure_code: str
-    quantity: str
+    quantity: Decimal = pydantic.Field(
+        description=(
+            "String representation of a Decimal that can be parsed by most libraries.\n"
+            "A ServiceLine quantity cannot contain more than one digit of precision.\n"
+            "Example: 1.1 is valid, 1.11 is not.\n"
+        )
+    )
     units: ServiceLineUnits
     claim_id: ClaimId
+    date_of_service_range: DateRangeOptionalEnd = pydantic.Field(
+        description=(
+            "A range of dates of service for this service line. If the service line is for a single date, the end date\n"
+            "will be empty.\n"
+        )
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.3.0/src/candid/resources/service_lines/types/service_line_adjustment.py` & `candidhealth-0.4.0/src/candid/resources/service_lines/types/service_line_adjustment.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/service_lines/types/service_line_base.py` & `candidhealth-0.4.0/src/candid/resources/individual/types/patient.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import pydantic
-
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.procedure_modifier import ProcedureModifier
+from ...commons.types.email import Email
+from ...commons.types.phone_number import PhoneNumber
+from .individual_id import IndividualId
+from .patient_base import PatientBase
 
 
-class ServiceLineBase(pydantic.BaseModel):
-    modifiers: typing.Optional[typing.List[ProcedureModifier]]
+class Patient(PatientBase):
+    individual_id: IndividualId
+    phone_numbers: typing.List[PhoneNumber]
+    phone_consent: bool
+    email: typing.Optional[Email]
+    email_consent: bool
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `candidhealth-0.3.0/src/candid/resources/service_lines/types/service_line_base_with_optionals.py` & `candidhealth-0.4.0/src/candid/resources/service_lines/types/service_line_base_with_optionals.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/service_lines/types/service_line_create.py` & `candidhealth-0.4.0/src/candid/resources/service_lines/types/service_line_create.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,29 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from ...commons.types.decimal import Decimal
 from ...commons.types.service_line_units import ServiceLineUnits
 from .drug_identification import DrugIdentification
 from .service_line_base import ServiceLineBase
 
 
 class ServiceLineCreate(ServiceLineBase):
     procedure_code: str
-    quantity: str
+    quantity: Decimal = pydantic.Field(
+        description=(
+            "String representation of a Decimal that can be parsed by most libraries.\n"
+            "A ServiceLine quantity cannot contain more than one digit of precision.\n"
+            "Example: 1.1 is valid, 1.11 is not.\n"
+        )
+    )
     units: ServiceLineUnits
     charge_amount_cents: typing.Optional[int] = pydantic.Field(
         description=(
             "The total amount charged for this service line taking quantity into account. For example, if a single unit\n"
             "costs 100 cents and 2 units were rendered, the charge_amount_cents should be 200. Should be greater than or\n"
             "equal to 0.\n"
         )
```

### Comparing `candidhealth-0.3.0/src/candid/resources/service_lines/types/service_line_denial_reason.py` & `candidhealth-0.4.0/src/candid/resources/work_queues/resources/v_1/types/work_queue.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ....core.datetime_utils import serialize_datetime
-from .denial_reason_content import DenialReasonContent
+from ......core.datetime_utils import serialize_datetime
+from .....commons.types.user_id import UserId
+from .....commons.types.work_queue_id import WorkQueueId
+from .work_queue_category import WorkQueueCategory
 
 
-class ServiceLineDenialReason(pydantic.BaseModel):
-    """
-    The reason a given service line was denied within a given time range.
-    A service line may be denied for different reasons over time, but only one reason at a time.
-    """
-
-    reason: typing.Optional[DenialReasonContent] = pydantic.Field(description=("Text of the denial reason\n"))
+class WorkQueue(pydantic.BaseModel):
+    work_queue_id: WorkQueueId
+    display_name: str
+    description: typing.Optional[str]
+    category: WorkQueueCategory
+    created_at: dt.datetime
+    created_by: UserId
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.3.0/src/candid/resources/service_lines/types/service_line_era_data.py` & `candidhealth-0.4.0/src/candid/resources/service_lines/types/service_line_era_data.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/tags/types/tag.py` & `candidhealth-0.4.0/src/candid/resources/work_queues/resources/v_1/types/work_queue_category.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .tag_create import TagCreate
+import pydantic
 
+from ......core.datetime_utils import serialize_datetime
+from .work_queue_category_type import WorkQueueCategoryType
 
-class Tag(TagCreate):
-    creator_id: str
+
+class WorkQueueCategory(pydantic.BaseModel):
+    type: WorkQueueCategoryType
+    display_name: str
+    description: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `candidhealth-0.3.0/src/candid/resources/tags/types/tag_color_enum.py` & `candidhealth-0.4.0/src/candid/resources/tags/types/tag_color_enum.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/tags/types/tag_create.py` & `candidhealth-0.4.0/src/candid/resources/tasks/resources/v_3/types/task_action.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ....core.datetime_utils import serialize_datetime
-from .tag_color_enum import TagColorEnum
-from .tag_id import TagId
+from ......core.datetime_utils import serialize_datetime
+from .task_action_execution_method import TaskActionExecutionMethod
 
 
-class TagCreate(pydantic.BaseModel):
-    tag_id: TagId
-    description: str
-    color: TagColorEnum
+class TaskAction(pydantic.BaseModel):
+    display_name: str
+    execution_method: TaskActionExecutionMethod
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.3.0/src/candid/resources/tasks/client.py` & `candidhealth-0.4.0/src/candid/resources/tasks/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/tasks/resources/v_3/client.py` & `candidhealth-0.4.0/src/candid/resources/tasks/resources/v_3/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/src/candid/resources/tasks/resources/v_3/types/task_action.py` & `candidhealth-0.4.0/src/candid/resources/tasks/resources/v_3/types/task_actions.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ......core.datetime_utils import serialize_datetime
-from .task_action_execution_method import TaskActionExecutionMethod
+from .task_action import TaskAction
 
 
-class TaskAction(pydantic.BaseModel):
-    display_name: str
-    execution_method: TaskActionExecutionMethod
+class TaskActions(pydantic.BaseModel):
+    actions: typing.List[TaskAction]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.3.0/src/candid/resources/users/resources/v_2/types/auth_zero_metadata.py` & `candidhealth-0.4.0/src/candid/resources/guarantor/resources/v_1/types/guarantor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import pydantic
-
 from ......core.datetime_utils import serialize_datetime
+from .....commons.types.email import Email
+from .....commons.types.phone_number import PhoneNumber
+from .guarantor_base import GuarantorBase
+from .guarantor_id import GuarantorId
 
 
-class AuthZeroMetadata(pydantic.BaseModel):
-    auth_0_id: str = pydantic.Field(alias="auth0_id")
+class Guarantor(GuarantorBase):
+    guarantor_id: GuarantorId
+    phone_numbers: typing.List[PhoneNumber]
+    phone_consent: bool
+    email: typing.Optional[Email]
+    email_consent: bool
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.3.0/src/candid/resources/work_queues/resources/v_1/types/work_queue_category_type.py` & `candidhealth-0.4.0/src/candid/resources/work_queues/resources/v_1/types/work_queue_category_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.3.0/PKG-INFO` & `candidhealth-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: candidhealth
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

