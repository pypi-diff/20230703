# Comparing `tmp/bacpypes3-0.0.77.tar.gz` & `tmp/bacpypes3-0.0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacpypes3-0.0.77.tar", last modified: Sat Jul  1 17:58:49 2023, max compression
+gzip compressed data, was "bacpypes3-0.0.78.tar", last modified: Mon Jul  3 03:40:21 2023, max compression
```

## Comparing `bacpypes3-0.0.77.tar` & `bacpypes3-0.0.78.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.507772 bacpypes3-0.0.77/
--rw-rw-r--   0 joel      (1000) joel      (1000)      666 2023-07-01 17:58:49.507772 bacpypes3-0.0.77/PKG-INFO
--rw-rw-r--   0 joel      (1000) joel      (1000)      346 2023-03-09 18:20:30.000000 bacpypes3-0.0.77/README.md
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.491772 bacpypes3-0.0.77/bacpypes3/
--rw-rw-r--   0 joel      (1000) joel      (1000)     1370 2023-07-01 17:57:36.000000 bacpypes3-0.0.77/bacpypes3/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    23928 2023-07-01 17:57:36.000000 bacpypes3-0.0.77/bacpypes3/__main__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    56648 2023-01-24 05:27:28.000000 bacpypes3-0.0.77/bacpypes3/apdu.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    34041 2023-07-01 17:57:36.000000 bacpypes3-0.0.77/bacpypes3/app.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    65777 2023-04-04 12:53:18.000000 bacpypes3-0.0.77/bacpypes3/appservice.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    20848 2023-05-31 11:51:39.000000 bacpypes3-0.0.77/bacpypes3/argparse.py
--rw-rw-r--   0 joel      (1000) joel      (1000)   112385 2023-06-23 03:49:41.000000 bacpypes3-0.0.77/bacpypes3/basetypes.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    16150 2023-04-03 15:32:38.000000 bacpypes3-0.0.77/bacpypes3/cmd.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     7934 2022-11-21 19:40:26.000000 bacpypes3-0.0.77/bacpypes3/comm.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     7128 2023-01-24 05:27:28.000000 bacpypes3-0.0.77/bacpypes3/console.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    64295 2023-04-07 19:15:02.000000 bacpypes3-0.0.77/bacpypes3/constructeddata.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    10659 2023-06-29 13:02:40.000000 bacpypes3-0.0.77/bacpypes3/debugging.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     9685 2023-02-08 13:29:16.000000 bacpypes3-0.0.77/bacpypes3/errors.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.495772 bacpypes3-0.0.77/bacpypes3/ipv4/
--rw-rw-r--   0 joel      (1000) joel      (1000)     9245 2023-06-26 19:19:16.000000 bacpypes3-0.0.77/bacpypes3/ipv4/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8238 2023-04-22 03:23:44.000000 bacpypes3-0.0.77/bacpypes3/ipv4/app.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    25882 2023-04-21 19:42:07.000000 bacpypes3-0.0.77/bacpypes3/ipv4/bvll.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4119 2023-02-12 01:55:32.000000 bacpypes3-0.0.77/bacpypes3/ipv4/link.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    61699 2023-04-21 19:25:10.000000 bacpypes3-0.0.77/bacpypes3/ipv4/service.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.495772 bacpypes3-0.0.77/bacpypes3/ipv6/
--rw-rw-r--   0 joel      (1000) joel      (1000)     6298 2023-01-09 14:29:42.000000 bacpypes3-0.0.77/bacpypes3/ipv6/__init__.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    32041 2023-01-24 14:48:16.000000 bacpypes3-0.0.77/bacpypes3/ipv6/bvll.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    57488 2023-02-01 12:39:44.000000 bacpypes3-0.0.77/bacpypes3/ipv6/service.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.495772 bacpypes3-0.0.77/bacpypes3/json/
--rw-rw-r--   0 joel      (1000) joel      (1000)      102 2023-01-24 13:54:53.000000 bacpypes3-0.0.77/bacpypes3/json/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      132 2022-09-06 15:15:46.000000 bacpypes3-0.0.77/bacpypes3/json/__main__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    16743 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/bacpypes3/json/util.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.495772 bacpypes3-0.0.77/bacpypes3/lib/
--rw-rw-r--   0 joel      (1000) joel      (1000)       41 2023-01-24 05:27:28.000000 bacpypes3-0.0.77/bacpypes3/lib/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    10085 2021-08-04 12:18:07.000000 bacpypes3-0.0.77/bacpypes3/lib/batchread.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.499772 bacpypes3-0.0.77/bacpypes3/local/
--rw-rw-r--   0 joel      (1000) joel      (1000)      463 2023-06-20 12:14:17.000000 bacpypes3-0.0.77/bacpypes3/local/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     5804 2023-06-21 18:50:45.000000 bacpypes3-0.0.77/bacpypes3/local/analog.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4447 2023-06-21 18:50:45.000000 bacpypes3-0.0.77/bacpypes3/local/binary.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     6059 2023-06-20 12:14:17.000000 bacpypes3-0.0.77/bacpypes3/local/cmd.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    18826 2023-06-20 12:14:17.000000 bacpypes3-0.0.77/bacpypes3/local/cov.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     5769 2023-01-24 13:31:42.000000 bacpypes3-0.0.77/bacpypes3/local/device.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    87515 2023-06-26 19:19:16.000000 bacpypes3-0.0.77/bacpypes3/local/event.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    14523 2023-06-21 18:50:45.000000 bacpypes3-0.0.77/bacpypes3/local/fault.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     5022 2023-07-01 17:57:36.000000 bacpypes3-0.0.77/bacpypes3/local/networkport.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    23309 2023-06-21 18:50:45.000000 bacpypes3-0.0.77/bacpypes3/local/object.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     1046 2023-01-03 14:48:04.000000 bacpypes3-0.0.77/bacpypes3/local/oos.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    24830 2023-02-06 04:19:11.000000 bacpypes3-0.0.77/bacpypes3/local/schedule.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    77433 2023-07-01 17:57:36.000000 bacpypes3-0.0.77/bacpypes3/netservice.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    28240 2023-01-24 05:27:28.000000 bacpypes3-0.0.77/bacpypes3/npdu.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    94171 2023-06-20 12:14:17.000000 bacpypes3-0.0.77/bacpypes3/object.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    65850 2023-06-26 19:19:16.000000 bacpypes3-0.0.77/bacpypes3/pdu.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    80966 2023-02-17 06:25:03.000000 bacpypes3-0.0.77/bacpypes3/primitivedata.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.499772 bacpypes3-0.0.77/bacpypes3/rdf/
--rw-rw-r--   0 joel      (1000) joel      (1000)      353 2023-01-24 13:54:37.000000 bacpypes3-0.0.77/bacpypes3/rdf/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      130 2022-08-22 23:43:00.000000 bacpypes3-0.0.77/bacpypes3/rdf/__main__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    10595 2023-05-04 14:15:16.000000 bacpypes3-0.0.77/bacpypes3/rdf/core.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    19634 2023-01-27 13:19:10.000000 bacpypes3-0.0.77/bacpypes3/rdf/util.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.499772 bacpypes3-0.0.77/bacpypes3/sc/
--rw-rw-r--   0 joel      (1000) joel      (1000)       65 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/bacpypes3/sc/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    33859 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/bacpypes3/sc/bvll.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    18081 2023-02-27 03:52:18.000000 bacpypes3-0.0.77/bacpypes3/sc/service.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.499772 bacpypes3-0.0.77/bacpypes3/service/
--rw-rw-r--   0 joel      (1000) joel      (1000)       78 2023-01-24 13:55:00.000000 bacpypes3-0.0.77/bacpypes3/service/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    22512 2023-04-03 19:06:43.000000 bacpypes3-0.0.77/bacpypes3/service/cov.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    22741 2023-04-04 12:42:09.000000 bacpypes3-0.0.77/bacpypes3/service/device.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    31277 2023-04-03 19:49:50.000000 bacpypes3-0.0.77/bacpypes3/service/object.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3869 2023-05-31 11:51:39.000000 bacpypes3-0.0.77/bacpypes3/settings.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.499772 bacpypes3-0.0.77/bacpypes3/vlan/
--rw-rw-r--   0 joel      (1000) joel      (1000)    11838 2023-07-01 17:57:36.000000 bacpypes3-0.0.77/bacpypes3/vlan/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     1692 2023-07-01 17:57:36.000000 bacpypes3-0.0.77/bacpypes3/vlan/link.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.495772 bacpypes3-0.0.77/bacpypes3.egg-info/
--rw-rw-r--   0 joel      (1000) joel      (1000)      666 2023-07-01 17:58:49.000000 bacpypes3-0.0.77/bacpypes3.egg-info/PKG-INFO
--rw-rw-r--   0 joel      (1000) joel      (1000)     3049 2023-07-01 17:58:49.000000 bacpypes3-0.0.77/bacpypes3.egg-info/SOURCES.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)        1 2023-07-01 17:58:49.000000 bacpypes3-0.0.77/bacpypes3.egg-info/dependency_links.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)        1 2021-06-28 12:41:48.000000 bacpypes3-0.0.77/bacpypes3.egg-info/not-zip-safe
--rw-rw-r--   0 joel      (1000) joel      (1000)       16 2023-07-01 17:58:49.000000 bacpypes3-0.0.77/bacpypes3.egg-info/top_level.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)      100 2022-08-22 00:12:37.000000 bacpypes3-0.0.77/pyproject.toml
--rw-rw-r--   0 joel      (1000) joel      (1000)       38 2023-07-01 17:58:49.507772 bacpypes3-0.0.77/setup.cfg
--rw-rw-r--   0 joel      (1000) joel      (1000)     1219 2023-05-04 14:51:12.000000 bacpypes3-0.0.77/setup.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.503772 bacpypes3-0.0.77/tests/
--rw-rw-r--   0 joel      (1000) joel      (1000)      351 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2298 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/clocked_test.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      372 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/conftest.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    49924 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/state_machine.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      644 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_1.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3054 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test__template.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.503772 bacpypes3-0.0.77/tests/test_constructed_data/
--rw-rw-r--   0 joel      (1000) joel      (1000)      247 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_constructed_data/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2616 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_constructed_data/test_any.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2526 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_constructed_data/test_array.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2894 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_constructed_data/test_choice.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2071 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_constructed_data/test_list.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4013 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_constructed_data/test_read_property_multiple.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    10217 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_constructed_data/test_sequence.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8422 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_constructed_data/test_sequence_of.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.503772 bacpypes3-0.0.77/tests/test_pdu/
--rw-rw-r--   0 joel      (1000) joel      (1000)      126 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_pdu/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    16509 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_pdu/test_address.py
--rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_pdu/test_pci.py
--rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_pdu/test_pdu.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.507772 bacpypes3-0.0.77/tests/test_primitive_data/
--rw-rw-r--   0 joel      (1000) joel      (1000)      456 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_primitive_data/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3309 2023-01-09 14:29:42.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_bit_string.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2629 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_boolean.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3204 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_character_string.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2671 2023-02-17 06:25:03.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_date.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2794 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_double.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3266 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_enumerated.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2632 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_integer.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2363 2022-10-03 15:42:31.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_null.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3739 2021-07-22 21:59:33.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_object_identifier.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2775 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_octet_string.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2785 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_real.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4262 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_tag.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2546 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_time.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3588 2021-06-28 12:37:49.000000 bacpypes3-0.0.77/tests/test_primitive_data/test_unsigned.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.507772 bacpypes3-0.0.77/tests/test_utilities/
--rw-rw-r--   0 joel      (1000) joel      (1000)      130 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_utilities/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    18594 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_utilities/test_state_machine.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-01 17:58:49.507772 bacpypes3-0.0.77/tests/test_vlan/
--rw-rw-r--   0 joel      (1000) joel      (1000)      200 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_vlan/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8287 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_vlan/test_ipv4_network.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     6304 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_vlan/test_ipv4_router.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8904 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/test_vlan/test_network.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    12098 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/trapped_classes.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     1397 2023-01-26 13:59:48.000000 bacpypes3-0.0.77/tests/utilities.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-03 03:40:21.695955 bacpypes3-0.0.78/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      666 2023-07-03 03:40:21.695955 bacpypes3-0.0.78/PKG-INFO
+-rw-rw-r--   0 joel      (1000) joel      (1000)      346 2023-03-09 18:20:30.000000 bacpypes3-0.0.78/README.md
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-03 03:40:21.683954 bacpypes3-0.0.78/bacpypes3/
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1370 2023-07-03 03:39:30.000000 bacpypes3-0.0.78/bacpypes3/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    23928 2023-07-01 17:57:36.000000 bacpypes3-0.0.78/bacpypes3/__main__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    56648 2023-01-24 05:27:28.000000 bacpypes3-0.0.78/bacpypes3/apdu.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    34041 2023-07-01 17:57:36.000000 bacpypes3-0.0.78/bacpypes3/app.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    65777 2023-04-04 12:53:18.000000 bacpypes3-0.0.78/bacpypes3/appservice.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    20848 2023-05-31 11:51:39.000000 bacpypes3-0.0.78/bacpypes3/argparse.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)   112385 2023-06-23 03:49:41.000000 bacpypes3-0.0.78/bacpypes3/basetypes.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    16150 2023-04-03 15:32:38.000000 bacpypes3-0.0.78/bacpypes3/cmd.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     7934 2022-11-21 19:40:26.000000 bacpypes3-0.0.78/bacpypes3/comm.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     7128 2023-01-24 05:27:28.000000 bacpypes3-0.0.78/bacpypes3/console.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    64295 2023-04-07 19:15:02.000000 bacpypes3-0.0.78/bacpypes3/constructeddata.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    10659 2023-06-29 13:02:40.000000 bacpypes3-0.0.78/bacpypes3/debugging.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     9685 2023-02-08 13:29:16.000000 bacpypes3-0.0.78/bacpypes3/errors.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-03 03:40:21.683954 bacpypes3-0.0.78/bacpypes3/ipv4/
+-rw-rw-r--   0 joel      (1000) joel      (1000)     9245 2023-06-26 19:19:16.000000 bacpypes3-0.0.78/bacpypes3/ipv4/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8238 2023-04-22 03:23:44.000000 bacpypes3-0.0.78/bacpypes3/ipv4/app.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    25882 2023-04-21 19:42:07.000000 bacpypes3-0.0.78/bacpypes3/ipv4/bvll.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4119 2023-02-12 01:55:32.000000 bacpypes3-0.0.78/bacpypes3/ipv4/link.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    61699 2023-04-21 19:25:10.000000 bacpypes3-0.0.78/bacpypes3/ipv4/service.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-03 03:40:21.683954 bacpypes3-0.0.78/bacpypes3/ipv6/
+-rw-rw-r--   0 joel      (1000) joel      (1000)     6298 2023-01-09 14:29:42.000000 bacpypes3-0.0.78/bacpypes3/ipv6/__init__.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    32041 2023-01-24 14:48:16.000000 bacpypes3-0.0.78/bacpypes3/ipv6/bvll.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    57488 2023-02-01 12:39:44.000000 bacpypes3-0.0.78/bacpypes3/ipv6/service.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-03 03:40:21.683954 bacpypes3-0.0.78/bacpypes3/json/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      102 2023-01-24 13:54:53.000000 bacpypes3-0.0.78/bacpypes3/json/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      132 2022-09-06 15:15:46.000000 bacpypes3-0.0.78/bacpypes3/json/__main__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    16743 2023-01-26 13:59:48.000000 bacpypes3-0.0.78/bacpypes3/json/util.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-03 03:40:21.683954 bacpypes3-0.0.78/bacpypes3/lib/
+-rw-rw-r--   0 joel      (1000) joel      (1000)       41 2023-01-24 05:27:28.000000 bacpypes3-0.0.78/bacpypes3/lib/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    10085 2021-08-04 12:18:07.000000 bacpypes3-0.0.78/bacpypes3/lib/batchread.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-03 03:40:21.687955 bacpypes3-0.0.78/bacpypes3/local/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      463 2023-06-20 12:14:17.000000 bacpypes3-0.0.78/bacpypes3/local/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     5804 2023-06-21 18:50:45.000000 bacpypes3-0.0.78/bacpypes3/local/analog.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4447 2023-06-21 18:50:45.000000 bacpypes3-0.0.78/bacpypes3/local/binary.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     6059 2023-06-20 12:14:17.000000 bacpypes3-0.0.78/bacpypes3/local/cmd.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    18826 2023-06-20 12:14:17.000000 bacpypes3-0.0.78/bacpypes3/local/cov.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     5769 2023-01-24 13:31:42.000000 bacpypes3-0.0.78/bacpypes3/local/device.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    87515 2023-06-26 19:19:16.000000 bacpypes3-0.0.78/bacpypes3/local/event.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    14523 2023-06-21 18:50:45.000000 bacpypes3-0.0.78/bacpypes3/local/fault.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     5022 2023-07-01 17:57:36.000000 bacpypes3-0.0.78/bacpypes3/local/networkport.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    23309 2023-06-21 18:50:45.000000 bacpypes3-0.0.78/bacpypes3/local/object.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1046 2023-01-03 14:48:04.000000 bacpypes3-0.0.78/bacpypes3/local/oos.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    24830 2023-02-06 04:19:11.000000 bacpypes3-0.0.78/bacpypes3/local/schedule.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    77562 2023-07-03 03:39:30.000000 bacpypes3-0.0.78/bacpypes3/netservice.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    28240 2023-01-24 05:27:28.000000 bacpypes3-0.0.78/bacpypes3/npdu.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    94171 2023-06-20 12:14:17.000000 bacpypes3-0.0.78/bacpypes3/object.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    65850 2023-06-26 19:19:16.000000 bacpypes3-0.0.78/bacpypes3/pdu.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    80966 2023-02-17 06:25:03.000000 bacpypes3-0.0.78/bacpypes3/primitivedata.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-03 03:40:21.687955 bacpypes3-0.0.78/bacpypes3/rdf/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      353 2023-01-24 13:54:37.000000 bacpypes3-0.0.78/bacpypes3/rdf/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      130 2022-08-22 23:43:00.000000 bacpypes3-0.0.78/bacpypes3/rdf/__main__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    10595 2023-05-04 14:15:16.000000 bacpypes3-0.0.78/bacpypes3/rdf/core.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    19634 2023-01-27 13:19:10.000000 bacpypes3-0.0.78/bacpypes3/rdf/util.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-03 03:40:21.687955 bacpypes3-0.0.78/bacpypes3/sc/
+-rw-rw-r--   0 joel      (1000) joel      (1000)       65 2021-06-28 12:37:49.000000 bacpypes3-0.0.78/bacpypes3/sc/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    33859 2021-06-28 12:37:49.000000 bacpypes3-0.0.78/bacpypes3/sc/bvll.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    18081 2023-02-27 03:52:18.000000 bacpypes3-0.0.78/bacpypes3/sc/service.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-03 03:40:21.687955 bacpypes3-0.0.78/bacpypes3/service/
+-rw-rw-r--   0 joel      (1000) joel      (1000)       78 2023-01-24 13:55:00.000000 bacpypes3-0.0.78/bacpypes3/service/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    22512 2023-04-03 19:06:43.000000 bacpypes3-0.0.78/bacpypes3/service/cov.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    22741 2023-04-04 12:42:09.000000 bacpypes3-0.0.78/bacpypes3/service/device.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    31277 2023-04-03 19:49:50.000000 bacpypes3-0.0.78/bacpypes3/service/object.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3869 2023-05-31 11:51:39.000000 bacpypes3-0.0.78/bacpypes3/settings.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-03 03:40:21.691954 bacpypes3-0.0.78/bacpypes3/vlan/
+-rw-rw-r--   0 joel      (1000) joel      (1000)    11838 2023-07-01 17:57:36.000000 bacpypes3-0.0.78/bacpypes3/vlan/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1692 2023-07-01 17:57:36.000000 bacpypes3-0.0.78/bacpypes3/vlan/link.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-03 03:40:21.683954 bacpypes3-0.0.78/bacpypes3.egg-info/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      666 2023-07-03 03:40:21.000000 bacpypes3-0.0.78/bacpypes3.egg-info/PKG-INFO
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3049 2023-07-03 03:40:21.000000 bacpypes3-0.0.78/bacpypes3.egg-info/SOURCES.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)        1 2023-07-03 03:40:21.000000 bacpypes3-0.0.78/bacpypes3.egg-info/dependency_links.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)        1 2021-06-28 12:41:48.000000 bacpypes3-0.0.78/bacpypes3.egg-info/not-zip-safe
+-rw-rw-r--   0 joel      (1000) joel      (1000)       16 2023-07-03 03:40:21.000000 bacpypes3-0.0.78/bacpypes3.egg-info/top_level.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)      100 2022-08-22 00:12:37.000000 bacpypes3-0.0.78/pyproject.toml
+-rw-rw-r--   0 joel      (1000) joel      (1000)       38 2023-07-03 03:40:21.695955 bacpypes3-0.0.78/setup.cfg
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1219 2023-05-04 14:51:12.000000 bacpypes3-0.0.78/setup.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-03 03:40:21.691954 bacpypes3-0.0.78/tests/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      351 2021-06-28 12:37:49.000000 bacpypes3-0.0.78/tests/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2298 2023-01-26 13:59:48.000000 bacpypes3-0.0.78/tests/clocked_test.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      372 2023-01-26 13:59:48.000000 bacpypes3-0.0.78/tests/conftest.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    49924 2023-01-26 13:59:48.000000 bacpypes3-0.0.78/tests/state_machine.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      644 2021-06-28 12:37:49.000000 bacpypes3-0.0.78/tests/test_1.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3054 2023-01-26 13:59:48.000000 bacpypes3-0.0.78/tests/test__template.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-03 03:40:21.691954 bacpypes3-0.0.78/tests/test_constructed_data/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      247 2023-01-26 13:59:48.000000 bacpypes3-0.0.78/tests/test_constructed_data/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2616 2023-01-26 13:59:48.000000 bacpypes3-0.0.78/tests/test_constructed_data/test_any.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2526 2023-01-26 13:59:48.000000 bacpypes3-0.0.78/tests/test_constructed_data/test_array.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2894 2023-01-26 13:59:48.000000 bacpypes3-0.0.78/tests/test_constructed_data/test_choice.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2071 2023-01-26 13:59:48.000000 bacpypes3-0.0.78/tests/test_constructed_data/test_list.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4013 2023-01-26 13:59:48.000000 bacpypes3-0.0.78/tests/test_constructed_data/test_read_property_multiple.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    10217 2023-01-26 13:59:48.000000 bacpypes3-0.0.78/tests/test_constructed_data/test_sequence.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8422 2023-01-26 13:59:48.000000 bacpypes3-0.0.78/tests/test_constructed_data/test_sequence_of.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-03 03:40:21.691954 bacpypes3-0.0.78/tests/test_pdu/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      126 2021-06-28 12:37:49.000000 bacpypes3-0.0.78/tests/test_pdu/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    16509 2023-01-26 13:59:48.000000 bacpypes3-0.0.78/tests/test_pdu/test_address.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.78/tests/test_pdu/test_pci.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.78/tests/test_pdu/test_pdu.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-03 03:40:21.695955 bacpypes3-0.0.78/tests/test_primitive_data/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      456 2021-06-28 12:37:49.000000 bacpypes3-0.0.78/tests/test_primitive_data/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3309 2023-01-09 14:29:42.000000 bacpypes3-0.0.78/tests/test_primitive_data/test_bit_string.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2629 2021-06-28 12:37:49.000000 bacpypes3-0.0.78/tests/test_primitive_data/test_boolean.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3204 2021-06-28 12:37:49.000000 bacpypes3-0.0.78/tests/test_primitive_data/test_character_string.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2671 2023-02-17 06:25:03.000000 bacpypes3-0.0.78/tests/test_primitive_data/test_date.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2794 2021-06-28 12:37:49.000000 bacpypes3-0.0.78/tests/test_primitive_data/test_double.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3266 2021-06-28 12:37:49.000000 bacpypes3-0.0.78/tests/test_primitive_data/test_enumerated.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2632 2021-06-28 12:37:49.000000 bacpypes3-0.0.78/tests/test_primitive_data/test_integer.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2363 2022-10-03 15:42:31.000000 bacpypes3-0.0.78/tests/test_primitive_data/test_null.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3739 2021-07-22 21:59:33.000000 bacpypes3-0.0.78/tests/test_primitive_data/test_object_identifier.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2775 2021-06-28 12:37:49.000000 bacpypes3-0.0.78/tests/test_primitive_data/test_octet_string.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2785 2021-06-28 12:37:49.000000 bacpypes3-0.0.78/tests/test_primitive_data/test_real.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4262 2021-06-28 12:37:49.000000 bacpypes3-0.0.78/tests/test_primitive_data/test_tag.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2546 2021-06-28 12:37:49.000000 bacpypes3-0.0.78/tests/test_primitive_data/test_time.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3588 2021-06-28 12:37:49.000000 bacpypes3-0.0.78/tests/test_primitive_data/test_unsigned.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-03 03:40:21.695955 bacpypes3-0.0.78/tests/test_utilities/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      130 2023-01-26 13:59:48.000000 bacpypes3-0.0.78/tests/test_utilities/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    18594 2023-01-26 13:59:48.000000 bacpypes3-0.0.78/tests/test_utilities/test_state_machine.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-07-03 03:40:21.695955 bacpypes3-0.0.78/tests/test_vlan/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      200 2023-01-26 13:59:48.000000 bacpypes3-0.0.78/tests/test_vlan/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8287 2023-01-26 13:59:48.000000 bacpypes3-0.0.78/tests/test_vlan/test_ipv4_network.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     6304 2023-01-26 13:59:48.000000 bacpypes3-0.0.78/tests/test_vlan/test_ipv4_router.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8904 2023-01-26 13:59:48.000000 bacpypes3-0.0.78/tests/test_vlan/test_network.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    12098 2023-01-26 13:59:48.000000 bacpypes3-0.0.78/tests/trapped_classes.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1397 2023-01-26 13:59:48.000000 bacpypes3-0.0.78/tests/utilities.py
```

### Comparing `bacpypes3-0.0.77/PKG-INFO` & `bacpypes3-0.0.78/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacpypes3
-Version: 0.0.77
+Version: 0.0.78
 Summary: BACnet Communications Library
 Home-page: https://github.com/JoelBender/bacpypes3
 Author: Joel Bender
 Author-email: joel@carrickbender.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bacpypes3-0.0.77/bacpypes3/__init__.py` & `bacpypes3-0.0.78/bacpypes3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 if _sys.platform not in _supported_platforms:
     _warnings.warn("unsupported platform", RuntimeWarning)
 
 #
 #   Project Metadata
 #
 
