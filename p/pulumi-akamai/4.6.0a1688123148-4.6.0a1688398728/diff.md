# Comparing `tmp/pulumi_akamai-4.6.0a1688123148.tar.gz` & `tmp/pulumi_akamai-4.6.0a1688398728.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_akamai-4.6.0a1688123148.tar", last modified: Fri Jun 30 11:10:27 2023, max compression
+gzip compressed data, was "pulumi_akamai-4.6.0a1688398728.tar", last modified: Mon Jul  3 15:43:49 2023, max compression
```

## Comparing `pulumi_akamai-4.6.0a1688123148.tar` & `pulumi_akamai-4.6.0a1688398728.tar`

### file list

```diff
@@ -1,246 +1,247 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:10:27.014758 pulumi_akamai-4.6.0a1688123148/
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-30 11:10:27.014758 pulumi_akamai-4.6.0a1688123148/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:10:27.010758 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/
--rw-r--r--   0 runner    (1001) docker     (123)    27467 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1554270 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    21333 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_advanced_settings_evasive_path_match.py
--rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_advanced_settings_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_advanced_settings_pragma_header.py
--rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_advanced_settings_prefetch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_api_constraints_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12592 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_api_request_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    14951 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_attack_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_by_pass_network_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    20518 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_configuration_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_custom_deny.py
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_custom_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12783 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_custom_rule_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    17001 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_eval_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_eval_penalty_box.py
--rw-r--r--   0 runner    (1001) docker     (123)    14538 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_eval_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    17481 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_ip_geo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_ip_geo_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_malware_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_malware_policy_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_malware_policy_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_malware_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_match_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_match_target_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    12987 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_penalty_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_rate_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_rate_policy_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_rate_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_reputation_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_reputation_profile_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    14387 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_reputation_profile_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_reputation_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    14063 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_rule_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)    17082 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_security_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_security_policy_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_selected_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_siem_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    19373 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_slow_post.py
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_slow_post_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_threat_intel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_version_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_waf_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_waf_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_wap_selected_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/appsec_advanced_settings_attack_payload_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11290 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/appsec_advanced_settings_request_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    19609 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/cloudlets_application_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/cloudlets_application_load_balancer_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19277 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/cloudlets_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/cloudlets_policy_activation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:10:27.010758 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    14717 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/cp_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    47004 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/cps_dv_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/cps_dv_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    44892 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/cps_third_party_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)    27347 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/cps_upload_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    58490 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/datastream.py
--rw-r--r--   0 runner    (1001) docker     (123)    78637 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/dns_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    21162 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/dns_zone.py
--rw-r--r--   0 runner    (1001) docker     (123)    22811 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edge_host_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    18627 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edge_kv.py
--rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edge_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edge_workers_activation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:10:27.010758 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edgedns/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edgedns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edgedns/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    78833 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edgedns/dns_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    21348 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edgedns/dns_zone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edgedns/get_authorities_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edgedns/get_dns_record_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edgedns/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edgekv_group_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_advanced_settings_evasive_path_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_advanced_settings_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_advanced_settings_pragma_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_advanced_settings_prefetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_api_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_api_request_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_attack_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_bypass_network_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_configuration_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_contracts_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_custom_deny.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_custom_rule_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_custom_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_eval_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_eval_penalty_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_eval_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_export_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_failover_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_hostname_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_hostname_coverage_match_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_hostname_coverage_overlapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_ip_geo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_malware_content_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_malware_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_malware_policy_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_match_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_penalty_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_rate_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_rate_policy_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_reputation_profile_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_reputation_profile_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_reputation_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_rule_upgrade_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_security_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9257 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_security_policy_protections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_selectable_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_selected_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_siem_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_siem_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_slow_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_threat_intel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_tuning_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_version_notes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_waf_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_wap_selected_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_appsec_advanced_settings_attack_payload_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_appsec_advanced_settings_request_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_authorities_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cloudlets_api_prioritization_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cloudlets_application_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cloudlets_application_load_balancer_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cloudlets_audience_segmentation_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cloudlets_edge_redirector_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cloudlets_forward_rewrite_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cloudlets_phased_release_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cloudlets_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cloudlets_request_control_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cloudlets_visitor_prioritization_match_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cp_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cps_csr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cps_deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)    11639 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cps_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cps_enrollments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cps_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_datastream_activation_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_datastream_dataset_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_datastreams.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_dns_record_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_edge_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_edge_worker_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_edge_workers_property_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_edge_workers_resource_tier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_edgekv_group_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_edgekv_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_gtm_default_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_iam_contact_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_iam_countries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_iam_grantable_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_iam_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_iam_states.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_iam_supported_langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_iam_timeout_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_iam_timezones.py
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_network_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_properties_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property_include.py
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property_include_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property_include_parents.py
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property_include_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property_includes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property_products.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property_rule_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property_rules_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property_rules_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    11604 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/gtm_asmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/gtm_cidrmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    29745 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/gtm_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44869 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/gtm_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/gtm_geomap.py
--rw-r--r--   0 runner    (1001) docker     (123)    55296 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/gtm_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    26762 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/gtm_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/iam_blocked_user_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/iam_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/iam_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    48065 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/iam_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/network_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/network_list_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/network_list_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/network_list_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)  1210373 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:10:27.014758 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/properties/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23565 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/properties/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/properties/cp_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    23031 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/properties/edge_host_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/properties/get_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/properties/get_cp_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/properties/get_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/properties/get_property_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    21783 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/properties/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42254 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/properties/property.py
--rw-r--r--   0 runner    (1001) docker     (123)    27517 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/properties/property_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    42054 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/property.py
--rw-r--r--   0 runner    (1001) docker     (123)    27267 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/property_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22902 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/property_include.py
--rw-r--r--   0 runner    (1001) docker     (123)    24971 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/property_include_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22466 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:10:27.014758 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/trafficmanagement/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/trafficmanagement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28679 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/trafficmanagement/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/trafficmanagement/get_gtm_default_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/trafficmanagement/gtm_a_smap.py
--rw-r--r--   0 runner    (1001) docker     (123)    11923 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/trafficmanagement/gtm_cidrmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    29991 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/trafficmanagement/gtm_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    45095 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/trafficmanagement/gtm_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/trafficmanagement/gtm_geomap.py
--rw-r--r--   0 runner    (1001) docker     (123)    55532 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/trafficmanagement/gtm_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    26998 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/trafficmanagement/gtm_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    26637 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai/trafficmanagement/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 11:10:27.010758 pulumi_akamai-4.6.0a1688123148/pulumi_akamai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/pulumi_akamai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 11:10:27.014758 pulumi_akamai-4.6.0a1688123148/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-30 11:10:26.000000 pulumi_akamai-4.6.0a1688123148/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:43:49.942645 pulumi_akamai-4.6.0a1688398728/
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-03 15:43:49.942645 pulumi_akamai-4.6.0a1688398728/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:43:49.934645 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/
+-rw-r--r--   0 runner    (1001) docker     (123)    27506 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1554270 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21333 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_advanced_settings_evasive_path_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_advanced_settings_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_advanced_settings_pragma_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_advanced_settings_prefetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_api_constraints_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12592 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_api_request_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14951 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_attack_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_by_pass_network_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20518 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_configuration_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_custom_deny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_custom_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12783 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_custom_rule_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17001 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_eval_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_eval_penalty_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14538 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_eval_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17481 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_ip_geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_ip_geo_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_malware_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_malware_policy_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_malware_policy_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_malware_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_match_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_match_target_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12987 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_penalty_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_rate_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_rate_policy_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_rate_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_reputation_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_reputation_profile_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14387 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_reputation_profile_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_reputation_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14063 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_rule_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17082 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_security_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_security_policy_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_selected_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17536 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_siem_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19373 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_slow_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_slow_post_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_threat_intel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_version_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15899 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_waf_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_waf_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_wap_selected_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/appsec_advanced_settings_attack_payload_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11290 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/appsec_advanced_settings_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19609 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cloudlets_application_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cloudlets_application_load_balancer_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19277 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cloudlets_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cloudlets_policy_activation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:43:49.938645 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14717 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cp_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47004 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cps_dv_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cps_dv_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44892 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cps_third_party_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27347 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cps_upload_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58490 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/datastream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78637 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/dns_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21162 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/dns_zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22811 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edge_host_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18627 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edge_kv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edge_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edge_workers_activation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:43:49.938645 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78911 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/dns_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21414 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/dns_zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/get_authorities_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/get_dns_record_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgekv_group_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_advanced_settings_evasive_path_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_advanced_settings_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_advanced_settings_pragma_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_advanced_settings_prefetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_api_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_api_request_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_attack_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_bypass_network_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_configuration_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_contracts_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_custom_deny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_custom_rule_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_custom_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_eval_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_eval_penalty_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_eval_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_export_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_failover_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_hostname_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_hostname_coverage_match_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_hostname_coverage_overlapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_ip_geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_malware_content_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_malware_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_malware_policy_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_match_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_penalty_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_rate_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_rate_policy_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_reputation_profile_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_reputation_profile_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_reputation_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_rule_upgrade_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_security_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9257 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_security_policy_protections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_selectable_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_selected_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_siem_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_siem_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_slow_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_threat_intel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_tuning_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_version_notes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_waf_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_wap_selected_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_appsec_advanced_settings_attack_payload_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_appsec_advanced_settings_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_authorities_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_api_prioritization_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_application_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_application_load_balancer_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_audience_segmentation_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_edge_redirector_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_forward_rewrite_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_phased_release_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_request_control_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_visitor_prioritization_match_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cp_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cps_csr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cps_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11639 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cps_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cps_enrollments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cps_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_datastream_activation_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_datastream_dataset_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_datastreams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_dns_record_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edge_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edge_worker_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edge_workers_property_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edge_workers_resource_tier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edgekv_group_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edgekv_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_gtm_default_datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_contact_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_grantable_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_supported_langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_timeout_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_timezones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_network_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_properties_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_include_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_include_parents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_include_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_includes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_products.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_rule_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_rules_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_rules_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11604 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_asmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_cidrmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29745 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44869 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_geomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55296 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26762 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/iam_blocked_user_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/iam_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/iam_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48065 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/iam_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/network_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/network_list_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/network_list_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/network_list_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1210373 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:43:49.938645 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23565 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14967 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/cp_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23127 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/edge_host_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/get_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/get_cp_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/get_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/get_property_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21783 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42326 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27649 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/property_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42054 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27267 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/property_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22902 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/property_include.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24971 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/property_include_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22466 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:43:49.942645 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28679 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/get_gtm_default_datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/gtm_a_smap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12007 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/gtm_cidrmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30093 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/gtm_datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45173 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/gtm_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/gtm_geomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55622 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/gtm_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27088 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/gtm_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26637 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:43:49.938645 pulumi_akamai-4.6.0a1688398728/pulumi_akamai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/pulumi_akamai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 15:43:49.942645 pulumi_akamai-4.6.0a1688398728/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-03 15:43:49.000000 pulumi_akamai-4.6.0a1688398728/setup.py
```

### Comparing `pulumi_akamai-4.6.0a1688123148/PKG-INFO` & `pulumi_akamai-4.6.0a1688398728/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_akamai
-Version: 4.6.0a1688123148
+Version: 4.6.0a1688398728
 Summary: A Pulumi package for creating and managing akamai cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-akamai
 Keywords: pulumi akamai
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_akamai-4.6.0a1688123148/README.md` & `pulumi_akamai-4.6.0a1688398728/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/__init__.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,14 +161,15 @@
 from .get_iam_supported_langs import *
 from .get_iam_timeout_policies import *
 from .get_iam_timezones import *
 from .get_network_lists import *
 from .get_properties import *
 from .get_properties_search import *
 from .get_property import *
