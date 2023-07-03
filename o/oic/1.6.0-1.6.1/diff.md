# Comparing `tmp/oic-1.6.0.tar.gz` & `tmp/oic-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oic-1.6.0.tar", last modified: Mon May 15 07:01:49 2023, max compression
+gzip compressed data, was "oic-1.6.1.tar", last modified: Mon Jul  3 07:08:43 2023, max compression
```

## Comparing `oic-1.6.0.tar` & `oic-1.6.1.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.541509 oic-1.6.0/
--rw-r--r--   0 tomas     (1000) tomas     (1000)      563 2021-02-12 13:09:56.000000 oic-1.6.0/LICENSE.txt
--rw-r--r--   0 tomas     (1000) tomas     (1000)       25 2021-02-12 13:09:56.000000 oic-1.6.0/MANIFEST.in
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5407 2023-05-15 07:01:49.541509 oic-1.6.0/PKG-INFO
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4493 2023-03-27 11:11:37.000000 oic-1.6.0/README.rst
--rw-r--r--   0 tomas     (1000) tomas     (1000)      281 2023-05-15 07:01:49.541509 oic-1.6.0/setup.cfg
--rwxr-xr-x   0 tomas     (1000) tomas     (1000)     3310 2023-05-02 08:00:09.000000 oic-1.6.0/setup.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.509509 oic-1.6.0/src/
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.513509 oic-1.6.0/src/oic/
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1450 2023-05-15 07:00:07.000000 oic-1.6.0/src/oic/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1492 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/exception.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.517509 oic-1.6.0/src/oic/extension/
--rw-r--r--   0 tomas     (1000) tomas     (1000)       22 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/extension/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    13270 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/extension/client.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     3802 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/extension/device_flow.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2232 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/extension/heart.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     8286 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/extension/message.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4191 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/extension/pop.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2817 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/extension/popjwt.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5495 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/extension/proof_of_possesion.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    29599 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/extension/provider.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5033 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/extension/signed_http_req.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)      256 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/extension/single.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2430 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/extension/sts.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5217 2023-05-02 08:00:09.000000 oic-1.6.0/src/oic/extension/token.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.521509 oic-1.6.0/src/oic/oauth2/
--rw-r--r--   0 tomas     (1000) tomas     (1000)    41235 2023-05-02 08:00:09.000000 oic-1.6.0/src/oic/oauth2/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5967 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/oauth2/base.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    11396 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/oauth2/consumer.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1111 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/oauth2/exception.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4766 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/oauth2/grant.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    39288 2023-05-02 08:00:09.000000 oic-1.6.0/src/oic/oauth2/message.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    38987 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/oauth2/provider.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     7251 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/oauth2/util.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.521509 oic-1.6.0/src/oic/oic/
--rw-r--r--   0 tomas     (1000) tomas     (1000)    65757 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/oic/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     7820 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/oic/claims_provider.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    18940 2023-05-02 08:00:12.000000 oic-1.6.0/src/oic/oic/consumer.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    40833 2023-05-02 08:00:09.000000 oic-1.6.0/src/oic/oic/message.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    83873 2023-05-02 08:00:09.000000 oic-1.6.0/src/oic/oic/provider.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)        0 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/py.typed
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.529509 oic-1.6.0/src/oic/utils/
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1063 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5983 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/aes.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.529509 oic-1.6.0/src/oic/utils/authn/
--rw-r--r--   0 tomas     (1000) tomas     (1000)       23 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/utils/authn/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     7098 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/authn/authn_context.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    18164 2022-03-08 09:59:02.000000 oic-1.6.0/src/oic/utils/authn/client.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1635 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/utils/authn/client_saml.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1981 2022-03-08 09:59:02.000000 oic-1.6.0/src/oic/utils/authn/javascript_login.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)      783 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/utils/authn/ldap_member.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     3217 2022-03-08 09:59:02.000000 oic-1.6.0/src/oic/utils/authn/ldapc.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2626 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/utils/authn/multi_auth.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    14777 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/authn/saml.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    13839 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/authn/user.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     7248 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/authn/user_cas.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1951 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/authz.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)      507 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/utils/claims.py
--rwxr-xr-x   0 tomas     (1000) tomas     (1000)     6200 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/client_management.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     3901 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/clientdb.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    19258 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/http_util.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     3615 2023-05-02 08:00:09.000000 oic-1.6.0/src/oic/utils/jwt.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    37029 2023-05-02 08:00:09.000000 oic-1.6.0/src/oic/utils/keyio.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1679 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/utils/restrict.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.529509 oic-1.6.0/src/oic/utils/rp/
--rw-r--r--   0 tomas     (1000) tomas     (1000)    15154 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/rp/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    12618 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/rp/oauth2.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1765 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/sanitize.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    32421 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/sdb.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     6122 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/session_backend.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2807 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/settings.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1601 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/shelve_wrapper.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     3635 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/stateless.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1640 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/utils/template_render.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    10293 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/time_util.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4535 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/utils/token_handler.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.533509 oic-1.6.0/src/oic/utils/userinfo/
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1316 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/utils/userinfo/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2307 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/userinfo/aa_info.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5011 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/userinfo/distaggr.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     3797 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/userinfo/ldap_info.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    10239 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/webfinger.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.513509 oic-1.6.0/src/oic.egg-info/
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5407 2023-05-15 07:01:49.000000 oic-1.6.0/src/oic.egg-info/PKG-INFO
--rw-r--r--   0 tomas     (1000) tomas     (1000)     3066 2023-05-15 07:01:49.000000 oic-1.6.0/src/oic.egg-info/SOURCES.txt
--rw-r--r--   0 tomas     (1000) tomas     (1000)        1 2023-05-15 07:01:49.000000 oic-1.6.0/src/oic.egg-info/dependency_links.txt
--rw-r--r--   0 tomas     (1000) tomas     (1000)       74 2023-05-15 07:01:49.000000 oic-1.6.0/src/oic.egg-info/entry_points.txt
--rw-r--r--   0 tomas     (1000) tomas     (1000)        1 2021-06-14 15:48:45.000000 oic-1.6.0/src/oic.egg-info/not-zip-safe
--rw-r--r--   0 tomas     (1000) tomas     (1000)      410 2023-05-15 07:01:49.000000 oic-1.6.0/src/oic.egg-info/requires.txt
--rw-r--r--   0 tomas     (1000) tomas     (1000)       95 2023-05-15 07:01:49.000000 oic-1.6.0/src/oic.egg-info/top_level.txt
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.541509 oic-1.6.0/tests/
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1672 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_aes.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2518 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_authn_context.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1041 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_authn_user.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1163 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_claims.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5260 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_claims_provider.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    12801 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_client.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1285 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_client_management.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4543 2023-03-27 11:11:37.000000 oic-1.6.0/tests/test_clientdb.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4372 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_grant.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     7590 2023-03-27 11:11:37.000000 oic-1.6.0/tests/test_http_util.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1522 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_jwt.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    19265 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_keyio.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    27204 2023-03-27 11:11:37.000000 oic-1.6.0/tests/test_oauth2.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    11031 2023-03-27 11:11:37.000000 oic-1.6.0/tests/test_oauth2_consumer.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    30827 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_oauth2_message.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    32548 2023-03-27 11:11:37.000000 oic-1.6.0/tests/test_oauth2_provider.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    52202 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_oic.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    43996 2023-05-02 08:00:12.000000 oic-1.6.0/tests/test_oic_consumer.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    12012 2023-03-27 11:11:37.000000 oic-1.6.0/tests/test_oic_consumer_logout.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    47073 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_oic_message.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    76101 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_oic_provider.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    40165 2023-03-27 11:11:37.000000 oic-1.6.0/tests/test_oic_provider_logout.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4670 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_pop.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     7936 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_popjwt.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2725 2023-03-27 11:11:37.000000 oic-1.6.0/tests/test_sanitize.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    27871 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_sdb.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1595 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_shelve_wrapper.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4871 2023-03-27 11:11:37.000000 oic-1.6.0/tests/test_signed_http_request.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)      914 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_stateless.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     6728 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_time_util.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    16929 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_token.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4695 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_token_handler.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4270 2023-03-27 11:11:37.000000 oic-1.6.0/tests/test_user.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    10676 2023-03-27 11:11:37.000000 oic-1.6.0/tests/test_util.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     7150 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_webfinger.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     8586 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_x_client.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    11688 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_x_dynreg.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    20499 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_x_provider.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.447884 oic-1.6.1/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      563 2021-02-12 13:09:56.000000 oic-1.6.1/LICENSE.txt
+-rw-r--r--   0 tomas     (1000) tomas     (1000)       25 2021-02-12 13:09:56.000000 oic-1.6.1/MANIFEST.in
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5407 2023-07-03 07:08:43.447884 oic-1.6.1/PKG-INFO
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4493 2023-03-27 11:11:37.000000 oic-1.6.1/README.rst
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      281 2023-07-03 07:08:43.447884 oic-1.6.1/setup.cfg
+-rwxr-xr-x   0 tomas     (1000) tomas     (1000)     3319 2023-07-03 07:05:06.000000 oic-1.6.1/setup.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.431884 oic-1.6.1/src/
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.435884 oic-1.6.1/src/oic/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1450 2023-07-03 07:07:13.000000 oic-1.6.1/src/oic/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1492 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/exception.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.435884 oic-1.6.1/src/oic/extension/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)       22 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/extension/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    13270 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/extension/client.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     3802 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/extension/device_flow.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2232 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/extension/heart.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     8286 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/extension/message.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4191 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/extension/pop.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2817 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/extension/popjwt.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5495 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/extension/proof_of_possesion.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    29599 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/extension/provider.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5033 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/extension/signed_http_req.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      256 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/extension/single.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2430 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/extension/sts.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5217 2023-05-02 08:00:09.000000 oic-1.6.1/src/oic/extension/token.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.439884 oic-1.6.1/src/oic/oauth2/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    41235 2023-05-02 08:00:09.000000 oic-1.6.1/src/oic/oauth2/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5967 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/oauth2/base.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    11396 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/oauth2/consumer.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1111 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/oauth2/exception.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4766 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/oauth2/grant.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    39288 2023-05-02 08:00:09.000000 oic-1.6.1/src/oic/oauth2/message.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    38987 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/oauth2/provider.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     7251 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/oauth2/util.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.439884 oic-1.6.1/src/oic/oic/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    65757 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/oic/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     7820 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/oic/claims_provider.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    18940 2023-05-02 08:00:12.000000 oic-1.6.1/src/oic/oic/consumer.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    40833 2023-05-02 08:00:09.000000 oic-1.6.1/src/oic/oic/message.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    83873 2023-05-02 08:00:09.000000 oic-1.6.1/src/oic/oic/provider.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)        0 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/py.typed
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.443884 oic-1.6.1/src/oic/utils/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1063 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5983 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/aes.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.443884 oic-1.6.1/src/oic/utils/authn/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)       23 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/utils/authn/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     7098 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/authn/authn_context.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    18164 2022-03-08 09:59:02.000000 oic-1.6.1/src/oic/utils/authn/client.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1635 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/utils/authn/client_saml.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1981 2022-03-08 09:59:02.000000 oic-1.6.1/src/oic/utils/authn/javascript_login.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      783 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/utils/authn/ldap_member.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     3217 2022-03-08 09:59:02.000000 oic-1.6.1/src/oic/utils/authn/ldapc.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2626 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/utils/authn/multi_auth.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    14777 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/authn/saml.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    13839 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/authn/user.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     7248 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/authn/user_cas.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1951 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/authz.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      507 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/utils/claims.py
+-rwxr-xr-x   0 tomas     (1000) tomas     (1000)     6200 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/client_management.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     3901 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/clientdb.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    19258 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/http_util.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     3615 2023-05-02 08:00:09.000000 oic-1.6.1/src/oic/utils/jwt.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    37029 2023-05-02 08:00:09.000000 oic-1.6.1/src/oic/utils/keyio.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1679 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/utils/restrict.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.443884 oic-1.6.1/src/oic/utils/rp/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    15154 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/rp/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    12618 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/rp/oauth2.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1765 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/sanitize.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    32421 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/sdb.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     6122 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/session_backend.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2825 2023-07-03 07:05:06.000000 oic-1.6.1/src/oic/utils/settings.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1601 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/shelve_wrapper.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     3635 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/stateless.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1640 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/utils/template_render.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    10293 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/time_util.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4535 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/utils/token_handler.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.443884 oic-1.6.1/src/oic/utils/userinfo/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1316 2021-02-12 13:09:56.000000 oic-1.6.1/src/oic/utils/userinfo/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2307 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/userinfo/aa_info.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5011 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/userinfo/distaggr.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     3797 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/userinfo/ldap_info.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    10239 2023-03-27 11:11:37.000000 oic-1.6.1/src/oic/utils/webfinger.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.435884 oic-1.6.1/src/oic.egg-info/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5407 2023-07-03 07:08:43.000000 oic-1.6.1/src/oic.egg-info/PKG-INFO
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     3066 2023-07-03 07:08:43.000000 oic-1.6.1/src/oic.egg-info/SOURCES.txt
+-rw-r--r--   0 tomas     (1000) tomas     (1000)        1 2023-07-03 07:08:43.000000 oic-1.6.1/src/oic.egg-info/dependency_links.txt
+-rw-r--r--   0 tomas     (1000) tomas     (1000)       74 2023-07-03 07:08:43.000000 oic-1.6.1/src/oic.egg-info/entry_points.txt
+-rw-r--r--   0 tomas     (1000) tomas     (1000)        1 2021-06-14 15:48:45.000000 oic-1.6.1/src/oic.egg-info/not-zip-safe
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      419 2023-07-03 07:08:43.000000 oic-1.6.1/src/oic.egg-info/requires.txt
+-rw-r--r--   0 tomas     (1000) tomas     (1000)       95 2023-07-03 07:08:43.000000 oic-1.6.1/src/oic.egg-info/top_level.txt
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-03 07:08:43.447884 oic-1.6.1/tests/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1672 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_aes.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2518 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_authn_context.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1041 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_authn_user.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1163 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_claims.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5260 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_claims_provider.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    12801 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_client.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1285 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_client_management.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4543 2023-03-27 11:11:37.000000 oic-1.6.1/tests/test_clientdb.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4372 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_grant.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     7590 2023-03-27 11:11:37.000000 oic-1.6.1/tests/test_http_util.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1522 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_jwt.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    19265 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_keyio.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    27204 2023-03-27 11:11:37.000000 oic-1.6.1/tests/test_oauth2.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    11031 2023-03-27 11:11:37.000000 oic-1.6.1/tests/test_oauth2_consumer.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    30827 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_oauth2_message.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    32548 2023-03-27 11:11:37.000000 oic-1.6.1/tests/test_oauth2_provider.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    52202 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_oic.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    43996 2023-05-02 08:00:12.000000 oic-1.6.1/tests/test_oic_consumer.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    12012 2023-03-27 11:11:37.000000 oic-1.6.1/tests/test_oic_consumer_logout.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    47073 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_oic_message.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    76101 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_oic_provider.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    40165 2023-03-27 11:11:37.000000 oic-1.6.1/tests/test_oic_provider_logout.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4670 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_pop.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     7936 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_popjwt.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2725 2023-03-27 11:11:37.000000 oic-1.6.1/tests/test_sanitize.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    27871 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_sdb.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1595 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_shelve_wrapper.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4871 2023-03-27 11:11:37.000000 oic-1.6.1/tests/test_signed_http_request.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      914 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_stateless.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     6728 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_time_util.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    16929 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_token.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4695 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_token_handler.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4270 2023-03-27 11:11:37.000000 oic-1.6.1/tests/test_user.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    10676 2023-03-27 11:11:37.000000 oic-1.6.1/tests/test_util.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     7150 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_webfinger.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     8586 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_x_client.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    11688 2021-02-12 13:09:56.000000 oic-1.6.1/tests/test_x_dynreg.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    20499 2023-05-02 08:00:09.000000 oic-1.6.1/tests/test_x_provider.py
```

### Comparing `oic-1.6.0/LICENSE.txt` & `oic-1.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/PKG-INFO` & `oic-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oic
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python implementation of OAuth2 and OpenID Connect
 Home-page: https://github.com/CZ-NIC/pyoidc/
 Author: Roland Hedberg
 Author-email: roland@catalogix.se
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `oic-1.6.0/README.rst` & `oic-1.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/setup.py` & `oic-1.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         'types': ['types-requests'],
         'ldap_authn': ['python-ldap'],
         'examples': ['beaker'],
     },
     install_requires=[
         "requests",
         "pycryptodomex",
-        "pydantic",
+        "pydantic-settings",
         "pyjwkest>=1.3.6",
         "mako",
         "cryptography",
         "defusedxml",
         'typing_extensions; python_version<"3.8"',
     ],
     tests_require=tests_requires,
```

