# Comparing `tmp/Bubot_Core-0.1.8.tar.gz` & `tmp/Bubot_Core-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bubot_Core-0.1.8.tar", last modified: Sun Mar  5 13:39:03 2023, max compression
+gzip compressed data, was "Bubot_Core-0.1.9.tar", last modified: Tue Mar  7 12:30:05 2023, max compression
```

## Comparing `Bubot_Core-0.1.8.tar` & `Bubot_Core-0.1.9.tar`

### file list

```diff
@@ -1,176 +1,169 @@
-drwxrwxrwx   0        0        0        0 2023-03-05 13:39:03.805680 Bubot_Core-0.1.8/
--rw-rw-rw-   0        0        0     1088 2022-09-02 16:51:13.000000 Bubot_Core-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      733 2023-03-05 13:39:03.804679 Bubot_Core-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      241 2022-10-16 23:19:29.000000 Bubot_Core-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2023-03-05 13:39:03.805680 Bubot_Core-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1220 2022-12-11 14:18:33.000000 Bubot_Core-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-05 13:39:03.204680 Bubot_Core-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-03-05 13:39:03.215681 Bubot_Core-0.1.8/src/Bubot/
-drwxrwxrwx   0        0        0        0 2023-03-05 13:39:03.675678 Bubot_Core-0.1.8/src/Bubot/Core/
--rw-rw-rw-   0        0        0     1505 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/Bubot/Core/BubotHelper.py
-drwxrwxrwx   0        0        0        0 2023-03-05 13:39:03.684680 Bubot_Core-0.1.8/src/Bubot/Core/DataBase/
--rw-rw-rw-   0        0        0     6465 2023-01-21 15:11:29.000000 Bubot_Core-0.1.8/src/Bubot/Core/DataBase/Mongo.py
--rw-rw-rw-   0        0        0     2378 2022-10-17 19:50:04.000000 Bubot_Core-0.1.8/src/Bubot/Core/DataBase/SqlLite.py
--rw-rw-rw-   0        0        0     9868 2022-10-16 12:31:44.000000 Bubot_Core-0.1.8/src/Bubot/Core/DeviceLink.py
--rw-rw-rw-   0        0        0     1038 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/Bubot/Core/DocumentObj.py
-drwxrwxrwx   0        0        0        0 2023-03-05 13:39:03.687681 Bubot_Core-0.1.8/src/Bubot/Core/FastStorage/
--rw-rw-rw-   0        0        0      240 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/Bubot/Core/FastStorage/Simple.py
--rw-rw-rw-   0        0        0      570 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/Bubot/Core/JasperReport.py
--rw-rw-rw-   0        0        0     2138 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/Bubot/Core/Logger.py
--rw-rw-rw-   0        0        0    11165 2023-02-25 13:00:20.000000 Bubot_Core-0.1.8/src/Bubot/Core/Obj.py
--rw-rw-rw-   0        0        0     5071 2023-02-08 21:18:21.000000 Bubot_Core-0.1.8/src/Bubot/Core/ObjApi.py
--rw-rw-rw-   0        0        0     1397 2022-11-21 15:52:53.000000 Bubot_Core-0.1.8/src/Bubot/Core/ObjForm.py
--rw-rw-rw-   0        0        0      747 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/Bubot/Core/ObjModel.py
--rw-rw-rw-   0        0        0      659 2023-02-08 20:10:49.000000 Bubot_Core-0.1.8/src/Bubot/Core/ObjSubtype.py
--rw-rw-rw-   0        0        0      647 2022-10-17 19:50:04.000000 Bubot_Core-0.1.8/src/Bubot/Core/ObjSubtypeApi.py
--rw-rw-rw-   0        0        0    10968 2022-10-16 12:31:21.000000 Bubot_Core-0.1.8/src/Bubot/Core/OcfMessage.py
--rw-rw-rw-   0        0        0      890 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/Bubot/Core/ReportHandler.py
--rw-rw-rw-   0        0        0     1671 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/Bubot/Core/TestHelper.py
--rw-rw-rw-   0        0        0     1500 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/Bubot/Core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-05 13:39:03.707679 Bubot_Core-0.1.8/src/Bubot/Ocf/
--rw-rw-rw-   0        0        0        0 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/Bubot/Ocf/ConnectivityAbstractionLayer.py
--rw-rw-rw-   0        0        0        0 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/Bubot/Ocf/DeviceClient.py
--rw-rw-rw-   0        0        0        0 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/Bubot/Ocf/DeviceServer.py
--rw-rw-rw-   0        0        0     2429 2022-10-17 19:50:04.000000 Bubot_Core-0.1.8/src/Bubot/Ocf/Helper.py
--rw-rw-rw-   0        0        0      455 2022-10-16 12:31:02.000000 Bubot_Core-0.1.8/src/Bubot/Ocf/OcfMessage.py
--rw-rw-rw-   0        0        0        0 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/Bubot/Ocf/PersistentStorage.py
--rw-rw-rw-   0        0        0        0 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/Bubot/Ocf/PolicyEngine.py
--rw-rw-rw-   0        0        0     1070 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/Bubot/Ocf/ResourceLayer.py
--rw-rw-rw-   0        0        0        0 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/Bubot/Ocf/Session.py
--rw-rw-rw-   0        0        0    17107 2022-10-17 19:50:04.000000 Bubot_Core-0.1.8/src/Bubot/Ocf/TransporLayer.py
-drwxrwxrwx   0        0        0        0 2023-03-05 13:39:03.737679 Bubot_Core-0.1.8/src/Bubot/OcfResource/
--rw-rw-rw-   0        0        0     2573 2022-10-16 12:30:40.000000 Bubot_Core-0.1.8/src/Bubot/OcfResource/OcfResource.py
--rw-rw-rw-   0        0        0      643 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/Bubot/OcfResource/OicRAcl2.py
--rw-rw-rw-   0        0        0      641 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/Bubot/OcfResource/OicRCred.py
--rw-rw-rw-   0        0        0     1081 2022-10-16 12:30:35.000000 Bubot_Core-0.1.8/src/Bubot/OcfResource/OicRDoxm.py
--rw-rw-rw-   0        0        0      642 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/Bubot/OcfResource/OicRPstat.py
--rw-rw-rw-   0        0        0      642 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/Bubot/OcfResource/OicRSdi.py
--rw-rw-rw-   0        0        0     2176 2022-10-16 12:30:29.000000 Bubot_Core-0.1.8/src/Bubot/OcfResource/OicWkRes.py
--rw-rw-rw-   0        0        0     1461 2022-09-02 18:33:46.000000 Bubot_Core-0.1.8/src/Bubot/__main__.py
-drwxrwxrwx   0        0        0        0 2023-03-05 13:39:03.200682 Bubot_Core-0.1.8/src/BubotObj/
-drwxrwxrwx   0        0        0        0 2023-03-05 13:39:03.220681 Bubot_Core-0.1.8/src/BubotObj/ObjSchema/
--rw-rw-rw-   0        0        0     2378 2022-10-17 19:50:04.000000 Bubot_Core-0.1.8/src/BubotObj/ObjSchema/ObjSchemaApi.py
-drwxrwxrwx   0        0        0        0 2023-03-05 13:39:03.197681 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/
-drwxrwxrwx   0        0        0        0 2023-03-05 13:39:03.200682 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/
-drwxrwxrwx   0        0        0        0 2023-03-05 13:39:03.230679 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/Console/
--rw-rw-rw-   0        0        0      159 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/Console/Console.json
--rw-rw-rw-   0        0        0     1240 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/Console/Console.py
--rw-rw-rw-   0        0        0       23 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/Console/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-05 13:39:03.257683 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/Device/
--rw-rw-rw-   0        0        0     2331 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/Device/Device.json
--rw-rw-rw-   0        0        0     1436 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/Device/Device.md
--rw-rw-rw-   0        0        0     9824 2022-09-11 06:40:19.000000 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/Device/Device.py
--rw-rw-rw-   0        0        0    13909 2022-10-23 17:16:50.000000 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/Device/DeviceCore.py
--rw-rw-rw-   0        0        0     3787 2022-10-23 17:16:50.000000 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/Device/MainLoopMixin.py
--rw-rw-rw-   0        0        0     1206 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/Device/QueueMixin.py
--rw-rw-rw-   0        0        0       23 2023-03-05 13:38:49.000000 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/Device/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-05 13:39:03.266681 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/EchoDevice/
--rw-rw-rw-   0        0        0       96 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/EchoDevice/EchoDevice.json
--rw-rw-rw-   0        0        0     1606 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/EchoDevice/EchoDevice.py
--rw-rw-rw-   0        0        0       23 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/EchoDevice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-05 13:39:03.268680 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/QueueWorker/
--rw-rw-rw-   0        0        0       96 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/QueueWorker/QueueWorker.json
--rw-rw-rw-   0        0        0      293 2023-02-28 14:52:32.000000 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/QueueWorker/QueueWorker.md
--rw-rw-rw-   0        0        0     1607 2023-02-28 14:52:32.000000 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/QueueWorker/QueueWorker.py
--rw-rw-rw-   0        0        0       23 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/QueueWorker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-05 13:39:03.283679 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/VirtualServer/
--rw-rw-rw-   0        0        0      182 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/VirtualServer/VirtualServer.json
--rw-rw-rw-   0        0        0      459 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/VirtualServer/VirtualServer.md
--rw-rw-rw-   0        0        0     7699 2022-10-17 19:50:04.000000 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/VirtualServer/VirtualServer.py
--rw-rw-rw-   0        0        0       47 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/VirtualServer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-05 13:39:03.201679 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/
-drwxrwxrwx   0        0        0        0 2023-03-05 13:39:03.615682 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/
--rw-rw-rw-   0        0        0      561 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/BuDeviceConfiguration.json
--rw-rw-rw-   0        0        0      561 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/BuSerialPortConfiguration.json
--rw-rw-rw-   0        0        0      142 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/__delete.json
--rw-rw-rw-   0        0        0     1149 2022-10-16 12:29:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/bubot.VirtualServer.con.json
--rw-rw-rw-   0        0        0        6 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/bubot.VirtualServer.mnt.json
--rw-rw-rw-   0        0        0     1323 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/bubot.WebServer.services.json
--rw-rw-rw-   0        0        0     1120 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/bubot.buffer.json
--rw-rw-rw-   0        0        0     1182 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/bubot.con.json
--rw-rw-rw-   0        0        0      769 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/bubot.mnt.json
--rw-rw-rw-   0        0        0      692 2022-09-03 20:12:37.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/bubot.storage.json
--rw-rw-rw-   0        0        0     1985 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.baseResource.json
--rw-rw-rw-   0        0        0     2146 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.baseresource.properties.json
--rw-rw-rw-   0        0        0     1589 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.collection.batch-retrieve.json
--rw-rw-rw-   0        0        0     2274 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.collection.batch-update.json
--rw-rw-rw-   0        0        0    12041 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.collection.json
--rw-rw-rw-   0        0        0      417 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.collection.linkslist.json
--rw-rw-rw-   0        0        0      691 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.common.properties.core.json
--rw-rw-rw-   0        0        0     1447 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.core.json
--rw-rw-rw-   0        0        0     1655 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.core.rw.json
--rw-rw-rw-   0        0        0     4869 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.oic-link.json
--rw-rw-rw-   0        0        0     1367 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.acl.json
--rw-rw-rw-   0        0        0     7723 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.acl2.json
--rw-rw-rw-   0        0        0     1358 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.amacl.json
--rw-rw-rw-   0        0        0      837 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.colour.rgb.json
--rw-rw-rw-   0        0        0     1036 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.cred.json
--rw-rw-rw-   0        0        0      871 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.crl.json
--rw-rw-rw-   0        0        0     2798 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.doxm.json
--rw-rw-rw-   0        0        0     1312 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.icon.json
--rw-rw-rw-   0        0        0      827 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.light.brightness.json
--rw-rw-rw-   0        0        0      720 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.mode-Update.json
--rw-rw-rw-   0        0        0      993 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.mode.json
--rw-rw-rw-   0        0        0     3796 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.openlevel.json
--rw-rw-rw-   0        0        0     2080 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.operational.state.json
--rw-rw-rw-   0        0        0     2646 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.pstat.json
--rw-rw-rw-   0        0        0     1263 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.sacl.json
--rw-rw-rw-   0        0        0     2060 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.sdi.json
--rw-rw-rw-   0        0        0      925 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.svc.json
--rw-rw-rw-   0        0        0      686 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.switch.binary.json
--rw-rw-rw-   0        0        0     1076 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.rd.publish.json
--rw-rw-rw-   0        0        0      856 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.rd.selection.json
--rw-rw-rw-   0        0        0      818 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sceneCollection-Update.json
--rw-rw-rw-   0        0        0     1312 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sceneCollection.json
--rw-rw-rw-   0        0        0     1936 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sceneMember.json
--rw-rw-rw-   0        0        0     3334 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.ace.json
--rw-rw-rw-   0        0        0     2425 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.cred.json
--rw-rw-rw-   0        0        0     1336 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.credtype.json
--rw-rw-rw-   0        0        0     1209 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.crmtype.json
--rw-rw-rw-   0        0        0     1034 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.crudntype.json
--rw-rw-rw-   0        0        0      999 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.didtype.json
--rw-rw-rw-   0        0        0     1085 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.dostype.json
--rw-rw-rw-   0        0        0     1113 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.doxmtype.json
--rw-rw-rw-   0        0        0     1285 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.dpmtype.json
--rw-rw-rw-   0        0        0     1556 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.optdatatype.json
--rw-rw-rw-   0        0        0     1237 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.pomtype.json
--rw-rw-rw-   0        0        0     1527 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.privdatatype.json
--rw-rw-rw-   0        0        0     1387 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.pubdatatype.json
--rw-rw-rw-   0        0        0      965 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.roletype.json
--rw-rw-rw-   0        0        0      936 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.sigtype.json
--rw-rw-rw-   0        0        0     1589 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.svc.json
--rw-rw-rw-   0        0        0     1203 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.svctype.json
--rw-rw-rw-   0        0        0     2211 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.types.json
--rw-rw-rw-   0        0        0     2562 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.con-Update.json
--rw-rw-rw-   0        0        0     2272 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.con.json
--rw-rw-rw-   0        0        0     1462 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.con.p-Update.json
--rw-rw-rw-   0        0        0     1420 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.con.p.json
--rw-rw-rw-   0        0        0     4421 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.d.json
--rw-rw-rw-   0        0        0     2014 2022-09-02 18:34:48.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.introspectionInfo.json
--rw-rw-rw-   0        0        0      863 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.mnt-Update.json
--rw-rw-rw-   0        0        0     1086 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.mnt.json
--rw-rw-rw-   0        0        0      988 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.nmon-Update.json
--rw-rw-rw-   0        0        0     2429 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.nmon.json
--rw-rw-rw-   0        0        0     3350 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.p.json
--rw-rw-rw-   0        0        0      480 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.res-ll.json
--rw-rw-rw-   0        0        0     1426 2022-09-01 18:50:02.000000 Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.res.json
-drwxrwxrwx   0        0        0        0 2023-03-05 13:39:03.748680 Bubot_Core-0.1.8/src/Bubot_Core.egg-info/
--rw-rw-rw-   0        0        0      733 2023-03-05 13:39:03.000000 Bubot_Core-0.1.8/src/Bubot_Core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6639 2023-03-05 13:39:03.000000 Bubot_Core-0.1.8/src/Bubot_Core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-05 13:39:03.000000 Bubot_Core-0.1.8/src/Bubot_Core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-03-05 13:39:03.000000 Bubot_Core-0.1.8/src/Bubot_Core.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-09-02 17:14:32.000000 Bubot_Core-0.1.8/src/Bubot_Core.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       48 2023-03-05 13:39:03.000000 Bubot_Core-0.1.8/src/Bubot_Core.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-03-05 13:39:03.000000 Bubot_Core-0.1.8/src/Bubot_Core.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-05 13:39:03.803681 Bubot_Core-0.1.8/tests/
--rw-rw-rw-   0        0        0    13849 2022-10-16 12:30:01.000000 Bubot_Core-0.1.8/tests/TestDevice.py
--rw-rw-rw-   0        0        0     2733 2022-09-02 16:51:13.000000 Bubot_Core-0.1.8/tests/TestDeviceLink.py
--rw-rw-rw-   0        0        0     4578 2022-09-02 16:51:13.000000 Bubot_Core-0.1.8/tests/TestHelper.py
--rw-rw-rw-   0        0        0     6542 2022-10-16 12:29:48.000000 Bubot_Core-0.1.8/tests/TestIotivityDevice.py
--rw-rw-rw-   0        0        0    16403 2022-09-02 16:51:13.000000 Bubot_Core-0.1.8/tests/TestIotivityServer.py
--rw-rw-rw-   0        0        0      953 2022-09-02 16:51:13.000000 Bubot_Core-0.1.8/tests/TestJsonSchema.py
--rw-rw-rw-   0        0        0     2922 2022-09-02 16:51:13.000000 Bubot_Core-0.1.8/tests/TestLgThingQ.py
--rw-rw-rw-   0        0        0     1281 2022-10-16 12:29:37.000000 Bubot_Core-0.1.8/tests/TestOcfMessage.py
--rw-rw-rw-   0        0        0        0 2022-09-02 16:51:13.000000 Bubot_Core-0.1.8/tests/TestQueueMixin.py
--rw-rw-rw-   0        0        0      768 2022-09-02 16:51:13.000000 Bubot_Core-0.1.8/tests/TestSocket.py
--rw-rw-rw-   0        0        0     3119 2022-09-02 16:51:13.000000 Bubot_Core-0.1.8/tests/TestVirtualServer.py
+drwxrwxrwx   0        0        0        0 2023-03-07 12:30:05.608868 Bubot_Core-0.1.9/
+-rw-rw-rw-   0        0        0     1088 2022-09-02 16:51:13.000000 Bubot_Core-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      733 2023-03-07 12:30:05.607869 Bubot_Core-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2022-10-16 23:19:29.000000 Bubot_Core-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-03-07 12:30:05.608868 Bubot_Core-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2022-12-11 14:18:33.000000 Bubot_Core-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-07 12:30:05.095867 Bubot_Core-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-03-07 12:30:05.105867 Bubot_Core-0.1.9/src/Bubot/
+drwxrwxrwx   0        0        0        0 2023-03-07 12:30:05.495865 Bubot_Core-0.1.9/src/Bubot/Core/
+-rw-rw-rw-   0        0        0     1505 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/Bubot/Core/BubotHelper.py
+drwxrwxrwx   0        0        0        0 2023-03-07 12:30:05.503867 Bubot_Core-0.1.9/src/Bubot/Core/DataBase/
+-rw-rw-rw-   0        0        0     6465 2023-01-21 15:11:29.000000 Bubot_Core-0.1.9/src/Bubot/Core/DataBase/Mongo.py
+-rw-rw-rw-   0        0        0     2378 2022-10-17 19:50:04.000000 Bubot_Core-0.1.9/src/Bubot/Core/DataBase/SqlLite.py
+-rw-rw-rw-   0        0        0     9868 2022-10-16 12:31:44.000000 Bubot_Core-0.1.9/src/Bubot/Core/DeviceLink.py
+-rw-rw-rw-   0        0        0     1038 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/Bubot/Core/DocumentObj.py
+drwxrwxrwx   0        0        0        0 2023-03-07 12:30:05.507867 Bubot_Core-0.1.9/src/Bubot/Core/FastStorage/
+-rw-rw-rw-   0        0        0      240 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/Bubot/Core/FastStorage/Simple.py
+-rw-rw-rw-   0        0        0      570 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/Bubot/Core/JasperReport.py
+-rw-rw-rw-   0        0        0     2138 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/Bubot/Core/Logger.py
+-rw-rw-rw-   0        0        0    11165 2023-02-25 13:00:20.000000 Bubot_Core-0.1.9/src/Bubot/Core/Obj.py
+-rw-rw-rw-   0        0        0     5071 2023-02-08 21:18:21.000000 Bubot_Core-0.1.9/src/Bubot/Core/ObjApi.py
+-rw-rw-rw-   0        0        0     1397 2022-11-21 15:52:53.000000 Bubot_Core-0.1.9/src/Bubot/Core/ObjForm.py
+-rw-rw-rw-   0        0        0      747 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/Bubot/Core/ObjModel.py
+-rw-rw-rw-   0        0        0      659 2023-02-08 20:10:49.000000 Bubot_Core-0.1.9/src/Bubot/Core/ObjSubtype.py
+-rw-rw-rw-   0        0        0      647 2022-10-17 19:50:04.000000 Bubot_Core-0.1.9/src/Bubot/Core/ObjSubtypeApi.py
+-rw-rw-rw-   0        0        0      890 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/Bubot/Core/ReportHandler.py
+-rw-rw-rw-   0        0        0     1671 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/Bubot/Core/TestHelper.py
+-rw-rw-rw-   0        0        0     1500 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/Bubot/Core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-07 12:30:05.521867 Bubot_Core-0.1.9/src/Bubot/Ocf/
+-rw-rw-rw-   0        0        0        0 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/Bubot/Ocf/ConnectivityAbstractionLayer.py
+-rw-rw-rw-   0        0        0        0 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/Bubot/Ocf/DeviceClient.py
+-rw-rw-rw-   0        0        0        0 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/Bubot/Ocf/DeviceServer.py
+-rw-rw-rw-   0        0        0     2429 2022-10-17 19:50:04.000000 Bubot_Core-0.1.9/src/Bubot/Ocf/Helper.py
+-rw-rw-rw-   0        0        0    10968 2022-10-16 12:31:21.000000 Bubot_Core-0.1.9/src/Bubot/Ocf/OcfMessage.py
+-rw-rw-rw-   0        0        0        0 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/Bubot/Ocf/PersistentStorage.py
+-rw-rw-rw-   0        0        0        0 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/Bubot/Ocf/PolicyEngine.py
+-rw-rw-rw-   0        0        0     1070 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/Bubot/Ocf/ResourceLayer.py
+-rw-rw-rw-   0        0        0        0 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/Bubot/Ocf/Session.py
+-rw-rw-rw-   0        0        0    17209 2023-03-07 12:08:52.000000 Bubot_Core-0.1.9/src/Bubot/Ocf/TransporLayer.py
+drwxrwxrwx   0        0        0        0 2023-03-07 12:30:05.548867 Bubot_Core-0.1.9/src/Bubot/OcfResource/
+-rw-rw-rw-   0        0        0     2573 2022-10-16 12:30:40.000000 Bubot_Core-0.1.9/src/Bubot/OcfResource/OcfResource.py
+-rw-rw-rw-   0        0        0      643 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/Bubot/OcfResource/OicRAcl2.py
+-rw-rw-rw-   0        0        0      641 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/Bubot/OcfResource/OicRCred.py
+-rw-rw-rw-   0        0        0     1081 2022-10-16 12:30:35.000000 Bubot_Core-0.1.9/src/Bubot/OcfResource/OicRDoxm.py
+-rw-rw-rw-   0        0        0      642 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/Bubot/OcfResource/OicRPstat.py
+-rw-rw-rw-   0        0        0      642 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/Bubot/OcfResource/OicRSdi.py
+-rw-rw-rw-   0        0        0     2176 2022-10-16 12:30:29.000000 Bubot_Core-0.1.9/src/Bubot/OcfResource/OicWkRes.py
+-rw-rw-rw-   0        0        0     1461 2022-09-02 18:33:46.000000 Bubot_Core-0.1.9/src/Bubot/__main__.py
+drwxrwxrwx   0        0        0        0 2023-03-07 12:30:05.093868 Bubot_Core-0.1.9/src/BubotObj/
+drwxrwxrwx   0        0        0        0 2023-03-07 12:30:05.109867 Bubot_Core-0.1.9/src/BubotObj/ObjSchema/
+-rw-rw-rw-   0        0        0     2378 2022-10-17 19:50:04.000000 Bubot_Core-0.1.9/src/BubotObj/ObjSchema/ObjSchemaApi.py
+drwxrwxrwx   0        0        0        0 2023-03-07 12:30:05.092867 Bubot_Core-0.1.9/src/BubotObj/OcfDevice/
+drwxrwxrwx   0        0        0        0 2023-03-07 12:30:05.093868 Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/
+drwxrwxrwx   0        0        0        0 2023-03-07 12:30:05.120867 Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/Console/
+-rw-rw-rw-   0        0        0      159 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/Console/Console.json
+-rw-rw-rw-   0        0        0     1240 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/Console/Console.py
+-rw-rw-rw-   0        0        0       23 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/Console/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-07 12:30:05.131868 Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/Device/
+-rw-rw-rw-   0        0        0     2331 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/Device/Device.json
+-rw-rw-rw-   0        0        0     1436 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/Device/Device.md
+-rw-rw-rw-   0        0        0     9802 2023-03-07 09:34:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/Device/Device.py
+-rw-rw-rw-   0        0        0    14033 2023-03-07 09:34:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/Device/DeviceCore.py
+-rw-rw-rw-   0        0        0     3787 2022-10-23 17:16:50.000000 Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/Device/MainLoopMixin.py
+-rw-rw-rw-   0        0        0     1206 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/Device/QueueMixin.py
+-rw-rw-rw-   0        0        0       23 2023-03-07 12:28:32.000000 Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/Device/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-07 12:30:05.140868 Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/EchoDevice/
+-rw-rw-rw-   0        0        0       96 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/EchoDevice/EchoDevice.json
+-rw-rw-rw-   0        0        0     1606 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/EchoDevice/EchoDevice.py
+-rw-rw-rw-   0        0        0       23 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/EchoDevice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-07 12:30:05.148867 Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/VirtualServer/
+-rw-rw-rw-   0        0        0      182 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/VirtualServer/VirtualServer.json
+-rw-rw-rw-   0        0        0      459 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/VirtualServer/VirtualServer.md
+-rw-rw-rw-   0        0        0     7800 2023-03-07 11:51:04.000000 Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/VirtualServer/VirtualServer.py
+-rw-rw-rw-   0        0        0       47 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/VirtualServer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-07 12:30:05.093868 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/
+drwxrwxrwx   0        0        0        0 2023-03-07 12:30:05.441867 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/
+-rw-rw-rw-   0        0        0      561 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/BuDeviceConfiguration.json
+-rw-rw-rw-   0        0        0      561 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/BuSerialPortConfiguration.json
+-rw-rw-rw-   0        0        0      142 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/__delete.json
+-rw-rw-rw-   0        0        0     1149 2022-10-16 12:29:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/bubot.VirtualServer.con.json
+-rw-rw-rw-   0        0        0        6 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/bubot.VirtualServer.mnt.json
+-rw-rw-rw-   0        0        0     1323 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/bubot.WebServer.services.json
+-rw-rw-rw-   0        0        0     1120 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/bubot.buffer.json
+-rw-rw-rw-   0        0        0     1182 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/bubot.con.json
+-rw-rw-rw-   0        0        0      769 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/bubot.mnt.json
+-rw-rw-rw-   0        0        0      692 2022-09-03 20:12:37.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/bubot.storage.json
+-rw-rw-rw-   0        0        0     1985 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.baseResource.json
+-rw-rw-rw-   0        0        0     2146 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.baseresource.properties.json
+-rw-rw-rw-   0        0        0     1589 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.collection.batch-retrieve.json
+-rw-rw-rw-   0        0        0     2274 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.collection.batch-update.json
+-rw-rw-rw-   0        0        0    12041 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.collection.json
+-rw-rw-rw-   0        0        0      417 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.collection.linkslist.json
+-rw-rw-rw-   0        0        0      691 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.common.properties.core.json
+-rw-rw-rw-   0        0        0     1447 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.core.json
+-rw-rw-rw-   0        0        0     1655 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.core.rw.json
+-rw-rw-rw-   0        0        0     4869 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.oic-link.json
+-rw-rw-rw-   0        0        0     1367 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.acl.json
+-rw-rw-rw-   0        0        0     7723 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.acl2.json
+-rw-rw-rw-   0        0        0     1358 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.amacl.json
+-rw-rw-rw-   0        0        0      837 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.colour.rgb.json
+-rw-rw-rw-   0        0        0     1036 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.cred.json
+-rw-rw-rw-   0        0        0      871 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.crl.json
+-rw-rw-rw-   0        0        0     2798 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.doxm.json
+-rw-rw-rw-   0        0        0     1312 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.icon.json
+-rw-rw-rw-   0        0        0      827 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.light.brightness.json
+-rw-rw-rw-   0        0        0      720 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.mode-Update.json
+-rw-rw-rw-   0        0        0      993 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.mode.json
+-rw-rw-rw-   0        0        0     3796 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.openlevel.json
+-rw-rw-rw-   0        0        0     2080 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.operational.state.json
+-rw-rw-rw-   0        0        0     2646 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.pstat.json
+-rw-rw-rw-   0        0        0     1263 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.sacl.json
+-rw-rw-rw-   0        0        0     2060 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.sdi.json
+-rw-rw-rw-   0        0        0      925 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.svc.json
+-rw-rw-rw-   0        0        0      686 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.switch.binary.json
+-rw-rw-rw-   0        0        0     1076 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.rd.publish.json
+-rw-rw-rw-   0        0        0      856 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.rd.selection.json
+-rw-rw-rw-   0        0        0      818 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sceneCollection-Update.json
+-rw-rw-rw-   0        0        0     1312 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sceneCollection.json
+-rw-rw-rw-   0        0        0     1936 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sceneMember.json
+-rw-rw-rw-   0        0        0     3334 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.ace.json
+-rw-rw-rw-   0        0        0     2425 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.cred.json
+-rw-rw-rw-   0        0        0     1336 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.credtype.json
+-rw-rw-rw-   0        0        0     1209 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.crmtype.json
+-rw-rw-rw-   0        0        0     1034 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.crudntype.json
+-rw-rw-rw-   0        0        0      999 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.didtype.json
+-rw-rw-rw-   0        0        0     1085 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.dostype.json
+-rw-rw-rw-   0        0        0     1113 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.doxmtype.json
+-rw-rw-rw-   0        0        0     1285 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.dpmtype.json
+-rw-rw-rw-   0        0        0     1556 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.optdatatype.json
+-rw-rw-rw-   0        0        0     1237 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.pomtype.json
+-rw-rw-rw-   0        0        0     1527 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.privdatatype.json
+-rw-rw-rw-   0        0        0     1387 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.pubdatatype.json
+-rw-rw-rw-   0        0        0      965 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.roletype.json
+-rw-rw-rw-   0        0        0      936 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.sigtype.json
+-rw-rw-rw-   0        0        0     1589 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.svc.json
+-rw-rw-rw-   0        0        0     1203 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.svctype.json
+-rw-rw-rw-   0        0        0     2211 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.types.json
+-rw-rw-rw-   0        0        0     2562 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.con-Update.json
+-rw-rw-rw-   0        0        0     2272 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.con.json
+-rw-rw-rw-   0        0        0     1462 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.con.p-Update.json
+-rw-rw-rw-   0        0        0     1420 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.con.p.json
+-rw-rw-rw-   0        0        0     4421 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.d.json
+-rw-rw-rw-   0        0        0     2014 2022-09-02 18:34:48.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.introspectionInfo.json
+-rw-rw-rw-   0        0        0      863 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.mnt-Update.json
+-rw-rw-rw-   0        0        0     1086 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.mnt.json
+-rw-rw-rw-   0        0        0      988 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.nmon-Update.json
+-rw-rw-rw-   0        0        0     2429 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.nmon.json
+-rw-rw-rw-   0        0        0     3350 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.p.json
+-rw-rw-rw-   0        0        0      480 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.res-ll.json
+-rw-rw-rw-   0        0        0     1426 2022-09-01 18:50:02.000000 Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.res.json
+drwxrwxrwx   0        0        0        0 2023-03-07 12:30:05.563868 Bubot_Core-0.1.9/src/Bubot_Core.egg-info/
+-rw-rw-rw-   0        0        0      733 2023-03-07 12:30:05.000000 Bubot_Core-0.1.9/src/Bubot_Core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6355 2023-03-07 12:30:05.000000 Bubot_Core-0.1.9/src/Bubot_Core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-07 12:30:05.000000 Bubot_Core-0.1.9/src/Bubot_Core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-03-07 12:30:05.000000 Bubot_Core-0.1.9/src/Bubot_Core.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-09-02 17:14:32.000000 Bubot_Core-0.1.9/src/Bubot_Core.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       48 2023-03-07 12:30:05.000000 Bubot_Core-0.1.9/src/Bubot_Core.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-03-07 12:30:05.000000 Bubot_Core-0.1.9/src/Bubot_Core.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-07 12:30:05.606867 Bubot_Core-0.1.9/tests/
+-rw-rw-rw-   0        0        0    13849 2022-10-16 12:30:01.000000 Bubot_Core-0.1.9/tests/TestDevice.py
+-rw-rw-rw-   0        0        0     2733 2022-09-02 16:51:13.000000 Bubot_Core-0.1.9/tests/TestDeviceLink.py
+-rw-rw-rw-   0        0        0     4578 2022-09-02 16:51:13.000000 Bubot_Core-0.1.9/tests/TestHelper.py
+-rw-rw-rw-   0        0        0     6542 2022-10-16 12:29:48.000000 Bubot_Core-0.1.9/tests/TestIotivityDevice.py
+-rw-rw-rw-   0        0        0    16403 2022-09-02 16:51:13.000000 Bubot_Core-0.1.9/tests/TestIotivityServer.py
+-rw-rw-rw-   0        0        0      953 2022-09-02 16:51:13.000000 Bubot_Core-0.1.9/tests/TestJsonSchema.py
+-rw-rw-rw-   0        0        0     2922 2022-09-02 16:51:13.000000 Bubot_Core-0.1.9/tests/TestLgThingQ.py
+-rw-rw-rw-   0        0        0     1274 2023-03-07 09:34:02.000000 Bubot_Core-0.1.9/tests/TestOcfMessage.py
+-rw-rw-rw-   0        0        0      768 2022-09-02 16:51:13.000000 Bubot_Core-0.1.9/tests/TestSocket.py
+-rw-rw-rw-   0        0        0     3119 2022-09-02 16:51:13.000000 Bubot_Core-0.1.9/tests/TestVirtualServer.py
```

### Comparing `Bubot_Core-0.1.8/LICENSE` & `Bubot_Core-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/PKG-INFO` & `Bubot_Core-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bubot_Core
-Version: 0.1.8
+Version: 0.1.9
 Summary: iot framework based on OCF specification
 Home-page: https://github.com/businka/Bubot_Core
 Author: Razgovorov Mikhail
 Author-email: 1338833@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Bubot_Core-0.1.8/setup.py` & `Bubot_Core-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/Core/BubotHelper.py` & `Bubot_Core-0.1.9/src/Bubot/Core/BubotHelper.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/Core/DataBase/Mongo.py` & `Bubot_Core-0.1.9/src/Bubot/Core/DataBase/Mongo.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/Core/DataBase/SqlLite.py` & `Bubot_Core-0.1.9/src/Bubot/Core/DataBase/SqlLite.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/Core/DeviceLink.py` & `Bubot_Core-0.1.9/src/Bubot/Core/DeviceLink.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/Core/DocumentObj.py` & `Bubot_Core-0.1.9/src/Bubot/Core/DocumentObj.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/Core/JasperReport.py` & `Bubot_Core-0.1.9/src/Bubot/Core/JasperReport.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/Core/Logger.py` & `Bubot_Core-0.1.9/src/Bubot/Core/Logger.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/Core/Obj.py` & `Bubot_Core-0.1.9/src/Bubot/Core/Obj.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/Core/ObjApi.py` & `Bubot_Core-0.1.9/src/Bubot/Core/ObjApi.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/Core/ObjForm.py` & `Bubot_Core-0.1.9/src/Bubot/Core/ObjForm.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/Core/ObjModel.py` & `Bubot_Core-0.1.9/src/Bubot/Core/ObjModel.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/Core/ObjSubtype.py` & `Bubot_Core-0.1.9/src/Bubot/Core/ObjSubtype.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/Core/ObjSubtypeApi.py` & `Bubot_Core-0.1.9/src/Bubot/Core/ObjSubtypeApi.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/Core/OcfMessage.py` & `Bubot_Core-0.1.9/src/Bubot/Ocf/OcfMessage.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/Core/ReportHandler.py` & `Bubot_Core-0.1.9/src/Bubot/Core/ReportHandler.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/Core/TestHelper.py` & `Bubot_Core-0.1.9/src/Bubot/Core/TestHelper.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/Core/__init__.py` & `Bubot_Core-0.1.9/src/Bubot/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/Ocf/Helper.py` & `Bubot_Core-0.1.9/src/Bubot/Ocf/Helper.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/Ocf/ResourceLayer.py` & `Bubot_Core-0.1.9/src/Bubot/Ocf/ResourceLayer.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/Ocf/TransporLayer.py` & `Bubot_Core-0.1.9/src/Bubot/Ocf/TransporLayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,20 +233,23 @@
             raise ExtException(parent=e)
 
     async def find_resource_by_link(self, link):
         self.device.log.debug('find resource by di {0} href {1}'.format(link.di, link.href))
 
         links = await self.discovery_resource(
             query=dict(di=[link.di], href=[link.href]))