+from .get_property_activation import *
 from .get_property_hostnames import *
 from .get_property_include import *
 from .get_property_include_activation import *
 from .get_property_include_parents import *
 from .get_property_include_rules import *
 from .get_property_includes import *
 from .get_property_products import *
```

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/_inputs.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/_utilities.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_activations.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_activations.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_advanced_settings_evasive_path_match.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_advanced_settings_evasive_path_match.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_advanced_settings_logging.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_advanced_settings_logging.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_advanced_settings_pragma_header.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_advanced_settings_pragma_header.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_advanced_settings_prefetch.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_advanced_settings_prefetch.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_api_constraints_protection.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_api_constraints_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_api_request_constraints.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_api_request_constraints.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_attack_group.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_attack_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_by_pass_network_list.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_by_pass_network_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_configuration.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_configuration_rename.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_configuration_rename.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_custom_deny.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_custom_deny.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_custom_rule.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_custom_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_custom_rule_action.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_custom_rule_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_eval.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_eval.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_eval_group.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_eval_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_eval_penalty_box.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_eval_penalty_box.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_eval_rule.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_eval_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_ip_geo.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_ip_geo.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_ip_geo_protection.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_ip_geo_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_malware_policy.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_malware_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_malware_policy_action.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_malware_policy_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_malware_policy_actions.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_malware_policy_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_malware_protection.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_malware_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_match_target.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_match_target.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_match_target_sequence.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_match_target_sequence.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_penalty_box.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_penalty_box.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_rate_policy.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_rate_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_rate_policy_action.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_rate_policy_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_rate_protection.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_rate_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_reputation_profile.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_reputation_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_reputation_profile_action.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_reputation_profile_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_reputation_profile_analysis.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_reputation_profile_analysis.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_reputation_protection.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_reputation_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_rule.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_rule_upgrade.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_rule_upgrade.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_security_policy.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_security_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_security_policy_rename.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_security_policy_rename.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_selected_hostnames.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_selected_hostnames.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_siem_settings.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_siem_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_slow_post.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_slow_post.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_slow_post_protection.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_slow_post_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_threat_intel.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_threat_intel.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_version_nodes.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_version_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_waf_mode.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_waf_mode.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_waf_protection.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_waf_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/app_sec_wap_selected_hostnames.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/app_sec_wap_selected_hostnames.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/appsec_advanced_settings_attack_payload_logging.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/appsec_advanced_settings_attack_payload_logging.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/appsec_advanced_settings_request_body.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/appsec_advanced_settings_request_body.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/cloudlets_application_load_balancer.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cloudlets_application_load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/cloudlets_application_load_balancer_activation.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cloudlets_application_load_balancer_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/cloudlets_policy.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cloudlets_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/cloudlets_policy_activation.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cloudlets_policy_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/config/outputs.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/config/vars.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/cp_code.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cp_code.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/cps_dv_enrollment.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cps_dv_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/cps_dv_validation.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cps_dv_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/cps_third_party_enrollment.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cps_third_party_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/cps_upload_certificate.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/cps_upload_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/datastream.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/datastream.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/dns_record.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/dns_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/dns_zone.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/dns_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edge_host_name.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edge_host_name.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edge_kv.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edge_kv.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edge_worker.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edge_worker.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edge_workers_activation.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edge_workers_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edgedns/_inputs.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edgedns/dns_record.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/dns_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1412,19 +1412,19 @@
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
 
-warnings.warn("""akamai.edgedns.DnsRecord has been deprecated in favor of akamai.DnsRecord""", DeprecationWarning)
+warnings.warn("""akamai.edgedns/dnsrecord.DnsRecord has been deprecated in favor of akamai.index/dnsrecord.DnsRecord""", DeprecationWarning)
 
 
 class DnsRecord(pulumi.CustomResource):
-    warnings.warn("""akamai.edgedns.DnsRecord has been deprecated in favor of akamai.DnsRecord""", DeprecationWarning)
+    warnings.warn("""akamai.edgedns/dnsrecord.DnsRecord has been deprecated in favor of akamai.index/dnsrecord.DnsRecord""", DeprecationWarning)
 
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  active: Optional[pulumi.Input[bool]] = None,
                  algorithm: Optional[pulumi.Input[int]] = None,
@@ -1564,15 +1564,15 @@
                  type_covered: Optional[pulumi.Input[str]] = None,
                  type_mnemonic: Optional[pulumi.Input[str]] = None,
                  type_value: Optional[pulumi.Input[int]] = None,
                  usage: Optional[pulumi.Input[int]] = None,
                  weight: Optional[pulumi.Input[int]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        pulumi.log.warn("""DnsRecord is deprecated: akamai.edgedns.DnsRecord has been deprecated in favor of akamai.DnsRecord""")
+        pulumi.log.warn("""DnsRecord is deprecated: akamai.edgedns/dnsrecord.DnsRecord has been deprecated in favor of akamai.index/dnsrecord.DnsRecord""")
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DnsRecordArgs.__new__(DnsRecordArgs)
```

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edgedns/dns_zone.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/dns_zone.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,19 +322,19 @@
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
 
