# Comparing `tmp/bce-python-sdk-0.8.83.tar.gz` & `tmp/bce-python-sdk-0.8.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bce-python-sdk-0.8.83.tar", last modified: Mon Mar 27 13:04:07 2023, max compression
+gzip compressed data, was "bce-python-sdk-0.8.87.tar", last modified: Mon Jul  3 11:45:00 2023, max compression
```

## Comparing `bce-python-sdk-0.8.83.tar` & `bce-python-sdk-0.8.87.tar`

### file list

```diff
@@ -1,173 +1,177 @@
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.718203 bce-python-sdk-0.8.83/
--rw-r--r--   0 aimingzhen   (502) staff       (20)      225 2023-03-27 13:04:07.718007 bce-python-sdk-0.8.83/PKG-INFO
--rw-r--r--   0 aimingzhen   (502) staff       (20)       40 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/README.txt
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.693150 bce-python-sdk-0.8.83/baidubce/
--rwxr-xr-x   0 aimingzhen   (502) staff       (20)      812 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/__init__.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.693866 bce-python-sdk-0.8.83/baidubce/auth/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/auth/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     1157 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/auth/bce_credentials.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     3211 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/auth/bce_v1_signer.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     3428 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/bce_base_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     2801 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/bce_client_configuration.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     1655 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/bce_response.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     3467 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/compat.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     1544 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/exception.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.695182 bce-python-sdk-0.8.83/baidubce/http/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/http/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     8574 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/http/bce_http_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     2930 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/http/handler.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)      722 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/http/http_content_types.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     2581 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/http/http_headers.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)      782 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/http/http_methods.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     1151 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/protocol.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)      835 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/region.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.695559 bce-python-sdk-0.8.83/baidubce/retry/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/retry/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     4926 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/retry/retry_policy.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.695753 bce-python-sdk-0.8.83/baidubce/services/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/__init__.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.696340 bce-python-sdk-0.8.83/baidubce/services/bbc/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bbc/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    35864 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bbc/bbc_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     1595 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bbc/bbc_model.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.697402 bce-python-sdk-0.8.83/baidubce/services/bcc/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bcc/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)   115530 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bcc/bcc_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     4603 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bcc/bcc_model.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)      948 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bcc/fpga_card_type.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     1054 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bcc/gpu_card_type.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.697826 bce-python-sdk-0.8.83/baidubce/services/bcm/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bcm/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     7419 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bcm/bcm_client.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.698459 bce-python-sdk-0.8.83/baidubce/services/bes/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bes/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    22810 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bes/bes_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     1784 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bes/bes_model.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.699128 bce-python-sdk-0.8.83/baidubce/services/blb/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/blb/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    88234 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/blb/app_blb_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    83658 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/blb/blb_client.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.699567 bce-python-sdk-0.8.83/baidubce/services/bmr/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bmr/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    20565 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bmr/bmr_client.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.700685 bce-python-sdk-0.8.83/baidubce/services/bos/
--rw-r--r--   0 aimingzhen   (502) staff       (20)      813 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bos/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    93955 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bos/bos_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     1832 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bos/bos_handler.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)      723 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bos/canned_acl.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)      729 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bos/storage_class.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.701616 bce-python-sdk-0.8.83/baidubce/services/bts/
--rw-r--r--   0 aimingzhen   (502) staff       (20)      749 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bts/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    19286 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bts/bts_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     8269 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bts/model.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     1521 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/bts/util.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.702271 bce-python-sdk-0.8.83/baidubce/services/cdn/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/cdn/__init__.py
--rwxr-xr-x   0 aimingzhen   (502) staff       (20)    59017 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/cdn/cdn_client.py
--rwxr-xr-x   0 aimingzhen   (502) staff       (20)     1252 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/cdn/cdn_stats_param.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.702787 bce-python-sdk-0.8.83/baidubce/services/cert/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/cert/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     4659 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/cert/cert_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     1622 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/cert/cert_model.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.703579 bce-python-sdk-0.8.83/baidubce/services/cfc/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/cfc/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    42843 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/cfc/cfc_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     3037 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/cfc/cfc_handler.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     5722 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/cfc/models.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.703973 bce-python-sdk-0.8.83/baidubce/services/ddc/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/ddc/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     6834 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/ddc/ddc_client.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.704341 bce-python-sdk-0.8.83/baidubce/services/dns/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/dns/__init__.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.704697 bce-python-sdk-0.8.83/baidubce/services/dns/api/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/dns/api/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     4350 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/dns/api/dns_api.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    15953 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/dns/dns_client.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.705034 bce-python-sdk-0.8.83/baidubce/services/dumap/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/dumap/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     3955 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/dumap/dumap_client.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.706395 bce-python-sdk-0.8.83/baidubce/services/eip/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/eip/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    13055 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/eip/eip_bp_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    14340 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/eip/eip_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    15561 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/eip/eip_group_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     1914 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/eip/eip_group_model.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     8798 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/eip/eip_tp_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     1769 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/eip/model.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.706925 bce-python-sdk-0.8.83/baidubce/services/endpoint/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/endpoint/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     9317 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/endpoint/endpoint_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     1592 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/endpoint/model.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.707362 bce-python-sdk-0.8.83/baidubce/services/iam/
--rw-r--r--   0 aimingzhen   (502) staff       (20)      668 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/iam/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    21995 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/iam/iam_client.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.707819 bce-python-sdk-0.8.83/baidubce/services/infinite/
--rw-r--r--   0 aimingzhen   (502) staff       (20)      655 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/infinite/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     8898 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/infinite/infinite_client.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.709069 bce-python-sdk-0.8.83/baidubce/services/kms/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/kms/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)      794 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/kms/keyspec_class.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    17789 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/kms/kms_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)      640 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/kms/origin_class.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)      633 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/kms/protectedby_class.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)      655 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/kms/publickeyencoding_class.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.709667 bce-python-sdk-0.8.83/baidubce/services/media/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/media/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    25881 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/media/media_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     2460 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/media/media_handler.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.710079 bce-python-sdk-0.8.83/baidubce/services/mms/
--rw-r--r--   0 aimingzhen   (502) staff       (20)      610 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/mms/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    19332 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/mms/mms_client.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.710489 bce-python-sdk-0.8.83/baidubce/services/mvs/
--rw-r--r--   0 aimingzhen   (502) staff       (20)      610 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/mvs/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     5802 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/mvs/mvs_client.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.711068 bce-python-sdk-0.8.83/baidubce/services/route/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/route/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     8382 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/route/route_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)      280 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/route/route_model.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.711778 bce-python-sdk-0.8.83/baidubce/services/scs/
--rw-r--r--   0 aimingzhen   (502) staff       (20)      707 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/scs/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     8355 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/scs/model.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    27357 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/scs/scs_client.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.712408 bce-python-sdk-0.8.83/baidubce/services/sms/
--rw-r--r--   0 aimingzhen   (502) staff       (20)      676 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/sms/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     3584 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/sms/model.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    22508 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/sms/sms_client.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.712797 bce-python-sdk-0.8.83/baidubce/services/sts/
--rw-r--r--   0 aimingzhen   (502) staff       (20)      669 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/sts/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     3687 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/sts/sts_client.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.713190 bce-python-sdk-0.8.83/baidubce/services/subnet/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/subnet/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    10363 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/subnet/subnet_client.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.713961 bce-python-sdk-0.8.83/baidubce/services/tsdb/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/tsdb/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     4845 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/tsdb/tsdb_admin_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     9337 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/tsdb/tsdb_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     1744 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/tsdb/tsdb_handler.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.714339 bce-python-sdk-0.8.83/baidubce/services/vca/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/vca/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     5273 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/vca/vca_client.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.714718 bce-python-sdk-0.8.83/baidubce/services/vcr/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/vcr/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    13004 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/vcr/vcr_client.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.716113 bce-python-sdk-0.8.83/baidubce/services/vpc/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/vpc/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    11761 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/vpc/acl_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    14538 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/vpc/nat_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     1688 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/vpc/nat_model.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    20077 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/vpc/peerconn_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     1681 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/vpc/peerconn_model.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     8718 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/vpc/vpc_client.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.716763 bce-python-sdk-0.8.83/baidubce/services/vpn/
--rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/vpn/__init__.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    19844 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/vpn/vpn_client.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)     2888 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/services/vpn/vpn_model.py
--rw-r--r--   0 aimingzhen   (502) staff       (20)    19730 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/baidubce/utils.py
-drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-03-27 13:04:07.717770 bce-python-sdk-0.8.83/bce_python_sdk.egg-info/
--rw-r--r--   0 aimingzhen   (502) staff       (20)      225 2023-03-27 13:04:07.000000 bce-python-sdk-0.8.83/bce_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 aimingzhen   (502) staff       (20)     4543 2023-03-27 13:04:07.000000 bce-python-sdk-0.8.83/bce_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 aimingzhen   (502) staff       (20)        1 2023-03-27 13:04:07.000000 bce-python-sdk-0.8.83/bce_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 aimingzhen   (502) staff       (20)       45 2023-03-27 13:04:07.000000 bce-python-sdk-0.8.83/bce_python_sdk.egg-info/requires.txt
--rw-r--r--   0 aimingzhen   (502) staff       (20)        9 2023-03-27 13:04:07.000000 bce-python-sdk-0.8.83/bce_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 aimingzhen   (502) staff       (20)       38 2023-03-27 13:04:07.718253 bce-python-sdk-0.8.83/setup.cfg
--rw-r--r--   0 aimingzhen   (502) staff       (20)     2794 2023-03-27 08:32:21.000000 bce-python-sdk-0.8.83/setup.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.400172 bce-python-sdk-0.8.87/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)      225 2023-07-03 11:45:00.399937 bce-python-sdk-0.8.87/PKG-INFO
+-rw-r--r--   0 aimingzhen   (502) staff       (20)       40 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/README.txt
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.372032 bce-python-sdk-0.8.87/baidubce/
+-rwxr-xr-x   0 aimingzhen   (502) staff       (20)      813 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/__init__.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.372680 bce-python-sdk-0.8.87/baidubce/auth/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/auth/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     1157 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/auth/bce_credentials.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     3211 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/auth/bce_v1_signer.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     3428 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/bce_base_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     2801 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/bce_client_configuration.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     1655 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/bce_response.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     3467 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/compat.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     1544 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/exception.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.373998 bce-python-sdk-0.8.87/baidubce/http/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/http/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     8574 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/http/bce_http_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     2930 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/http/handler.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)      722 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/http/http_content_types.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     2627 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/http/http_headers.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)      782 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/http/http_methods.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     1151 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/protocol.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)      835 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/region.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.374476 bce-python-sdk-0.8.87/baidubce/retry/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/retry/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     4926 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/retry/retry_policy.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.374717 bce-python-sdk-0.8.87/baidubce/services/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/__init__.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.375325 bce-python-sdk-0.8.87/baidubce/services/bbc/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bbc/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    35864 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bbc/bbc_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     1595 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bbc/bbc_model.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.376540 bce-python-sdk-0.8.87/baidubce/services/bcc/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bcc/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)   214596 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bcc/bcc_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     5919 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bcc/bcc_model.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)      948 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bcc/fpga_card_type.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     1054 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bcc/gpu_card_type.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.376950 bce-python-sdk-0.8.87/baidubce/services/bcm/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bcm/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     7419 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bcm/bcm_client.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.378449 bce-python-sdk-0.8.87/baidubce/services/bes/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bes/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    22810 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bes/bes_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     1784 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bes/bes_model.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.379140 bce-python-sdk-0.8.87/baidubce/services/blb/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/blb/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    88234 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/blb/app_blb_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    83658 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/blb/blb_client.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.379581 bce-python-sdk-0.8.87/baidubce/services/bmr/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bmr/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    20565 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bmr/bmr_client.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.380740 bce-python-sdk-0.8.87/baidubce/services/bos/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)      813 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bos/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    96086 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bos/bos_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     1832 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bos/bos_handler.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)      723 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bos/canned_acl.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)      729 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bos/storage_class.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.381597 bce-python-sdk-0.8.87/baidubce/services/bts/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)      749 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bts/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    19286 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bts/bts_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     8269 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bts/model.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     1521 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/bts/util.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.382277 bce-python-sdk-0.8.87/baidubce/services/cdn/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/cdn/__init__.py
+-rwxr-xr-x   0 aimingzhen   (502) staff       (20)    59017 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/cdn/cdn_client.py
+-rwxr-xr-x   0 aimingzhen   (502) staff       (20)     1252 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/cdn/cdn_stats_param.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.382951 bce-python-sdk-0.8.87/baidubce/services/cert/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/cert/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     4659 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/cert/cert_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     1622 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/cert/cert_model.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.383871 bce-python-sdk-0.8.87/baidubce/services/cfc/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/cfc/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    42843 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/cfc/cfc_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     3037 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/cfc/cfc_handler.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     5722 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/cfc/models.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.384294 bce-python-sdk-0.8.87/baidubce/services/ddc/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/ddc/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     6834 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/ddc/ddc_client.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.384698 bce-python-sdk-0.8.87/baidubce/services/dns/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/dns/__init__.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.385131 bce-python-sdk-0.8.87/baidubce/services/dns/api/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/dns/api/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     4350 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/dns/api/dns_api.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    15953 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/dns/dns_client.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.385541 bce-python-sdk-0.8.87/baidubce/services/dumap/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/dumap/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     3955 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/dumap/dumap_client.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.387003 bce-python-sdk-0.8.87/baidubce/services/eip/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/eip/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    13055 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/eip/eip_bp_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    14340 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/eip/eip_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    15561 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/eip/eip_group_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     1914 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/eip/eip_group_model.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     8798 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/eip/eip_tp_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     1769 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/eip/model.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.387607 bce-python-sdk-0.8.87/baidubce/services/endpoint/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/endpoint/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     9317 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/endpoint/endpoint_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     1592 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/endpoint/model.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.388012 bce-python-sdk-0.8.87/baidubce/services/iam/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)      668 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/iam/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    21995 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/iam/iam_client.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.388431 bce-python-sdk-0.8.87/baidubce/services/infinite/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)      655 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/infinite/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     8898 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/infinite/infinite_client.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.389693 bce-python-sdk-0.8.87/baidubce/services/kms/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/kms/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)      794 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/kms/keyspec_class.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    17789 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/kms/kms_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)      640 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/kms/origin_class.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)      633 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/kms/protectedby_class.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)      655 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/kms/publickeyencoding_class.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.390319 bce-python-sdk-0.8.87/baidubce/services/media/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/media/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    25881 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/media/media_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     2460 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/media/media_handler.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.390747 bce-python-sdk-0.8.87/baidubce/services/mms/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)      610 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/mms/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    19332 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/mms/mms_client.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.391137 bce-python-sdk-0.8.87/baidubce/services/mvs/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)      610 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/mvs/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     5802 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/mvs/mvs_client.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.391764 bce-python-sdk-0.8.87/baidubce/services/rds/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)      707 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/rds/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     9387 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/rds/model.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    37115 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/rds/rds_client.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.392432 bce-python-sdk-0.8.87/baidubce/services/route/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/route/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     8382 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/route/route_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)      280 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/route/route_model.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.393093 bce-python-sdk-0.8.87/baidubce/services/scs/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)      707 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/scs/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     8355 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/scs/model.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    27357 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/scs/scs_client.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.393802 bce-python-sdk-0.8.87/baidubce/services/sms/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)      676 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/sms/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     3584 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/sms/model.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    22508 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/sms/sms_client.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.394271 bce-python-sdk-0.8.87/baidubce/services/sts/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)      669 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/sts/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     3687 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/sts/sts_client.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.394657 bce-python-sdk-0.8.87/baidubce/services/subnet/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/subnet/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    10363 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/subnet/subnet_client.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.395509 bce-python-sdk-0.8.87/baidubce/services/tsdb/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/tsdb/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     4845 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/tsdb/tsdb_admin_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     9337 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/tsdb/tsdb_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     1744 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/tsdb/tsdb_handler.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.395915 bce-python-sdk-0.8.87/baidubce/services/vca/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/vca/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     5273 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/vca/vca_client.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.396338 bce-python-sdk-0.8.87/baidubce/services/vcr/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/vcr/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    13004 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/vcr/vcr_client.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.397895 bce-python-sdk-0.8.87/baidubce/services/vpc/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/vpc/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    11761 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/vpc/acl_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    14538 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/vpc/nat_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     1688 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/vpc/nat_model.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    20077 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/vpc/peerconn_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     1681 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/vpc/peerconn_model.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     8718 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/vpc/vpc_client.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.398556 bce-python-sdk-0.8.87/baidubce/services/vpn/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        0 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/vpn/__init__.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    19844 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/vpn/vpn_client.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     2888 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/services/vpn/vpn_model.py
+-rw-r--r--   0 aimingzhen   (502) staff       (20)    19730 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/baidubce/utils.py
+drwxr-xr-x   0 aimingzhen   (502) staff       (20)        0 2023-07-03 11:45:00.399655 bce-python-sdk-0.8.87/bce_python_sdk.egg-info/
+-rw-r--r--   0 aimingzhen   (502) staff       (20)      225 2023-07-03 11:45:00.000000 bce-python-sdk-0.8.87/bce_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     4644 2023-07-03 11:45:00.000000 bce-python-sdk-0.8.87/bce_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        1 2023-07-03 11:45:00.000000 bce-python-sdk-0.8.87/bce_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 aimingzhen   (502) staff       (20)       45 2023-07-03 11:45:00.000000 bce-python-sdk-0.8.87/bce_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 aimingzhen   (502) staff       (20)        9 2023-07-03 11:45:00.000000 bce-python-sdk-0.8.87/bce_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 aimingzhen   (502) staff       (20)       38 2023-07-03 11:45:00.400227 bce-python-sdk-0.8.87/setup.cfg
+-rw-r--r--   0 aimingzhen   (502) staff       (20)     2833 2023-05-18 03:36:02.000000 bce-python-sdk-0.8.87/setup.py
```

### Comparing `bce-python-sdk-0.8.83/baidubce/__init__.py` & `bce-python-sdk-0.8.87/baidubce/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,11 +13,12 @@
 """
 This module defines some common string constants.
 """
 from builtins import str
 from builtins import bytes
 from . import protocol
 