-        if isinstance(links, dict):
-            for di in links:
-                if di == link.di:
-                    for ref in links[di].links:
-                        if ref == link.href:
-                            return links[di].links[ref]
+        if isinstance(links, list):
+            for _link in links:
+                if _link['di'] == link.di:
+
+                    link.data['eps'] = [{'ep'}]
+                    return link
+                    # for ref in links[di].links:
+                    #     if ref == link.href:
+                    #         return links[di].links[ref]
         return None
 
     pass
 
     @property
     def eps_coap_ipv4(self):
         if not self.coap:
```

### Comparing `Bubot_Core-0.1.8/src/Bubot/OcfResource/OcfResource.py` & `Bubot_Core-0.1.9/src/Bubot/OcfResource/OcfResource.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/OcfResource/OicRAcl2.py` & `Bubot_Core-0.1.9/src/Bubot/OcfResource/OicRAcl2.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/OcfResource/OicRCred.py` & `Bubot_Core-0.1.9/src/Bubot/OcfResource/OicRCred.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/OcfResource/OicRDoxm.py` & `Bubot_Core-0.1.9/src/Bubot/OcfResource/OicRDoxm.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/OcfResource/OicRPstat.py` & `Bubot_Core-0.1.9/src/Bubot/OcfResource/OicRPstat.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/OcfResource/OicRSdi.py` & `Bubot_Core-0.1.9/src/Bubot/OcfResource/OicRSdi.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/OcfResource/OicWkRes.py` & `Bubot_Core-0.1.9/src/Bubot/OcfResource/OicWkRes.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot/__main__.py` & `Bubot_Core-0.1.9/src/Bubot/__main__.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/ObjSchema/ObjSchemaApi.py` & `Bubot_Core-0.1.9/src/BubotObj/ObjSchema/ObjSchemaApi.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/Console/Console.py` & `Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/Console/Console.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/Device/Device.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/Device/Device.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/Device/Device.md` & `Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/Device/Device.md`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/Device/Device.py` & `Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/Device/Device.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 """
 
 import asyncio
 import json
 import logging
 import os
 import re
-from os import path
 from typing import TypeVar, Type
 from uuid import uuid4
 
 # from .QueueMixin import QueueMixin
-from Bubot.Core.OcfMessage import OcfRequest
+from Bubot.Ocf.OcfMessage import OcfRequest
 from Bubot.Helpers.ExtException import ExtException, ExtTimeoutError, NotFound
 from Bubot.Helpers.Helper import Helper
 from BubotObj.OcfDevice.subtype.Device.MainLoopMixin import MainLoopMixin
 
 from .__init__ import __version__ as device_version
 
 # _logger = logging.getLogger('OcfDevice')
```

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/Device/DeviceCore.py` & `Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/Device/DeviceCore.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import logging
 import os.path
 from uuid import uuid4
 
 from Bubot.Core.BubotHelper import BubotHelper
 from Bubot.Core.DeviceLink import ResourceLink