-__version__ = "0.0.77"
+__version__ = "0.0.78"
 __author__ = "Joel Bender"
 __email__ = "joel@carrickbender.com"
 
 #
 #   Settings and Debugging
 #
```

### Comparing `bacpypes3-0.0.77/bacpypes3/__main__.py` & `bacpypes3-0.0.78/bacpypes3/__main__.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/apdu.py` & `bacpypes3-0.0.78/bacpypes3/apdu.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/app.py` & `bacpypes3-0.0.78/bacpypes3/app.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/appservice.py` & `bacpypes3-0.0.78/bacpypes3/appservice.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/argparse.py` & `bacpypes3-0.0.78/bacpypes3/argparse.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/basetypes.py` & `bacpypes3-0.0.78/bacpypes3/basetypes.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/cmd.py` & `bacpypes3-0.0.78/bacpypes3/cmd.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/comm.py` & `bacpypes3-0.0.78/bacpypes3/comm.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/console.py` & `bacpypes3-0.0.78/bacpypes3/console.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/constructeddata.py` & `bacpypes3-0.0.78/bacpypes3/constructeddata.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/debugging.py` & `bacpypes3-0.0.78/bacpypes3/debugging.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/errors.py` & `bacpypes3-0.0.78/bacpypes3/errors.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/ipv4/__init__.py` & `bacpypes3-0.0.78/bacpypes3/ipv4/__init__.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/ipv4/app.py` & `bacpypes3-0.0.78/bacpypes3/ipv4/app.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/ipv4/bvll.py` & `bacpypes3-0.0.78/bacpypes3/ipv4/bvll.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/ipv4/link.py` & `bacpypes3-0.0.78/bacpypes3/ipv4/link.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/ipv4/service.py` & `bacpypes3-0.0.78/bacpypes3/ipv4/service.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/ipv6/__init__.py` & `bacpypes3-0.0.78/bacpypes3/ipv6/__init__.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/ipv6/bvll.py` & `bacpypes3-0.0.78/bacpypes3/ipv6/bvll.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/ipv6/service.py` & `bacpypes3-0.0.78/bacpypes3/ipv6/service.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/json/util.py` & `bacpypes3-0.0.78/bacpypes3/json/util.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/lib/batchread.py` & `bacpypes3-0.0.78/bacpypes3/lib/batchread.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/local/analog.py` & `bacpypes3-0.0.78/bacpypes3/local/analog.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/local/binary.py` & `bacpypes3-0.0.78/bacpypes3/local/binary.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/local/cmd.py` & `bacpypes3-0.0.78/bacpypes3/local/cmd.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/local/cov.py` & `bacpypes3-0.0.78/bacpypes3/local/cov.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/local/device.py` & `bacpypes3-0.0.78/bacpypes3/local/device.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/local/event.py` & `bacpypes3-0.0.78/bacpypes3/local/event.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/local/fault.py` & `bacpypes3-0.0.78/bacpypes3/local/fault.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/local/networkport.py` & `bacpypes3-0.0.78/bacpypes3/local/networkport.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/local/object.py` & `bacpypes3-0.0.78/bacpypes3/local/object.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/local/oos.py` & `bacpypes3-0.0.78/bacpypes3/local/oos.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/local/schedule.py` & `bacpypes3-0.0.78/bacpypes3/local/schedule.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/netservice.py` & `bacpypes3-0.0.78/bacpypes3/netservice.py`

 * *Files 0% similar despite different names*

```diff
@@ -602,26 +602,28 @@
             # set the destination
             npdu.pduDestination = LocalBroadcast()
             npdu.npduDADR = pdu.pduDestination
 
             # send it to the local adapter
             await local_adapter.process_npdu(npdu)
 