-SDK_VERSION = b'0.8.83'
+
+SDK_VERSION = b'0.8.87'
 DEFAULT_SERVICE_DOMAIN = b'bcebos.com'
 URL_PREFIX = b'/v1'
 DEFAULT_ENCODING = 'UTF-8'
```

### Comparing `bce-python-sdk-0.8.83/baidubce/auth/bce_credentials.py` & `bce-python-sdk-0.8.87/baidubce/auth/bce_credentials.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/auth/bce_v1_signer.py` & `bce-python-sdk-0.8.87/baidubce/auth/bce_v1_signer.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/bce_base_client.py` & `bce-python-sdk-0.8.87/baidubce/bce_base_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/bce_client_configuration.py` & `bce-python-sdk-0.8.87/baidubce/bce_client_configuration.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/bce_response.py` & `bce-python-sdk-0.8.87/baidubce/bce_response.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/compat.py` & `bce-python-sdk-0.8.87/baidubce/compat.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/exception.py` & `bce-python-sdk-0.8.87/baidubce/exception.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/http/bce_http_client.py` & `bce-python-sdk-0.8.87/baidubce/http/bce_http_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/http/handler.py` & `bce-python-sdk-0.8.87/baidubce/http/handler.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/http/http_content_types.py` & `bce-python-sdk-0.8.87/baidubce/http/http_content_types.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/http/http_headers.py` & `bce-python-sdk-0.8.87/baidubce/http/http_headers.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,14 +98,16 @@
 
 BOS_RESTORE_TIER = b"x-bce-restore-tier"
 
 BOS_RESTORE_DAYS = b"x-bce-restore-days"
 
 BOS_SYMLINK_TARGET = b"x-bce-symlink-target"
 
