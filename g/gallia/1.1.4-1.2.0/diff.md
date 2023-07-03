# Comparing `tmp/gallia-1.1.4.tar.gz` & `tmp/gallia-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gallia-1.1.4.tar", max compression
+gzip compressed data, was "gallia-1.2.0.tar", max compression
```

## Comparing `gallia-1.1.4.tar` & `gallia-1.2.0.tar`

### file list

```diff
@@ -1,91 +1,89 @@
--rw-r--r--   0        0        0    10280 2023-01-25 14:57:12.959765 gallia-1.1.4/LICENSE
-drwxr-xr-x   0        0        0        0 2023-01-25 14:57:12.959765 gallia-1.1.4/LICENSES/
--rw-r--r--   0        0        0     2869 2023-01-25 14:57:12.959765 gallia-1.1.4/README.md
--rw-r--r--   0        0        0     3161 2023-01-25 14:57:12.963765 gallia-1.1.4/pyproject.toml
--rw-r--r--   0        0        0       88 2023-01-25 14:57:12.963765 gallia-1.1.4/src/cursed_hr/__init__.py
--rw-r--r--   0        0        0    51103 2023-01-25 14:57:12.963765 gallia-1.1.4/src/cursed_hr/cursed_hr.py
--rw-r--r--   0        0        0       88 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/__init__.py
--rw-r--r--   0        0        0     9730 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/cli.py
--rw-r--r--   0        0        0      353 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/command/__init__.py
--rw-r--r--   0        0        0    20534 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/command/base.py
--rw-r--r--   0        0        0     8653 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/command/uds.py
--rw-r--r--   0        0        0     2298 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/__init__.py
--rw-r--r--   0        0        0       88 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/discover/__init__.py
--rw-r--r--   0        0        0     9333 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/discover/find_xcp.py
--rw-r--r--   0        0        0       88 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/discover/uds/__init__.py
--rw-r--r--   0        0        0     4895 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/discover/uds/doip.py
--rw-r--r--   0        0        0     9552 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/discover/uds/isotp.py
--rw-r--r--   0        0        0        0 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/fuzz/__init__.py
--rw-r--r--   0        0        0        0 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/fuzz/uds/__init__.py
--rw-r--r--   0        0        0     7801 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/fuzz/uds/pdu.py
--rw-r--r--   0        0        0       88 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/primitive/__init__.py
--rw-r--r--   0        0        0        0 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/primitive/generic/__init__.py
--rw-r--r--   0        0        0      686 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/primitive/generic/pdu.py
--rw-r--r--   0        0        0       88 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/primitive/uds/__init__.py
--rw-r--r--   0        0        0     8371 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/primitive/uds/dtc.py
--rw-r--r--   0        0        0     1947 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/primitive/uds/ecu_reset.py
--rw-r--r--   0        0        0     4384 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/primitive/uds/iocbi.py
--rw-r--r--   0        0        0     1669 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/primitive/uds/ping.py
--rw-r--r--   0        0        0     1513 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/primitive/uds/read_by_identifier.py
--rw-r--r--   0        0        0     1874 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/primitive/uds/read_error_log.py
--rw-r--r--   0        0        0     1723 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/primitive/uds/rmba.py
--rw-r--r--   0        0        0     5558 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/primitive/uds/rtcl.py
--rw-r--r--   0        0        0     2317 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/primitive/uds/send_pdu.py
--rw-r--r--   0        0        0      792 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/primitive/uds/test_xcp.py
--rw-r--r--   0        0        0      708 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/primitive/uds/vin.py
--rw-r--r--   0        0        0     2045 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/primitive/uds/wmba.py
--rw-r--r--   0        0        0     1785 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/primitive/uds/write_by_identifier.py
--rw-r--r--   0        0        0       88 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/scan/__init__.py
--rw-r--r--   0        0        0       88 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/scan/uds/__init__.py
--rw-r--r--   0        0        0     9283 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/scan/uds/identifiers.py
--rw-r--r--   0        0        0     4241 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/scan/uds/memory.py
--rw-r--r--   0        0        0     7195 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/scan/uds/reset.py
--rw-r--r--   0        0        0     7879 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/scan/uds/sa_dump_seeds.py
--rw-r--r--   0        0        0     6461 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/scan/uds/services.py
--rw-r--r--   0        0        0    10817 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/scan/uds/sessions.py
--rw-r--r--   0        0        0        0 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/script/__init__.py
--rw-r--r--   0        0        0     3549 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/commands/script/vecu.py
--rw-r--r--   0        0        0     2170 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/config.py
--rw-r--r--   0        0        0       88 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/db/__init__.py
--rw-r--r--   0        0        0    16343 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/db/handler.py
--rw-r--r--   0        0        0      232 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/db/log.py
--rw-r--r--   0        0        0     5992 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/dumpcap.py
--rw-r--r--   0        0        0    25816 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/log.py
--rw-r--r--   0        0        0     4717 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/plugins.py
--rw-r--r--   0        0        0     2796 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/powersupply.py
--rw-r--r--   0        0        0        0 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/py.typed
--rw-r--r--   0        0        0       88 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/services/__init__.py
--rw-r--r--   0        0        0      702 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/services/uds/__init__.py
--rw-r--r--   0        0        0       88 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/services/uds/core/__init__.py
--rw-r--r--   0        0        0    48578 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/services/uds/core/client.py
--rw-r--r--   0        0        0     8554 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/services/uds/core/constants.py
--rw-r--r--   0        0        0    13749 2023-01-25 14:57:12.963765 gallia-1.1.4/src/gallia/services/uds/core/exception.py
--rw-r--r--   0        0        0   111436 2023-01-25 14:57:12.967765 gallia-1.1.4/src/gallia/services/uds/core/service.py
--rw-r--r--   0        0        0     7820 2023-01-25 14:57:12.967765 gallia-1.1.4/src/gallia/services/uds/core/utils.py
--rw-r--r--   0        0        0    20116 2023-01-25 14:57:12.967765 gallia-1.1.4/src/gallia/services/uds/ecu.py
--rw-r--r--   0        0        0     3567 2023-01-25 14:57:12.967765 gallia-1.1.4/src/gallia/services/uds/helpers.py
--rw-r--r--   0        0        0     5112 2023-01-25 14:57:12.967765 gallia-1.1.4/src/gallia/services/uds/nrv.py
--rw-r--r--   0        0        0    32677 2023-01-25 14:57:12.967765 gallia-1.1.4/src/gallia/services/uds/server.py
--rw-r--r--   0        0        0     2880 2023-01-25 14:57:12.967765 gallia-1.1.4/src/gallia/services/xcp/__init__.py
--rw-r--r--   0        0        0    22658 2023-01-25 14:57:12.967765 gallia-1.1.4/src/gallia/services/xcp/types.py
--rw-r--r--   0        0        0      638 2023-01-25 14:57:12.967765 gallia-1.1.4/src/gallia/transports/__init__.py
--rw-r--r--   0        0        0     6758 2023-01-25 14:57:12.967765 gallia-1.1.4/src/gallia/transports/base.py
--rw-r--r--   0        0        0    13232 2023-01-25 14:57:12.967765 gallia-1.1.4/src/gallia/transports/can.py
--rw-r--r--   0        0        0    18450 2023-01-25 14:57:12.967765 gallia-1.1.4/src/gallia/transports/doip.py
--rw-r--r--   0        0        0     2646 2023-01-25 14:57:12.967765 gallia-1.1.4/src/gallia/transports/tcp.py
--rw-r--r--   0        0        0     6446 2023-01-25 14:57:12.967765 gallia-1.1.4/src/gallia/utils.py
--rw-r--r--   0        0        0     4069 2023-01-25 14:57:12.967765 gallia-1.1.4/src/gallia/xdg.py
--rw-r--r--   0        0        0     2546 2023-01-25 14:57:12.967765 gallia-1.1.4/src/hr/__init__.py
--rw-r--r--   0        0        0      306 2023-01-25 14:57:12.967765 gallia-1.1.4/src/opennetzteil/__init__.py
--rw-r--r--   0        0        0     3356 2023-01-25 14:57:12.967765 gallia-1.1.4/src/opennetzteil/cli.py
--rw-r--r--   0        0        0        0 2023-01-25 14:57:12.967765 gallia-1.1.4/src/opennetzteil/devices/__init__.py
--rw-r--r--   0        0        0        0 2023-01-25 14:57:12.967765 gallia-1.1.4/src/opennetzteil/devices/http/__init__.py
--rw-r--r--   0        0        0     3672 2023-01-25 14:57:12.967765 gallia-1.1.4/src/opennetzteil/devices/http/client.py
--rw-r--r--   0        0        0        0 2023-01-25 14:57:12.967765 gallia-1.1.4/src/opennetzteil/devices/rnd/__init__.py
--rw-r--r--   0        0        0        0 2023-01-25 14:57:12.967765 gallia-1.1.4/src/opennetzteil/devices/rs/__init__.py
--rw-r--r--   0        0        0     4340 2023-01-25 14:57:12.967765 gallia-1.1.4/src/opennetzteil/devices/rs/hmc804.py
--rw-r--r--   0        0        0      144 2023-01-25 14:57:12.967765 gallia-1.1.4/src/opennetzteil/exceptions.py
--rw-r--r--   0        0        0     3099 2023-01-25 14:57:12.967765 gallia-1.1.4/src/opennetzteil/netzteil.py
--rw-r--r--   0        0        0        0 2023-01-25 14:57:12.967765 gallia-1.1.4/src/opennetzteil/py.typed
--rw-r--r--   0        0        0     5217 1970-01-01 00:00:00.000000 gallia-1.1.4/setup.py
--rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 gallia-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0    10280 2023-07-03 11:57:04.989813 gallia-1.2.0/LICENSE
+drwxr-xr-x   0        0        0        0 2023-07-03 11:57:04.989813 gallia-1.2.0/LICENSES/
+-rw-r--r--   0        0        0     2995 2023-07-03 11:57:04.989813 gallia-1.2.0/README.md
+-rw-r--r--   0        0        0     2777 2023-07-03 11:57:04.993813 gallia-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       88 2023-07-03 11:57:04.993813 gallia-1.2.0/src/cursed_hr/__init__.py
+-rw-r--r--   0        0        0    51310 2023-07-03 11:57:04.993813 gallia-1.2.0/src/cursed_hr/cursed_hr.py
+-rw-r--r--   0        0        0       88 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/__init__.py
+-rw-r--r--   0        0        0    11338 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/cli.py
+-rw-r--r--   0        0        0      353 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/command/__init__.py
+-rw-r--r--   0        0        0    20846 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/command/base.py
+-rw-r--r--   0        0        0     8653 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/command/uds.py
+-rw-r--r--   0        0        0     2371 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/__init__.py
+-rw-r--r--   0        0        0       88 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/discover/__init__.py
+-rw-r--r--   0        0        0     9349 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/discover/find_xcp.py
+-rw-r--r--   0        0        0       88 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/discover/uds/__init__.py
+-rw-r--r--   0        0        0     4912 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/discover/uds/doip.py
+-rw-r--r--   0        0        0     9552 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/discover/uds/isotp.py
+-rw-r--r--   0        0        0        0 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/fuzz/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/fuzz/uds/__init__.py
+-rw-r--r--   0        0        0     7800 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/fuzz/uds/pdu.py
+-rw-r--r--   0        0        0       88 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/primitive/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/primitive/generic/__init__.py
+-rw-r--r--   0        0        0      686 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/primitive/generic/pdu.py
+-rw-r--r--   0        0        0       88 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/primitive/uds/__init__.py
+-rw-r--r--   0        0        0     8371 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/primitive/uds/dtc.py
+-rw-r--r--   0        0        0     1947 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/primitive/uds/ecu_reset.py
+-rw-r--r--   0        0        0     4384 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/primitive/uds/iocbi.py
+-rw-r--r--   0        0        0     1669 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/primitive/uds/ping.py
+-rw-r--r--   0        0        0     1513 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/primitive/uds/read_by_identifier.py
+-rw-r--r--   0        0        0     1874 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/primitive/uds/read_error_log.py
+-rw-r--r--   0        0        0     1723 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/primitive/uds/rmba.py
+-rw-r--r--   0        0        0     5558 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/primitive/uds/rtcl.py
+-rw-r--r--   0        0        0     2317 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/primitive/uds/send_pdu.py
+-rw-r--r--   0        0        0     1928 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/primitive/uds/test_xcp.py
+-rw-r--r--   0        0        0      708 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/primitive/uds/vin.py
+-rw-r--r--   0        0        0     2045 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/primitive/uds/wmba.py
+-rw-r--r--   0        0        0     1785 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/primitive/uds/write_by_identifier.py
+-rw-r--r--   0        0        0       88 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/scan/__init__.py
+-rw-r--r--   0        0        0       88 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/scan/uds/__init__.py
+-rw-r--r--   0        0        0     9273 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/scan/uds/identifiers.py
+-rw-r--r--   0        0        0     4241 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/scan/uds/memory.py
+-rw-r--r--   0        0        0     7145 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/scan/uds/reset.py
+-rw-r--r--   0        0        0     7879 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/scan/uds/sa_dump_seeds.py
+-rw-r--r--   0        0        0     6453 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/scan/uds/services.py
+-rw-r--r--   0        0        0    10736 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/scan/uds/sessions.py
+-rw-r--r--   0        0        0        0 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/script/__init__.py
+-rw-r--r--   0        0        0     3530 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/commands/script/vecu.py
+-rw-r--r--   0        0        0     2194 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/config.py
+-rw-r--r--   0        0        0       88 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/db/__init__.py
+-rw-r--r--   0        0        0    16788 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/db/handler.py
+-rw-r--r--   0        0        0      232 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/db/log.py
+-rw-r--r--   0        0        0     6009 2023-07-03 11:57:04.993813 gallia-1.2.0/src/gallia/dumpcap.py
+-rw-r--r--   0        0        0    25801 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/log.py
+-rw-r--r--   0        0        0     4761 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/plugins.py
+-rw-r--r--   0        0        0     2797 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/powersupply.py
+-rw-r--r--   0        0        0        0 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/py.typed
+-rw-r--r--   0        0        0       88 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/services/__init__.py
+-rw-r--r--   0        0        0      702 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/services/uds/__init__.py
+-rw-r--r--   0        0        0       88 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/services/uds/core/__init__.py
+-rw-r--r--   0        0        0    48629 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/services/uds/core/client.py
+-rw-r--r--   0        0        0     8554 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/services/uds/core/constants.py
+-rw-r--r--   0        0        0    13749 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/services/uds/core/exception.py
+-rw-r--r--   0        0        0   111131 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/services/uds/core/service.py
+-rw-r--r--   0        0        0     7816 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/services/uds/core/utils.py
+-rw-r--r--   0        0        0    20142 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/services/uds/ecu.py
+-rw-r--r--   0        0        0     3567 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/services/uds/helpers.py
+-rw-r--r--   0        0        0     5112 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/services/uds/nrv.py
+-rw-r--r--   0        0        0    32455 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/services/uds/server.py
+-rw-r--r--   0        0        0     3911 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/services/xcp/__init__.py
+-rw-r--r--   0        0        0    22657 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/services/xcp/types.py
+-rw-r--r--   0        0        0      638 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/transports/__init__.py
+-rw-r--r--   0        0        0     6758 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/transports/base.py
+-rw-r--r--   0        0        0    13274 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/transports/can.py
+-rw-r--r--   0        0        0    18904 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/transports/doip.py
+-rw-r--r--   0        0        0     2646 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/transports/tcp.py
+-rw-r--r--   0        0        0     6711 2023-07-03 11:57:04.997813 gallia-1.2.0/src/gallia/utils.py
+-rw-r--r--   0        0        0     2545 2023-07-03 11:57:04.997813 gallia-1.2.0/src/hr/__init__.py
+-rw-r--r--   0        0        0      306 2023-07-03 11:57:04.997813 gallia-1.2.0/src/opennetzteil/__init__.py
+-rw-r--r--   0        0        0     3357 2023-07-03 11:57:04.997813 gallia-1.2.0/src/opennetzteil/cli.py
+-rw-r--r--   0        0        0        0 2023-07-03 11:57:04.997813 gallia-1.2.0/src/opennetzteil/devices/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 11:57:04.997813 gallia-1.2.0/src/opennetzteil/devices/http/__init__.py
+-rw-r--r--   0        0        0     3631 2023-07-03 11:57:04.997813 gallia-1.2.0/src/opennetzteil/devices/http/client.py
+-rw-r--r--   0        0        0        0 2023-07-03 11:57:04.997813 gallia-1.2.0/src/opennetzteil/devices/rnd/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 11:57:04.997813 gallia-1.2.0/src/opennetzteil/devices/rs/__init__.py
+-rw-r--r--   0        0        0     4321 2023-07-03 11:57:04.997813 gallia-1.2.0/src/opennetzteil/devices/rs/hmc804.py
+-rw-r--r--   0        0        0      144 2023-07-03 11:57:04.997813 gallia-1.2.0/src/opennetzteil/exceptions.py
+-rw-r--r--   0        0        0     3099 2023-07-03 11:57:04.997813 gallia-1.2.0/src/opennetzteil/netzteil.py
+-rw-r--r--   0        0        0        0 2023-07-03 11:57:04.997813 gallia-1.2.0/src/opennetzteil/py.typed
+-rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 gallia-1.2.0/PKG-INFO
```

### Comparing `gallia-1.1.4/LICENSE` & `gallia-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/README.md` & `gallia-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 [![docs](https://img.shields.io/badge/-docs-green)](https://fraunhofer-aisec.github.io/gallia)
 [![docs](https://readthedocs.org/projects/docs/badge/?version=latest)](https://gallia.readthedocs.io/en/latest)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gallia)](https://pypi.python.org/pypi/gallia/)
 [![PyPI - License](https://img.shields.io/pypi/l/gallia)](https://www.apache.org/licenses/LICENSE-2.0.html)
 [![PyPI](https://img.shields.io/pypi/v/gallia)](https://pypi.python.org/pypi/gallia/)
 
+[![Packaging status](https://repology.org/badge/vertical-allrepos/gallia.svg)](https://repology.org/project/gallia/versions)
+
 Gallia is an extendable pentesting framework with the focus on the automotive domain.
 The scope of the toolchain is conducting penetration tests from a single ECU up to whole cars.
 Currently, the main focus lies on the [UDS](https://www.iso.org/standard/72439.html) interface.
 Acting as a generic interface, the logging functionality implements reproducible tests and enables post-processing tasks.
 The [rendered documentation](https://fraunhofer-aisec.github.io/gallia) is available via Github Pages.
 Alternatively, the documentation is hosted on [readthedocs](https://gallia.readthedocs.io/en/latest) as well.
 The documentation for the current [stable](https://gallia.readthedocs.io/en/stable) realease is available on readthedocs.
```

### Comparing `gallia-1.1.4/pyproject.toml` & `gallia-1.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "gallia"
-version = "1.1.4"
+version = "1.2.0"
 description = "Extendable Pentesting Framework"
 license = "Apache-2.0"
 readme = "README.md"
 documentation = "https://fraunhofer-aisec.github.io/gallia"
 repository = "https://github.com/Fraunhofer-AISEC/gallia"
 authors = ["AISEC Pentesting Team"]
 maintainers = [
@@ -31,99 +31,88 @@
     { include = "hr", from = "src" },
     { include = "opennetzteil", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 aiohttp = "^3.8"
-aiofiles = "^22.1"
+aiofiles = ">=22.1,<24.0"
 aiosqlite = ">=0.18"
-argcomplete = "^2.0"
+argcomplete = ">=2,<4"
 zstandard = ">=0.19"
-python-can = "^4.0"
+python-can = "^4.2"
 tabulate = ">=0.9"
 construct = "^2.10.67"
-tomli = { version = "^2.0.1", python = "<3.11" }
-msgspec = ">=0.11,<0.13"
-pydantic = "^1.10"
+tomli = { version = "^2.0", python = "<3.11" }
+msgspec = ">=0.11,<0.17"
+pydantic = "^2.0"
 pygit2 = "^1.10"
+platformdirs = ">=2.6,<4.0"
+exitcode = "^0.1.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.10"
-Sphinx = "^5.2"
-isort = "^5.10"
-mypy = "^0.991"
-pylint = "^2.15.0"
+black = ">=22.10,<24.0"
+Sphinx = ">=5.2,<7.0"
+mypy = "^1.0"
 pylsp-mypy = "^0.6"
 pylsp-rope = "^0.1"
 pytest = "^7.1"
-pytest-asyncio = "^0.20"
+pytest-asyncio = ">=0.20,<0.22"
 python-lsp-black = "^1.1"
 python-lsp-server = "^1.5"
-types-aiofiles = "^22.1"
+types-aiofiles = "^23.1"
 types-tabulate = "^0.9"
-myst-parser = "^0.18"
+myst-parser = ">=0.18,<2.1"
 sphinx-rtd-theme = "^1.0"
 reuse = "^1.0.0"
 construct-typing = "^0.5.2"
 pytest-cov = "^4.0"
-pyls-isort = "^0.2.2"
-ruff = "^0.0.192"
-flake8 = "^6.0.0"
+ruff = ">=0.0.260,<0.0.276"
+python-lsp-ruff = "^1.1.0"
 
 [tool.poetry.scripts]
 "gallia" = "gallia.cli:main"
 "netzteil" = "opennetzteil.cli:main"
 "cursed-hr" = "cursed_hr.cursed_hr:main"
 "hr" = "hr:main"
 
 [tool.mypy]
 strict = true
+plugins = [
+    "pydantic.mypy"
+]
 
 [[tool.mypy.overrides]]
 module = [
     "argcomplete",
     "pygit2",
 ]
 ignore_missing_imports = true
 
 [tool.ruff]
-line-length = 120
 target-version = "py310"
+select = [
+    # TODO: Enable this
+    # "B",    # flake8-bugbear
+    "C4",   # flake8-comprehensions
+    "E",    # pycodestlye
+    "F",    # pyflakes
+    "I",    # isort
+    "PL",   # pylint
+    "PTH",  # flake8-use-pathlib
+    "TID",  # flake8-tidy-imports
+    "UP",   # pyupgrade
+]
+ignore = [
+    "E501",     # line length
+    "PLR2004",  # magic value used in comparison
+    "PLR0911",  # too many return statements
+    "PLR0912",  # too many branches
+    "PLR0915",  # too many statements
+    "PLC1901",  # empty string is falsey
+]
 
 [tool.black]
 target-version = ['py310']
 
-[tool.isort]
-profile = "black"
-py_version= "310"
-
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
-
-[tool.pylint.messages_control]
-disable = [
-    "broad-except",
-    "duplicate-code",  # https://github.com/Fraunhofer-AISEC/gallia/issues/306
-    "fixme",
-    "invalid-name",
-    "line-too-long",  # handled by black
-    "logging-fstring-interpolation",  # https://github.com/Fraunhofer-AISEC/gallia/issues/234
-    "logging-not-lazy",  # https://github.com/Fraunhofer-AISEC/gallia/issues/234
-    "missing-class-docstring",
-    "missing-class-docstring",
-    "missing-function-docstring",
-    "missing-module-docstring",
-    "no-member",  # mypy handles this better
-    "no-name-in-module",  # mypy handles this better
-    "too-few-public-methods",
-    "too-many-arguments",
-    "too-many-branches",
-    "too-many-instance-attributes",
-    "too-many-lines",
-    "too-many-locals",
-    "too-many-nested-blocks",
-    "too-many-public-methods",
-    "too-many-return-statements",
-    "too-many-statements",
-    "unused-argument",
-]
```

### Comparing `gallia-1.1.4/src/cursed_hr/cursed_hr.py` & `gallia-1.2.0/src/cursed_hr/cursed_hr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 # SPDX-FileCopyrightText: AISEC Pentesting Team
 #
 # SPDX-License-Identifier: Apache-2.0
 
-# pylint: disable=too-many-lines,eval-used
-
 from __future__ import annotations
 
 import curses
 import curses.ascii
 import gzip
 import json
 import mmap
 import shutil
 import tempfile
 import warnings
-from argparse import ArgumentParser
+from argparse import ArgumentParser, BooleanOptionalAction
 from array import array
 from binascii import unhexlify
 from copy import deepcopy
 from dataclasses import dataclass
 from datetime import datetime
 from enum import IntEnum, unique
 from math import ceil
 from pathlib import Path
 from typing import Any, BinaryIO, cast
 
 import zstandard as zstd
-
 from gallia.log import PenlogPriority, PenlogRecord
 from gallia.services.uds.core.service import NegativeResponse, UDSRequest, UDSResponse
 
 
 @unique
 class InterpretationColor(IntEnum):
     DEFAULT = 42
@@ -168,26 +165,28 @@
     """
 
     def __init__(
         self,
         in_file: Path,
         priority: PenlogPriority = PenlogPriority.DEBUG,
         filters: list[str] | None = None,
+        use_prefix: bool = True,
     ):
         self.in_file = in_file
-        self.level_pointers: list[array[int]] = list(array("L") for _ in range(9))
+        self.level_pointers: list[array[int]] = [array("L") for _ in range(9)]
         self.entry_positions = array("L")
         self.configuration_history = [
             Configuration(
                 priority_zones=[PriorityZone(0, None, priority)],
                 filter=filters if filters is not None else [],
                 interpret=False,
             )
         ]
         self.configuration_index = 0
+        self.use_prefix = use_prefix
 
         try:
             self.window = self.init_curses()
             self.color_ids = self.define_colors()
             self.file = self.uncompressed_file()
 
             try:
@@ -227,15 +226,15 @@
             PenlogPriority.WARNING: (104, curses.COLOR_YELLOW),
             PenlogPriority.NOTICE: (105, -1),
             PenlogPriority.INFO: (106, -1),
             PenlogPriority.DEBUG: (107, 8),
             PenlogPriority.TRACE: (108, curses.COLOR_BLUE),
         }
 
-        for (identifier, value) in prio_colors.values():
+        for identifier, value in prio_colors.values():
             curses.init_pair(identifier, value, -1)
 
         curses.init_pair(InterpretationColor.DEFAULT, 8, -1)
         curses.init_pair(InterpretationColor.UDS_REQUEST, curses.COLOR_CYAN, -1)
         curses.init_pair(
             InterpretationColor.UDS_POSITIVE_RESPONSE, curses.COLOR_GREEN, -1
         )
@@ -258,24 +257,24 @@
             if self.in_file.suffix in [".zst", ".gz"]:
                 self.window.erase()
                 self.window.addstr(
                     f"Loading contents from {self.in_file}: Decompressing file ..."
                 )
                 self.window.refresh()
 
-                file = tempfile.TemporaryFile()  # pylint: disable=consider-using-with
+                file = tempfile.TemporaryFile()
 
                 match self.in_file.suffix:
                     case ".zst":
                         with self.in_file.open("rb") as in_file:
                             decomp = zstd.ZstdDecompressor()
                             decomp.copy_stream(in_file, file)
                     case ".gz":
                         with gzip.open(self.in_file, "rb") as in_file:
-                            shutil.copyfileobj(in_file, file)
+                            shutil.copyfileobj(in_file, file)  # type: ignore
             else:
                 file = self.in_file.open("rb")
 
             file.flush()
 
             return file  # type: ignore
         except Exception as e:
@@ -369,15 +368,15 @@
         :params entry_id: The index of the entry.
         :return: The zone into which the entry with the given id falls.
         """
         for zone in self.configuration.priority_zones:
             if entry_id >= zone.start and (zone.end is None or entry_id <= zone.end):
                 return zone
 
-        assert False
+        raise AssertionError()
 
     def update_zones(self, new_zone: PriorityZone) -> None:
         """
         Inserts the given zone into the current set of zones.
 
         Adds a new list of zones into the zone history, which contains the previous zones and the new zone.
         In the process of integrating the new zone, itself as well as old zones may be altered or completely removed.
@@ -481,20 +480,22 @@
         :param entry_id: The index of the entry.
         :return: The formatted display entries for the given entry.
         """
         entry = self.entries[entry_id]
         _, max_width = self.window.getmaxyx()
 
         prefix = ""
-        prefix += entry.datetime.strftime("%b %d %H:%M:%S.%f")[:-3]
-        prefix += " "
-        prefix += entry.module
-        if entry.tags is not None:
-            prefix += f" [{', '.join(entry.tags)}]"
-        prefix += ": "
+
+        if self.use_prefix:
+            prefix += entry.datetime.strftime("%b %d %H:%M:%S.%f")[:-3]
+            prefix += " "
+            prefix += entry.module
+            if entry.tags is not None:
+                prefix += f" [{', '.join(entry.tags)}]"
+            prefix += ": "
 
         residual_width = max_width - len(prefix) - 1
 
         user_defined_lines = entry.data.splitlines()
 
         if len(user_defined_lines) == 0:
             user_defined_lines = [""]
@@ -1046,20 +1047,19 @@
                     if cursor[0] > 0:
                         cursor = (cursor[0] - 1, cursor[1])
                     else:
                         line_up()
                 case "KEY_DOWN":
                     if cursor[0] < max_lines - 1:
                         cursor = cursor[0] + 1, cursor[1]
+                    elif display_entries[0].last_line:
+                        entry_start = min(len(self.entries) - 1, entry_start + 1)
+                        line_start = 0
                     else:
-                        if display_entries[0].last_line:
-                            entry_start = min(len(self.entries) - 1, entry_start + 1)
-                            line_start = 0
-                        else:
-                            line_start += 1
+                        line_start += 1
                 case "KEY_PPAGE":
                     if cursor[0] > 0:
                         cursor = (0, cursor[1])
                     else:
                         page_up()
                 case "KEY_NPAGE":
                     if cursor[0] < len(display_entries) - 1:
@@ -1141,17 +1141,17 @@
                         self.configuration_index + 1,
                     )
                 case "i":
                     self.new_configuration()
                     self.configuration.interpret = not self.configuration.interpret
                 case "f":
                     # fh is short for filter_history to reduce long unreadable lines
-                    fh_tmp = list(
+                    fh_tmp = [
                         "; ".join(filter_commands) for filter_commands in filter_history
-                    )
+                    ]
                     fh_tmp.append("")
                     fh_index = len(fh_tmp) - 1
 
                     filter_cursor = len(fh_tmp[fh_index])
                     input_format = curses.color_pair(0)
 
                     self.display(
@@ -1214,14 +1214,16 @@
                         self.display(
                             display_entries,
                             [FormattedText(fh_tmp[fh_index], input_format)],
                         )
                         self.window.move(
                             max_lines, min(filter_cursor, len(fh_tmp[fh_index]))
                         )
+                case "x":
+                    self.use_prefix = not self.use_prefix
 
             display_entries = self.calculate_display_entries(entry_start, line_start)
 
             previous_entry_start = 0
             previous_line_start = 0
 
             while len(display_entries) < max_lines and (
@@ -1311,17 +1313,17 @@
         data="data",
         host="host",
         priority=PenlogPriority.INFO,
         datetime=datetime.fromtimestamp(0),
         tags=[],
     )
 
-    commands = list(
+    commands = [
         command.strip() for command in text.split(";") if len(command.strip()) > 0
-    )
+    ]
 
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", SyntaxWarning)
 
         for command in commands:
             eval(command, test_entry.__dict__)
 
@@ -1331,13 +1333,14 @@
 def main() -> None:
     parser = ArgumentParser()
     parser.add_argument("file", type=Path)
     parser.add_argument(
         "--priority", "-p", type=PenlogPriority.from_str, default=PenlogPriority.DEBUG
     )
     parser.add_argument("--filter", "-f", type=parse_filter, default=None)
+    parser.add_argument("--prefix", action=BooleanOptionalAction, default=True)
     args = parser.parse_args()
-    CursedHR(args.file, args.priority, args.filter)
+    CursedHR(args.file, args.priority, args.filter, args.prefix)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `gallia-1.1.4/src/gallia/cli.py` & `gallia-1.2.0/src/gallia/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from collections.abc import Iterable
 from importlib.metadata import EntryPoint, version
 from pathlib import Path
 from pprint import pprint
 from typing import Any
 
 import argcomplete
+import exitcode
 
 from gallia.command.base import BaseCommand
 from gallia.commands import registry as cmd_registry
 from gallia.config import Config, load_config_file
 from gallia.log import setup_logging
 from gallia.plugins import (
     Parsers,
@@ -55,14 +56,19 @@
     )
     parser.add_argument(
         "--show-defaults",
         action="store_true",
         help="show defaults of all flags",
     )
     parser.add_argument(
+        "--show-cli",
+        action="store_true",
+        help="show the subcommand tree",
+    )
+    parser.add_argument(
         "--show-plugins",
         action="store_true",
         help="show loaded plugins",
     )
     parser.add_argument(
         "--template",
         action="store_true",
@@ -197,20 +203,18 @@
         sys.exit(1)
 
 
 def _get_cli_defaults(parser: argparse.ArgumentParser, out: dict[str, Any]) -> None:
     for action in parser.__dict__["_actions"]:
         if isinstance(
             action,
-            (
-                argparse._StoreAction,  # pylint: disable=protected-access
-                argparse._StoreTrueAction,  # pylint: disable=protected-access
-                argparse._StoreFalseAction,  # pylint: disable=protected-access
-                argparse.BooleanOptionalAction,
-            ),
+            argparse._StoreAction
+            | argparse._StoreTrueAction
+            | argparse._StoreFalseAction
+            | argparse.BooleanOptionalAction,
         ):
             opts = action.__dict__["option_strings"]
             if len(opts) == 2:
                 if opts[0].startswith("--"):
                     opts_str = opts[0]
                 else:
                     opts_str = opts[1]
@@ -231,27 +235,75 @@
 
                 d = d[key]
 
                 if i == len(keys) - 2:
                     d[keys[-1]] = value
                     break
 
-        if isinstance(
-            action, argparse._SubParsersAction  # pylint: disable=protected-access
-        ):
+        if isinstance(action, argparse._SubParsersAction):
             for subparser in action.__dict__["choices"].values():
                 _get_cli_defaults(subparser, out)
 
 
 def get_cli_defaults(parser: argparse.ArgumentParser) -> dict[str, Any]:
     out: dict[str, Any] = {}
     _get_cli_defaults(parser, out)
     return out
 
 
+def _get_command_tree(parser: argparse.ArgumentParser, out: dict[str, Any]) -> None:
+    for action in parser.__dict__["_actions"]:
+        if isinstance(action, argparse._SubParsersAction):
+            for cmd, subparser in action.__dict__["choices"].items():
+                out[cmd] = {}
+                d = out[cmd]
+                _get_command_tree(subparser, d)
+
+
+def get_command_tree(parser: argparse.ArgumentParser) -> dict[str, Any]:
+    out: dict[str, Any] = {"gallia": {}}
+    _get_command_tree(parser, out["gallia"])
+    return out
+
+
+def _print_tree(
+    current: str,
+    tree: dict[str, Any],
+    marker: str,
+    level_markers: list[bool],
+) -> None:
+    indent = " " * len(marker)
+    connection = "|" + indent[:-1]
+    level = len(level_markers)
+
+    def mapper(draw: bool) -> str:
+        return connection if draw else indent
+
+    markers = "".join(map(mapper, level_markers[:-1]))
+    markers += marker if level > 0 else ""
+
+    print(f"{markers}{current}")
+    for i, child in enumerate(tree.keys()):
+        is_last = i == len(tree.keys()) - 1
+        _print_tree(child, tree[child], marker, [*level_markers, not is_last])
+
+
+def print_tree(tree: dict[str, Any]) -> None:
+    # Assumption: first level of dict has only one element -> root node.
+    if len(tree) != 1:
+        raise ValueError("invalid tree")
+
+    root = list(tree.keys())[0]
+    _print_tree(root, tree[root], "+-", [])
+
+
+def cmd_show_cli(parser: argparse.ArgumentParser) -> None:
+    print_tree(get_command_tree(parser))
+
+
 def cmd_show_defaults(parser: argparse.ArgumentParser) -> None:
     pprint(get_cli_defaults(parser))
 
 
 def _print_plugin(description: str, eps: list[EntryPoint]) -> None:
     print(f"{description}:")
     for ep in eps:
@@ -324,41 +376,45 @@
     # Load plugins.
     for fn in load_cli_init_plugins():
         fn(parsers)
 
     try:
         config, config_path = load_config_file()
     except ValueError as e:
-        print(f"invalid config: {e}")
-        sys.exit(1)
+        print(f"invalid config: {e}", file=sys.stderr)
+        sys.exit(exitcode.CONFIG)
 
     build_cli(parsers, config, registry)
 
     parser = parsers["parser"]
     argcomplete.autocomplete(parser)
     args = parser.parse_args()
 
     if args.show_config:
         cmd_show_config(args, config, config_path)
-        sys.exit(0)
+        sys.exit(exitcode.OK)
 
     if args.show_defaults:
         cmd_show_defaults(parser)
-        sys.exit(0)
+        sys.exit(exitcode.OK)
+
+    if args.show_cli:
+        cmd_show_cli(parser)
+        sys.exit(exitcode.OK)
 
     if args.show_plugins:
         cmd_show_plugins()
-        sys.exit(0)
+        sys.exit(exitcode.OK)
 
     if args.template:
         cmd_template(args)
-        sys.exit(0)
+        sys.exit(exitcode.OK)
 
     if not hasattr(args, "run_func"):
         args.help_func()
-        parser.exit(1)
+        parser.exit(exitcode.USAGE)
 
     sys.exit(args.run_func(args))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `gallia-1.1.4/src/gallia/command/base.py` & `gallia-1.2.0/src/gallia/command/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,42 +6,35 @@
 import asyncio
 import fcntl
 import os
 import os.path
 import shutil
 import signal
 import sys
-import traceback
 from abc import ABC, abstractmethod
 from argparse import ArgumentParser, Namespace
 from datetime import datetime, timezone
-from enum import Enum, IntEnum, unique
+from enum import Enum, unique
 from pathlib import Path
 from subprocess import CalledProcessError, run
 from tempfile import gettempdir
 from typing import cast
 
+import exitcode
 import msgspec
 
 from gallia.config import Config
 from gallia.db.handler import DBHandler
 from gallia.dumpcap import Dumpcap
 from gallia.log import Loglevel, get_logger, setup_logging, tz
 from gallia.plugins import load_transport
 from gallia.powersupply import PowerSupply, PowerSupplyURI
 from gallia.services.uds.core.exception import UDSException
 from gallia.transports import BaseTransport, TargetURI
-from gallia.utils import camel_to_snake
-
-
-@unique
-class ExitCodes(IntEnum):
-    SUCCESS = 0
-    GENERIC_ERROR = 1
-    UNHANDLED_EXCEPTION = 2
+from gallia.utils import camel_to_snake, dump_args
 
 
 @unique
 class FileNames(Enum):
     PROPERTIES_PRE = "PROPERTIES_PRE.json"
     PROPERTIES_POST = "PROPERTIES_POST.json"
     META = "META.json"
@@ -52,26 +45,32 @@
 @unique
 class HookVariant(Enum):
     PRE = "pre"
     POST = "post"
 
 
 class CommandMeta(msgspec.Struct):
-    group: str
+    command: str | None
+    group: str | None
     subgroup: str | None
-    command: str
+
+    def json(self) -> str:
+        return msgspec.json.encode(self).decode()
 
 
 class RunMeta(msgspec.Struct):
     command: list[str]
     command_meta: CommandMeta
     start_time: str
     end_time: str
     exit_code: int
 
+    def json(self) -> str:
+        return msgspec.json.encode(self).decode()
+
 
 class BaseCommand(ABC):
     """BaseCommand is the baseclass for all gallia commands.
     This class can be used in standalone scripts via the
     gallia command line interface facility.
 
     This class needs to be subclassed and all the abstract
@@ -105,25 +104,25 @@
     CATCHED_EXCEPTIONS: list[type[Exception]] = []
 
     def __init__(self, parser: ArgumentParser, config: Config = Config()) -> None:
         self.id = camel_to_snake(self.__class__.__name__)
         self.logger = get_logger(self.LOGGER_NAME)
         self.parser = parser
         self.config = config
-        self.artifacts_dir = Path(".")
+        self.artifacts_dir = Path()
         self.run_meta = RunMeta(
             command=sys.argv,
             command_meta=CommandMeta(
                 command=self.COMMAND,
                 group=self.GROUP,
                 subgroup=self.SUBGROUP,
             ),
             start_time=datetime.now(tz).isoformat(),
             exit_code=0,
-            end_time=0,
+            end_time="",
         )
         self._lock_file_fd: int | None = None
         self.configure_class_parser()
         self.configure_parser()
 
     @abstractmethod
     def run(self, args: Namespace) -> int:
@@ -151,29 +150,32 @@
         script = args.pre_hook if variant == HookVariant.PRE else args.post_hook
         if script is None or script == "":
             return
 
         hook_id = f"{variant.value}-hook"
 
         argv = sys.argv[:]
-        argv[0] = os.path.basename(argv[0])
+        argv[0] = Path(argv[0]).name
         env = {
             "GALLIA_ARTIFACTS_DIR": str(self.artifacts_dir),
             "GALLIA_HOOK": variant.value,
             "GALLIA_INVOCATION": " ".join(argv),
         } | os.environ
 
+        if variant == HookVariant.POST:
+            env["GALLIA_META"] = self.run_meta.json()
+
         if self.COMMAND is not None:
-            env |= {"GALLIA_COMMAND": self.COMMAND}
+            env["GALLIA_COMMAND"] = self.COMMAND
         if self.GROUP is not None:
-            env |= {"GALLIA_GROUP": self.GROUP}
+            env["GALLIA_GROUP"] = self.GROUP
         if self.SUBGROUP is not None:
-            env |= {"GALLIA_GROUP": self.SUBGROUP}
+            env["GALLIA_GROUP"] = self.SUBGROUP
         if exit_code is not None:
-            env |= {"GALLIA_EXIT_CODE": str(exit_code)}
+            env["GALLIA_EXIT_CODE"] = str(exit_code)
 
         try:
             p = run(
                 script,
                 env=env,
                 text=True,
                 capture_output=True,
@@ -337,15 +339,15 @@
 
     def entry_point(self, args: Namespace) -> int:
         if (p := args.lock_file) is not None:
             try:
                 self._aquire_flock(p)
             except OSError as e:
                 self.logger.critical(f"Unable to lock {p}: {e}")
-                return ExitCodes.GENERIC_ERROR
+                return exitcode.OSFILE
 
         if self.HAS_ARTIFACTS_DIR:
             self.artifacts_dir = self.prepare_artifactsdir(
                 args.artifacts_base,
                 args.artifacts_dir,
             )
             setup_logging(
@@ -367,37 +369,38 @@
         # Ensure that META.json gets written in the case a
         # command calls sys.exit().
         except SystemExit as e:
             match e.code:
                 case int():
                     exit_code = e.code
                 case _:
-                    exit_code = ExitCodes.GENERIC_ERROR
+                    exit_code = exitcode.SOFTWARE
         except Exception as e:
             for t in self.CATCHED_EXCEPTIONS:
                 if isinstance(e, t):
-                    exit_code = ExitCodes.GENERIC_ERROR
-                    self.logger.critical(repr(e))
+                    # TODO: Map the exitcode to superclass of builtin exceptions.
+                    exit_code = exitcode.IOERR
+                    self.logger.critical(f"catched by default handler: {e!r}")
+                    self.logger.debug(e, exc_info=True)
                     break
             else:
-                exit_code = ExitCodes.UNHANDLED_EXCEPTION
-                traceback.print_exc()
+                exit_code = exitcode.SOFTWARE
+                self.logger.critical(e, exc_info=True)
         finally:
+            self.run_meta.exit_code = exit_code
+            self.run_meta.end_time = datetime.now(tz).isoformat()
+
             if self.HAS_ARTIFACTS_DIR:
-                self.run_meta.exit_code = exit_code
-                self.run_meta.end_time = datetime.now(tz).isoformat()
-                data = msgspec.json.encode(self.run_meta)
-                self.artifacts_dir.joinpath(FileNames.META.value).write_bytes(
-                    data + b"\n"
+                self.artifacts_dir.joinpath(FileNames.META.value).write_text(
+                    self.run_meta.json() + "\n"
                 )
                 self.logger.info(f"Stored artifacts at {self.artifacts_dir}")
 
         if args.hooks:
-            code = exit_code.value if isinstance(exit_code, ExitCodes) else exit_code
-            self.run_hook(HookVariant.POST, args, code)
+            self.run_hook(HookVariant.POST, args, exit_code)
 
         if self._lock_file_fd is not None:
             self._release_flock()
 
         return exit_code
 
 
@@ -421,15 +424,15 @@
     def run(self, args: Namespace) -> int:
         self.setup(args)
         try:
             self.main(args)
         finally:
             self.teardown(args)
 
-        return ExitCodes.SUCCESS
+        return exitcode.OK
 
 
 class AsyncScript(BaseCommand, ABC):
     """AsyncScript is a base class for a asyncronous gallia command.
     To implement an async script, create a subclass and implement
     the .main() method."""
 
@@ -450,15 +453,15 @@
         try:
             await self.main(args)
         finally:
             await self.teardown(args)
 
     def run(self, args: Namespace) -> int:
         asyncio.run(self._run(args))
-        return ExitCodes.SUCCESS
+        return exitcode.OK
 
 
 class Scanner(AsyncScript, ABC):
     """Scanner is a base class for all scanning related commands.
     A scanner has the following properties:
 
     - It is async.
@@ -496,25 +499,28 @@
         if args.db is not None:
             self.db_handler = DBHandler(args.db)
             await self.db_handler.connect()
 
             await self.db_handler.insert_run_meta(
                 script=sys.argv[0].split()[-1],
                 arguments=sys.argv[1:],
+                command_meta=msgspec.json.encode(self.run_meta.command_meta),
+                settings=dump_args(args),
                 start_time=datetime.now(timezone.utc).astimezone(),
                 path=self.artifacts_dir,
             )
 
     async def _db_finish_run_meta(self, args: Namespace, exit_code: int) -> None:
         if self.db_handler is not None and self.db_handler.connection is not None:
             if self.db_handler.meta is not None:
                 try:
                     await self.db_handler.complete_run_meta(
                         datetime.now(timezone.utc).astimezone(),
                         exit_code,
+                        self.artifacts_dir,
                     )
                 except Exception as e:
                     self.logger.warning(
                         f"Could not write the run meta to the database: {e!r}"
                     )
 
             try:
```

### Comparing `gallia-1.1.4/src/gallia/command/uds.py` & `gallia-1.2.0/src/gallia/command/uds.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/commands/__init__.py` & `gallia-1.2.0/src/gallia/commands/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from gallia.commands.primitive.uds.iocbi import IOCBIPrimitive
 from gallia.commands.primitive.uds.ping import PingPrimitive
 from gallia.commands.primitive.uds.read_by_identifier import ReadByIdentifierPrimitive
 from gallia.commands.primitive.uds.read_error_log import ReadErrorLogPrimitive
 from gallia.commands.primitive.uds.rmba import RMBAPrimitive
 from gallia.commands.primitive.uds.rtcl import RTCLPrimitive
 from gallia.commands.primitive.uds.send_pdu import SendPDUPrimitive
+from gallia.commands.primitive.uds.test_xcp import SimpleTestXCP
 from gallia.commands.primitive.uds.vin import VINPrimitive
 from gallia.commands.primitive.uds.wmba import WMBAPrimitive
 from gallia.commands.primitive.uds.write_by_identifier import WriteByIdentifierPrimitive
 from gallia.commands.scan.uds.identifiers import ScanIdentifiers
 from gallia.commands.scan.uds.memory import MemoryFunctionsScanner
 from gallia.commands.scan.uds.reset import ResetScanner
 from gallia.commands.scan.uds.sa_dump_seeds import SASeedsDumper
@@ -50,10 +51,11 @@
     RTCLPrimitive,
     ReadErrorLogPrimitive,
     GenericPDUPrimitive,
     SendPDUPrimitive,
     WMBAPrimitive,
     VirtualECU,
     WriteByIdentifierPrimitive,
+    SimpleTestXCP,
 ]
 
-__all__ = list(map(lambda x: x.__name__, registry))
+__all__ = [x.__name__ for x in registry]
```

### Comparing `gallia-1.1.4/src/gallia/commands/discover/find_xcp.py` & `gallia-1.2.0/src/gallia/commands/discover/find_xcp.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 
     async def test_tcp(self, args: Namespace) -> None:
         # TODO: rewrite as async
 
         data = bytes([0xFF, 0x00])
         endpoints = []
         for port in args.tcp_ports.split(","):
-            port = int(port, 0)
+            port = int(port, 0)  # noqa
             self.logger.info(f"Testing TCP port: {port}")
             server = (args.xcp_ip, port)
             self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self.socket.settimeout(0.2)
             try:
                 self.socket.connect(server)
             except Exception as e:
@@ -149,15 +149,15 @@
 
     async def test_udp(self, args: Namespace) -> None:
         # TODO: rewrite as async
 
         data = bytes([0xFF, 0x00])
         endpoints = []
         for port in args.udp_ports.split(","):
-            port = int(port, 0)
+            port = int(port, 0)  # noqa
             self.logger.info(f"Testing UDP port: {port}")
             self.socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
             self.socket.settimeout(0.5)
             server = (args.xcp_ip, port)
             self.socket.sendto(self.pack_xcp_eth(data), server)
             try:
                 _, _, data_ret = self.unpack_xcp_eth(self.socket.recv(1024))
```

### Comparing `gallia-1.1.4/src/gallia/commands/discover/uds/doip.py` & `gallia-1.2.0/src/gallia/commands/discover/uds/doip.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             "--stop",
             metavar="INT",
             type=auto_int,
             default=0xFFFF,
             help="set end address",
         )
 
-    async def probe(
+    async def probe(  # noqa: PLR0913
         self,
         conn: DoIPConnection,
         host: str,
         port: int,
         src_addr: int,
         target_addr: int,
         activation_type: RoutingActivationRequestTypes,
```

### Comparing `gallia-1.1.4/src/gallia/commands/discover/uds/isotp.py` & `gallia-1.2.0/src/gallia/commands/discover/uds/isotp.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/commands/fuzz/uds/pdu.py` & `gallia-1.2.0/src/gallia/commands/fuzz/uds/pdu.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,14 @@
             help="can ids to observe while fuzzing",
         )
 
     def generate_payload(self, args: Namespace) -> bytes:
         return random.randbytes(random.randint(args.min_length, args.max_length))
 
     async def observe_can_messages(self, can_ids: list[int], args: Namespace) -> None:
-
         can_url = args.target.url._replace(scheme=RawCANTransport.SCHEME)
         transport = await RawCANTransport.connect(TargetURI(can_url.geturl()))
         transport.set_filter(can_ids, inv_filter=False)
 
         try:
             can_msgs: dict[int, bytes] = {}
             self.logger.debug("Started observe messages task")
```

### Comparing `gallia-1.1.4/src/gallia/commands/primitive/generic/pdu.py` & `gallia-1.2.0/src/gallia/commands/primitive/generic/pdu.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/commands/primitive/uds/dtc.py` & `gallia-1.2.0/src/gallia/commands/primitive/uds/dtc.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/commands/primitive/uds/ecu_reset.py` & `gallia-1.2.0/src/gallia/commands/primitive/uds/ecu_reset.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/commands/primitive/uds/iocbi.py` & `gallia-1.2.0/src/gallia/commands/primitive/uds/iocbi.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/commands/primitive/uds/ping.py` & `gallia-1.2.0/src/gallia/commands/primitive/uds/ping.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/commands/primitive/uds/read_by_identifier.py` & `gallia-1.2.0/src/gallia/commands/primitive/uds/read_by_identifier.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/commands/primitive/uds/read_error_log.py` & `gallia-1.2.0/src/gallia/commands/primitive/uds/read_error_log.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/commands/primitive/uds/rmba.py` & `gallia-1.2.0/src/gallia/commands/primitive/uds/rmba.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/commands/primitive/uds/rtcl.py` & `gallia-1.2.0/src/gallia/commands/primitive/uds/rtcl.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/commands/primitive/uds/send_pdu.py` & `gallia-1.2.0/src/gallia/commands/primitive/uds/send_pdu.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/commands/primitive/uds/vin.py` & `gallia-1.2.0/src/gallia/commands/primitive/uds/vin.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/commands/primitive/uds/wmba.py` & `gallia-1.2.0/src/gallia/commands/primitive/uds/wmba.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/commands/primitive/uds/write_by_identifier.py` & `gallia-1.2.0/src/gallia/commands/primitive/uds/write_by_identifier.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/commands/scan/uds/identifiers.py` & `gallia-1.2.0/src/gallia/commands/scan/uds/identifiers.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,27 +95,27 @@
             help="Stop scanning in session if service seems to be not available",
         )
 
     async def main(self, args: Namespace) -> None:
         if args.sessions is None:
             self.logger.info("No sessions specified, starting with session scan")
             # Only until 0x80 because the eight bit is "SuppressResponse"
-            sessions = list(
+            sessions = [
                 s
                 for s in range(1, 0x80)
                 if s not in args.skip or args.skip[s] is not None
-            )
+            ]
             sessions = await self.ecu.find_sessions(sessions)
             self.logger.result(f"Found {len(sessions)} sessions: {g_repr(sessions)}")
         else:
-            sessions = list(
+            sessions = [
                 s
                 for s in args.sessions
                 if s not in args.skip or args.skip[s] is not None
-            )
+            ]
 
         self.logger.info(f"testing sessions {g_repr(sessions)}")
 
         # TODO: Unified shortened output necessary here
         self.logger.info(f"skipping identifiers {reprlib.repr(args.skip)}")
 
         for session in sessions:
@@ -148,15 +148,15 @@
                 if args.end > 0xFF:
                     self.logger.warning(
                         "Service 0x27 SecurityAccess only accepts subFunctions (1-byte identifiers); "
                         + f"limiting END to {g_repr(0xff)} instead of {g_repr(args.end)}"
                     )
                     args.end = 0xFF
 
-            for (DID, sub_function) in product(
+            for DID, sub_function in product(
                 range(args.start, args.end + 1), sub_functions
             ):
                 if session in args.skip and DID in args.skip[session]:
                     self.logger.info(f"{g_repr(DID)}: skipped")
                     continue
 
                 if args.check_session and DID % args.check_session == 0:
```

### Comparing `gallia-1.1.4/src/gallia/commands/scan/uds/memory.py` & `gallia-1.2.0/src/gallia/commands/scan/uds/memory.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/commands/scan/uds/reset.py` & `gallia-1.2.0/src/gallia/commands/scan/uds/reset.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,34 +59,34 @@
         l_ok: dict[int, list[int]] = {}
         l_timeout: dict[int, list[int]] = {}
         l_error: dict[int, list[Any]] = {}
 
         if args.sessions is None:
             self.logger.info("No sessions specified, starting with session scan")
             # Only until 0x80 because the eight bit is "SuppressResponse"
-            sessions = list(
+            sessions = [
                 s
                 for s in range(1, 0x80)
                 if s not in args.skip or args.skip[s] is not None
-            )
+            ]
             sessions = await self.ecu.find_sessions(sessions)
             self.logger.result(f"Found {len(sessions)} sessions: {g_repr(sessions)}")
         else:
-            sessions = list(
+            sessions = [
                 s
                 for s in args.sessions
                 if s not in args.skip or args.skip[s] is not None
-            )
+            ]
 
         self.logger.info(f"testing sessions {g_repr(sessions)}")
 
         # TODO: Unified shortened output necessary here
         self.logger.info(f"skipping identifiers {reprlib.repr(args.skip)}")
 
-        for session in sessions:  # pylint: disable=too-many-nested-blocks
+        for session in sessions:
             self.logger.notice(f"Switching to session {g_repr(session)}")
             resp: UDSResponse = await self.ecu.set_session(session)
             if isinstance(resp, NegativeResponse):
                 self.logger.warning(
                     f"Switching to session {g_repr(session)} failed: {resp}"
                 )
                 continue
```

### Comparing `gallia-1.1.4/src/gallia/commands/scan/uds/sa_dump_seeds.py` & `gallia-1.2.0/src/gallia/commands/scan/uds/sa_dump_seeds.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/commands/scan/uds/services.py` & `gallia-1.2.0/src/gallia/commands/scan/uds/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,27 +83,27 @@
     async def main(self, args: Namespace) -> None:
         self.ecu.max_retry = 1
         found: dict[int, dict[int, Any]] = {}
 
         if args.sessions is None:
             self.logger.info("No sessions specified, starting with session scan")
             # Only until 0x80 because the eight bit is "SuppressResponse"
-            sessions = list(
+            sessions = [
                 s
                 for s in range(1, 0x80)
                 if s not in args.skip or args.skip[s] is not None
-            )
+            ]
             sessions = await self.ecu.find_sessions(sessions)
             self.logger.result(f"Found {len(sessions)} sessions: {g_repr(sessions)}")
         else:
-            sessions = list(
+            sessions = [
                 s
                 for s in args.sessions
                 if s not in args.skip or args.skip[s] is not None
-            )
+            ]
 
         self.logger.info(f"testing sessions {g_repr(sessions)}")
 
         # TODO: Unified shortened output necessary here
         self.logger.info(f"skipping identifiers {reprlib.repr(args.skip)}")
 
         for session in sessions:
```

### Comparing `gallia-1.1.4/src/gallia/commands/scan/uds/sessions.py` & `gallia-1.2.0/src/gallia/commands/scan/uds/sessions.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,14 @@
         negative_results: list[dict[str, Any]] = []
         activated_sessions: set[int] = set()
         search_sessions: list[int] = []
 
         sessions = list(range(1, 0x80))
         depth = 0
 
-        # pylint: disable=too-many-nested-blocks
         while (args.depth is None or depth < args.depth) and len(found[depth]) > 0:
             depth += 1
 
             found[depth] = []
             self.logger.info(f"Depth: {depth}")
 
             for stack in found[depth - 1]:
@@ -229,15 +228,15 @@
                             f"Could not change to session {g_repr(session)}: Timeout"
                         )
                         continue
 
         self.logger.result("Scan finished; Found the following sessions:")
         previous_session = 0
 
-        for res in sorted(positive_results, key=lambda x: x["session"]):  # type: ignore
+        for res in sorted(positive_results, key=lambda x: x["session"]):
             session = res["session"]
 
             if session != previous_session:
                 previous_session = session
                 self.logger.result(f"* Session {g_repr(session)} ")
 
                 if self.db_handler is not None:
@@ -250,15 +249,15 @@
             )
 
         self.logger.result(
             "The following sessions were identified but could not be activated:"
         )
         previous_session = 0
 
-        for res in sorted(negative_results, key=lambda x: x["session"]):  # type: ignore
+        for res in sorted(negative_results, key=lambda x: x["session"]):
             session = res["session"]
 
             if (
                 session not in activated_sessions
                 and res["error"] != UDSErrorCodes.subFunctionNotSupportedInActiveSession
             ):
                 if session != previous_session:
```

### Comparing `gallia-1.1.4/src/gallia/commands/script/vecu.py` & `gallia-1.2.0/src/gallia/commands/script/vecu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # SPDX-FileCopyrightText: AISEC Pentesting Team
 #
 # SPDX-License-Identifier: Apache-2.0
 
-# pylint: disable=eval-used
-
 import json
 import random
 import sys
 from argparse import Namespace
 from pathlib import Path
 
 from gallia.command import AsyncScript
@@ -80,15 +78,15 @@
         server: UDSServer
 
         if cmd == "db":
             server = DBUDSServer(args.path, args.ecu, args.properties)
         elif cmd == "rng":
             server = RandomUDSServer(args.seed)
         else:
-            assert False
+            raise AssertionError()
 
         for key, value in vars(args).items():
             if key.startswith(dynamic_attr_prefix) and value is not None:
                 setattr(
                     server,
                     key[len(dynamic_attr_prefix) :],
                     eval(
```

### Comparing `gallia-1.1.4/src/gallia/config.py` & `gallia-1.2.0/src/gallia/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 # SPDX-License-Identifier: Apache-2.0
 
 import os
 import sys
 from pathlib import Path
 from typing import Any
 
+from platformdirs import user_config_path
 from pygit2 import discover_repository
 
-from gallia.xdg import xdg_config_dirs
-
 # TODO: Remove this check when dropping Python 3.10.
 if sys.version_info[1] < 11:
     import tomli as tomllib
 else:
     import tomllib
 
 
@@ -42,20 +41,20 @@
         case None:
             return None
 
     raise ValueError(f"unexpected return from pygit2 {res}")
 
 
 def get_config_dirs() -> list[Path]:
-    dirs = xdg_config_dirs()
+    user_conf = user_config_path("gallia")
     git_root = get_git_root()
     cwd = Path.cwd()
     if git_root is not None:
-        return [cwd, git_root] + dirs
-    return [cwd] + dirs
+        return [cwd, git_root, user_conf]
+    return [cwd, user_conf]
 
 
 def search_config(
     filename: Path | None = None,
     extra_paths: list[Path] | None = None,
 ) -> Path | None:
     name = filename if filename is not None else Path("gallia.toml")
```

### Comparing `gallia-1.1.4/src/gallia/db/handler.py` & `gallia-1.2.0/src/gallia/db/handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from gallia.services.uds.core.utils import g_repr
 
 
 def bytes_repr(data: bytes) -> str:
     return bytes_repr_(data, False, None)
 
 
-schema_version = "1.0"
+schema_version = "3"
 
 DB_SCHEMA = f"""
 CREATE TABLE IF NOT EXISTS version (
   schema text unique,
   version text
 );
 CREATE TABLE IF NOT EXISTS ecu (
@@ -46,20 +46,23 @@
   url text not null unique,
   ecu int references ecu(id) on update cascade on delete set null
 );
 CREATE TABLE IF NOT EXISTS run_meta (
   id integer primary key,
   script text not null,
   arguments json not null check(json_valid(arguments)),
+  command_meta json not null check(json_valid(arguments)),
+  settings json not null check(json_valid(arguments)),
   start_time real not null,
   start_timezone text not null,
   end_time real,
   end_timezone text check((end_timezone is null) = (end_time is null)),
   exit_code int,
-  path text
+  path text,
+  exclude BOOLEAN
 );
 CREATE TABLE IF NOT EXISTS error_log (
   level int not null,
   time real not null,
   timezone text not null,
   message text not null,
   meta int references run_meta(id) not null
@@ -187,45 +190,57 @@
         # This could be a much more complex version to support some older version as well
         # Additionally one might bind certain features to this version or trigger a database migration, etc
         if version != schema_version:
             raise ValueError(
                 f"The version of the database schema is not supported! ({version} != {schema_version})"
             )
 
-    async def insert_run_meta(
-        self, script: str, arguments: list[str], start_time: datetime, path: Path
+    async def insert_run_meta(  # noqa: CODE
+        self,
+        script: str,
+        arguments: list[str],
+        command_meta: bytes,
+        settings: dict[str, str | int | float],
+        start_time: datetime,
+        path: Path,
     ) -> None:
         assert self.connection is not None, "Not connected to the database"
 
         query = (
-            "INSERT INTO run_meta(script, arguments, start_time, start_timezone, path) VALUES "
-            "(?, ?, ?, ?, ?)"
+            "INSERT INTO "
+            "run_meta(script, arguments, command_meta, settings, start_time, start_timezone, path, exclude) "
+            "VALUES (?, ?, ?, ?, ?, ?, ?, FALSE)"
         )
         cursor = await self.connection.execute(
             query,
             (
                 script,
                 json.dumps(arguments),
+                command_meta,
+                json.dumps(settings),
                 start_time.timestamp(),
                 start_time.tzname(),
                 str(path),
             ),
         )
 
         self.meta = cursor.lastrowid
 
         await self.connection.commit()
 
-    async def complete_run_meta(self, end_time: datetime, exit_code: int) -> None:
+    async def complete_run_meta(
+        self, end_time: datetime, exit_code: int, path: Path
+    ) -> None:
         assert self.connection is not None, "Not connected to the database"
         assert self.meta is not None, "Run meta not yet created"
 
-        query = "UPDATE run_meta SET end_time = ?, end_timezone = ?, exit_code = ? WHERE id = ?"
+        query = "UPDATE run_meta SET end_time = ?, end_timezone = ?, exit_code = ?, path = ? WHERE id = ?"
         await self.connection.execute(
-            query, (end_time.timestamp(), end_time.tzname(), exit_code, self.meta)
+            query,
+            (end_time.timestamp(), end_time.tzname(), exit_code, str(path), self.meta),
         )
         await self.connection.commit()
 
     async def insert_scan_run(self, target: str) -> None:
         assert self.connection is not None, "Not connected to the database"
         assert self.meta is not None, "Run meta not yet created"
 
@@ -282,15 +297,15 @@
             "INSERT OR IGNORE INTO address(url) VALUES(?)", (target,)
         )
 
         query = "INSERT INTO discovery_result(address, run) VALUES ((SELECT id FROM address WHERE url = ?), ?)"
 
         await self.connection.execute(query, (target, self.discovery_run))
 
-    async def insert_scan_result(
+    async def insert_scan_result(  # noqa: PLR0913
         self,
         state: dict[str, Any],
         request: UDSRequest,
         response: UDSResponse | None,
         exception: Exception | None,
         send_time: datetime,
         receive_time: datetime | None,
@@ -309,44 +324,44 @@
         if isinstance(request, SubFunctionRequest):
             request_attributes["sub_function"] = request.sub_function
 
         for attr, value in request.__dict__.items():
             if not attr.startswith("_"):
                 request_attributes[attr] = value
 
-                if isinstance(value, (bytes, bytearray)):
+                if isinstance(value, bytes | bytearray):
                     request_attributes[attr] = bytes_repr(value)
                 elif (
                     isinstance(value, list)
                     and len(value) > 0
-                    and isinstance(value[0], (bytes, bytearray))
+                    and isinstance(value[0], bytes | bytearray)
                 ):
-                    request_attributes[attr] = list(bytes_repr(v) for v in value)
+                    request_attributes[attr] = [bytes_repr(v) for v in value]
 
         if response is not None:
             response_attributes = {"service_id": response.service_id}
 
             if isinstance(response, PositiveResponse):
                 response_attributes["data"] = bytes_repr(response.data)
 
             if isinstance(response, SubFunctionResponse):
                 response_attributes["sub_function"] = response.sub_function
 
             for attr, value in response.__dict__.items():
                 if not attr.startswith("_") and attr not in ["trigger_request"]:
                     response_attributes[attr] = value
 
-                    if isinstance(value, (bytes, bytearray)):
+                    if isinstance(value, bytes | bytearray):
                         response_attributes[attr] = bytes_repr(value)
                     elif (
                         isinstance(value, list)
                         and len(value) > 0
-                        and isinstance(value[0], (bytes, bytearray))
+                        and isinstance(value[0], bytes | bytearray)
                     ):
-                        response_attributes[attr] = list(bytes_repr(v) for v in value)
+                        response_attributes[attr] = [bytes_repr(v) for v in value]
 
         query = (
             "INSERT INTO scan_result(run, state, request_pdu, request_time, request_timezone, request_data, "
             "response_pdu, response_time, response_timezone, response_data, exception, log_mode) "
             "VALUES(?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)"
         )
 
@@ -409,15 +424,15 @@
             "     address ad "
             "WHERE st.run = sr.id AND sr.address = ad.id "
             "AND ad.url = ?"
         )
         parameters = (self.target,)
 
         cursor: aiosqlite.Cursor = await self.connection.execute(query, parameters)
-        return list(x[0] for x in await cursor.fetchall())
+        return [x[0] for x in await cursor.fetchall()]
 
     async def get_session_transition(self, destination: int) -> list[int] | None:
         assert self.connection is not None, "Not connected to the database"
         assert self.target is not None, "Scan run not yet created, target unknown"
 
         query = (
             "SELECT steps "
```

### Comparing `gallia-1.1.4/src/gallia/dumpcap.py` & `gallia-1.2.0/src/gallia/dumpcap.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from gallia.transports import ISOTPTransport, RawCANTransport, TargetURI
 from gallia.utils import auto_int, split_host_port
 
 
 class Dumpcap:
     BUFSIZE = io.DEFAULT_BUFFER_SIZE
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         proc: subprocess.Process,
         logger: Logger,
         artifacts_dir: Path,
         outfile: Path,
         cleanup: int = 2,
     ) -> None:
```

### Comparing `gallia-1.1.4/src/gallia/log.py` & `gallia-1.2.0/src/gallia/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 import mmap
 import os
 import shutil
 import socket
 import sys
 import tempfile
 import traceback
+from collections.abc import Iterator
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum, IntEnum, unique
 from logging.handlers import QueueHandler, QueueListener
 from pathlib import Path
 from queue import Queue
 from types import TracebackType
-from typing import TYPE_CHECKING, Any, BinaryIO, Iterator, TextIO, cast
+from typing import TYPE_CHECKING, Any, BinaryIO, TextIO, TypeAlias, cast
 
 import msgspec
 import zstandard
 
 if TYPE_CHECKING:
     from logging import _ExcInfoType
 
@@ -53,23 +54,23 @@
 
 def set_color_mode(mode: ColorMode, stream: TextIO = sys.stderr) -> None:
     """Sets the color mode of the console log handler.
 
     :param mode: The available options are described in :class:`ColorMode`.
     :param stream: Used as a reference for :attr:`ColorMode.AUTO`.
     """
-    global _COLORS_ENABLED  # pylint: disable=global-statement
+    global _COLORS_ENABLED  # noqa: PLW0603
     match mode:
         case ColorMode.ALWAYS:
-            _COLORS_ENABLED = True
+            _COLORS_ENABLED = True  # noqa: PLW0603
         case ColorMode.AUTO:
             if os.getenv("NO_COLOR") is not None:
-                _COLORS_ENABLED = False
+                _COLORS_ENABLED = False  # noqa: PLW0603
             else:
-                _COLORS_ENABLED = stream.isatty()
+                _COLORS_ENABLED = stream.isatty()  # noqa: PLW0603
         case ColorMode.NEVER:
             _COLORS_ENABLED = False
 
 
 # https://stackoverflow.com/a/35804945
 def _add_logging_level(level_name: str, level_num: int) -> None:
     method_name = level_name.lower()
@@ -82,15 +83,15 @@
         raise AttributeError(f"{method_name} already defined in logger class")
 
     # This method was inspired by the answers to Stack Overflow post
     # http://stackoverflow.com/q/2183233/2988730, especially
     # http://stackoverflow.com/a/13638084/2988730
     def for_level(self, message, *args, **kwargs):  # type: ignore
         if self.isEnabledFor(level_num):
-            self._log(  # pylint: disable=protected-access
+            self._log(
                 level_num,
                 message,
                 args,
                 **kwargs,
             )
 
     def to_root(message, *args, **kwargs):  # type: ignore
@@ -335,15 +336,15 @@
     line: str | None = None
     stacktrace: str | None = None
     _python_level_no: int | None = None
     _python_level_name: str | None = None
     _python_func_name: str | None = None
 
 
-_PenlogRecord = _PenlogRecordV1 | _PenlogRecordV2
+_PenlogRecord: TypeAlias = _PenlogRecordV1 | _PenlogRecordV2
 
 
 def _colorize_msg(data: str, levelno: int) -> str:
     if not sys.stderr.isatty():
         return data
 
     out = ""
@@ -368,15 +369,15 @@
     out += style
     out += data
     out += _Color.RESET.value
 
     return out
 
 
-def _format_record(
+def _format_record(  # noqa: PLR0913
     dt: datetime,
     name: str,
     data: str,
     levelno: int,
     tags: list[str] | None,
     stacktrace: str | None,
     colored: bool = False,
@@ -440,15 +441,15 @@
     @classmethod
     def parse_json(cls, data: bytes) -> PenlogRecord:
         if data.startswith(b"<"):
             data = data[data.index(b">") + 1 :]
 
         # PenlogRecordV1 has no version field, thus the tagged
         # union based approach does not work.
-        record = _PenlogRecord
+        record: _PenlogRecord
         try:
             record = msgspec.json.decode(data, type=_PenlogRecordV2)
         except msgspec.ValidationError:
             record = msgspec.json.decode(data, type=_PenlogRecordV1)
 
         match record:
             case _PenlogRecordV1():
@@ -484,17 +485,17 @@
                     host=record.host,
                     data=record.data,
                     datetime=datetime.fromisoformat(record.datetime),
                     priority=PenlogPriority(record.priority),
                     tags=record.tags,
                     line=record.line,
                     stacktrace=record.stacktrace,
-                    _python_level_no=record._python_level_no,  # pylint: disable=protected-access
-                    _python_level_name=record._python_level_name,  # pylint: disable=protected-access
-                    _python_func_name=record._python_func_name,  # pylint: disable=protected-access
+                    _python_level_no=record._python_level_no,
+                    _python_level_name=record._python_level_name,
+                    _python_func_name=record._python_func_name,
                 )
         raise ValueError("unknown record version")
 
     def to_log_record(self) -> logging.LogRecord:
         level = self.priority.to_level()
         timestamp = self.datetime.timestamp()
         msecs = (timestamp - int(timestamp)) * 1000
@@ -547,23 +548,23 @@
             match path.suffix:
                 case ".zst":
                     with self.path.open("rb") as f:
                         decomp = zstandard.ZstdDecompressor()
                         decomp.copy_stream(f, tmpfile)
                 case ".gz":
                     with gzip.open(self.path, "rb") as f:
-                        shutil.copyfileobj(f, tmpfile)
+                        shutil.copyfileobj(f, tmpfile)  # type: ignore
 
             tmpfile.flush()
             return cast(BinaryIO, tmpfile)
 
         if path.is_fifo() or self._test_mmap(path) is False:
             tmpfile = tempfile.TemporaryFile()
             with path.open("rb") as f:
-                shutil.copyfileobj(f, tmpfile)
+                shutil.copyfileobj(f, tmpfile)  # type: ignore
             tmpfile.flush()
             return cast(BinaryIO, tmpfile)
 
         return self.path.open("rb")
 
     def _parse_file_structure(self) -> None:
         old_offset = self.file_mmap.tell()
```

### Comparing `gallia-1.1.4/src/gallia/plugins.py` & `gallia-1.2.0/src/gallia/plugins.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # SPDX-FileCopyrightText: AISEC Pentesting Team
 #
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import argparse
+from collections.abc import Callable
 from importlib.metadata import EntryPoint, entry_points
-from typing import TYPE_CHECKING, Callable, TypedDict
+from typing import TYPE_CHECKING, TypedDict
 
 from gallia.services.uds.ecu import ECU
 from gallia.transports import BaseTransport, TargetURI, registry
 
 if TYPE_CHECKING:
     from gallia.command import BaseCommand
 
@@ -119,15 +120,15 @@
     for transport in transports:
         if target.scheme == transport.SCHEME:
             return transport
 
     raise ValueError(f"no transport for {target}")
 
 
-def add_cli_group(
+def add_cli_group(  # noqa: PLR0913
     parent: Parsers,
     group: str,
     help_: str,
     metavar: str,
     description: str | None = None,
     epilog: str | None = None,
 ) -> None:
```

### Comparing `gallia-1.1.4/src/gallia/powersupply.py` & `gallia-1.2.0/src/gallia/powersupply.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 
 from __future__ import annotations
 
 import asyncio
 from collections.abc import Awaitable, Callable
 from functools import partial
 
-from gallia.log import get_logger
-from gallia.transports import TargetURI
 from opennetzteil import netzteile
 from opennetzteil.netzteil import BaseNetzteil
 
+from gallia.log import get_logger
+from gallia.transports import TargetURI
+
 
 class PowerSupplyURI(TargetURI):
     @property
     def id(self) -> int:
         if "id" in self.qs:
             return int(self.qs["id"][0], 0)
         return 0
```

### Comparing `gallia-1.1.4/src/gallia/services/uds/__init__.py` & `gallia-1.2.0/src/gallia/services/uds/__init__.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/services/uds/core/client.py` & `gallia-1.2.0/src/gallia/services/uds/core/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,15 @@
         :param config: Passed on to request_pdu().
         :return: The response of the server.
         """
         return await self.request(
             service.WriteDataByIdentifierRequest(data_identifier, data_record), config
         )
 
-    async def write_memory_by_address(
+    async def write_memory_by_address(  # noqa: PLR0913
         self,
         memory_address: int,
         data_record: bytes,
         memory_size: int | None = None,
         address_and_length_format_identifier: int | None = None,
         config: UDSRequestConfig | None = None,
     ) -> service.NegativeResponse | service.WriteMemoryByAddressResponse:
@@ -798,15 +798,15 @@
         return await self.request(
             service.RequestRoutineResultsRequest(
                 routine_identifier, routine_control_option_record, suppress_response
             ),
             config,
         )
 
-    async def request_download(
+    async def request_download(  # noqa: PLR0913
         self,
         memory_address: int,
         memory_size: int,
         compression_method: int = 0x0,
         encryption_method: int = 0x0,
         address_and_length_format_identifier: int | None = None,
         config: UDSRequestConfig | None = None,
@@ -833,15 +833,15 @@
                 compression_method,
                 encryption_method,
                 address_and_length_format_identifier,
             ),
             config,
         )
 
-    async def request_upload(
+    async def request_upload(  # noqa: PLR0913
         self,
         memory_address: int,
         memory_size: int,
         compression_method: int = 0x0,
         encryption_method: int = 0x0,
         address_and_length_format_identifier: int | None = None,
         config: UDSRequestConfig | None = None,
```

### Comparing `gallia-1.1.4/src/gallia/services/uds/core/constants.py` & `gallia-1.2.0/src/gallia/services/uds/core/constants.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/services/uds/core/exception.py` & `gallia-1.2.0/src/gallia/services/uds/core/exception.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/services/uds/core/service.py` & `gallia-1.2.0/src/gallia/services/uds/core/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # SPDX-FileCopyrightText: AISEC Pentesting Team
 #
 # SPDX-License-Identifier: Apache-2.0
 
-# pylint: disable=too-many-lines, useless-super-delegation
-
 from __future__ import annotations
 
 import inspect
 import struct
 from abc import ABC, abstractmethod
 from collections.abc import Sequence
 from struct import pack
@@ -121,25 +119,23 @@
         return f"{title}({attributes})"
 
     @staticmethod
     def parse_dynamic(pdu: bytes) -> UDSRequest:
         try:
             logger.trace("Dynamically parsing request")
             logger.trace(f" - Got PDU {pdu.hex()}")
-            # pylint: disable=protected-access
             request_service = UDSService._SERVICES[UDSIsoServices(pdu[0])]
 
             logger.trace(f" - Inferred service {request_service.__name__}")
 
             if (request_type := request_service.Request) is not None:
                 logger.trace(f" - Trying {request_type.__name__}")
                 return request_type.from_pdu(pdu)
             if issubclass(request_service, SpecializedSubFunctionService):
                 logger.trace(" - Trying to infer subFunction")
-                # pylint: disable=protected-access
                 request_sub_function = request_service._sub_function_type(pdu)
                 logger.trace(f" - Inferred subFunction {request_sub_function.__name__}")
                 assert (request_type := request_sub_function.Request) is not None
                 logger.trace(f" - Trying {request_type.__name__}")
                 return request_type.from_pdu(pdu)
 
             raise ValueError("Request cannot be parsed")
@@ -223,15 +219,14 @@
 
         response_type: type[PositiveResponse]
 
         logger.trace("Dynamically parsing response")
         logger.trace(f" - Got PDU {pdu.hex()}")
 
         try:
-            # pylint: disable=protected-access
             response_service = UDSService._SERVICES[UDSIsoServices(pdu[0] - 0x40)]
         except Exception:
             logger.trace(
                 " - Falling back to raw response because the service is unknown"
             )
             return RawPositiveResponse(pdu)
 
@@ -243,15 +238,14 @@
             if len(pdu) < 2:
                 raise ValueError(
                     "Message of subfunction service contains no subfunction"
                 )
 
             logger.trace(" - Trying to infer subfunction")
             try:
-                # pylint: disable=protected-access
                 response_sub_function = response_service._sub_function_type(pdu)
             except ValueError as e:
                 logger.trace(f" - Falling back to raw response because {str(e)}")
                 return RawPositiveResponse(pdu)
 
             logger.trace(f" - Inferred subFunction {response_sub_function.__name__}")
             assert (response_type_ := response_sub_function.Response) is not None
@@ -502,17 +496,15 @@
 
 
 class SpecializedSubFunctionResponse(
     SubFunctionResponse, ABC, service_id=None, minimal_length=2, maximal_length=None
 ):
     SUB_FUNCTION_ID: int
 
-    def __init_subclass__(
-        cls, /, sub_function_id: int, **kwargs: Any  # pylint: disable=arguments-differ
-    ) -> None:
+    def __init_subclass__(cls, /, sub_function_id: int, **kwargs: Any) -> None:
         super().__init_subclass__(**kwargs)
 
         cls.SUB_FUNCTION_ID = sub_function_id
 
     def __init__(self) -> None:
         super().__init__()
 
@@ -537,17 +529,15 @@
     service_id=None,
     response_type=SpecializedSubFunctionResponse,  # type: ignore
     minimal_length=2,
     maximal_length=None,
 ):
     SUB_FUNCTION_ID: int
 
-    def __init_subclass__(
-        cls, /, sub_function_id: int, **kwargs: Any  # pylint: disable=arguments-differ
-    ) -> None:
+    def __init_subclass__(cls, /, sub_function_id: int, **kwargs: Any) -> None:
         super().__init_subclass__(**kwargs)
 
         cls.SUB_FUNCTION_ID = sub_function_id
 
     def __init__(self, suppress_response: bool) -> None:
         super().__init__(suppress_response)
 
@@ -3098,15 +3088,15 @@
 class _RequestUpOrDownloadRequest(
     UDSRequest,
     service_id=None,
     response_type=_RequestUpOrDownloadResponse,
     minimal_length=4,
     maximal_length=None,
 ):
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         memory_address: int,
         memory_size: int,
         compression_method: int = 0x0,
         encryption_method: int = 0x0,
         address_and_length_format_identifier: int | None = None,
     ) -> None:
@@ -3181,15 +3171,15 @@
 class RequestDownloadRequest(
     _RequestUpOrDownloadRequest,
     service_id=UDSIsoServices.RequestDownload,
     response_type=RequestDownloadResponse,
     minimal_length=4,
     maximal_length=None,
 ):
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         memory_address: int,
         memory_size: int,
         compression_method: int = 0x0,
         encryption_method: int = 0x0,
         address_and_length_format_identifier: int | None = None,
     ) -> None:
@@ -3237,15 +3227,15 @@
 class RequestUploadRequest(
     _RequestUpOrDownloadRequest,
     service_id=UDSIsoServices.RequestUpload,
     response_type=RequestUploadResponse,
     minimal_length=4,
     maximal_length=None,
 ):
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         memory_address: int,
         memory_size: int,
         compression_method: int = 0x0,
         encryption_method: int = 0x0,
         address_and_length_format_identifier: int | None = None,
     ) -> None:
```

### Comparing `gallia-1.1.4/src/gallia/services/uds/core/utils.py` & `gallia-1.2.0/src/gallia/services/uds/core/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,44 +58,47 @@
     if prefix:
         s = f"0x{s}"
 
     return s
 
 
 def any_repr(x: Any) -> str:
-    if isinstance(x, bool):
-        return repr(x)
-    if isinstance(x, int):
-        return int_repr(x)
-    if isinstance(x, (bytes, bytearray)):
-        return bytes_repr(x)
-    if isinstance(x, list):
-        return f'[{", ".join(any_repr(y) for y in x)}]'
+    match x:
+        case bool():
+            return repr(x)
+        case int():
+            return int_repr(x)
+        case bytes() | bytearray():
+            return bytes_repr(x)
+        case list():
+            return f'[{", ".join(any_repr(y) for y in x)}]'
 
     return str(x)
 
 
 def g_repr(x: Any) -> str:
     """
     Object string representation with default gallia output settings.
     """
-    if isinstance(x, Enum):
-        return str(x.name)
-    if isinstance(x, bool):
-        return repr(x)
-    if isinstance(x, int):
-        return int_repr(x)
-    if isinstance(x, str):
-        return x
-    if isinstance(x, (bytes, bytearray)):
-        return bytes_repr(x)
-    if isinstance(x, list):
-        return f'[{", ".join(g_repr(y) for y in x)}]'
-    if isinstance(x, dict):
-        return f'{{{", ".join(f"{g_repr(k)}: {g_repr(v)}" for k, v in x.items())}}}'
+    match x:
+        case Enum():
+            return str(x.name)
+        case bool():
+            return repr(x)
+        case int():
+            return int_repr(x)
+        case str():
+            return x
+        case bytes() | bytearray():
+            return bytes_repr(x)
+        case list():
+            return f'[{", ".join(g_repr(y) for y in x)}]'
+        case dict():
+            return f'{{{", ".join(f"{g_repr(k)}: {g_repr(v)}" for k, v in x.items())}}}'
+
     # XXX: Avoid the import which causes cyclic imports.
     # TODO: Find out how to replace this helper.
     if type(x).__name__ == "NegativeResponse":
         return str(x)
     return repr(x)
```

### Comparing `gallia-1.1.4/src/gallia/services/uds/ecu.py` & `gallia-1.2.0/src/gallia/services/uds/ecu.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
     def __init__(
         self,
         transport: BaseTransport,
         timeout: float,
         max_retry: int = 1,
         power_supply: PowerSupply | None = None,
     ) -> None:
-
         super().__init__(transport, timeout, max_retry)
         self.logger = get_logger("ecu")
         self.tester_present_task: Task[None] | None = None
         self.tester_present_interval: float | None = None
         self.power_supply = power_supply
         self.state = ECUState()
         self.db_handler: DBHandler | None = None
@@ -216,14 +215,15 @@
             self.logger.debug("no power_supply available")
             return False
 
         async def callback() -> None:
             await self.wait_for_ecu()
 
         await self.power_supply.power_cycle(sleep, callback)
+        self.state.reset()
         return True
 
     async def leave_session(
         self, level: int, config: UDSRequestConfig | None = None
     ) -> bool:
         """leave_session() is a hook which can be called explicitly by a
         scanner when a session is to be disabled. Use this hook if resetting
```

### Comparing `gallia-1.1.4/src/gallia/services/uds/helpers.py` & `gallia-1.2.0/src/gallia/services/uds/helpers.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/services/uds/nrv.py` & `gallia-1.2.0/src/gallia/services/uds/nrv.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/services/uds/server.py` & `gallia-1.2.0/src/gallia/services/uds/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,19 +67,15 @@
 
             return service.NegativeResponse(request.service_id, nrc)
 
         return None
 
     def _is_sub_function_service(self, service_id: int) -> bool:
         try:
-            service_class = (
-                service.UDSService._SERVICES[  # pylint: disable=protected-access
-                    UDSIsoServices(service_id)
-                ]
-            )
+            service_class = service.UDSService._SERVICES[UDSIsoServices(service_id)]
 
             return (
                 issubclass(service_class, service.SpecializedSubFunctionService)
                 or service_class.Request is not None
                 and issubclass(service_class.Request, service.SubFunctionRequest)
             )
         except Exception:
@@ -229,15 +225,14 @@
 
     async def setup(self) -> None:
         pass
 
     async def teardown(self) -> None:
         pass
 
-    # pylint: disable=too-many-return-statements
     async def respond_without_state_change(
         self, request: service.UDSRequest
     ) -> service.UDSResponse | None:
         response: service.UDSResponse | None
 
         if (
             self.use_default_response_if_service_not_supported
@@ -392,15 +387,15 @@
 
         self.logger.notice(f"Initialized random UDS server with seed {self.seed}")
         self.logger.info(
             json.dumps(
                 {
                     int_repr(session): {
                         f"{int_repr(s.value)} ({service_repr(s)})": str(
-                            list(int_repr(sf) for sf in sfs)
+                            [int_repr(sf) for sf in sfs]
                         )
                         if sfs is not None
                         else None
                         for s, sfs in services.items()
                     }
                     for session, services in self.services.items()
                 },
@@ -411,90 +406,92 @@
 
     def randomize(self) -> None:
         rng = RNG(self.seed)
 
         level = 0
         default_session = 1
         level_sessions = {default_session}
-        session_transitions: list[set[int]] = list(set() for _ in range(0x7F))
+        session_transitions: list[set[int]] = [set() for _ in range(0x7F)]
         session_transitions[default_session] = {default_session}
         combined_sessions = self.mandatory_sessions + self.optional_sessions
 
         while len(level_sessions) > 0:
             p_transition = self.p_session / len(level_sessions) / 2 ** (level + 0.5)
             next_level_sessions = set()
-            available_sessions = list(
-                i for i, l in enumerate(session_transitions) if len(l) > 0
-            )
+            available_sessions = [
+                i for i, l in enumerate(session_transitions) if len(l) > 0  # noqa: E741
+            ]
 
             for session in level_sessions:
-                transitions = list(
+                transitions = [
                     session
                     for session in combined_sessions
                     if rng.random() < p_transition
-                )
+                ]
                 session_transitions[session].update(transitions)
                 next_level_sessions.update(transitions)
 
             for session in next_level_sessions:
                 session_transitions[session].add(default_session)
 
             level_sessions = next_level_sessions - set(available_sessions)
             level += 1
 
         for session in self.mandatory_sessions:
             if len(session_transitions[session]) == 0:
-                available_sessions = list(
-                    i for i, l in enumerate(session_transitions) if len(l) > 0
-                )
+                available_sessions = [
+                    i
+                    for i, l in enumerate(session_transitions)  # noqa: E741
+                    if len(l) > 0
+                ]
                 session_transitions[rng.choice(available_sessions)].add(session)
                 session_transitions[session] = {default_session}
 
         self.services = {}
 
         for session, session_specific_transitions in enumerate(session_transitions):
             if len(session_specific_transitions) == 0:
                 continue
 
             self.services[session] = {}
 
-            for supported_service in self.mandatory_services + list(
+            for supported_service in self.mandatory_services + [
                 s for s in self.optional_services if rng.random() < self.p_service
-            ):
+            ]:
                 supported_sub_functions: list[int] | None = None
 
                 if self._is_sub_function_service(supported_service):
                     # For SecurityAccess there are always two consecutive sub functions, the uneven one for RequestSeed,
                     # the even one (+1) for SendKey
                     if supported_service == UDSIsoServices.TesterPresent:
                         supported_sub_functions = [0]
                     elif supported_service == UDSIsoServices.DiagnosticSessionControl:
                         supported_sub_functions = sorted(session_specific_transitions)
                     elif supported_service == UDSIsoServices.SecurityAccess:
-                        supported_sub_functions_tmp = list(
+                        supported_sub_functions_tmp = [
                             sf
                             for sf in range(1, 0x7E, 2)
                             if rng.random() < self.p_sub_function / 2
-                        )
+                        ]
                         supported_sub_functions = []
 
                         for sf in supported_sub_functions_tmp:
                             supported_sub_functions.append(sf)
                             supported_sub_functions.append(sf + 1)
                     elif supported_service == UDSIsoServices.RoutineControl:
-                        supported_sub_functions = list(sf.value for sf in RCSubFuncs)
+                        supported_sub_functions = [sf.value for sf in RCSubFuncs]
                     # Currently only this sub function is supported so it doesn't make sense to gamble a lot here
                     elif supported_service == UDSIsoServices.ReadDTCInformation:
                         supported_sub_functions = [RDTCISubFuncs.RDTCBSM]
                     else:
-                        supported_sub_functions = list(
+                        supported_sub_functions = [
                             sf
                             for sf in range(1, 0x80, 1)
                             if rng.random() < self.p_sub_function
-                        )
+                        ]
 
                 self.services[session][supported_service] = supported_sub_functions
 
     @property
     def supported_services(
         self,
     ) -> dict[int, dict[UDSIsoServices, list[int] | None]]:
@@ -504,26 +501,23 @@
         return RNG(
             str(self.seed)
             + "|"
             + str(self.state.session)
             + "|".join(str(arg) for arg in args)
         )
 
-    # pylint: disable=too-many-return-statements
     async def respond_after_default(
         self, request: service.UDSRequest
     ) -> service.UDSResponse | None:
         # Service specific handling starts here
         # It is assumed, that the service and sub-function, if any, are both supported
         # Furthermore, it is assumed that the request is a valid request for that particular service and sub-function
         if isinstance(request, service.ECUResetRequest):
             return self.ecu_reset(request)
-        if isinstance(
-            request, service._SecurityAccessRequest  # pylint: disable=protected-access
-        ):
+        if isinstance(request, service._SecurityAccessRequest):
             return self.security_access(request)
         if isinstance(request, service.RoutineControlRequest):
             return self.routine_control(request)
         if isinstance(request, service.ReadDataByIdentifierRequest):
             return self.read_data_by_identifier(request)
         if isinstance(request, service.WriteDataByIdentifierRequest):
             return self.write_data_by_identifier(request)
@@ -581,15 +575,15 @@
             if request.security_key == expected_key:
                 return service.SecurityAccessResponse(request.security_access_type)
 
             return service.NegativeResponse(
                 request.service_id, UDSErrorCodes.invalidKey
             )
 
-        assert False
+        raise AssertionError()
 
     def routine_control(
         self, request: service.RoutineControlRequest
     ) -> service.UDSResponse:
         rng = self.stateful_rng(request.service_id, request.routine_identifier)
 
         if not rng.random_bool(self.p_identifier):
@@ -766,25 +760,25 @@
 
         for key, value in self.state.__dict__.items():
             if value is None:
                 query += f"json_extract(r.state, '$.{key}') IS NULL AND "
             else:
                 query += f"json_extract(r.state, '$.{key}') = ? AND "
                 parameters.append(
-                    value if isinstance(value, (int, float)) else json.dumps(value)
+                    value if isinstance(value, int | float) else json.dumps(value)
                 )
 
         if self.properties is not None:
             for key, value in self.properties.items():
                 if value is None:
                     query += f"json_extract(s.properties_pre, '$.{key}') IS NULL AND "
                 else:
                     query += f"json_extract(s.properties_pre, '$.{key}') = ? AND "
                     parameters.append(
-                        value if isinstance(value, (int, float)) else json.dumps(value)
+                        value if isinstance(value, int | float) else json.dumps(value)
                     )
 
         query += "r.request_pdu = ? "
 
         final_query = f"{query} AND r.id > ? ORDER BY r.id LIMIT 1 "
 
         parameters += [bytes_repr(request.pdu, False, None), self.last_response]
```

### Comparing `gallia-1.1.4/src/gallia/services/xcp/__init__.py` & `gallia-1.2.0/src/gallia/services/xcp/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # SPDX-License-Identifier: Apache-2.0
 
 from typing import Any
 
 from gallia.log import get_logger
 from gallia.services.xcp import types
 from gallia.transports import BaseTransport
+from gallia.transports.can import RawCANTransport
 
 
 class XCPService:
     def __init__(self, transport: BaseTransport, timeout: float = 1.0) -> None:
         self.logger = get_logger("xcp")
         self.timeout = timeout
         self.transport = transport
@@ -70,7 +71,42 @@
         self.logger.result(f"XCP GET_ID({id_}) -> OK")
 
     async def upload(self, length: int) -> None:
         self.logger.info(f"XCP GET_UPLOAD({length}")
         resp = await self.request(bytes([0xF5, length]))
         self.logger.info(resp)
         self.logger.result(f"XCP GET_UPLOAD({length} -> OK")
+
+
+class CANXCPSerivce(XCPService):
+    def __init__(
+        self,
+        transport: RawCANTransport,
+        master_id: int,
+        slave_id: int,
+        timeout: float = 1.0,
+    ):
+        self.master_id = master_id
+        self.slave_id = slave_id
+
+        super().__init__(transport, timeout)
+
+    async def request(self, data: bytes, timeout: float | None = None) -> bytes:
+        t = timeout if timeout else self.timeout
+
+        assert isinstance(self.transport, RawCANTransport)
+
+        await self.transport.sendto(data, self.slave_id, t)
+        while True:
+            dst_, resp = await self.transport.recvfrom(t)
+
+            if dst_ == self.master_id:
+                break
+
+        header = types.Response.parse(resp)
+        self.logger.info(header)
+        if int(header.type) != 255:
+            raise ValueError(
+                f"Unknown response type: {header.type}, maybe no XCP packet?"
+            )
+        # strip header byte
+        return resp[1:]
```

### Comparing `gallia-1.1.4/src/gallia/services/xcp/types.py` & `gallia-1.2.0/src/gallia/services/xcp/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
     SYSID = 7
     # Extensions by Vector Informatik.
     VECTOR_MAPNAMES = 0xDB
     VECTOR_MDI = 0xDC
 
 
 class Command(enum.IntEnum):
-
     # STD
 
     # Mandatory Commands
     CONNECT = 0xFF
     DISCONNECT = 0xFE
     GET_STATUS = 0xFD
     SYNCH = 0xFC
```

### Comparing `gallia-1.1.4/src/gallia/transports/__init__.py` & `gallia-1.2.0/src/gallia/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/transports/base.py` & `gallia-1.2.0/src/gallia/transports/base.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/transports/can.py` & `gallia-1.2.0/src/gallia/transports/can.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 from __future__ import annotations
 
 import asyncio
 import errno
 import socket as s
 import struct
 import time
-from typing import cast
 
-from can import Message  # type: ignore
-from pydantic import BaseModel, validator
+from can import Message
+from pydantic import BaseModel, field_validator
 
 from gallia.transports.base import BaseTransport, TargetURI
 from gallia.utils import auto_int
 
 CANFD_MTU = 72
 CAN_MTU = 16
 
@@ -54,22 +53,25 @@
     frame_txtime: int = 10
     ext_address: int | None = None
     rx_ext_address: int | None = None
     tx_padding: int | None = None
     rx_padding: int | None = None
     tx_dl: int = 64
 
-    _auto_int = validator(
+    @field_validator(
         "src_addr",
         "dst_addr",
         "ext_address",
         "rx_ext_address",
-        pre=True,
-        allow_reuse=True,
-    )(auto_int)
+        "tx_padding",
+        "rx_padding",
+        mode="before",
+    )
+    def auto_int(cls, v: str) -> int:
+        return auto_int(v)
 
 
 class ISOTPTransport(BaseTransport, scheme="isotp"):
     def __init__(self, target: TargetURI, config: ISOTPConfig, sock: s.socket) -> None:
         super().__init__(target)
         self._sock = sock
         self.config = config
@@ -109,28 +111,27 @@
         sock.bind((t.hostname, dst_addr, src_addr))
 
         return cls(t, config, sock)
 
     @staticmethod
     def _calc_flags(can_id: int, extended: bool = False) -> int:
         if extended:
-            can_id = can_id & s.CAN_EFF_MASK
-            return can_id | s.CAN_EFF_FLAG
+            return (can_id & s.CAN_EFF_MASK) | s.CAN_EFF_FLAG
         return can_id & s.CAN_SFF_MASK
 
     @staticmethod
-    def _setsockopts(
+    def _setsockopts(  # noqa: PLR0913
         sock: s.socket,
         frame_txtime: int,
         tx_padding: int | None = None,
         rx_padding: int | None = None,
         ext_address: int | None = None,
         rx_ext_address: int | None = None,
-        flags: int = 0,
     ) -> None:
+        flags = 0
         if ext_address is not None:
             flags |= CAN_ISOTP_EXTEND_ADDR
         else:
             ext_address = 0
 
         if rx_ext_address is not None:
             flags |= CAN_ISOTP_RX_EXT_ADDR
@@ -205,23 +206,22 @@
         self.logger.trace(data.hex(), extra={"tags": tags})
         return data
 
     async def close(self) -> None:
         pass
 
 
-class CANMessage(Message):  # type: ignore
-
+class CANMessage(Message):
     # https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/tree/include/uapi/linux/can.h
     CAN_HEADER_FMT = struct.Struct("=IBB2x")
     CANFD_BRS = 0x01
     CANFD_ESI = 0x02
 
     def _compose_arbitration_id(self) -> int:
-        can_id = cast(int, self.arbitration_id)
+        can_id = self.arbitration_id
         if self.is_extended_id:
             can_id |= s.CAN_EFF_FLAG
         if self.is_remote_frame:
             can_id |= s.CAN_RTR_FLAG
         if self.is_error_frame:
             can_id |= s.CAN_ERR_FLAG
         return can_id
@@ -280,19 +280,20 @@
 
 
 class RawCANConfig(BaseModel):
     is_extended: bool = False
     is_fd: bool = False
     dst_id: int | None = None
 
-    _auto_int = validator(
+    @field_validator(
         "dst_id",
-        pre=True,
-        allow_reuse=True,
-    )(auto_int)
+        mode="before",
+    )
+    def auto_int(cls, v: str) -> int:
+        return auto_int(v)
 
 
 class RawCANTransport(BaseTransport, scheme="can-raw"):
     # Flags for setsockopt CAN_RAW_FILTER
     CAN_INV_FILTER = 0x20000000
 
     def __init__(self, target: TargetURI, config: RawCANConfig, sock: s.socket) -> None:
@@ -325,15 +326,15 @@
     def set_filter(self, can_ids: list[int], inv_filter: bool = False) -> None:
         if not can_ids:
             return
         filter_mask = s.CAN_EFF_MASK if self.config.is_extended else s.CAN_SFF_MASK
         data = b""
         for can_id in can_ids:
             if inv_filter:
-                can_id |= self.CAN_INV_FILTER
+                can_id |= self.CAN_INV_FILTER  # noqa: PLW2901
             data += struct.pack("@II", can_id, filter_mask)
         self._sock.setsockopt(s.SOL_CAN_RAW, s.CAN_RAW_FILTER, data)
         if inv_filter:
             self._sock.setsockopt(s.SOL_CAN_RAW, s.CAN_RAW_JOIN_FILTERS, 1)
 
     async def read(
         self,
```

### Comparing `gallia-1.1.4/src/gallia/transports/doip.py` & `gallia-1.2.0/src/gallia/transports/doip.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 from __future__ import annotations
 
 import asyncio
 import struct
 from dataclasses import dataclass
 from enum import IntEnum, unique
 
-from pydantic import BaseModel
+from pydantic import BaseModel, field_validator
 
 from gallia.log import get_logger
 from gallia.transports.base import BaseTransport, TargetURI
+from gallia.utils import auto_int
 
 
 @unique
 class ProtocolVersions(IntEnum):
     ISO_13400_2_2010 = 0x01
     ISO_13400_2_2012 = 0x02
 
@@ -292,15 +293,15 @@
         self.logger = get_logger("doip")
         self.reader = reader
         self.writer = writer
         self.src_addr = src_addr
         self.target_addr = target_addr
         self._read_queue: asyncio.Queue[DoIPFrame] = asyncio.Queue()
         self._read_task = asyncio.create_task(self._read_worker())
-        self._closed = False
+        self._is_closed = False
         self._mutex = asyncio.Lock()
 
     @classmethod
     async def connect(
         cls,
         host: str,
         port: int,
@@ -346,15 +347,15 @@
                 await self._read_queue.put((hdr, data))
         except asyncio.CancelledError:
             self.logger.debug("read worker cancelled")
 
     async def read_frame_unsafe(self) -> DoIPFrame:
         # Avoid waiting on the queue forever when
         # the connection has been terminated.
-        if self._closed:
+        if self._is_closed:
             raise ConnectionError()
         return await self._read_queue.get()
 
     async def read_frame(self) -> DoIPFrame:
         async with self._mutex:
             return await self.read_frame_unsafe()
 
@@ -495,33 +496,50 @@
         )
         payload = AliveCheckResponse(
             SourceAddress=self.src_addr,
         )
         await self.write_request_raw(hdr, payload)
 
     async def close(self) -> None:
+        if self._is_closed:
+            return
+        self._is_closed = True
         self._read_task.cancel()
         self.writer.close()
         await self.writer.wait_closed()
 
 
 class DoIPConfig(BaseModel):
     src_addr: int
     target_addr: int
     activation_type: int = RoutingActivationRequestTypes.WWH_OBD.value
 
+    @field_validator(
+        "src_addr",
+        "target_addr",
+        "activation_type",
+        mode="before",
+    )
+    def auto_int(cls, v: str) -> int:
+        return auto_int(v)
+
 
 class DoIPTransport(BaseTransport, scheme="doip"):
     def __init__(
-        self, target: TargetURI, port: int, config: DoIPConfig, conn: DoIPConnection
+        self,
+        target: TargetURI,
+        port: int,
+        config: DoIPConfig,
+        conn: DoIPConnection,
     ):
         super().__init__(target)
         self.port = port
         self.config = config
         self._conn = conn
+        self._is_closed = False
 
     @staticmethod
     async def _connect(
         hostname: str,
         port: int,
         src_addr: int,
         target_addr: int,
@@ -536,15 +554,17 @@
         await conn.write_routing_activation_request(
             RoutingActivationRequestTypes(activation_type)
         )
         return conn
 
     @classmethod
     async def connect(
-        cls, target: str | TargetURI, timeout: float | None = None
+        cls,
+        target: str | TargetURI,
+        timeout: float | None = None,
     ) -> DoIPTransport:
         t = target if isinstance(target, TargetURI) else TargetURI(target)
         cls.check_scheme(t)
 
         if t.hostname is None:
             raise ValueError("no hostname specified")
 
@@ -559,15 +579,17 @@
                 config.activation_type,
             ),
             timeout,
         )
         return cls(t, port, config, conn)
 
     async def close(self) -> None:
-        self.is_closed = True
+        if self._is_closed:
+            return
+        self._is_closed = True
         await self._conn.close()
 
     async def read(
         self,
         timeout: float | None = None,
         tags: list[str] | None = None,
     ) -> bytes:
@@ -581,10 +603,10 @@
         self,
         data: bytes,
         timeout: float | None = None,
         tags: list[str] | None = None,
     ) -> int:
         await asyncio.wait_for(self._conn.write_diag_request(data), timeout)
 
-        t = tags + ["read"] if tags is not None else ["read"]
+        t = tags + ["write"] if tags is not None else ["write"]
         self.logger.trace(data.hex(), extra={"tags": t})
         return len(data)
```

### Comparing `gallia-1.1.4/src/gallia/transports/tcp.py` & `gallia-1.2.0/src/gallia/transports/tcp.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/src/gallia/utils.py` & `gallia-1.2.0/src/gallia/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,27 +136,28 @@
 
                         for session_id in session_ids:
                             skip_sids[session_id] = None
                     else:
                         session_ids_tmp, identifier_ids_tmp = session_skips.split(":")
                         session_ids = _unravel(session_ids_tmp)
                         identifier_ids = _unravel(identifier_ids_tmp)
+                        skips = session_skips
 
                         for session_id in session_ids:
                             if session_id not in skip_sids:
                                 skip_sids[session_id] = []
 
-                            session_skips = skip_sids[session_id]
+                            skips = skip_sids[session_id]
 
-                            if session_skips is not None:
-                                session_skips += identifier_ids
+                            if skips is not None:
+                                skips += identifier_ids
 
             setattr(namespace, self.dest, skip_sids)
         except Exception as e:
-            raise ArgumentError(self, "The argument is malformed!") from e
+            raise ArgumentError(self, "malformed argument") from e
 
 
 T = TypeVar("T")
 
 
 async def catch_and_log_exception(
     func: Callable[..., Awaitable[T]],
@@ -208,7 +209,17 @@
 
     loader = importlib.util.LazyLoader(spec.loader)
     spec.loader = loader
     module = importlib.util.module_from_spec(spec)
     sys.modules[name] = module
     loader.exec_module(module)
     return module
+
+
+def dump_args(args: Namespace) -> dict[str, str | int | float]:
+    settings = {}
+    for key, value in args.__dict__.items():
+        match value:
+            case str() | int() | float():
+                settings[key] = value
+
+    return settings
```

### Comparing `gallia-1.1.4/src/hr/__init__.py` & `gallia-1.2.0/src/hr/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import argparse
 import sys
 from itertools import islice
 from pathlib import Path
 from typing import cast
 
 import msgspec
-
 from gallia.log import ColorMode, PenlogPriority, PenlogReader, set_color_mode
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser()
     parser.add_argument("FILE", nargs="+", type=Path)
     parser.add_argument(
@@ -58,22 +57,22 @@
     return parser.parse_args()
 
 
 def _main() -> int:
     args = parse_args()
 
     for file in args.FILE:
-        file = cast(Path, file)
-        if not (file.is_file() or file.is_fifo() or file != "-"):
-            print(f"not a regular file: {file}", file=sys.stderr)
+        path = cast(Path, file)
+        if not (path.is_file() or path.is_fifo() or path != "-"):
+            print(f"not a regular file: {path}", file=sys.stderr)
             return 1
 
         set_color_mode(ColorMode(args.color), stream=sys.stdout)
 
-        with PenlogReader(file) as reader:
+        with PenlogReader(path) as reader:
             record_generator = reader.records(args.priority, reverse=args.reverse)
             if args.head:
                 record_generator = islice(record_generator, args.lines)
             elif args.tail:
                 record_generator = reader.records(args.priority, offset=-args.lines)
 
             for record in record_generator:
```

### Comparing `gallia-1.1.4/src/opennetzteil/cli.py` & `gallia-1.2.0/src/opennetzteil/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import sys
 from argparse import ArgumentParser, Namespace
 
 from gallia.command import AsyncScript
 from gallia.config import load_config_file
 from gallia.powersupply import PowerSupplyURI
 from gallia.utils import strtobool
+
 from opennetzteil import netzteile
 
 
 class CLI(AsyncScript):
     COMMAND = "netzteil-cli"
 
     def configure_parser(self) -> None:
```

### Comparing `gallia-1.1.4/src/opennetzteil/devices/http/client.py` & `gallia-1.2.0/src/opennetzteil/devices/http/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 from __future__ import annotations
 
 from typing import Any, cast
 from urllib.parse import urljoin
 
 import aiohttp
-
 from gallia.transports import TargetURI
+
 from opennetzteil.exceptions import OperationNotSupportedError
 from opennetzteil.netzteil import BaseNetzteil
 
 
 class HTTPNetzteil(BaseNetzteil):
     URL_PREFIX = "/_netzteil/api/"
     PRODUCT_ID = "opennetzteil"
 
-    def __init__(  # pylint: disable=super-init-not-called
+    def __init__(
         self,
         session: aiohttp.ClientSession,
         host: str,
         device: int,
     ):
         self.host = host
         self.baseurl = urljoin(host, self.URL_PREFIX)
```

### Comparing `gallia-1.1.4/src/opennetzteil/devices/rs/hmc804.py` & `gallia-1.2.0/src/opennetzteil/devices/rs/hmc804.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from __future__ import annotations
 
 import asyncio
 from typing import Any
 
 from gallia.utils import strtobool
+
 from opennetzteil.exceptions import OperationNotSupportedError
 from opennetzteil.netzteil import BaseNetzteil
 
 
 class HMC804(BaseNetzteil):
     """Rohde&Schwarz power supply: R&S HMC804x
     https://www.rohde-schwarz.com/de/produkte/messtechnik/dc-netzgeraete/rs-hmc804x-dc-netzgeraeteserie_63493-61542.html
@@ -57,16 +58,15 @@
         _, writer = await self._connect()
         for datum in data_list:
             await self._send_line(writer, datum)
         await self._close_conn(writer)
 
     async def get_ident(self) -> str:
         cmd = "*IDN?"
-        resp = await self._request(cmd)
-        return resp
+        return await self._request(cmd)
 
     async def get_master(self) -> bool:
         cmd = "OUTP:MAST:STAT?"
         resp = await self._request(cmd)
         return strtobool(resp)
 
     async def set_master(self, enabled: bool) -> None:
```

### Comparing `gallia-1.1.4/src/opennetzteil/netzteil.py` & `gallia-1.2.0/src/opennetzteil/netzteil.py`

 * *Files identical despite different names*

### Comparing `gallia-1.1.4/PKG-INFO` & `gallia-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gallia
-Version: 1.1.4
+Version: 1.2.0
 Summary: Extendable Pentesting Framework
 Home-page: https://github.com/Fraunhofer-AISEC/gallia
 License: Apache-2.0
 Keywords: pentesting,automotive,uds
 Author: AISEC Pentesting Team
 Maintainer: Stefan Tatschner
 Maintainer-email: stefan.tatschner@aisec.fraunhofer.de
@@ -12,25 +12,27 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiofiles (>=22.1,<23.0)
+Requires-Dist: aiofiles (>=22.1,<24.0)
 Requires-Dist: aiohttp (>=3.8,<4.0)
 Requires-Dist: aiosqlite (>=0.18)
-Requires-Dist: argcomplete (>=2.0,<3.0)
+Requires-Dist: argcomplete (>=2,<4)
 Requires-Dist: construct (>=2.10.67,<3.0.0)
-Requires-Dist: msgspec (>=0.11,<0.13)
-Requires-Dist: pydantic (>=1.10,<2.0)
+Requires-Dist: exitcode (>=0.1.0,<0.2.0)
+Requires-Dist: msgspec (>=0.11,<0.17)
+Requires-Dist: platformdirs (>=2.6,<4.0)
+Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: pygit2 (>=1.10,<2.0)
-Requires-Dist: python-can (>=4.0,<5.0)
+Requires-Dist: python-can (>=4.2,<5.0)
 Requires-Dist: tabulate (>=0.9)
-Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
+Requires-Dist: tomli (>=2.0,<3.0) ; python_version < "3.11"
 Requires-Dist: zstandard (>=0.19)
 Project-URL: Documentation, https://fraunhofer-aisec.github.io/gallia
 Project-URL: Repository, https://github.com/Fraunhofer-AISEC/gallia
 Description-Content-Type: text/markdown
 
 <!--
 SPDX-FileCopyrightText: AISEC Pentesting Team
@@ -42,14 +44,16 @@
 
 [![docs](https://img.shields.io/badge/-docs-green)](https://fraunhofer-aisec.github.io/gallia)
 [![docs](https://readthedocs.org/projects/docs/badge/?version=latest)](https://gallia.readthedocs.io/en/latest)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gallia)](https://pypi.python.org/pypi/gallia/)
 [![PyPI - License](https://img.shields.io/pypi/l/gallia)](https://www.apache.org/licenses/LICENSE-2.0.html)
 [![PyPI](https://img.shields.io/pypi/v/gallia)](https://pypi.python.org/pypi/gallia/)
 
+[![Packaging status](https://repology.org/badge/vertical-allrepos/gallia.svg)](https://repology.org/project/gallia/versions)
+
 Gallia is an extendable pentesting framework with the focus on the automotive domain.
 The scope of the toolchain is conducting penetration tests from a single ECU up to whole cars.
 Currently, the main focus lies on the [UDS](https://www.iso.org/standard/72439.html) interface.
 Acting as a generic interface, the logging functionality implements reproducible tests and enables post-processing tasks.
 The [rendered documentation](https://fraunhofer-aisec.github.io/gallia) is available via Github Pages.
 Alternatively, the documentation is hosted on [readthedocs](https://gallia.readthedocs.io/en/latest) as well.
 The documentation for the current [stable](https://gallia.readthedocs.io/en/stable) realease is available on readthedocs.
```