-warnings.warn("""akamai.edgedns.DnsZone has been deprecated in favor of akamai.DnsZone""", DeprecationWarning)
+warnings.warn("""akamai.edgedns/dnszone.DnsZone has been deprecated in favor of akamai.index/dnszone.DnsZone""", DeprecationWarning)
 
 
 class DnsZone(pulumi.CustomResource):
-    warnings.warn("""akamai.edgedns.DnsZone has been deprecated in favor of akamai.DnsZone""", DeprecationWarning)
+    warnings.warn("""akamai.edgedns/dnszone.DnsZone has been deprecated in favor of akamai.index/dnszone.DnsZone""", DeprecationWarning)
 
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  contract: Optional[pulumi.Input[str]] = None,
@@ -384,15 +384,15 @@
                  sign_and_serve: Optional[pulumi.Input[bool]] = None,
                  sign_and_serve_algorithm: Optional[pulumi.Input[str]] = None,
                  target: Optional[pulumi.Input[str]] = None,
                  tsig_key: Optional[pulumi.Input[pulumi.InputType['DnsZoneTsigKeyArgs']]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        pulumi.log.warn("""DnsZone is deprecated: akamai.edgedns.DnsZone has been deprecated in favor of akamai.DnsZone""")
+        pulumi.log.warn("""DnsZone is deprecated: akamai.edgedns/dnszone.DnsZone has been deprecated in favor of akamai.index/dnszone.DnsZone""")
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DnsZoneArgs.__new__(DnsZoneArgs)
```

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edgedns/get_authorities_set.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/get_authorities_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 __all__ = [
     'GetAuthoritiesSetResult',
     'AwaitableGetAuthoritiesSetResult',
     'get_authorities_set',
     'get_authorities_set_output',
 ]
 
-warnings.warn("""akamai.edgedns.getAuthoritiesSet has been deprecated in favor of akamai.getAuthoritiesSet""", DeprecationWarning)
+warnings.warn("""akamai.edgedns/getauthoritiesset.getAuthoritiesSet has been deprecated in favor of akamai.index/getauthoritiesset.getAuthoritiesSet""", DeprecationWarning)
 
 @pulumi.output_type
 class GetAuthoritiesSetResult:
     """
     A collection of values returned by getAuthoritiesSet.
     """
     def __init__(__self__, authorities=None, contract=None, id=None):
@@ -65,15 +65,15 @@
 
 
 def get_authorities_set(contract: Optional[str] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetAuthoritiesSetResult:
     """
     Use this data source to access information about an existing resource.
     """
-    pulumi.log.warn("""get_authorities_set is deprecated: akamai.edgedns.getAuthoritiesSet has been deprecated in favor of akamai.getAuthoritiesSet""")
+    pulumi.log.warn("""get_authorities_set is deprecated: akamai.edgedns/getauthoritiesset.getAuthoritiesSet has been deprecated in favor of akamai.index/getauthoritiesset.getAuthoritiesSet""")
     __args__ = dict()
     __args__['contract'] = contract
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:edgedns/getAuthoritiesSet:getAuthoritiesSet', __args__, opts=opts, typ=GetAuthoritiesSetResult).value
 
     return AwaitableGetAuthoritiesSetResult(
         authorities=__ret__.authorities,
@@ -83,9 +83,9 @@
 
 @_utilities.lift_output_func(get_authorities_set)
 def get_authorities_set_output(contract: Optional[pulumi.Input[str]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAuthoritiesSetResult]:
     """
     Use this data source to access information about an existing resource.
     """
-    pulumi.log.warn("""get_authorities_set is deprecated: akamai.edgedns.getAuthoritiesSet has been deprecated in favor of akamai.getAuthoritiesSet""")
+    pulumi.log.warn("""get_authorities_set is deprecated: akamai.edgedns/getauthoritiesset.getAuthoritiesSet has been deprecated in favor of akamai.index/getauthoritiesset.getAuthoritiesSet""")
     ...
```

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edgedns/get_dns_record_set.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/get_dns_record_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 __all__ = [
     'GetDnsRecordSetResult',
     'AwaitableGetDnsRecordSetResult',
     'get_dns_record_set',
     'get_dns_record_set_output',
 ]
 
-warnings.warn("""akamai.edgedns.getDnsRecordSet has been deprecated in favor of akamai.getDnsRecordSet""", DeprecationWarning)
+warnings.warn("""akamai.edgedns/getdnsrecordset.getDnsRecordSet has been deprecated in favor of akamai.index/getdnsrecordset.getDnsRecordSet""", DeprecationWarning)
 
 @pulumi.output_type
 class GetDnsRecordSetResult:
     """
     A collection of values returned by getDnsRecordSet.
     """
     def __init__(__self__, host=None, id=None, rdatas=None, record_type=None, zone=None):
@@ -85,15 +85,15 @@
 def get_dns_record_set(host: Optional[str] = None,
                        record_type: Optional[str] = None,
                        zone: Optional[str] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDnsRecordSetResult:
     """
     Use this data source to access information about an existing resource.
     """
-    pulumi.log.warn("""get_dns_record_set is deprecated: akamai.edgedns.getDnsRecordSet has been deprecated in favor of akamai.getDnsRecordSet""")
+    pulumi.log.warn("""get_dns_record_set is deprecated: akamai.edgedns/getdnsrecordset.getDnsRecordSet has been deprecated in favor of akamai.index/getdnsrecordset.getDnsRecordSet""")
     __args__ = dict()
     __args__['host'] = host
     __args__['recordType'] = record_type
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:edgedns/getDnsRecordSet:getDnsRecordSet', __args__, opts=opts, typ=GetDnsRecordSetResult).value
 
@@ -109,9 +109,9 @@
 def get_dns_record_set_output(host: Optional[pulumi.Input[str]] = None,
                               record_type: Optional[pulumi.Input[str]] = None,
                               zone: Optional[pulumi.Input[str]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDnsRecordSetResult]:
     """
     Use this data source to access information about an existing resource.
     """
-    pulumi.log.warn("""get_dns_record_set is deprecated: akamai.edgedns.getDnsRecordSet has been deprecated in favor of akamai.getDnsRecordSet""")
+    pulumi.log.warn("""get_dns_record_set is deprecated: akamai.edgedns/getdnsrecordset.getDnsRecordSet has been deprecated in favor of akamai.index/getdnsrecordset.getDnsRecordSet""")
     ...
```

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edgedns/outputs.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgedns/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/edgekv_group_items.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/edgekv_group_items.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_advanced_settings_evasive_path_match.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_advanced_settings_evasive_path_match.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_advanced_settings_logging.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_advanced_settings_logging.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_advanced_settings_pragma_header.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_advanced_settings_pragma_header.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_advanced_settings_prefetch.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_advanced_settings_prefetch.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_api_endpoints.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_api_endpoints.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_api_request_constraints.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_api_request_constraints.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_attack_groups.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_attack_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_bypass_network_lists.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_bypass_network_lists.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_configuration.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_configuration_version.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_configuration_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_contracts_groups.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_contracts_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_custom_deny.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_custom_deny.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_custom_rule_actions.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_custom_rule_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_custom_rules.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_custom_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_eval.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_eval.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_eval_groups.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_eval_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_eval_penalty_box.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_eval_penalty_box.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_eval_rules.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_eval_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_export_configuration.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_export_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_failover_hostnames.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_failover_hostnames.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_hostname_coverage.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_hostname_coverage.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_hostname_coverage_match_targets.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_hostname_coverage_match_targets.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_hostname_coverage_overlapping.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_hostname_coverage_overlapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_ip_geo.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_ip_geo.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_malware_content_types.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_malware_content_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_malware_policies.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_malware_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_malware_policy_actions.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_malware_policy_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_match_targets.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_match_targets.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_penalty_box.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_penalty_box.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_rate_policies.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_rate_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_rate_policy_actions.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_rate_policy_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_reputation_profile_actions.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_reputation_profile_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_reputation_profile_analysis.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_reputation_profile_analysis.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_reputation_profiles.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_reputation_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_rule_upgrade_details.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_rule_upgrade_details.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_rules.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_security_policy.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_security_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_security_policy_protections.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_security_policy_protections.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_selectable_hostnames.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_selectable_hostnames.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_selected_hostnames.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_selected_hostnames.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_siem_definitions.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_siem_definitions.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_siem_settings.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_siem_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_slow_post.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_slow_post.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_threat_intel.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_threat_intel.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_tuning_recommendations.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_tuning_recommendations.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_version_notes.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_version_notes.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_waf_mode.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_waf_mode.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_app_sec_wap_selected_hostnames.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_app_sec_wap_selected_hostnames.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_appsec_advanced_settings_attack_payload_logging.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_appsec_advanced_settings_attack_payload_logging.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_appsec_advanced_settings_request_body.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_appsec_advanced_settings_request_body.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_authorities_set.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_authorities_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cloudlets_api_prioritization_match_rule.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_api_prioritization_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cloudlets_application_load_balancer.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_application_load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cloudlets_application_load_balancer_match_rule.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_application_load_balancer_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cloudlets_audience_segmentation_match_rule.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_audience_segmentation_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cloudlets_edge_redirector_match_rule.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_edge_redirector_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cloudlets_forward_rewrite_match_rule.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_forward_rewrite_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cloudlets_phased_release_match_rule.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_phased_release_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cloudlets_policy.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cloudlets_request_control_match_rule.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_request_control_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cloudlets_visitor_prioritization_match_rule.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cloudlets_visitor_prioritization_match_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_contract.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_contract.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_contracts.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_contracts.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cp_code.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cp_code.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cps_csr.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cps_csr.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cps_deployments.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cps_deployments.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cps_enrollment.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cps_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cps_enrollments.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cps_enrollments.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_cps_warnings.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_cps_warnings.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_datastream_activation_history.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_datastream_activation_history.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_datastream_dataset_fields.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_datastream_dataset_fields.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_datastreams.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_datastreams.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_dns_record_set.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_dns_record_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_edge_worker.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edge_worker.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_edge_worker_activation.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edge_worker_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_edge_workers_property_rules.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edge_workers_property_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_edge_workers_resource_tier.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edge_workers_resource_tier.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_edgekv_group_items.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edgekv_group_items.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_edgekv_groups.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_edgekv_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_group.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_groups.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_gtm_default_datacenter.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_gtm_default_datacenter.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_iam_contact_types.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_contact_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_iam_countries.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_countries.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_iam_grantable_roles.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_grantable_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_iam_roles.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_iam_states.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_states.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_iam_supported_langs.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_supported_langs.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_iam_timeout_policies.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_timeout_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_iam_timezones.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_iam_timezones.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_network_lists.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_network_lists.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_properties.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_properties.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_properties_search.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_properties_search.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property_hostnames.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_hostnames.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property_include.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_include.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property_include_activation.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_include_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property_include_parents.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_include_parents.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property_include_rules.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_include_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property_includes.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_includes.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property_products.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_products.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property_rule_formats.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_rule_formats.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property_rules.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property_rules_builder.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_rules_builder.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/get_property_rules_template.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_rules_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/gtm_asmap.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_asmap.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/gtm_cidrmap.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_cidrmap.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/gtm_datacenter.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_datacenter.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/gtm_domain.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/gtm_geomap.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_geomap.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/gtm_property.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/gtm_resource.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/gtm_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/iam_blocked_user_properties.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/iam_blocked_user_properties.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/iam_group.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/iam_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/iam_role.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/iam_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/iam_user.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/iam_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/network_list.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/network_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/network_list_activations.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/network_list_activations.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/network_list_description.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/network_list_description.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/network_list_subscription.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/network_list_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/outputs.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/properties/__init__.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/properties/_inputs.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/properties/cp_code.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/cp_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,19 +209,19 @@
         return pulumi.get(self, "product_id")
 
     @product_id.setter
     def product_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "product_id", value)
 
 
-warnings.warn("""akamai.properties.CpCode has been deprecated in favor of akamai.CpCode""", DeprecationWarning)
+warnings.warn("""akamai.properties/cpcode.CpCode has been deprecated in favor of akamai.index/cpcode.CpCode""", DeprecationWarning)
 
 
 class CpCode(pulumi.CustomResource):
-    warnings.warn("""akamai.properties.CpCode has been deprecated in favor of akamai.CpCode""", DeprecationWarning)
+    warnings.warn("""akamai.properties/cpcode.CpCode has been deprecated in favor of akamai.index/cpcode.CpCode""", DeprecationWarning)
 
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  contract: Optional[pulumi.Input[str]] = None,
                  contract_id: Optional[pulumi.Input[str]] = None,
@@ -263,15 +263,15 @@
                  contract_id: Optional[pulumi.Input[str]] = None,
                  group: Optional[pulumi.Input[str]] = None,
                  group_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  product: Optional[pulumi.Input[str]] = None,
                  product_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        pulumi.log.warn("""CpCode is deprecated: akamai.properties.CpCode has been deprecated in favor of akamai.CpCode""")
+        pulumi.log.warn("""CpCode is deprecated: akamai.properties/cpcode.CpCode has been deprecated in favor of akamai.index/cpcode.CpCode""")
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = CpCodeArgs.__new__(CpCodeArgs)
```

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/properties/edge_host_name.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/edge_host_name.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,19 +319,19 @@
         return pulumi.get(self, "use_cases")
 
     @use_cases.setter
     def use_cases(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "use_cases", value)
 
 
-warnings.warn("""akamai.properties.EdgeHostName has been deprecated in favor of akamai.EdgeHostName""", DeprecationWarning)
+warnings.warn("""akamai.properties/edgehostname.EdgeHostName has been deprecated in favor of akamai.index/edgehostname.EdgeHostName""", DeprecationWarning)
 
 
 class EdgeHostName(pulumi.CustomResource):
-    warnings.warn("""akamai.properties.EdgeHostName has been deprecated in favor of akamai.EdgeHostName""", DeprecationWarning)
+    warnings.warn("""akamai.properties/edgehostname.EdgeHostName has been deprecated in favor of akamai.index/edgehostname.EdgeHostName""", DeprecationWarning)
 
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  certificate: Optional[pulumi.Input[int]] = None,
                  contract: Optional[pulumi.Input[str]] = None,
@@ -383,15 +383,15 @@
                  group_id: Optional[pulumi.Input[str]] = None,
                  ip_behavior: Optional[pulumi.Input[str]] = None,
                  product: Optional[pulumi.Input[str]] = None,
                  product_id: Optional[pulumi.Input[str]] = None,
                  status_update_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  use_cases: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        pulumi.log.warn("""EdgeHostName is deprecated: akamai.properties.EdgeHostName has been deprecated in favor of akamai.EdgeHostName""")
+        pulumi.log.warn("""EdgeHostName is deprecated: akamai.properties/edgehostname.EdgeHostName has been deprecated in favor of akamai.index/edgehostname.EdgeHostName""")
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = EdgeHostNameArgs.__new__(EdgeHostNameArgs)
```

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/properties/get_activation.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/get_property_activation.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 
 __all__ = [
-    'GetActivationResult',
-    'AwaitableGetActivationResult',
-    'get_activation',
-    'get_activation_output',
+    'GetPropertyActivationResult',
+    'AwaitableGetPropertyActivationResult',
+    'get_property_activation',
+    'get_property_activation_output',
 ]
 
 @pulumi.output_type
-class GetActivationResult:
+class GetPropertyActivationResult:
     """
-    A collection of values returned by getActivation.
+    A collection of values returned by getPropertyActivation.
     """
     def __init__(__self__, activation_id=None, contacts=None, errors=None, id=None, network=None, note=None, property_id=None, status=None, version=None, warnings=None):
         if activation_id and not isinstance(activation_id, str):
             raise TypeError("Expected argument 'activation_id' to be a str")
         pulumi.set(__self__, "activation_id", activation_id)
         if contacts and not isinstance(contacts, list):
             raise TypeError("Expected argument 'contacts' to be a list")
@@ -103,61 +103,61 @@
 
     @property
     @pulumi.getter
     def warnings(self) -> str:
         return pulumi.get(self, "warnings")
 
 
-class AwaitableGetActivationResult(GetActivationResult):
+class AwaitableGetPropertyActivationResult(GetPropertyActivationResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetActivationResult(
+        return GetPropertyActivationResult(
             activation_id=self.activation_id,
             contacts=self.contacts,
             errors=self.errors,
             id=self.id,
             network=self.network,
             note=self.note,
             property_id=self.property_id,
             status=self.status,
             version=self.version,
             warnings=self.warnings)
 
 
-def get_activation(network: Optional[str] = None,
-                   property_id: Optional[str] = None,
-                   version: Optional[int] = None,
-                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetActivationResult:
+def get_property_activation(network: Optional[str] = None,
+                            property_id: Optional[str] = None,
+                            version: Optional[int] = None,
+                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertyActivationResult:
     """
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     __args__['network'] = network
     __args__['propertyId'] = property_id
     __args__['version'] = version
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('akamai:properties/getActivation:getActivation', __args__, opts=opts, typ=GetActivationResult).value
+    __ret__ = pulumi.runtime.invoke('akamai:index/getPropertyActivation:getPropertyActivation', __args__, opts=opts, typ=GetPropertyActivationResult).value
 
-    return AwaitableGetActivationResult(
+    return AwaitableGetPropertyActivationResult(
         activation_id=__ret__.activation_id,
         contacts=__ret__.contacts,
         errors=__ret__.errors,
         id=__ret__.id,
         network=__ret__.network,
         note=__ret__.note,
         property_id=__ret__.property_id,
         status=__ret__.status,
         version=__ret__.version,
         warnings=__ret__.warnings)
 
 
-@_utilities.lift_output_func(get_activation)
-def get_activation_output(network: Optional[pulumi.Input[Optional[str]]] = None,
-                          property_id: Optional[pulumi.Input[str]] = None,
-                          version: Optional[pulumi.Input[int]] = None,
-                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetActivationResult]:
+@_utilities.lift_output_func(get_property_activation)
+def get_property_activation_output(network: Optional[pulumi.Input[Optional[str]]] = None,
+                                   property_id: Optional[pulumi.Input[str]] = None,
+                                   version: Optional[pulumi.Input[int]] = None,
+                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyActivationResult]:
     """
     Use this data source to access information about an existing resource.
     """
     ...
```

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/properties/get_cp_code.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/get_cp_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 __all__ = [
     'GetCpCodeResult',
     'AwaitableGetCpCodeResult',
     'get_cp_code',
     'get_cp_code_output',
 ]
 
-warnings.warn("""akamai.properties.getCpCode has been deprecated in favor of akamai.getCpCode""", DeprecationWarning)
+warnings.warn("""akamai.properties/getcpcode.getCpCode has been deprecated in favor of akamai.index/getcpcode.getCpCode""", DeprecationWarning)
 
 @pulumi.output_type
 class GetCpCodeResult:
     """
     A collection of values returned by getCpCode.
     """
     def __init__(__self__, contract=None, contract_id=None, group=None, group_id=None, id=None, name=None, product_ids=None):
@@ -113,15 +113,15 @@
                 group: Optional[str] = None,
                 group_id: Optional[str] = None,
                 name: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCpCodeResult:
     """
     Use this data source to access information about an existing resource.
     """
-    pulumi.log.warn("""get_cp_code is deprecated: akamai.properties.getCpCode has been deprecated in favor of akamai.getCpCode""")
+    pulumi.log.warn("""get_cp_code is deprecated: akamai.properties/getcpcode.getCpCode has been deprecated in favor of akamai.index/getcpcode.getCpCode""")
     __args__ = dict()
     __args__['contract'] = contract
     __args__['contractId'] = contract_id
     __args__['group'] = group
     __args__['groupId'] = group_id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -143,9 +143,9 @@
                        group: Optional[pulumi.Input[Optional[str]]] = None,
                        group_id: Optional[pulumi.Input[Optional[str]]] = None,
                        name: Optional[pulumi.Input[str]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCpCodeResult]:
     """
     Use this data source to access information about an existing resource.
     """
-    pulumi.log.warn("""get_cp_code is deprecated: akamai.properties.getCpCode has been deprecated in favor of akamai.getCpCode""")
+    pulumi.log.warn("""get_cp_code is deprecated: akamai.properties/getcpcode.getCpCode has been deprecated in favor of akamai.index/getcpcode.getCpCode""")
     ...
```

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/properties/get_property.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/get_property.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 __all__ = [
     'GetPropertyResult',
     'AwaitableGetPropertyResult',
     'get_property',
     'get_property_output',
 ]
 
-warnings.warn("""akamai.properties.getProperty has been deprecated in favor of akamai.getProperty""", DeprecationWarning)
+warnings.warn("""akamai.properties/getproperty.getProperty has been deprecated in favor of akamai.index/getproperty.getProperty""", DeprecationWarning)
 
 @pulumi.output_type
 class GetPropertyResult:
     """
     A collection of values returned by getProperty.
     """
     def __init__(__self__, id=None, name=None, rules=None, version=None):
@@ -75,15 +75,15 @@
 
 def get_property(name: Optional[str] = None,
                  version: Optional[int] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertyResult:
     """
     Use this data source to access information about an existing resource.
     """
-    pulumi.log.warn("""get_property is deprecated: akamai.properties.getProperty has been deprecated in favor of akamai.getProperty""")
+    pulumi.log.warn("""get_property is deprecated: akamai.properties/getproperty.getProperty has been deprecated in favor of akamai.index/getproperty.getProperty""")
     __args__ = dict()
     __args__['name'] = name
     __args__['version'] = version
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:properties/getProperty:getProperty', __args__, opts=opts, typ=GetPropertyResult).value
 
     return AwaitableGetPropertyResult(
@@ -96,9 +96,9 @@
 @_utilities.lift_output_func(get_property)
 def get_property_output(name: Optional[pulumi.Input[str]] = None,
                         version: Optional[pulumi.Input[Optional[int]]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyResult]:
     """
     Use this data source to access information about an existing resource.
     """
-    pulumi.log.warn("""get_property is deprecated: akamai.properties.getProperty has been deprecated in favor of akamai.getProperty""")
+    pulumi.log.warn("""get_property is deprecated: akamai.properties/getproperty.getProperty has been deprecated in favor of akamai.index/getproperty.getProperty""")
     ...
```

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/properties/get_property_rules.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/get_property_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 __all__ = [
     'GetPropertyRulesResult',
     'AwaitableGetPropertyRulesResult',
     'get_property_rules',
     'get_property_rules_output',
 ]
 
-warnings.warn("""akamai.properties.getPropertyRules has been deprecated in favor of akamai.getPropertyRules""", DeprecationWarning)
+warnings.warn("""akamai.properties/getpropertyrules.getPropertyRules has been deprecated in favor of akamai.index/getpropertyrules.getPropertyRules""", DeprecationWarning)
 
 @pulumi.output_type
 class GetPropertyRulesResult:
     """
     A collection of values returned by getPropertyRules.
     """
     def __init__(__self__, contract_id=None, errors=None, group_id=None, id=None, property_id=None, rule_format=None, rules=None, version=None):
@@ -114,15 +114,15 @@
                        property_id: Optional[str] = None,
                        rule_format: Optional[str] = None,
                        version: Optional[int] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPropertyRulesResult:
     """
     Use this data source to access information about an existing resource.
     """
-    pulumi.log.warn("""get_property_rules is deprecated: akamai.properties.getPropertyRules has been deprecated in favor of akamai.getPropertyRules""")
+    pulumi.log.warn("""get_property_rules is deprecated: akamai.properties/getpropertyrules.getPropertyRules has been deprecated in favor of akamai.index/getpropertyrules.getPropertyRules""")
     __args__ = dict()
     __args__['contractId'] = contract_id
     __args__['groupId'] = group_id
     __args__['propertyId'] = property_id
     __args__['ruleFormat'] = rule_format
     __args__['version'] = version
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -145,9 +145,9 @@
                               property_id: Optional[pulumi.Input[str]] = None,
                               rule_format: Optional[pulumi.Input[Optional[str]]] = None,
                               version: Optional[pulumi.Input[Optional[int]]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPropertyRulesResult]:
     """
     Use this data source to access information about an existing resource.
     """
-    pulumi.log.warn("""get_property_rules is deprecated: akamai.properties.getPropertyRules has been deprecated in favor of akamai.getPropertyRules""")
+    pulumi.log.warn("""get_property_rules is deprecated: akamai.properties/getpropertyrules.getPropertyRules has been deprecated in favor of akamai.index/getpropertyrules.getPropertyRules""")
     ...
```

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/properties/outputs.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/properties/property.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/property.py`

 * *Files 1% similar despite different names*

```diff
@@ -587,19 +587,19 @@
         return pulumi.get(self, "variables")
 
     @variables.setter
     def variables(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "variables", value)
 
 
-warnings.warn("""akamai.properties.Property has been deprecated in favor of akamai.Property""", DeprecationWarning)
+warnings.warn("""akamai.properties/property.Property has been deprecated in favor of akamai.index/property.Property""", DeprecationWarning)
 
 
 class Property(pulumi.CustomResource):
-    warnings.warn("""akamai.properties.Property has been deprecated in favor of akamai.Property""", DeprecationWarning)
+    warnings.warn("""akamai.properties/property.Property has been deprecated in favor of akamai.index/property.Property""", DeprecationWarning)
 
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  contacts: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  contract: Optional[pulumi.Input[str]] = None,
@@ -665,15 +665,15 @@
                  product: Optional[pulumi.Input[str]] = None,
                  product_id: Optional[pulumi.Input[str]] = None,
                  rule_format: Optional[pulumi.Input[str]] = None,
                  rule_warnings: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PropertyRuleWarningArgs']]]]] = None,
                  rules: Optional[pulumi.Input[str]] = None,
                  variables: Optional[pulumi.Input[str]] = None,
                  __props__=None):
-        pulumi.log.warn("""Property is deprecated: akamai.properties.Property has been deprecated in favor of akamai.Property""")
+        pulumi.log.warn("""Property is deprecated: akamai.properties/property.Property has been deprecated in favor of akamai.index/property.Property""")
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PropertyArgs.__new__(PropertyArgs)
```

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/properties/property_activation.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/properties/property_activation.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,19 +359,19 @@
         return pulumi.get(self, "property")
 
     @property.setter
     def property(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "property", value)
 
 
-warnings.warn("""akamai.properties.PropertyActivation has been deprecated in favor of akamai.PropertyActivation""", DeprecationWarning)
+warnings.warn("""akamai.properties/propertyactivation.PropertyActivation has been deprecated in favor of akamai.index/propertyactivation.PropertyActivation""", DeprecationWarning)
 
 
 class PropertyActivation(pulumi.CustomResource):
-    warnings.warn("""akamai.properties.PropertyActivation has been deprecated in favor of akamai.PropertyActivation""", DeprecationWarning)
+    warnings.warn("""akamai.properties/propertyactivation.PropertyActivation has been deprecated in favor of akamai.index/propertyactivation.PropertyActivation""", DeprecationWarning)
 
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  activation_id: Optional[pulumi.Input[str]] = None,
                  auto_acknowledge_rule_warnings: Optional[pulumi.Input[bool]] = None,
@@ -424,15 +424,15 @@
                  note: Optional[pulumi.Input[str]] = None,
                  property: Optional[pulumi.Input[str]] = None,
                  property_id: Optional[pulumi.Input[str]] = None,
                  rule_errors: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PropertyActivationRuleErrorArgs']]]]] = None,
                  rule_warnings: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['PropertyActivationRuleWarningArgs']]]]] = None,
                  version: Optional[pulumi.Input[int]] = None,
                  __props__=None):