### Comparing `oic-1.6.0/src/oic/__init__.py` & `oic-1.6.1/src/oic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         warnings.warn(
             "No good random number generator available on this platform. "
             "Security tokens will be weak and guessable.",
             RuntimeWarning,
         )
 
 __author__ = "Roland Hedberg"
-__version__ = "1.6.0"
+__version__ = "1.6.1"
 
 
 OIDCONF_PATTERN = "%s/.well-known/openid-configuration"
 CC_METHOD = {"S256": hashlib.sha256, "S384": hashlib.sha384, "S512": hashlib.sha512}
 
 
 def rndstr(size=16):
```

### Comparing `oic-1.6.0/src/oic/exception.py` & `oic-1.6.1/src/oic/exception.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/extension/client.py` & `oic-1.6.1/src/oic/extension/client.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/extension/device_flow.py` & `oic-1.6.1/src/oic/extension/device_flow.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/extension/heart.py` & `oic-1.6.1/src/oic/extension/heart.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/extension/message.py` & `oic-1.6.1/src/oic/extension/message.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/extension/pop.py` & `oic-1.6.1/src/oic/extension/pop.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/extension/popjwt.py` & `oic-1.6.1/src/oic/extension/popjwt.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/extension/proof_of_possesion.py` & `oic-1.6.1/src/oic/extension/proof_of_possesion.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/extension/provider.py` & `oic-1.6.1/src/oic/extension/provider.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/extension/signed_http_req.py` & `oic-1.6.1/src/oic/extension/signed_http_req.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/extension/sts.py` & `oic-1.6.1/src/oic/extension/sts.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/extension/token.py` & `oic-1.6.1/src/oic/extension/token.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/oauth2/__init__.py` & `oic-1.6.1/src/oic/oauth2/__init__.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/oauth2/base.py` & `oic-1.6.1/src/oic/oauth2/base.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/oauth2/consumer.py` & `oic-1.6.1/src/oic/oauth2/consumer.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/oauth2/exception.py` & `oic-1.6.1/src/oic/oauth2/exception.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/oauth2/grant.py` & `oic-1.6.1/src/oic/oauth2/grant.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/oauth2/message.py` & `oic-1.6.1/src/oic/oauth2/message.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/oauth2/provider.py` & `oic-1.6.1/src/oic/oauth2/provider.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/oauth2/util.py` & `oic-1.6.1/src/oic/oauth2/util.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/oic/__init__.py` & `oic-1.6.1/src/oic/oic/__init__.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/oic/claims_provider.py` & `oic-1.6.1/src/oic/oic/claims_provider.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/oic/consumer.py` & `oic-1.6.1/src/oic/oic/consumer.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/oic/message.py` & `oic-1.6.1/src/oic/oic/message.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/oic/provider.py` & `oic-1.6.1/src/oic/oic/provider.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/__init__.py` & `oic-1.6.1/src/oic/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/aes.py` & `oic-1.6.1/src/oic/utils/aes.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/authn/authn_context.py` & `oic-1.6.1/src/oic/utils/authn/authn_context.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/authn/client.py` & `oic-1.6.1/src/oic/utils/authn/client.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/authn/client_saml.py` & `oic-1.6.1/src/oic/utils/authn/client_saml.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/authn/javascript_login.py` & `oic-1.6.1/src/oic/utils/authn/javascript_login.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/authn/ldap_member.py` & `oic-1.6.1/src/oic/utils/authn/ldap_member.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/authn/ldapc.py` & `oic-1.6.1/src/oic/utils/authn/ldapc.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/authn/multi_auth.py` & `oic-1.6.1/src/oic/utils/authn/multi_auth.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/authn/saml.py` & `oic-1.6.1/src/oic/utils/authn/saml.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/authn/user.py` & `oic-1.6.1/src/oic/utils/authn/user.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/authn/user_cas.py` & `oic-1.6.1/src/oic/utils/authn/user_cas.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/authz.py` & `oic-1.6.1/src/oic/utils/authz.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/client_management.py` & `oic-1.6.1/src/oic/utils/client_management.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/clientdb.py` & `oic-1.6.1/src/oic/utils/clientdb.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/http_util.py` & `oic-1.6.1/src/oic/utils/http_util.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/jwt.py` & `oic-1.6.1/src/oic/utils/jwt.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/keyio.py` & `oic-1.6.1/src/oic/utils/keyio.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/restrict.py` & `oic-1.6.1/src/oic/utils/restrict.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/rp/__init__.py` & `oic-1.6.1/src/oic/utils/rp/__init__.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/rp/oauth2.py` & `oic-1.6.1/src/oic/utils/rp/oauth2.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/sanitize.py` & `oic-1.6.1/src/oic/utils/sanitize.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/sdb.py` & `oic-1.6.1/src/oic/utils/sdb.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/session_backend.py` & `oic-1.6.1/src/oic/utils/session_backend.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/settings.py` & `oic-1.6.1/src/oic/utils/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
     This part is under development.
     Most of the configuration options are being converted from keyword arguments to settings class.
     Using the settings class is optional for now, but will become a necessity later on.
 
 In order to configure some objects in PyOIDC, you need a settings object.
 If you need to add some settings, make sure that you settings class inherits from the appropriate class in this module.
 