+BOS_SYMLINK_BUCKET = b"x-bce-symlink-bucket"
+
 BOS_FORBID_OVERWRITE = b"x-bce-forbid-overwrite"
 
 BOS_TRAFFIC_LIMIT = b"x-bce-traffic-limit"
 
 # STS HTTP Headers
 
 STS_SECURITY_TOKEN = b"x-bce-security-token"
```

### Comparing `bce-python-sdk-0.8.83/baidubce/http/http_methods.py` & `bce-python-sdk-0.8.87/baidubce/http/http_methods.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/protocol.py` & `bce-python-sdk-0.8.87/baidubce/protocol.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/region.py` & `bce-python-sdk-0.8.87/baidubce/region.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/retry/retry_policy.py` & `bce-python-sdk-0.8.87/baidubce/retry/retry_policy.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/bbc/bbc_client.py` & `bce-python-sdk-0.8.87/baidubce/services/bbc/bbc_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/bbc/bbc_model.py` & `bce-python-sdk-0.8.87/baidubce/services/bbc/bbc_model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/bcc/fpga_card_type.py` & `bce-python-sdk-0.8.87/baidubce/services/bcc/fpga_card_type.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/bcc/gpu_card_type.py` & `bce-python-sdk-0.8.87/baidubce/services/bcc/gpu_card_type.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/bcm/bcm_client.py` & `bce-python-sdk-0.8.87/baidubce/services/bcm/bcm_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/bes/bes_client.py` & `bce-python-sdk-0.8.87/baidubce/services/bes/bes_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/bes/bes_model.py` & `bce-python-sdk-0.8.87/baidubce/services/bes/bes_model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/blb/app_blb_client.py` & `bce-python-sdk-0.8.87/baidubce/services/blb/app_blb_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/blb/blb_client.py` & `bce-python-sdk-0.8.87/baidubce/services/blb/blb_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/bmr/bmr_client.py` & `bce-python-sdk-0.8.87/baidubce/services/bmr/bmr_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/bos/__init__.py` & `bce-python-sdk-0.8.87/baidubce/services/bos/__init__.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/bos/bos_client.py` & `bce-python-sdk-0.8.87/baidubce/services/bos/bos_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1957,14 +1957,15 @@
             part_list.append({
                 "partNumber": part_number,
                 "eTag": response.metadata.etag
             })
             _logger.debug("upload task success with partNumber={}!".format(part_number))
         except Exception as e:
             _logger.debug("upload task failed with partNumber={}!".format(part_number))