-        pulumi.log.warn("""PropertyActivation is deprecated: akamai.properties.PropertyActivation has been deprecated in favor of akamai.PropertyActivation""")
+        pulumi.log.warn("""PropertyActivation is deprecated: akamai.properties/propertyactivation.PropertyActivation has been deprecated in favor of akamai.index/propertyactivation.PropertyActivation""")
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PropertyActivationArgs.__new__(PropertyActivationArgs)
```

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/property.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/property.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/property_activation.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/property_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/property_include.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/property_include.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/property_include_activation.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/property_include_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/provider.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/trafficmanagement/__init__.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/trafficmanagement/_inputs.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/trafficmanagement/get_gtm_default_datacenter.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/get_gtm_default_datacenter.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 __all__ = [
     'GetGtmDefaultDatacenterResult',
     'AwaitableGetGtmDefaultDatacenterResult',
     'get_gtm_default_datacenter',
     'get_gtm_default_datacenter_output',
 ]
 
-warnings.warn("""akamai.trafficmanagement.getGtmDefaultDatacenter has been deprecated in favor of akamai.getGtmDefaultDatacenter""", DeprecationWarning)
+warnings.warn("""akamai.trafficmanagement/getgtmdefaultdatacenter.getGtmDefaultDatacenter has been deprecated in favor of akamai.index/getgtmdefaultdatacenter.getGtmDefaultDatacenter""", DeprecationWarning)
 
 @pulumi.output_type
 class GetGtmDefaultDatacenterResult:
     """
     A collection of values returned by getGtmDefaultDatacenter.
     """
     def __init__(__self__, datacenter=None, datacenter_id=None, domain=None, id=None, nickname=None):
@@ -84,15 +84,15 @@
 
 def get_gtm_default_datacenter(datacenter: Optional[int] = None,
                                domain: Optional[str] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetGtmDefaultDatacenterResult:
     """
     Use this data source to access information about an existing resource.
     """
-    pulumi.log.warn("""get_gtm_default_datacenter is deprecated: akamai.trafficmanagement.getGtmDefaultDatacenter has been deprecated in favor of akamai.getGtmDefaultDatacenter""")
+    pulumi.log.warn("""get_gtm_default_datacenter is deprecated: akamai.trafficmanagement/getgtmdefaultdatacenter.getGtmDefaultDatacenter has been deprecated in favor of akamai.index/getgtmdefaultdatacenter.getGtmDefaultDatacenter""")
     __args__ = dict()
     __args__['datacenter'] = datacenter
     __args__['domain'] = domain
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('akamai:trafficmanagement/getGtmDefaultDatacenter:getGtmDefaultDatacenter', __args__, opts=opts, typ=GetGtmDefaultDatacenterResult).value
 
     return AwaitableGetGtmDefaultDatacenterResult(
@@ -106,9 +106,9 @@
 @_utilities.lift_output_func(get_gtm_default_datacenter)
 def get_gtm_default_datacenter_output(datacenter: Optional[pulumi.Input[Optional[int]]] = None,
                                       domain: Optional[pulumi.Input[str]] = None,
                                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGtmDefaultDatacenterResult]:
     """
     Use this data source to access information about an existing resource.
     """
-    pulumi.log.warn("""get_gtm_default_datacenter is deprecated: akamai.trafficmanagement.getGtmDefaultDatacenter has been deprecated in favor of akamai.getGtmDefaultDatacenter""")
+    pulumi.log.warn("""get_gtm_default_datacenter is deprecated: akamai.trafficmanagement/getgtmdefaultdatacenter.getGtmDefaultDatacenter has been deprecated in favor of akamai.index/getgtmdefaultdatacenter.getGtmDefaultDatacenter""")
     ...
```

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/trafficmanagement/gtm_a_smap.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/gtm_a_smap.py`

 * *Files 7% similar despite different names*

```diff
@@ -143,19 +143,19 @@
         return pulumi.get(self, "wait_on_complete")
 
     @wait_on_complete.setter
     def wait_on_complete(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "wait_on_complete", value)
 
 