-            # make it look routed
-            if _debug:
-                NetworkServiceAccessPoint._debug("    - adding SADR")
-            npdu.npduSADR = RemoteStation(
-                local_adapter.adapterNet,  # type: ignore[arg-type]
-                local_adapter.adapterAddr.addrAddr,  # type: ignore[union-attr]
-            )
+            # make sure we're really a router
+            if len(self.adapters) > 1:
+                # make it look routed
+                if _debug:
+                    NetworkServiceAccessPoint._debug("    - adding SADR")
+                npdu.npduSADR = RemoteStation(
+                    local_adapter.adapterNet,  # type: ignore[arg-type]
+                    local_adapter.adapterAddr.addrAddr,  # type: ignore[union-attr]
+                )
 
-            # send it to all of the other connected adapters
-            for xadapter in self.adapters.values():
-                if xadapter is not local_adapter:
-                    await xadapter.process_npdu(npdu)
+                # send it to all of the other connected adapters
+                for xadapter in self.adapters.values():
+                    if xadapter is not local_adapter:
+                        await xadapter.process_npdu(npdu)
             return
 
         # remote broadcast
         if (npdu.pduDestination.addrType != Address.remoteBroadcastAddr) and (
             npdu.pduDestination.addrType != Address.remoteStationAddr
         ):
             raise RuntimeError(
```

### Comparing `bacpypes3-0.0.77/bacpypes3/npdu.py` & `bacpypes3-0.0.78/bacpypes3/npdu.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/object.py` & `bacpypes3-0.0.78/bacpypes3/object.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/pdu.py` & `bacpypes3-0.0.78/bacpypes3/pdu.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/primitivedata.py` & `bacpypes3-0.0.78/bacpypes3/primitivedata.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/rdf/core.py` & `bacpypes3-0.0.78/bacpypes3/rdf/core.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/rdf/util.py` & `bacpypes3-0.0.78/bacpypes3/rdf/util.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/sc/bvll.py` & `bacpypes3-0.0.78/bacpypes3/sc/bvll.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/sc/service.py` & `bacpypes3-0.0.78/bacpypes3/sc/service.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/service/cov.py` & `bacpypes3-0.0.78/bacpypes3/service/cov.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/service/device.py` & `bacpypes3-0.0.78/bacpypes3/service/device.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/service/object.py` & `bacpypes3-0.0.78/bacpypes3/service/object.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/settings.py` & `bacpypes3-0.0.78/bacpypes3/settings.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/vlan/__init__.py` & `bacpypes3-0.0.78/bacpypes3/vlan/__init__.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3/vlan/link.py` & `bacpypes3-0.0.78/bacpypes3/vlan/link.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/bacpypes3.egg-info/PKG-INFO` & `bacpypes3-0.0.78/bacpypes3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacpypes3
-Version: 0.0.77
+Version: 0.0.78
 Summary: BACnet Communications Library
 Home-page: https://github.com/JoelBender/bacpypes3
 Author: Joel Bender
 Author-email: joel@carrickbender.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bacpypes3-0.0.77/bacpypes3.egg-info/SOURCES.txt` & `bacpypes3-0.0.78/bacpypes3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/setup.py` & `bacpypes3-0.0.78/setup.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/clocked_test.py` & `bacpypes3-0.0.78/tests/clocked_test.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/state_machine.py` & `bacpypes3-0.0.78/tests/state_machine.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_1.py` & `bacpypes3-0.0.78/tests/test_1.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test__template.py` & `bacpypes3-0.0.78/tests/test__template.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_constructed_data/test_any.py` & `bacpypes3-0.0.78/tests/test_constructed_data/test_any.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_constructed_data/test_array.py` & `bacpypes3-0.0.78/tests/test_constructed_data/test_array.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_constructed_data/test_choice.py` & `bacpypes3-0.0.78/tests/test_constructed_data/test_choice.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_constructed_data/test_list.py` & `bacpypes3-0.0.78/tests/test_constructed_data/test_list.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_constructed_data/test_read_property_multiple.py` & `bacpypes3-0.0.78/tests/test_constructed_data/test_read_property_multiple.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_constructed_data/test_sequence.py` & `bacpypes3-0.0.78/tests/test_constructed_data/test_sequence.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_constructed_data/test_sequence_of.py` & `bacpypes3-0.0.78/tests/test_constructed_data/test_sequence_of.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_pdu/test_address.py` & `bacpypes3-0.0.78/tests/test_pdu/test_address.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_primitive_data/test_bit_string.py` & `bacpypes3-0.0.78/tests/test_primitive_data/test_bit_string.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_primitive_data/test_boolean.py` & `bacpypes3-0.0.78/tests/test_primitive_data/test_boolean.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_primitive_data/test_character_string.py` & `bacpypes3-0.0.78/tests/test_primitive_data/test_character_string.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_primitive_data/test_date.py` & `bacpypes3-0.0.78/tests/test_primitive_data/test_date.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_primitive_data/test_double.py` & `bacpypes3-0.0.78/tests/test_primitive_data/test_double.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_primitive_data/test_enumerated.py` & `bacpypes3-0.0.78/tests/test_primitive_data/test_enumerated.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_primitive_data/test_integer.py` & `bacpypes3-0.0.78/tests/test_primitive_data/test_integer.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_primitive_data/test_null.py` & `bacpypes3-0.0.78/tests/test_primitive_data/test_null.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_primitive_data/test_object_identifier.py` & `bacpypes3-0.0.78/tests/test_primitive_data/test_object_identifier.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_primitive_data/test_octet_string.py` & `bacpypes3-0.0.78/tests/test_primitive_data/test_octet_string.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_primitive_data/test_real.py` & `bacpypes3-0.0.78/tests/test_primitive_data/test_real.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_primitive_data/test_tag.py` & `bacpypes3-0.0.78/tests/test_primitive_data/test_tag.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_primitive_data/test_time.py` & `bacpypes3-0.0.78/tests/test_primitive_data/test_time.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_primitive_data/test_unsigned.py` & `bacpypes3-0.0.78/tests/test_primitive_data/test_unsigned.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_utilities/test_state_machine.py` & `bacpypes3-0.0.78/tests/test_utilities/test_state_machine.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_vlan/test_ipv4_network.py` & `bacpypes3-0.0.78/tests/test_vlan/test_ipv4_network.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_vlan/test_ipv4_router.py` & `bacpypes3-0.0.78/tests/test_vlan/test_ipv4_router.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/test_vlan/test_network.py` & `bacpypes3-0.0.78/tests/test_vlan/test_network.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/trapped_classes.py` & `bacpypes3-0.0.78/tests/trapped_classes.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.77/tests/utilities.py` & `bacpypes3-0.0.78/tests/utilities.py`

 * *Files identical despite different names*