-from Bubot.Core.OcfMessage import OcfResponse, OcfRequest
+from Bubot.Ocf.OcfMessage import OcfResponse, OcfRequest
 from Bubot.Helpers.ExtException import ExtException, KeyNotFound
 from Bubot.Helpers.Helper import Helper
 from Bubot.Ocf.ResourceLayer import ResourceLayer
 from Bubot.Ocf.TransporLayer import TransportLayer
 
 
 # self.logger = logging.getLogger('DeviceCore')
@@ -136,14 +136,17 @@
         raise NotImplementedError()
         # listener = self.listener.get(name, [])
         # task = []
         # for device in listener:
         #     task.append(self.send_event_change(name, device))
         # await asyncio.gather(task)
 
+    async def discovery_resource(self, **kwargs):
+        return await self.transport_layer.discovery_resource(**kwargs)
+
     async def send_event_change(self, resource_name, receiver):
         pass
 
     @property
     def link(self):
         return self.get_link()
```

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/Device/MainLoopMixin.py` & `Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/Device/MainLoopMixin.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/Device/QueueMixin.py` & `Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/Device/QueueMixin.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/EchoDevice/EchoDevice.py` & `Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/EchoDevice/EchoDevice.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfDevice/subtype/VirtualServer/VirtualServer.py` & `Bubot_Core-0.1.9/src/BubotObj/OcfDevice/subtype/VirtualServer/VirtualServer.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                 await asyncio.sleep(0.5)
             except asyncio.CancelledError:
                 return
             except Exception as e:
                 import sys, traceback
                 print('Whoops! Problem:', file=sys.stderr)
                 traceback.print_exc(file=sys.stderr)
-            executor.shutdown()
+        executor.shutdown()
 
     async def on_pending(self):
         if multiprocessing.current_process().name == 'MainProcess':
             self.queue = multiprocessing.Queue(-1)
             self.task_logger = self.loop.create_task(self.logger())
 
         links = self.get_param('/oic/con', 'running_devices')
@@ -78,15 +78,15 @@
         except asyncio.CancelledError:
             pass
 
         for di in list(self._running_devices.keys()):
             device = self._running_devices.pop(di)
             self.log.debug(f'Begin cancelled {device.__class__.__name__} {di}')
             if isinstance(device, multiprocessing.Process):
-                res = await self.find_resource_by_link(ResourceLink.init_from_link(dict(di=di, href='/oic/mnt')))
+                res = await self.transport_layer.find_resource_by_link(ResourceLink.init_from_link(dict(di=di, href='/oic/mnt')))
                 await self.request('update', res, dict(currentMachineState='cancelled'))
                 for i in range(15):
                     if not device.is_alive():
                         break
                     self.log.debug('wait cancelled {}'.format(di))
                     await asyncio.sleep(i)
             else:
@@ -155,15 +155,16 @@
         di = link.get('di')
         try:
             class_name = link['dmno']
         except KeyError:
             raise KeyNotFound(detail='dmno', action='action_run_device') from None
         if di and di in self._running_devices:
             raise Exception('device is already running')
-        if class_name == 'VirtualServer':
+        device_class = self.get_device_class(class_name)
+        if issubclass(device_class, VirtualServer):# == 'VirtualServer':
             process = multiprocessing.Process(
                 target=self.device_process,
                 args=(class_name, di, self.queue, dict(path=self.path)),
                 daemon=True
             )
             process.start()
             self._running_devices[link['di']] = process
```

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/BuDeviceConfiguration.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/BuDeviceConfiguration.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/BuSerialPortConfiguration.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/BuSerialPortConfiguration.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/bubot.VirtualServer.con.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/bubot.VirtualServer.con.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/bubot.WebServer.services.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/bubot.WebServer.services.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/bubot.buffer.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/bubot.buffer.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/bubot.con.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/bubot.con.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/bubot.mnt.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/bubot.mnt.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/bubot.storage.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/bubot.storage.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.baseResource.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.baseResource.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.baseresource.properties.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.baseresource.properties.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.collection.batch-retrieve.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.collection.batch-retrieve.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.collection.batch-update.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.collection.batch-update.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.collection.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.collection.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.common.properties.core.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.common.properties.core.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.core.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.core.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.core.rw.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.core.rw.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.oic-link.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.oic-link.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.acl.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.acl.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.acl2.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.acl2.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.amacl.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.amacl.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.colour.rgb.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.colour.rgb.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.cred.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.cred.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.crl.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.crl.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.doxm.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.doxm.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.icon.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.icon.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.light.brightness.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.light.brightness.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.mode-Update.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.mode-Update.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.mode.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.mode.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.openlevel.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.openlevel.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.operational.state.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.operational.state.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.pstat.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.pstat.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.sacl.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.sacl.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.sdi.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.sdi.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.svc.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.svc.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.r.switch.binary.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.r.switch.binary.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.rd.publish.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.rd.publish.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.rd.selection.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.rd.selection.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sceneCollection-Update.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sceneCollection-Update.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sceneCollection.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sceneCollection.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sceneMember.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sceneMember.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.ace.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.ace.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.cred.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.cred.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.credtype.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.credtype.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.crmtype.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.crmtype.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.crudntype.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.crudntype.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.didtype.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.didtype.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.dostype.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.dostype.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.doxmtype.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.doxmtype.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.dpmtype.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.dpmtype.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.optdatatype.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.optdatatype.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.pomtype.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.pomtype.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.privdatatype.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.privdatatype.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.pubdatatype.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.pubdatatype.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.roletype.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.roletype.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.sigtype.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.sigtype.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.svc.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.svc.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.sec.svctype.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.sec.svctype.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.types.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.types.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.con-Update.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.con-Update.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.con.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.con.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.con.p-Update.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.con.p-Update.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.con.p.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.con.p.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.d.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.d.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.introspectionInfo.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.introspectionInfo.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.mnt-Update.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.mnt-Update.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.mnt.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.mnt.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.nmon-Update.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.nmon-Update.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.nmon.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.nmon.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.p.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.p.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/BubotObj/OcfSchema/schema/oic.wk.res.json` & `Bubot_Core-0.1.9/src/BubotObj/OcfSchema/schema/oic.wk.res.json`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/src/Bubot_Core.egg-info/PKG-INFO` & `Bubot_Core-0.1.9/src/Bubot_Core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bubot-Core
-Version: 0.1.8
+Version: 0.1.9
 Summary: iot framework based on OCF specification
 Home-page: https://github.com/businka/Bubot_Core
 Author: Razgovorov Mikhail
 Author-email: 1338833@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Bubot_Core-0.1.8/src/Bubot_Core.egg-info/SOURCES.txt` & `Bubot_Core-0.1.9/src/Bubot_Core.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,14 @@
 src/BubotObj/OcfDevice/subtype/Device/DeviceCore.py
 src/BubotObj/OcfDevice/subtype/Device/MainLoopMixin.py
 src/BubotObj/OcfDevice/subtype/Device/QueueMixin.py
 src/BubotObj/OcfDevice/subtype/Device/__init__.py
 src/BubotObj/OcfDevice/subtype/EchoDevice/EchoDevice.json
 src/BubotObj/OcfDevice/subtype/EchoDevice/EchoDevice.py
 src/BubotObj/OcfDevice/subtype/EchoDevice/__init__.py
-src/BubotObj/OcfDevice/subtype/QueueWorker/QueueWorker.json
-src/BubotObj/OcfDevice/subtype/QueueWorker/QueueWorker.md
-src/BubotObj/OcfDevice/subtype/QueueWorker/QueueWorker.py
-src/BubotObj/OcfDevice/subtype/QueueWorker/__init__.py
 src/BubotObj/OcfDevice/subtype/VirtualServer/VirtualServer.json
 src/BubotObj/OcfDevice/subtype/VirtualServer/VirtualServer.md
 src/BubotObj/OcfDevice/subtype/VirtualServer/VirtualServer.py
 src/BubotObj/OcfDevice/subtype/VirtualServer/__init__.py
 src/BubotObj/OcfSchema/schema/BuDeviceConfiguration.json
 src/BubotObj/OcfSchema/schema/BuSerialPortConfiguration.json
 src/BubotObj/OcfSchema/schema/__delete.json
@@ -105,15 +101,14 @@
 src/Bubot/Core/Logger.py
 src/Bubot/Core/Obj.py
 src/Bubot/Core/ObjApi.py
 src/Bubot/Core/ObjForm.py
 src/Bubot/Core/ObjModel.py
 src/Bubot/Core/ObjSubtype.py
 src/Bubot/Core/ObjSubtypeApi.py
-src/Bubot/Core/OcfMessage.py
 src/Bubot/Core/ReportHandler.py
 src/Bubot/Core/TestHelper.py
 src/Bubot/Core/__init__.py
 src/Bubot/Core/DataBase/Mongo.py
 src/Bubot/Core/DataBase/SqlLite.py
 src/Bubot/Core/FastStorage/Simple.py
 src/Bubot/Ocf/ConnectivityAbstractionLayer.py
@@ -144,10 +139,9 @@
 tests/TestDeviceLink.py
 tests/TestHelper.py
 tests/TestIotivityDevice.py
 tests/TestIotivityServer.py
 tests/TestJsonSchema.py
 tests/TestLgThingQ.py
 tests/TestOcfMessage.py
-tests/TestQueueMixin.py
 tests/TestSocket.py
 tests/TestVirtualServer.py
```