-warnings.warn("""akamai.trafficmanagement.GtmASmap has been deprecated in favor of akamai.GtmAsmap""", DeprecationWarning)
+warnings.warn("""akamai.trafficmanagement/gtmasmap.GtmASmap has been deprecated in favor of akamai.index/gtmasmap.GtmAsmap""", DeprecationWarning)
 
 
 class GtmASmap(pulumi.CustomResource):
-    warnings.warn("""akamai.trafficmanagement.GtmASmap has been deprecated in favor of akamai.GtmAsmap""", DeprecationWarning)
+    warnings.warn("""akamai.trafficmanagement/gtmasmap.GtmASmap has been deprecated in favor of akamai.index/gtmasmap.GtmAsmap""", DeprecationWarning)
 
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  assignments: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GtmASmapAssignmentArgs']]]]] = None,
                  default_datacenter: Optional[pulumi.Input[pulumi.InputType['GtmASmapDefaultDatacenterArgs']]] = None,
@@ -193,15 +193,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  assignments: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GtmASmapAssignmentArgs']]]]] = None,
                  default_datacenter: Optional[pulumi.Input[pulumi.InputType['GtmASmapDefaultDatacenterArgs']]] = None,
                  domain: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  wait_on_complete: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
-        pulumi.log.warn("""GtmASmap is deprecated: akamai.trafficmanagement.GtmASmap has been deprecated in favor of akamai.GtmAsmap""")
+        pulumi.log.warn("""GtmASmap is deprecated: akamai.trafficmanagement/gtmasmap.GtmASmap has been deprecated in favor of akamai.index/gtmasmap.GtmAsmap""")
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = GtmASmapArgs.__new__(GtmASmapArgs)
```

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/trafficmanagement/gtm_cidrmap.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/gtm_cidrmap.py`

 * *Files 5% similar despite different names*