+            raise e
             #_logger.debug(e)
 
     @required(bucket_name=(bytes, str), key=(bytes, str), file_name=(bytes, str))
     def put_super_obejct_from_file(self, bucket_name, key, file_name, chunk_size=5,
             thread_num=None,
             uploadTaskHandle=None,
             content_type=None,
@@ -2187,19 +2188,17 @@
                 http_methods.POST,
                 bucket_name,
                 key,
                 headers=headers,
                 params={b'fetch': b''},
                 config=config)
 
-    @required(bucket_name=(bytes, str), key=(bytes, str), symlink=(bytes, str), forbid_overwrite=(bool))
-    def put_object_symlink(self, bucket_name, key, symlink, forbid_overwrite=None, 
-            user_metadata=None,
-            storage_class=None,
-            config=None):
+    @required(bucket_name=(bytes, str), target_key=(bytes, str), symlink=(bytes, str), forbid_overwrite=(bool))
+    def put_object_symlink(self, bucket_name, target_key, symlink, forbid_overwrite=None, 
+            user_metadata=None, storage_class=None, target_bucket=None, config=None):
         """
         put object symlink
 
         :type bucket: string
         :param bucket: None
 
         :type key: string
@@ -2207,24 +2206,26 @@
 
         :type symlink: string
         :type symlink_key: symlink name
 
         :return:
             **HttpResponse Class**
         """