-The settings make use of `pydantic <https://docs.pydantic.dev/usage/settings/>`_ library.
+The settings make use of `pydantic-settings <https://docs.pydantic.dev/usage/settings/>`_ library.
 It is possible to instance them directly or use environment values to fill the settings.
 """
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import requests
-from pydantic import BaseSettings
+from pydantic_settings import BaseSettings
 
 
 class PyoidcSettings(BaseSettings):
     """Main class for all settings shared among consumer and client."""
 
     verify_ssl: Union[bool, str] = True
     """
```

### Comparing `oic-1.6.0/src/oic/utils/shelve_wrapper.py` & `oic-1.6.1/src/oic/utils/shelve_wrapper.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/stateless.py` & `oic-1.6.1/src/oic/utils/stateless.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/template_render.py` & `oic-1.6.1/src/oic/utils/template_render.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/time_util.py` & `oic-1.6.1/src/oic/utils/time_util.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/token_handler.py` & `oic-1.6.1/src/oic/utils/token_handler.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/userinfo/__init__.py` & `oic-1.6.1/src/oic/utils/userinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/userinfo/aa_info.py` & `oic-1.6.1/src/oic/utils/userinfo/aa_info.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/userinfo/distaggr.py` & `oic-1.6.1/src/oic/utils/userinfo/distaggr.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/userinfo/ldap_info.py` & `oic-1.6.1/src/oic/utils/userinfo/ldap_info.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic/utils/webfinger.py` & `oic-1.6.1/src/oic/utils/webfinger.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/src/oic.egg-info/PKG-INFO` & `oic-1.6.1/src/oic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oic
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python implementation of OAuth2 and OpenID Connect
 Home-page: https://github.com/CZ-NIC/pyoidc/
 Author: Roland Hedberg
 Author-email: roland@catalogix.se
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `oic-1.6.0/src/oic.egg-info/SOURCES.txt` & `oic-1.6.1/src/oic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_aes.py` & `oic-1.6.1/tests/test_aes.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_authn_context.py` & `oic-1.6.1/tests/test_authn_context.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_authn_user.py` & `oic-1.6.1/tests/test_authn_user.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_claims.py` & `oic-1.6.1/tests/test_claims.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_claims_provider.py` & `oic-1.6.1/tests/test_claims_provider.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_client.py` & `oic-1.6.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_client_management.py` & `oic-1.6.1/tests/test_client_management.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_clientdb.py` & `oic-1.6.1/tests/test_clientdb.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_grant.py` & `oic-1.6.1/tests/test_grant.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_http_util.py` & `oic-1.6.1/tests/test_http_util.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_jwt.py` & `oic-1.6.1/tests/test_jwt.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_keyio.py` & `oic-1.6.1/tests/test_keyio.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_oauth2.py` & `oic-1.6.1/tests/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_oauth2_consumer.py` & `oic-1.6.1/tests/test_oauth2_consumer.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_oauth2_message.py` & `oic-1.6.1/tests/test_oauth2_message.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_oauth2_provider.py` & `oic-1.6.1/tests/test_oauth2_provider.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_oic.py` & `oic-1.6.1/tests/test_oic.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_oic_consumer.py` & `oic-1.6.1/tests/test_oic_consumer.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_oic_consumer_logout.py` & `oic-1.6.1/tests/test_oic_consumer_logout.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_oic_message.py` & `oic-1.6.1/tests/test_oic_message.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_oic_provider.py` & `oic-1.6.1/tests/test_oic_provider.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_oic_provider_logout.py` & `oic-1.6.1/tests/test_oic_provider_logout.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_pop.py` & `oic-1.6.1/tests/test_pop.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_popjwt.py` & `oic-1.6.1/tests/test_popjwt.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_sanitize.py` & `oic-1.6.1/tests/test_sanitize.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_sdb.py` & `oic-1.6.1/tests/test_sdb.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_shelve_wrapper.py` & `oic-1.6.1/tests/test_shelve_wrapper.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_signed_http_request.py` & `oic-1.6.1/tests/test_signed_http_request.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_stateless.py` & `oic-1.6.1/tests/test_stateless.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_time_util.py` & `oic-1.6.1/tests/test_time_util.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_token.py` & `oic-1.6.1/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_token_handler.py` & `oic-1.6.1/tests/test_token_handler.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_user.py` & `oic-1.6.1/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_util.py` & `oic-1.6.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_webfinger.py` & `oic-1.6.1/tests/test_webfinger.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_x_client.py` & `oic-1.6.1/tests/test_x_client.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_x_dynreg.py` & `oic-1.6.1/tests/test_x_dynreg.py`

 * *Files identical despite different names*

### Comparing `oic-1.6.0/tests/test_x_provider.py` & `oic-1.6.1/tests/test_x_provider.py`

 * *Files identical despite different names*