```diff
@@ -143,19 +143,19 @@
         return pulumi.get(self, "wait_on_complete")
 
     @wait_on_complete.setter
     def wait_on_complete(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "wait_on_complete", value)
 
 
-warnings.warn("""akamai.trafficmanagement.GtmCidrmap has been deprecated in favor of akamai.GtmCidrmap""", DeprecationWarning)
+warnings.warn("""akamai.trafficmanagement/gtmcidrmap.GtmCidrmap has been deprecated in favor of akamai.index/gtmcidrmap.GtmCidrmap""", DeprecationWarning)
 
 
 class GtmCidrmap(pulumi.CustomResource):
-    warnings.warn("""akamai.trafficmanagement.GtmCidrmap has been deprecated in favor of akamai.GtmCidrmap""", DeprecationWarning)
+    warnings.warn("""akamai.trafficmanagement/gtmcidrmap.GtmCidrmap has been deprecated in favor of akamai.index/gtmcidrmap.GtmCidrmap""", DeprecationWarning)
 
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  assignments: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GtmCidrmapAssignmentArgs']]]]] = None,
                  default_datacenter: Optional[pulumi.Input[pulumi.InputType['GtmCidrmapDefaultDatacenterArgs']]] = None,
@@ -193,15 +193,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  assignments: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GtmCidrmapAssignmentArgs']]]]] = None,
                  default_datacenter: Optional[pulumi.Input[pulumi.InputType['GtmCidrmapDefaultDatacenterArgs']]] = None,
                  domain: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  wait_on_complete: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
-        pulumi.log.warn("""GtmCidrmap is deprecated: akamai.trafficmanagement.GtmCidrmap has been deprecated in favor of akamai.GtmCidrmap""")
+        pulumi.log.warn("""GtmCidrmap is deprecated: akamai.trafficmanagement/gtmcidrmap.GtmCidrmap has been deprecated in favor of akamai.index/gtmcidrmap.GtmCidrmap""")
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = GtmCidrmapArgs.__new__(GtmCidrmapArgs)
```

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/trafficmanagement/gtm_datacenter.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/gtm_datacenter.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,19 +432,19 @@
         return pulumi.get(self, "wait_on_complete")
 
     @wait_on_complete.setter
     def wait_on_complete(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "wait_on_complete", value)
 
 