-        key = compat.convert_to_bytes(key)
+        target_key = compat.convert_to_bytes(target_key)
         symlink = compat.convert_to_bytes(symlink)
         headers = self._prepare_object_headers(user_metadata=user_metadata,
                 storage_class=storage_class)
-        headers[http_headers.BOS_SYMLINK_TARGET] = key
+        headers[http_headers.BOS_SYMLINK_TARGET] = target_key
         if forbid_overwrite is not None:
             if forbid_overwrite:
                 headers[http_headers.BOS_FORBID_OVERWRITE] = b'true'
             else:
                 headers[http_headers.BOS_FORBID_OVERWRITE] = b'false'
+        if target_bucket is not None:
+            headers[http_headers.BOS_SYMLINK_BUCKET] = compat.convert_to_bytes(target_bucket)
         return self._send_request(http_methods.PUT,
                            bucket_name,
                            symlink,
                            headers=headers,
                            params={b'symlink': b''},
                            config=config)
 
@@ -2267,16 +2268,18 @@
         :param config:
         :return:
         """
         key = compat.convert_to_bytes(key)
         headers = headers or {}
         if "inputSerialization" in select_object_args and "json" in select_object_args["inputSerialization"]:
             select_type = b"json"
-        else:
+        elif "inputSerialization" in select_object_args and "csv" in select_object_args["inputSerialization"]:
             select_type = b"csv"
+        else:
+            select_type = b"parquet"
         select_response = SelectResponse()
         self._send_request(
             http_methods.POST,
             bucket_name,
             key,
             body=json.dumps({'selectRequest': select_object_args}, default=BosClient._dump_acl_object),
             headers=headers,
@@ -2291,16 +2294,17 @@
         """
         get user quota
 
         :param config:
         :return:
         """
         return self._send_request(
-            http_methods.GET, params={b'userQuota': b''})
+            http_methods.GET, params={b'userQuota': b''}, config=config,)
     
+    @required(max_bucket_count=(int), max_capacity_mega_bytes=(int))
     def put_user_quota(self, max_bucket_count, max_capacity_mega_bytes, config=None):
         """
         put user quota
 
         :type max_bucket_count: int
         :param max_bucket_count: max bucket count
 