### Comparing `Bubot_Core-0.1.8/tests/TestDevice.py` & `Bubot_Core-0.1.9/tests/TestDevice.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/tests/TestDeviceLink.py` & `Bubot_Core-0.1.9/tests/TestDeviceLink.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/tests/TestHelper.py` & `Bubot_Core-0.1.9/tests/TestHelper.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/tests/TestIotivityDevice.py` & `Bubot_Core-0.1.9/tests/TestIotivityDevice.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/tests/TestIotivityServer.py` & `Bubot_Core-0.1.9/tests/TestIotivityServer.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/tests/TestJsonSchema.py` & `Bubot_Core-0.1.9/tests/TestJsonSchema.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/tests/TestLgThingQ.py` & `Bubot_Core-0.1.9/tests/TestLgThingQ.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/tests/TestOcfMessage.py` & `Bubot_Core-0.1.9/tests/TestOcfMessage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from unittest import TestCase
-from Bubot.Core.OcfMessage import OcfRequest, OcfResponse
-from Bubot.Core.Coap.coap import Message, Code
+from Bubot.Ocf.OcfMessage import OcfRequest, OcfResponse
+from Bubot.Core.Coap.coap import Message
 
 
 class TestOcfMessage(TestCase):
     def setUp(self):
         self.link = None
 
     def test_retrieve(self):
```

### Comparing `Bubot_Core-0.1.8/tests/TestSocket.py` & `Bubot_Core-0.1.9/tests/TestSocket.py`

 * *Files identical despite different names*

### Comparing `Bubot_Core-0.1.8/tests/TestVirtualServer.py` & `Bubot_Core-0.1.9/tests/TestVirtualServer.py`

 * *Files identical despite different names*