-warnings.warn("""akamai.trafficmanagement.GtmDatacenter has been deprecated in favor of akamai.GtmDatacenter""", DeprecationWarning)
+warnings.warn("""akamai.trafficmanagement/gtmdatacenter.GtmDatacenter has been deprecated in favor of akamai.index/gtmdatacenter.GtmDatacenter""", DeprecationWarning)
 
 
 class GtmDatacenter(pulumi.CustomResource):
-    warnings.warn("""akamai.trafficmanagement.GtmDatacenter has been deprecated in favor of akamai.GtmDatacenter""", DeprecationWarning)
+    warnings.warn("""akamai.trafficmanagement/gtmdatacenter.GtmDatacenter has been deprecated in favor of akamai.index/gtmdatacenter.GtmDatacenter""", DeprecationWarning)
 
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  city: Optional[pulumi.Input[str]] = None,
                  clone_of: Optional[pulumi.Input[int]] = None,
@@ -498,15 +498,15 @@
                  domain: Optional[pulumi.Input[str]] = None,
                  latitude: Optional[pulumi.Input[float]] = None,
                  longitude: Optional[pulumi.Input[float]] = None,
                  nickname: Optional[pulumi.Input[str]] = None,
                  state_or_province: Optional[pulumi.Input[str]] = None,
                  wait_on_complete: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
-        pulumi.log.warn("""GtmDatacenter is deprecated: akamai.trafficmanagement.GtmDatacenter has been deprecated in favor of akamai.GtmDatacenter""")
+        pulumi.log.warn("""GtmDatacenter is deprecated: akamai.trafficmanagement/gtmdatacenter.GtmDatacenter has been deprecated in favor of akamai.index/gtmdatacenter.GtmDatacenter""")
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = GtmDatacenterArgs.__new__(GtmDatacenterArgs)
```

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/trafficmanagement/gtm_domain.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/gtm_domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -610,19 +610,19 @@
         return pulumi.get(self, "wait_on_complete")
 
     @wait_on_complete.setter
     def wait_on_complete(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "wait_on_complete", value)
 
 
-warnings.warn("""akamai.trafficmanagement.GtmDomain has been deprecated in favor of akamai.GtmDomain""", DeprecationWarning)
+warnings.warn("""akamai.trafficmanagement/gtmdomain.GtmDomain has been deprecated in favor of akamai.index/gtmdomain.GtmDomain""", DeprecationWarning)
 
 
 class GtmDomain(pulumi.CustomResource):
-    warnings.warn("""akamai.trafficmanagement.GtmDomain has been deprecated in favor of akamai.GtmDomain""", DeprecationWarning)
+    warnings.warn("""akamai.trafficmanagement/gtmdomain.GtmDomain has been deprecated in favor of akamai.index/gtmdomain.GtmDomain""", DeprecationWarning)
 
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  cname_coalescing_enabled: Optional[pulumi.Input[bool]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
@@ -680,15 +680,15 @@
                  group: Optional[pulumi.Input[str]] = None,
                  load_feedback: Optional[pulumi.Input[bool]] = None,
                  load_imbalance_percentage: Optional[pulumi.Input[float]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  wait_on_complete: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
-        pulumi.log.warn("""GtmDomain is deprecated: akamai.trafficmanagement.GtmDomain has been deprecated in favor of akamai.GtmDomain""")
+        pulumi.log.warn("""GtmDomain is deprecated: akamai.trafficmanagement/gtmdomain.GtmDomain has been deprecated in favor of akamai.index/gtmdomain.GtmDomain""")
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = GtmDomainArgs.__new__(GtmDomainArgs)
```

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/trafficmanagement/gtm_geomap.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/gtm_geomap.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,19 +143,19 @@
         return pulumi.get(self, "wait_on_complete")
 
     @wait_on_complete.setter
     def wait_on_complete(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "wait_on_complete", value)
 
 