@@ -2310,39 +2314,44 @@
         :param config:
         :return:
         """
         return self._send_request(
             http_methods.PUT,
             body=json.dumps({'maxBucketCount': max_bucket_count, 
                             'maxCapacityMegaBytes': max_capacity_mega_bytes}),
-            params={b'userQuota': b''})
+            params={b'userQuota': b''}, config=config)
 
     def delete_user_quota(self, config=None):
         """
         delete user quota
 
         :param config:
         :return:
         """
         return self._send_request(
-            http_methods.DELETE, params={b'userQuota': b''})        
-        
+            http_methods.DELETE, params={b'userQuota': b''}, config=config)
+
+
+    @required(bucket_name=(bytes, str))
     def get_notification(self, bucket_name, config=None):
         """
         get notification
 
         :type bucket_name: string
         :param bucket_name: bucket name
 
         :param config:
         :return:
         """
         return self._send_request(
-            http_methods.GET, bucket_name=bucket_name, params={b'notification': b''})
+            http_methods.GET, bucket_name=bucket_name, 
+            params={b'notification': b''}, config=config,)
     
+
+    @required(bucket_name=(bytes, str), notifications=(list, ))
     def put_notification(self, bucket_name, notifications, config=None):
         """
         put user quota
 
         :type bucket_name: string
         :param bucket_name: bucket
 