-warnings.warn("""akamai.trafficmanagement.GtmGeomap has been deprecated in favor of akamai.GtmGeomap""", DeprecationWarning)
+warnings.warn("""akamai.trafficmanagement/gtmgeomap.GtmGeomap has been deprecated in favor of akamai.index/gtmgeomap.GtmGeomap""", DeprecationWarning)
 
 
 class GtmGeomap(pulumi.CustomResource):
-    warnings.warn("""akamai.trafficmanagement.GtmGeomap has been deprecated in favor of akamai.GtmGeomap""", DeprecationWarning)
+    warnings.warn("""akamai.trafficmanagement/gtmgeomap.GtmGeomap has been deprecated in favor of akamai.index/gtmgeomap.GtmGeomap""", DeprecationWarning)
 
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  assignments: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GtmGeomapAssignmentArgs']]]]] = None,
                  default_datacenter: Optional[pulumi.Input[pulumi.InputType['GtmGeomapDefaultDatacenterArgs']]] = None,
@@ -193,15 +193,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  assignments: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GtmGeomapAssignmentArgs']]]]] = None,
                  default_datacenter: Optional[pulumi.Input[pulumi.InputType['GtmGeomapDefaultDatacenterArgs']]] = None,
                  domain: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  wait_on_complete: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
-        pulumi.log.warn("""GtmGeomap is deprecated: akamai.trafficmanagement.GtmGeomap has been deprecated in favor of akamai.GtmGeomap""")
+        pulumi.log.warn("""GtmGeomap is deprecated: akamai.trafficmanagement/gtmgeomap.GtmGeomap has been deprecated in favor of akamai.index/gtmgeomap.GtmGeomap""")
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = GtmGeomapArgs.__new__(GtmGeomapArgs)
```

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/trafficmanagement/gtm_property.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/gtm_property.py`

 * *Files 1% similar despite different names*

```diff
@@ -812,19 +812,19 @@
         return pulumi.get(self, "weighted_hash_bits_for_ipv6")
 
     @weighted_hash_bits_for_ipv6.setter
     def weighted_hash_bits_for_ipv6(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "weighted_hash_bits_for_ipv6", value)
 
 
-warnings.warn("""akamai.trafficmanagement.GtmProperty has been deprecated in favor of akamai.GtmProperty""", DeprecationWarning)
+warnings.warn("""akamai.trafficmanagement/gtmproperty.GtmProperty has been deprecated in favor of akamai.index/gtmproperty.GtmProperty""", DeprecationWarning)
 
 
 class GtmProperty(pulumi.CustomResource):
-    warnings.warn("""akamai.trafficmanagement.GtmProperty has been deprecated in favor of akamai.GtmProperty""", DeprecationWarning)
+    warnings.warn("""akamai.trafficmanagement/gtmproperty.GtmProperty has been deprecated in favor of akamai.index/gtmproperty.GtmProperty""", DeprecationWarning)
 
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  backup_cname: Optional[pulumi.Input[str]] = None,
                  backup_ip: Optional[pulumi.Input[str]] = None,
@@ -916,15 +916,15 @@
                  stickiness_bonus_percentage: Optional[pulumi.Input[int]] = None,
                  traffic_targets: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GtmPropertyTrafficTargetArgs']]]]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  unreachable_threshold: Optional[pulumi.Input[float]] = None,
                  use_computed_targets: Optional[pulumi.Input[bool]] = None,
                  wait_on_complete: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
-        pulumi.log.warn("""GtmProperty is deprecated: akamai.trafficmanagement.GtmProperty has been deprecated in favor of akamai.GtmProperty""")
+        pulumi.log.warn("""GtmProperty is deprecated: akamai.trafficmanagement/gtmproperty.GtmProperty has been deprecated in favor of akamai.index/gtmproperty.GtmProperty""")
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = GtmPropertyArgs.__new__(GtmPropertyArgs)
```

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/trafficmanagement/gtm_resource.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/gtm_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,19 +382,19 @@
         return pulumi.get(self, "wait_on_complete")
 
     @wait_on_complete.setter
     def wait_on_complete(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "wait_on_complete", value)
 
 
-warnings.warn("""akamai.trafficmanagement.GtmResource has been deprecated in favor of akamai.GtmResource""", DeprecationWarning)
+warnings.warn("""akamai.trafficmanagement/gtmresource.GtmResource has been deprecated in favor of akamai.index/gtmresource.GtmResource""", DeprecationWarning)
 
 
 class GtmResource(pulumi.CustomResource):
-    warnings.warn("""akamai.trafficmanagement.GtmResource has been deprecated in favor of akamai.GtmResource""", DeprecationWarning)
+    warnings.warn("""akamai.trafficmanagement/gtmresource.GtmResource has been deprecated in favor of akamai.index/gtmresource.GtmResource""", DeprecationWarning)
 
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  aggregation_type: Optional[pulumi.Input[str]] = None,
                  constrained_property: Optional[pulumi.Input[str]] = None,
@@ -452,15 +452,15 @@
                  max_u_multiplicative_increment: Optional[pulumi.Input[float]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  resource_instances: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GtmResourceResourceInstanceArgs']]]]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  upper_bound: Optional[pulumi.Input[int]] = None,
                  wait_on_complete: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
-        pulumi.log.warn("""GtmResource is deprecated: akamai.trafficmanagement.GtmResource has been deprecated in favor of akamai.GtmResource""")
+        pulumi.log.warn("""GtmResource is deprecated: akamai.trafficmanagement/gtmresource.GtmResource has been deprecated in favor of akamai.index/gtmresource.GtmResource""")
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = GtmResourceArgs.__new__(GtmResourceArgs)
```

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai/trafficmanagement/outputs.py` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai/trafficmanagement/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai.egg-info/PKG-INFO` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-akamai
-Version: 4.6.0a1688123148
+Version: 4.6.0a1688398728
 Summary: A Pulumi package for creating and managing akamai cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-akamai
 Keywords: pulumi akamai
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_akamai-4.6.0a1688123148/pulumi_akamai.egg-info/SOURCES.txt` & `pulumi_akamai-4.6.0a1688398728/pulumi_akamai.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,15 @@
 pulumi_akamai/get_iam_supported_langs.py
 pulumi_akamai/get_iam_timeout_policies.py
 pulumi_akamai/get_iam_timezones.py
 pulumi_akamai/get_network_lists.py
 pulumi_akamai/get_properties.py
 pulumi_akamai/get_properties_search.py
 pulumi_akamai/get_property.py
+pulumi_akamai/get_property_activation.py
 pulumi_akamai/get_property_hostnames.py
 pulumi_akamai/get_property_include.py
 pulumi_akamai/get_property_include_activation.py
 pulumi_akamai/get_property_include_parents.py
 pulumi_akamai/get_property_include_rules.py
 pulumi_akamai/get_property_includes.py
 pulumi_akamai/get_property_products.py
```

### Comparing `pulumi_akamai-4.6.0a1688123148/setup.py` & `pulumi_akamai-4.6.0a1688398728/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.6.0a1688123148"
-PLUGIN_VERSION = "4.6.0-alpha.1688123148+ef66745c"
+VERSION = "4.6.0a1688398728"
+PLUGIN_VERSION = "4.6.0-alpha.1688398728+6ae4f9e0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'akamai', PLUGIN_VERSION])
         except OSError as error:
```