@@ -2351,28 +2360,81 @@
 
         :param config:
         :return:
         """
         return self._send_request(
             http_methods.PUT, bucket_name=bucket_name,
             body=json.dumps({'notifications': notifications}),
-            params={b'notification': b''})
-
+            params={b'notification': b''}, config=config,)
+    @required(bucket_name=(bytes, str))
     def delete_notification(self, bucket_name, config=None):
         """
         delete notification
 
         :type bucket_name: string
         :param bucket_name: bucket name
 
         :param config:
         :return:
         """
         return self._send_request(
-            http_methods.DELETE, bucket_name=bucket_name, params={b'notification': b''})        
+            http_methods.DELETE, bucket_name=bucket_name, params={b'notification': b''},
+            config=config,)
+
+    @required(bucket_name=(bytes, str), mirror_args=(list, ))
+    def put_bucket_mirroring(self, bucket_name, mirror_args, config=None):
+        """
+        put bucket mirroring
+
+        :type bucket_name: string
+        :param bucket_name: bucket name
+
+        :param mirror_args: mirror conf
+        :return:
+        """
+        return self._send_request(
+            http_methods.PUT,
+            bucket_name=bucket_name,
+            body=json.dumps({'bucketMirroringConfiguration': mirror_args}, default=BosClient._dump_acl_object),
+            params={b'mirroring': b''},
+            config=config,
+            )
+
+    @required(bucket_name=(bytes, str))
+    def get_bucket_mirroring(self, bucket_name, config=None):
+        """
+        get bucket mirroring
+
+        :type bucket_name: string
+        :param bucket_name: bucket name
+
+        :return:
+        """
+        return self._send_request(
+            http_methods.GET,
+            bucket_name=bucket_name,
+            params={b'mirroring': b''},
+            config=config,
+            )
+    @required(bucket_name=(bytes, str))
+    def delete_bucket_mirroring(self, bucket_name, config=None):
+        """
+        delete bucket mirroring
+
+        :type bucket_name: string
+        :param bucket_name: bucket name
+
+        :return:
+        """
+        return self._send_request(
+            http_methods.DELETE,
+            bucket_name=bucket_name,
+            params={b'mirroring': b''},
+            config=config,
+            )
         
 
     @staticmethod
     def _prepare_object_headers(
             content_length=None,
             content_md5=None,
             content_type=None,
```

### Comparing `bce-python-sdk-0.8.83/baidubce/services/bos/bos_handler.py` & `bce-python-sdk-0.8.87/baidubce/services/bos/bos_handler.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/bos/canned_acl.py` & `bce-python-sdk-0.8.87/baidubce/services/bos/canned_acl.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/bos/storage_class.py` & `bce-python-sdk-0.8.87/baidubce/services/bos/storage_class.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/bts/__init__.py` & `bce-python-sdk-0.8.87/baidubce/services/bts/__init__.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/bts/bts_client.py` & `bce-python-sdk-0.8.87/baidubce/services/bts/bts_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/bts/model.py` & `bce-python-sdk-0.8.87/baidubce/services/bts/model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/bts/util.py` & `bce-python-sdk-0.8.87/baidubce/services/bts/util.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/cdn/cdn_client.py` & `bce-python-sdk-0.8.87/baidubce/services/cdn/cdn_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/cdn/cdn_stats_param.py` & `bce-python-sdk-0.8.87/baidubce/services/cdn/cdn_stats_param.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/cert/cert_client.py` & `bce-python-sdk-0.8.87/baidubce/services/cert/cert_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/cert/cert_model.py` & `bce-python-sdk-0.8.87/baidubce/services/cert/cert_model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/cfc/cfc_client.py` & `bce-python-sdk-0.8.87/baidubce/services/cfc/cfc_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/cfc/cfc_handler.py` & `bce-python-sdk-0.8.87/baidubce/services/cfc/cfc_handler.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/cfc/models.py` & `bce-python-sdk-0.8.87/baidubce/services/cfc/models.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/ddc/ddc_client.py` & `bce-python-sdk-0.8.87/baidubce/services/ddc/ddc_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/dns/api/dns_api.py` & `bce-python-sdk-0.8.87/baidubce/services/dns/api/dns_api.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/dns/dns_client.py` & `bce-python-sdk-0.8.87/baidubce/services/dns/dns_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/dumap/dumap_client.py` & `bce-python-sdk-0.8.87/baidubce/services/dumap/dumap_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/eip/eip_bp_client.py` & `bce-python-sdk-0.8.87/baidubce/services/eip/eip_bp_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/eip/eip_client.py` & `bce-python-sdk-0.8.87/baidubce/services/eip/eip_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/eip/eip_group_client.py` & `bce-python-sdk-0.8.87/baidubce/services/eip/eip_group_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/eip/eip_group_model.py` & `bce-python-sdk-0.8.87/baidubce/services/eip/eip_group_model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/eip/eip_tp_client.py` & `bce-python-sdk-0.8.87/baidubce/services/eip/eip_tp_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/eip/model.py` & `bce-python-sdk-0.8.87/baidubce/services/eip/model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/endpoint/endpoint_client.py` & `bce-python-sdk-0.8.87/baidubce/services/endpoint/endpoint_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/endpoint/model.py` & `bce-python-sdk-0.8.87/baidubce/services/endpoint/model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/iam/__init__.py` & `bce-python-sdk-0.8.87/baidubce/services/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/iam/iam_client.py` & `bce-python-sdk-0.8.87/baidubce/services/iam/iam_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/infinite/__init__.py` & `bce-python-sdk-0.8.87/baidubce/services/infinite/__init__.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/infinite/infinite_client.py` & `bce-python-sdk-0.8.87/baidubce/services/infinite/infinite_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/kms/keyspec_class.py` & `bce-python-sdk-0.8.87/baidubce/services/kms/keyspec_class.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/kms/kms_client.py` & `bce-python-sdk-0.8.87/baidubce/services/kms/kms_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/kms/origin_class.py` & `bce-python-sdk-0.8.87/baidubce/services/kms/origin_class.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/kms/protectedby_class.py` & `bce-python-sdk-0.8.87/baidubce/services/kms/protectedby_class.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/kms/publickeyencoding_class.py` & `bce-python-sdk-0.8.87/baidubce/services/kms/publickeyencoding_class.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/media/media_client.py` & `bce-python-sdk-0.8.87/baidubce/services/media/media_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/media/media_handler.py` & `bce-python-sdk-0.8.87/baidubce/services/media/media_handler.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/mms/__init__.py` & `bce-python-sdk-0.8.87/baidubce/services/mms/__init__.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/mms/mms_client.py` & `bce-python-sdk-0.8.87/baidubce/services/mms/mms_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/mvs/__init__.py` & `bce-python-sdk-0.8.87/baidubce/services/mvs/__init__.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/mvs/mvs_client.py` & `bce-python-sdk-0.8.87/baidubce/services/mvs/mvs_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/route/route_client.py` & `bce-python-sdk-0.8.87/baidubce/services/route/route_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/scs/__init__.py` & `bce-python-sdk-0.8.87/baidubce/services/rds/__init__.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/scs/model.py` & `bce-python-sdk-0.8.87/baidubce/services/scs/model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/scs/scs_client.py` & `bce-python-sdk-0.8.87/baidubce/services/scs/scs_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/sms/__init__.py` & `bce-python-sdk-0.8.87/baidubce/services/sms/__init__.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/sms/model.py` & `bce-python-sdk-0.8.87/baidubce/services/sms/model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/sms/sms_client.py` & `bce-python-sdk-0.8.87/baidubce/services/sms/sms_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/sts/__init__.py` & `bce-python-sdk-0.8.87/baidubce/services/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/sts/sts_client.py` & `bce-python-sdk-0.8.87/baidubce/services/sts/sts_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/subnet/subnet_client.py` & `bce-python-sdk-0.8.87/baidubce/services/subnet/subnet_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/tsdb/tsdb_admin_client.py` & `bce-python-sdk-0.8.87/baidubce/services/tsdb/tsdb_admin_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/tsdb/tsdb_client.py` & `bce-python-sdk-0.8.87/baidubce/services/tsdb/tsdb_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/tsdb/tsdb_handler.py` & `bce-python-sdk-0.8.87/baidubce/services/tsdb/tsdb_handler.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/vca/vca_client.py` & `bce-python-sdk-0.8.87/baidubce/services/vca/vca_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/vcr/vcr_client.py` & `bce-python-sdk-0.8.87/baidubce/services/vcr/vcr_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/vpc/acl_client.py` & `bce-python-sdk-0.8.87/baidubce/services/vpc/acl_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/vpc/nat_client.py` & `bce-python-sdk-0.8.87/baidubce/services/vpc/nat_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/vpc/nat_model.py` & `bce-python-sdk-0.8.87/baidubce/services/vpc/nat_model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/vpc/peerconn_client.py` & `bce-python-sdk-0.8.87/baidubce/services/vpc/peerconn_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/vpc/peerconn_model.py` & `bce-python-sdk-0.8.87/baidubce/services/vpc/peerconn_model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/vpc/vpc_client.py` & `bce-python-sdk-0.8.87/baidubce/services/vpc/vpc_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/vpn/vpn_client.py` & `bce-python-sdk-0.8.87/baidubce/services/vpn/vpn_client.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/services/vpn/vpn_model.py` & `bce-python-sdk-0.8.87/baidubce/services/vpn/vpn_model.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/baidubce/utils.py` & `bce-python-sdk-0.8.87/baidubce/utils.py`

 * *Files identical despite different names*

### Comparing `bce-python-sdk-0.8.83/bce_python_sdk.egg-info/SOURCES.txt` & `bce-python-sdk-0.8.87/bce_python_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,17 @@
 baidubce/services/media/__init__.py
 baidubce/services/media/media_client.py
 baidubce/services/media/media_handler.py
 baidubce/services/mms/__init__.py
 baidubce/services/mms/mms_client.py
 baidubce/services/mvs/__init__.py
 baidubce/services/mvs/mvs_client.py
+baidubce/services/rds/__init__.py
+baidubce/services/rds/model.py
+baidubce/services/rds/rds_client.py
 baidubce/services/route/__init__.py
 baidubce/services/route/route_client.py
 baidubce/services/route/route_model.py
 baidubce/services/scs/__init__.py
 baidubce/services/scs/model.py
 baidubce/services/scs/scs_client.py
 baidubce/services/sms/__init__.py
```

### Comparing `bce-python-sdk-0.8.83/setup.py` & `bce-python-sdk-0.8.87/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,16 @@
               'baidubce.services.bcm',
               'baidubce.services.kms',
               'baidubce.services.cert',
               'baidubce.services.bes',
               'baidubce.services.scs',
               'baidubce.services.ddc',
               'baidubce.services.dns',
-              'baidubce.services.dns.api'
+              'baidubce.services.dns.api',
+              'baidubce.services.rds'
               ],
     url='http://bce.baidu.com',
     license='Apache License 2.0',
     author='',
     author_email='',
     description='BCE SDK for python'
 )
```

