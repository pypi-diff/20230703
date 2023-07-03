# Comparing `tmp/mypy-boto3-mediaconvert-1.26.98.tar.gz` & `tmp/mypy-boto3-mediaconvert-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediaconvert-1.26.98.tar", last modified: Thu Mar 23 19:33:06 2023, max compression
+gzip compressed data, was "mypy-boto3-mediaconvert-1.27.0.tar", last modified: Mon Jul  3 19:51:06 2023, max compression
```

## Comparing `mypy-boto3-mediaconvert-1.26.98.tar` & `mypy-boto3-mediaconvert-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:06.811666 mypy-boto3-mediaconvert-1.26.98/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    32943 2023-03-23 19:33:06.803666 mypy-boto3-mediaconvert-1.26.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31436 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:06.795666 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22513 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22473 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    54757 2023-03-23 19:32:21.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    54755 2023-03-23 19:32:21.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   102152 2023-03-23 19:32:24.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   102127 2023-03-23 19:32:23.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:06.803666 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    32943 2023-03-23 19:33:06.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-23 19:33:06.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:06.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:06.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-23 19:33:06.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-23 19:33:06.000000 mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 19:33:06.811666 mypy-boto3-mediaconvert-1.26.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-03-23 19:32:20.000000 mypy-boto3-mediaconvert-1.26.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:06.015640 mypy-boto3-mediaconvert-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:41:49.000000 mypy-boto3-mediaconvert-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    33211 2023-07-03 19:51:06.015640 mypy-boto3-mediaconvert-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31706 2023-07-03 19:41:49.000000 mypy-boto3-mediaconvert-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:06.015640 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-03 19:41:49.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-03 19:41:49.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 19:41:49.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22513 2023-07-03 19:41:50.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22473 2023-07-03 19:41:50.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    55528 2023-07-03 19:41:51.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55526 2023-07-03 19:41:50.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-07-03 19:41:50.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-03 19:41:50.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:41:49.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   103367 2023-07-03 19:41:53.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103342 2023-07-03 19:41:52.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:41:49.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:06.015640 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33211 2023-07-03 19:51:05.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 19:51:05.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:05.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:05.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:05.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:51:05.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:06.015640 mypy-boto3-mediaconvert-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-03 19:41:49.000000 mypy-boto3-mediaconvert-1.27.0/setup.py
```

### Comparing `mypy-boto3-mediaconvert-1.26.98/LICENSE` & `mypy-boto3-mediaconvert-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.26.98/PKG-INFO` & `mypy-boto3-mediaconvert-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediaconvert
-Version: 1.26.98
-Summary: Type annotations for boto3.MediaConvert 1.26.98 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.MediaConvert 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-mediaconvert"></a>
 
 # mypy-boto3-mediaconvert
 
 [![PyPI - mypy-boto3-mediaconvert](https://img.shields.io/pypi/v/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconvert?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConvert 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[boto3.MediaConvert 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mediaconvert docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,14 +325,17 @@
     Ac3DynamicRangeCompressionLineType,
     Ac3DynamicRangeCompressionProfileType,
     Ac3DynamicRangeCompressionRfType,
     Ac3LfeFilterType,
     Ac3MetadataControlType,
     AccelerationModeType,
     AccelerationStatusType,
+    AdvancedInputFilterAddTextureType,
+    AdvancedInputFilterSharpenType,
+    AdvancedInputFilterType,
     AfdSignalingType,
     AlphaBehaviorType,
     AncillaryConvert608To708Type,
     AncillaryTerminateCaptionsType,
     AntiAliasType,
     AudioChannelTagType,
     AudioCodecType,
@@ -368,14 +371,15 @@
     BurninSubtitleBackgroundColorType,
     BurninSubtitleFallbackFontType,
     BurninSubtitleFontColorType,
     BurninSubtitleOutlineColorType,
     BurninSubtitleShadowColorType,
     BurninSubtitleTeletextSpacingType,
     CaptionDestinationTypeType,
+    CaptionSourceConvertPaintOnToPopOnType,
     CaptionSourceTypeType,
     CmafClientCacheType,
     CmafCodecSpecificationType,
     CmafEncryptionTypeType,
     CmafImageBasedTrickPlayType,
     CmafInitializationVectorInManifestType,
     CmafIntervalCadenceType,
@@ -542,14 +546,15 @@
     HlsIntervalCadenceType,
     HlsKeyProviderTypeType,
     HlsManifestCompressionType,
     HlsManifestDurationFormatType,
     HlsOfflineEncryptedType,
     HlsOutputSelectionType,
     HlsProgramDateTimeType,
+    HlsProgressiveWriteHlsManifestType,
     HlsSegmentControlType,
     HlsSegmentLengthControlType,
     HlsStreamInfResolutionType,
     HlsTargetDurationCompatibilityModeType,
     HlsTimedMetadataId3FrameType,
     ImscAccessibilitySubsType,
     ImscStylePassthroughType,
@@ -741,14 +746,15 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediaconvert.type_defs import (
     AacSettingsTypeDef,
     Ac3SettingsTypeDef,
     AccelerationSettingsTypeDef,
+    AdvancedInputFilterSettingsTypeDef,
     AiffSettingsTypeDef,
     AllowedRenditionSizeTypeDef,
     AncillarySourceSettingsTypeDef,
     AssociateCertificateRequestRequestTypeDef,
     AudioChannelTaggingSettingsTypeDef,
     Eac3AtmosSettingsTypeDef,
     Eac3SettingsTypeDef,
@@ -793,24 +799,23 @@
     Hdr10MetadataTypeDef,
     F4vSettingsTypeDef,
     M3u8SettingsTypeDef,
     MovSettingsTypeDef,
     Mp4SettingsTypeDef,
     MpdSettingsTypeDef,
     HopDestinationTypeDef,
-    ResponseMetadataTypeDef,
     ReservationPlanSettingsTypeDef,
     DashAdditionalManifestTypeDef,
     SpekeKeyProviderTypeDef,
     DashIsoImageBasedTrickPlaySettingsTypeDef,
     DeinterlacerTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
     DescribeEndpointsRequestRequestTypeDef,
     EndpointTypeDef,
     DisassociateCertificateRequestRequestTypeDef,
     DolbyVisionLevel6MetadataTypeDef,
     DvbNitSettingsTypeDef,
     DvbSdtSettingsTypeDef,
     DvbTdtSettingsTypeDef,
@@ -839,33 +844,40 @@
     JobMessagesTypeDef,
     KantarWatermarkSettingsTypeDef,
     NielsenConfigurationTypeDef,
     NielsenNonLinearWatermarkSettingsTypeDef,
     TimecodeConfigTypeDef,
     QueueTransitionTypeDef,
     TimingTypeDef,
+    WarningGroupTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ResourceTagsTypeDef,
     M2tsScte35EsamTypeDef,
     MotionImageInsertionFramerateTypeDef,
     MotionImageInsertionOffsetTypeDef,
     Mpeg2SettingsTypeDef,
     MsSmoothAdditionalManifestTypeDef,
     MxfXavcProfileSettingsTypeDef,
     NexGuardFileMarkerSettingsTypeDef,
     NoiseReducerFilterSettingsTypeDef,
     NoiseReducerSpatialFilterSettingsTypeDef,
     NoiseReducerTemporalFilterSettingsTypeDef,
     VideoDetailTypeDef,
+    PaginatorConfigTypeDef,
     ProresSettingsTypeDef,
     ReservationPlanTypeDef,
+    ResponseMetadataTypeDef,
     S3DestinationAccessControlTypeDef,
     S3EncryptionSettingsTypeDef,
     TagResourceRequestRequestTypeDef,
     TimecodeBurninTypeDef,
     UntagResourceRequestRequestTypeDef,
     Vc3SettingsTypeDef,
     Vp8SettingsTypeDef,
@@ -886,19 +898,14 @@
     ColorCorrectorTypeDef,
     VideoSelectorTypeDef,
     CreateQueueRequestRequestTypeDef,
     UpdateQueueRequestRequestTypeDef,
     DashIsoEncryptionSettingsTypeDef,
     HlsEncryptionSettingsTypeDef,
     MsSmoothEncryptionSettingsTypeDef,
-    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
-    ListPresetsRequestListPresetsPaginateTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
     DescribeEndpointsResponseTypeDef,
     DolbyVisionTypeDef,
     EsamSettingsTypeDef,
     GetPolicyResponseTypeDef,
     PutPolicyRequestRequestTypeDef,
     PutPolicyResponseTypeDef,
     H264SettingsTypeDef,
```

### Comparing `mypy-boto3-mediaconvert-1.26.98/README.md` & `mypy-boto3-mediaconvert-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-mediaconvert"></a>
 
 # mypy-boto3-mediaconvert
 
 [![PyPI - mypy-boto3-mediaconvert](https://img.shields.io/pypi/v/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconvert?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConvert 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[boto3.MediaConvert 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mediaconvert docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/).
 
 See how it helps to find and fix potential bugs:
 
@@ -293,14 +293,17 @@
     Ac3DynamicRangeCompressionLineType,
     Ac3DynamicRangeCompressionProfileType,
     Ac3DynamicRangeCompressionRfType,
     Ac3LfeFilterType,
     Ac3MetadataControlType,
     AccelerationModeType,
     AccelerationStatusType,
+    AdvancedInputFilterAddTextureType,
+    AdvancedInputFilterSharpenType,
+    AdvancedInputFilterType,
     AfdSignalingType,
     AlphaBehaviorType,
     AncillaryConvert608To708Type,
     AncillaryTerminateCaptionsType,
     AntiAliasType,
     AudioChannelTagType,
     AudioCodecType,
@@ -336,14 +339,15 @@
     BurninSubtitleBackgroundColorType,
     BurninSubtitleFallbackFontType,
     BurninSubtitleFontColorType,
     BurninSubtitleOutlineColorType,
     BurninSubtitleShadowColorType,
     BurninSubtitleTeletextSpacingType,
     CaptionDestinationTypeType,
+    CaptionSourceConvertPaintOnToPopOnType,
     CaptionSourceTypeType,
     CmafClientCacheType,
     CmafCodecSpecificationType,
     CmafEncryptionTypeType,
     CmafImageBasedTrickPlayType,
     CmafInitializationVectorInManifestType,
     CmafIntervalCadenceType,
@@ -510,14 +514,15 @@
     HlsIntervalCadenceType,
     HlsKeyProviderTypeType,
     HlsManifestCompressionType,
     HlsManifestDurationFormatType,
     HlsOfflineEncryptedType,
     HlsOutputSelectionType,
     HlsProgramDateTimeType,
+    HlsProgressiveWriteHlsManifestType,
     HlsSegmentControlType,
     HlsSegmentLengthControlType,
     HlsStreamInfResolutionType,
     HlsTargetDurationCompatibilityModeType,
     HlsTimedMetadataId3FrameType,
     ImscAccessibilitySubsType,
     ImscStylePassthroughType,
@@ -709,14 +714,15 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediaconvert.type_defs import (
     AacSettingsTypeDef,
     Ac3SettingsTypeDef,
     AccelerationSettingsTypeDef,
+    AdvancedInputFilterSettingsTypeDef,
     AiffSettingsTypeDef,
     AllowedRenditionSizeTypeDef,
     AncillarySourceSettingsTypeDef,
     AssociateCertificateRequestRequestTypeDef,
     AudioChannelTaggingSettingsTypeDef,
     Eac3AtmosSettingsTypeDef,
     Eac3SettingsTypeDef,
@@ -761,24 +767,23 @@
     Hdr10MetadataTypeDef,
     F4vSettingsTypeDef,
     M3u8SettingsTypeDef,
     MovSettingsTypeDef,
     Mp4SettingsTypeDef,
     MpdSettingsTypeDef,
     HopDestinationTypeDef,
-    ResponseMetadataTypeDef,
     ReservationPlanSettingsTypeDef,
     DashAdditionalManifestTypeDef,
     SpekeKeyProviderTypeDef,
     DashIsoImageBasedTrickPlaySettingsTypeDef,
     DeinterlacerTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
     DescribeEndpointsRequestRequestTypeDef,
     EndpointTypeDef,
     DisassociateCertificateRequestRequestTypeDef,
     DolbyVisionLevel6MetadataTypeDef,
     DvbNitSettingsTypeDef,
     DvbSdtSettingsTypeDef,
     DvbTdtSettingsTypeDef,
@@ -807,33 +812,40 @@
     JobMessagesTypeDef,
     KantarWatermarkSettingsTypeDef,
     NielsenConfigurationTypeDef,
     NielsenNonLinearWatermarkSettingsTypeDef,
     TimecodeConfigTypeDef,
     QueueTransitionTypeDef,
     TimingTypeDef,
+    WarningGroupTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ResourceTagsTypeDef,
     M2tsScte35EsamTypeDef,
     MotionImageInsertionFramerateTypeDef,
     MotionImageInsertionOffsetTypeDef,
     Mpeg2SettingsTypeDef,
     MsSmoothAdditionalManifestTypeDef,
     MxfXavcProfileSettingsTypeDef,
     NexGuardFileMarkerSettingsTypeDef,
     NoiseReducerFilterSettingsTypeDef,
     NoiseReducerSpatialFilterSettingsTypeDef,
     NoiseReducerTemporalFilterSettingsTypeDef,
     VideoDetailTypeDef,
+    PaginatorConfigTypeDef,
     ProresSettingsTypeDef,
     ReservationPlanTypeDef,
+    ResponseMetadataTypeDef,
     S3DestinationAccessControlTypeDef,
     S3EncryptionSettingsTypeDef,
     TagResourceRequestRequestTypeDef,
     TimecodeBurninTypeDef,
     UntagResourceRequestRequestTypeDef,
     Vc3SettingsTypeDef,
     Vp8SettingsTypeDef,
@@ -854,19 +866,14 @@
     ColorCorrectorTypeDef,
     VideoSelectorTypeDef,
     CreateQueueRequestRequestTypeDef,
     UpdateQueueRequestRequestTypeDef,
     DashIsoEncryptionSettingsTypeDef,
     HlsEncryptionSettingsTypeDef,
     MsSmoothEncryptionSettingsTypeDef,
-    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
-    ListPresetsRequestListPresetsPaginateTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
     DescribeEndpointsResponseTypeDef,
     DolbyVisionTypeDef,
     EsamSettingsTypeDef,
     GetPolicyResponseTypeDef,
     PutPolicyRequestRequestTypeDef,
     PutPolicyResponseTypeDef,
     H264SettingsTypeDef,
```

### Comparing `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/__init__.py` & `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/__init__.pyi` & `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/__main__.py` & `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaConvert 1.26.98\nVersion:         1.26.98\nBuilder"
-        " version: 7.14.2\nDocs:           "
+        "Type annotations for boto3.MediaConvert 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.98")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/client.py` & `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/client.pyi` & `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/literals.py` & `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,17 @@
     "Ac3DynamicRangeCompressionLineType",
     "Ac3DynamicRangeCompressionProfileType",
     "Ac3DynamicRangeCompressionRfType",
     "Ac3LfeFilterType",
     "Ac3MetadataControlType",
     "AccelerationModeType",
     "AccelerationStatusType",
+    "AdvancedInputFilterAddTextureType",
+    "AdvancedInputFilterSharpenType",
+    "AdvancedInputFilterType",
     "AfdSignalingType",
     "AlphaBehaviorType",
     "AncillaryConvert608To708Type",
     "AncillaryTerminateCaptionsType",
     "AntiAliasType",
     "AudioChannelTagType",
     "AudioCodecType",
@@ -75,14 +78,15 @@
     "BurninSubtitleBackgroundColorType",
     "BurninSubtitleFallbackFontType",
     "BurninSubtitleFontColorType",
     "BurninSubtitleOutlineColorType",
     "BurninSubtitleShadowColorType",
     "BurninSubtitleTeletextSpacingType",
     "CaptionDestinationTypeType",
+    "CaptionSourceConvertPaintOnToPopOnType",
     "CaptionSourceTypeType",
     "CmafClientCacheType",
     "CmafCodecSpecificationType",
     "CmafEncryptionTypeType",
     "CmafImageBasedTrickPlayType",
     "CmafInitializationVectorInManifestType",
     "CmafIntervalCadenceType",
@@ -249,14 +253,15 @@
     "HlsIntervalCadenceType",
     "HlsKeyProviderTypeType",
     "HlsManifestCompressionType",
     "HlsManifestDurationFormatType",
     "HlsOfflineEncryptedType",
     "HlsOutputSelectionType",
     "HlsProgramDateTimeType",
+    "HlsProgressiveWriteHlsManifestType",
     "HlsSegmentControlType",
     "HlsSegmentLengthControlType",
     "HlsStreamInfResolutionType",
     "HlsTargetDurationCompatibilityModeType",
     "HlsTimedMetadataId3FrameType",
     "ImscAccessibilitySubsType",
     "ImscStylePassthroughType",
@@ -465,14 +470,17 @@
 Ac3DynamicRangeCompressionRfType = Literal[
     "FILM_LIGHT", "FILM_STANDARD", "MUSIC_LIGHT", "MUSIC_STANDARD", "NONE", "SPEECH"
 ]
 Ac3LfeFilterType = Literal["DISABLED", "ENABLED"]
 Ac3MetadataControlType = Literal["FOLLOW_INPUT", "USE_CONFIGURED"]
 AccelerationModeType = Literal["DISABLED", "ENABLED", "PREFERRED"]
 AccelerationStatusType = Literal["ACCELERATED", "IN_PROGRESS", "NOT_ACCELERATED", "NOT_APPLICABLE"]
+AdvancedInputFilterAddTextureType = Literal["DISABLED", "ENABLED"]
+AdvancedInputFilterSharpenType = Literal["HIGH", "LOW", "OFF"]
+AdvancedInputFilterType = Literal["DISABLED", "ENABLED"]
 AfdSignalingType = Literal["AUTO", "FIXED", "NONE"]
 AlphaBehaviorType = Literal["DISCARD", "REMAP_TO_LUMA"]
 AncillaryConvert608To708Type = Literal["DISABLED", "UPCONVERT"]
 AncillaryTerminateCaptionsType = Literal["DISABLED", "END_OF_INPUT"]
 AntiAliasType = Literal["DISABLED", "ENABLED"]
 AudioChannelTagType = Literal[
     "C", "CS", "L", "LC", "LFE", "LS", "LSD", "R", "RC", "RS", "RSD", "TCS", "VHC", "VHL", "VHR"
@@ -537,14 +545,15 @@
     "SCTE20_PLUS_EMBEDDED",
     "SMI",
     "SRT",
     "TELETEXT",
     "TTML",
     "WEBVTT",
 ]
+CaptionSourceConvertPaintOnToPopOnType = Literal["DISABLED", "ENABLED"]
 CaptionSourceTypeType = Literal[
     "ANCILLARY",
     "DVB_SUB",
     "EMBEDDED",
     "IMSC",
     "NULL_SOURCE",
     "SCC",
@@ -623,15 +632,17 @@
 DashIsoPtsOffsetHandlingForBFramesType = Literal["MATCH_INITIAL_PTS", "ZERO_BASED"]
 DashIsoSegmentControlType = Literal["SEGMENTED_FILES", "SINGLE_FILE"]
 DashIsoSegmentLengthControlType = Literal["EXACT", "GOP_MULTIPLE"]
 DashIsoVideoCompositionOffsetsType = Literal["SIGNED", "UNSIGNED"]
 DashIsoWriteSegmentTimelineInRepresentationType = Literal["DISABLED", "ENABLED"]
 DashManifestStyleType = Literal["BASIC", "COMPACT", "DISTINCT"]
 DecryptionModeType = Literal["AES_CBC", "AES_CTR", "AES_GCM"]
-DeinterlaceAlgorithmType = Literal["BLEND", "BLEND_TICKER", "INTERPOLATE", "INTERPOLATE_TICKER"]
+DeinterlaceAlgorithmType = Literal[
+    "BLEND", "BLEND_TICKER", "INTERPOLATE", "INTERPOLATE_TICKER", "LINEAR_INTERPOLATION"
+]
 DeinterlacerControlType = Literal["FORCE_ALL_FRAMES", "NORMAL"]
 DeinterlacerModeType = Literal["ADAPTIVE", "DEINTERLACE", "INVERSE_TELECINE"]
 DescribeEndpointsModeType = Literal["DEFAULT", "GET_ONLY"]
 DescribeEndpointsPaginatorName = Literal["describe_endpoints"]
 DolbyVisionLevel6ModeType = Literal["PASSTHROUGH", "RECALCULATE", "SPECIFY"]
 DolbyVisionMappingType = Literal["HDR10_1000", "HDR10_NOMAP"]
 DolbyVisionProfileType = Literal["PROFILE_5", "PROFILE_8_1"]
@@ -820,14 +831,15 @@
 HlsIntervalCadenceType = Literal["FOLLOW_CUSTOM", "FOLLOW_IFRAME"]
 HlsKeyProviderTypeType = Literal["SPEKE", "STATIC_KEY"]
 HlsManifestCompressionType = Literal["GZIP", "NONE"]
 HlsManifestDurationFormatType = Literal["FLOATING_POINT", "INTEGER"]
 HlsOfflineEncryptedType = Literal["DISABLED", "ENABLED"]
 HlsOutputSelectionType = Literal["MANIFESTS_AND_SEGMENTS", "SEGMENTS_ONLY"]
 HlsProgramDateTimeType = Literal["EXCLUDE", "INCLUDE"]
+HlsProgressiveWriteHlsManifestType = Literal["DISABLED", "ENABLED"]
 HlsSegmentControlType = Literal["SEGMENTED_FILES", "SINGLE_FILE"]
 HlsSegmentLengthControlType = Literal["EXACT", "GOP_MULTIPLE"]
 HlsStreamInfResolutionType = Literal["EXCLUDE", "INCLUDE"]
 HlsTargetDurationCompatibilityModeType = Literal["LEGACY", "SPEC_COMPLIANT"]
 HlsTimedMetadataId3FrameType = Literal["NONE", "PRIV", "TDRL"]
 ImscAccessibilitySubsType = Literal["DISABLED", "ENABLED"]
 ImscStylePassthroughType = Literal["DISABLED", "ENABLED"]
@@ -1110,15 +1122,15 @@
 Mpeg2SyntaxType = Literal["DEFAULT", "D_10"]
 Mpeg2TelecineType = Literal["HARD", "NONE", "SOFT"]
 Mpeg2TemporalAdaptiveQuantizationType = Literal["DISABLED", "ENABLED"]
 MsSmoothAudioDeduplicationType = Literal["COMBINE_DUPLICATE_STREAMS", "NONE"]
 MsSmoothFragmentLengthControlType = Literal["EXACT", "GOP_MULTIPLE"]
 MsSmoothManifestEncodingType = Literal["UTF16", "UTF8"]
 MxfAfdSignalingType = Literal["COPY_FROM_VIDEO", "NO_COPY"]
-MxfProfileType = Literal["D_10", "OP1A", "XAVC", "XDCAM"]
+MxfProfileType = Literal["D_10", "OP1A", "XAVC", "XDCAM", "XDCAM_RDD9"]
 MxfXavcDurationModeType = Literal["ALLOW_ANY_DURATION", "DROP_FRAMES_FOR_COMPLIANCE"]
 NielsenActiveWatermarkProcessTypeType = Literal["CBET", "NAES2_AND_NW", "NAES2_AND_NW_AND_CBET"]
 NielsenSourceWatermarkStatusTypeType = Literal["CLEAN", "WATERMARKED"]
 NielsenUniqueTicPerAudioTrackTypeType = Literal[
     "RESERVE_UNIQUE_TICS_PER_TRACK", "SAME_TICS_PER_TRACK"
 ]
 NoiseFilterPostTemporalSharpeningStrengthType = Literal["HIGH", "LOW", "MEDIUM"]
@@ -1233,14 +1245,15 @@
 VideoCodecType = Literal[
     "AV1",
     "AVC_INTRA",
     "FRAME_CAPTURE",
     "H_264",
     "H_265",
     "MPEG2",
+    "PASSTHROUGH",
     "PRORES",
     "VC3",
     "VP8",
     "VP9",
     "XAVC",
 ]
 VideoTimecodeInsertionType = Literal["DISABLED", "PIC_TIMING_SEI"]
@@ -1296,14 +1309,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -1343,14 +1357,15 @@
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
+    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -1492,14 +1507,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -1518,16 +1534,19 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
+    "payment-cryptography",
+    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -1611,15 +1630,17 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/literals.pyi` & `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,17 @@
     "Ac3DynamicRangeCompressionLineType",
     "Ac3DynamicRangeCompressionProfileType",
     "Ac3DynamicRangeCompressionRfType",
     "Ac3LfeFilterType",
     "Ac3MetadataControlType",
     "AccelerationModeType",
     "AccelerationStatusType",
+    "AdvancedInputFilterAddTextureType",
+    "AdvancedInputFilterSharpenType",
+    "AdvancedInputFilterType",
     "AfdSignalingType",
     "AlphaBehaviorType",
     "AncillaryConvert608To708Type",
     "AncillaryTerminateCaptionsType",
     "AntiAliasType",
     "AudioChannelTagType",
     "AudioCodecType",
@@ -74,14 +77,15 @@
     "BurninSubtitleBackgroundColorType",
     "BurninSubtitleFallbackFontType",
     "BurninSubtitleFontColorType",
     "BurninSubtitleOutlineColorType",
     "BurninSubtitleShadowColorType",
     "BurninSubtitleTeletextSpacingType",
     "CaptionDestinationTypeType",
+    "CaptionSourceConvertPaintOnToPopOnType",
     "CaptionSourceTypeType",
     "CmafClientCacheType",
     "CmafCodecSpecificationType",
     "CmafEncryptionTypeType",
     "CmafImageBasedTrickPlayType",
     "CmafInitializationVectorInManifestType",
     "CmafIntervalCadenceType",
@@ -248,14 +252,15 @@
     "HlsIntervalCadenceType",
     "HlsKeyProviderTypeType",
     "HlsManifestCompressionType",
     "HlsManifestDurationFormatType",
     "HlsOfflineEncryptedType",
     "HlsOutputSelectionType",
     "HlsProgramDateTimeType",
+    "HlsProgressiveWriteHlsManifestType",
     "HlsSegmentControlType",
     "HlsSegmentLengthControlType",
     "HlsStreamInfResolutionType",
     "HlsTargetDurationCompatibilityModeType",
     "HlsTimedMetadataId3FrameType",
     "ImscAccessibilitySubsType",
     "ImscStylePassthroughType",
@@ -463,14 +468,17 @@
 Ac3DynamicRangeCompressionRfType = Literal[
     "FILM_LIGHT", "FILM_STANDARD", "MUSIC_LIGHT", "MUSIC_STANDARD", "NONE", "SPEECH"
 ]
 Ac3LfeFilterType = Literal["DISABLED", "ENABLED"]
 Ac3MetadataControlType = Literal["FOLLOW_INPUT", "USE_CONFIGURED"]
 AccelerationModeType = Literal["DISABLED", "ENABLED", "PREFERRED"]
 AccelerationStatusType = Literal["ACCELERATED", "IN_PROGRESS", "NOT_ACCELERATED", "NOT_APPLICABLE"]
+AdvancedInputFilterAddTextureType = Literal["DISABLED", "ENABLED"]
+AdvancedInputFilterSharpenType = Literal["HIGH", "LOW", "OFF"]
+AdvancedInputFilterType = Literal["DISABLED", "ENABLED"]
 AfdSignalingType = Literal["AUTO", "FIXED", "NONE"]
 AlphaBehaviorType = Literal["DISCARD", "REMAP_TO_LUMA"]
 AncillaryConvert608To708Type = Literal["DISABLED", "UPCONVERT"]
 AncillaryTerminateCaptionsType = Literal["DISABLED", "END_OF_INPUT"]
 AntiAliasType = Literal["DISABLED", "ENABLED"]
 AudioChannelTagType = Literal[
     "C", "CS", "L", "LC", "LFE", "LS", "LSD", "R", "RC", "RS", "RSD", "TCS", "VHC", "VHL", "VHR"
@@ -535,14 +543,15 @@
     "SCTE20_PLUS_EMBEDDED",
     "SMI",
     "SRT",
     "TELETEXT",
     "TTML",
     "WEBVTT",
 ]
+CaptionSourceConvertPaintOnToPopOnType = Literal["DISABLED", "ENABLED"]
 CaptionSourceTypeType = Literal[
     "ANCILLARY",
     "DVB_SUB",
     "EMBEDDED",
     "IMSC",
     "NULL_SOURCE",
     "SCC",
@@ -621,15 +630,17 @@
 DashIsoPtsOffsetHandlingForBFramesType = Literal["MATCH_INITIAL_PTS", "ZERO_BASED"]
 DashIsoSegmentControlType = Literal["SEGMENTED_FILES", "SINGLE_FILE"]
 DashIsoSegmentLengthControlType = Literal["EXACT", "GOP_MULTIPLE"]
 DashIsoVideoCompositionOffsetsType = Literal["SIGNED", "UNSIGNED"]
 DashIsoWriteSegmentTimelineInRepresentationType = Literal["DISABLED", "ENABLED"]
 DashManifestStyleType = Literal["BASIC", "COMPACT", "DISTINCT"]
 DecryptionModeType = Literal["AES_CBC", "AES_CTR", "AES_GCM"]
-DeinterlaceAlgorithmType = Literal["BLEND", "BLEND_TICKER", "INTERPOLATE", "INTERPOLATE_TICKER"]
+DeinterlaceAlgorithmType = Literal[
+    "BLEND", "BLEND_TICKER", "INTERPOLATE", "INTERPOLATE_TICKER", "LINEAR_INTERPOLATION"
+]
 DeinterlacerControlType = Literal["FORCE_ALL_FRAMES", "NORMAL"]
 DeinterlacerModeType = Literal["ADAPTIVE", "DEINTERLACE", "INVERSE_TELECINE"]
 DescribeEndpointsModeType = Literal["DEFAULT", "GET_ONLY"]
 DescribeEndpointsPaginatorName = Literal["describe_endpoints"]
 DolbyVisionLevel6ModeType = Literal["PASSTHROUGH", "RECALCULATE", "SPECIFY"]
 DolbyVisionMappingType = Literal["HDR10_1000", "HDR10_NOMAP"]
 DolbyVisionProfileType = Literal["PROFILE_5", "PROFILE_8_1"]
@@ -818,14 +829,15 @@
 HlsIntervalCadenceType = Literal["FOLLOW_CUSTOM", "FOLLOW_IFRAME"]
 HlsKeyProviderTypeType = Literal["SPEKE", "STATIC_KEY"]
 HlsManifestCompressionType = Literal["GZIP", "NONE"]
 HlsManifestDurationFormatType = Literal["FLOATING_POINT", "INTEGER"]
 HlsOfflineEncryptedType = Literal["DISABLED", "ENABLED"]
 HlsOutputSelectionType = Literal["MANIFESTS_AND_SEGMENTS", "SEGMENTS_ONLY"]
 HlsProgramDateTimeType = Literal["EXCLUDE", "INCLUDE"]
+HlsProgressiveWriteHlsManifestType = Literal["DISABLED", "ENABLED"]
 HlsSegmentControlType = Literal["SEGMENTED_FILES", "SINGLE_FILE"]
 HlsSegmentLengthControlType = Literal["EXACT", "GOP_MULTIPLE"]
 HlsStreamInfResolutionType = Literal["EXCLUDE", "INCLUDE"]
 HlsTargetDurationCompatibilityModeType = Literal["LEGACY", "SPEC_COMPLIANT"]
 HlsTimedMetadataId3FrameType = Literal["NONE", "PRIV", "TDRL"]
 ImscAccessibilitySubsType = Literal["DISABLED", "ENABLED"]
 ImscStylePassthroughType = Literal["DISABLED", "ENABLED"]
@@ -1108,15 +1120,15 @@
 Mpeg2SyntaxType = Literal["DEFAULT", "D_10"]
 Mpeg2TelecineType = Literal["HARD", "NONE", "SOFT"]
 Mpeg2TemporalAdaptiveQuantizationType = Literal["DISABLED", "ENABLED"]
 MsSmoothAudioDeduplicationType = Literal["COMBINE_DUPLICATE_STREAMS", "NONE"]
 MsSmoothFragmentLengthControlType = Literal["EXACT", "GOP_MULTIPLE"]
 MsSmoothManifestEncodingType = Literal["UTF16", "UTF8"]
 MxfAfdSignalingType = Literal["COPY_FROM_VIDEO", "NO_COPY"]
-MxfProfileType = Literal["D_10", "OP1A", "XAVC", "XDCAM"]
+MxfProfileType = Literal["D_10", "OP1A", "XAVC", "XDCAM", "XDCAM_RDD9"]
 MxfXavcDurationModeType = Literal["ALLOW_ANY_DURATION", "DROP_FRAMES_FOR_COMPLIANCE"]
 NielsenActiveWatermarkProcessTypeType = Literal["CBET", "NAES2_AND_NW", "NAES2_AND_NW_AND_CBET"]
 NielsenSourceWatermarkStatusTypeType = Literal["CLEAN", "WATERMARKED"]
 NielsenUniqueTicPerAudioTrackTypeType = Literal[
     "RESERVE_UNIQUE_TICS_PER_TRACK", "SAME_TICS_PER_TRACK"
 ]
 NoiseFilterPostTemporalSharpeningStrengthType = Literal["HIGH", "LOW", "MEDIUM"]
@@ -1231,14 +1243,15 @@
 VideoCodecType = Literal[
     "AV1",
     "AVC_INTRA",
     "FRAME_CAPTURE",
     "H_264",
     "H_265",
     "MPEG2",
+    "PASSTHROUGH",
     "PRORES",
     "VC3",
     "VP8",
     "VP9",
     "XAVC",
 ]
 VideoTimecodeInsertionType = Literal["DISABLED", "PIC_TIMING_SEI"]
@@ -1294,14 +1307,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -1341,14 +1355,15 @@
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
+    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -1490,14 +1505,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -1516,16 +1532,19 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
+    "payment-cryptography",
+    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -1609,15 +1628,17 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/paginator.py` & `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#describeendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Mode: DescribeEndpointsModeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.DescribeEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#describeendpointspaginator)
         """
 
 
@@ -93,15 +93,15 @@
 
     def paginate(
         self,
         *,
         Category: str = ...,
         ListBy: JobTemplateListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listjobtemplatespaginator)
         """
 
 
@@ -113,15 +113,15 @@
 
     def paginate(
         self,
         *,
         Order: OrderType = ...,
         Queue: str = ...,
         Status: JobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listjobspaginator)
         """
 
 
@@ -133,15 +133,15 @@
 
     def paginate(
         self,
         *,
         Category: str = ...,
         ListBy: PresetListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPresetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListPresets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listpresetspaginator)
         """
 
 
@@ -152,13 +152,13 @@
     """
 
     def paginate(
         self,
         *,
         ListBy: QueueListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listqueuespaginator)
         """
```

### Comparing `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/paginator.pyi` & `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#describeendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Mode: DescribeEndpointsModeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.DescribeEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#describeendpointspaginator)
         """
 
 class ListJobTemplatesPaginator(Paginator):
@@ -89,15 +89,15 @@
 
     def paginate(
         self,
         *,
         Category: str = ...,
         ListBy: JobTemplateListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listjobtemplatespaginator)
         """
 
 class ListJobsPaginator(Paginator):
@@ -108,15 +108,15 @@
 
     def paginate(
         self,
         *,
         Order: OrderType = ...,
         Queue: str = ...,
         Status: JobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listjobspaginator)
         """
 
 class ListPresetsPaginator(Paginator):
@@ -127,15 +127,15 @@
 
     def paginate(
         self,
         *,
         Category: str = ...,
         ListBy: PresetListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPresetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListPresets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listpresetspaginator)
         """
 
 class ListQueuesPaginator(Paginator):
@@ -145,13 +145,13 @@
     """
 
     def paginate(
         self,
         *,
         ListBy: QueueListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listqueuespaginator)
         """
```

### Comparing `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/type_defs.py` & `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,17 @@
     Ac3DynamicRangeCompressionLineType,
     Ac3DynamicRangeCompressionProfileType,
     Ac3DynamicRangeCompressionRfType,
     Ac3LfeFilterType,
     Ac3MetadataControlType,
     AccelerationModeType,
     AccelerationStatusType,
+    AdvancedInputFilterAddTextureType,
+    AdvancedInputFilterSharpenType,
+    AdvancedInputFilterType,
     AfdSignalingType,
     AlphaBehaviorType,
     AncillaryConvert608To708Type,
     AncillaryTerminateCaptionsType,
     AntiAliasType,
     AudioChannelTagType,
     AudioCodecType,
@@ -70,14 +73,15 @@
     BurninSubtitleFallbackFontType,
     BurninSubtitleFontColorType,
     BurninSubtitleOutlineColorType,
     BurninSubtitleShadowColorType,
     BurnInSubtitleStylePassthroughType,
     BurninSubtitleTeletextSpacingType,
     CaptionDestinationTypeType,
+    CaptionSourceConvertPaintOnToPopOnType,
     CaptionSourceTypeType,
     CmafClientCacheType,
     CmafCodecSpecificationType,
     CmafEncryptionTypeType,
     CmafImageBasedTrickPlayType,
     CmafInitializationVectorInManifestType,
     CmafIntervalCadenceType,
@@ -241,14 +245,15 @@
     HlsIntervalCadenceType,
     HlsKeyProviderTypeType,
     HlsManifestCompressionType,
     HlsManifestDurationFormatType,
     HlsOfflineEncryptedType,
     HlsOutputSelectionType,
     HlsProgramDateTimeType,
+    HlsProgressiveWriteHlsManifestType,
     HlsSegmentControlType,
     HlsSegmentLengthControlType,
     HlsStreamInfResolutionType,
     HlsTargetDurationCompatibilityModeType,
     HlsTimedMetadataId3FrameType,
     ImscAccessibilitySubsType,
     ImscStylePassthroughType,
@@ -426,14 +431,15 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AacSettingsTypeDef",
     "Ac3SettingsTypeDef",
     "AccelerationSettingsTypeDef",
+    "AdvancedInputFilterSettingsTypeDef",
     "AiffSettingsTypeDef",
     "AllowedRenditionSizeTypeDef",
     "AncillarySourceSettingsTypeDef",
     "AssociateCertificateRequestRequestTypeDef",
     "AudioChannelTaggingSettingsTypeDef",
     "Eac3AtmosSettingsTypeDef",
     "Eac3SettingsTypeDef",
@@ -478,24 +484,23 @@
     "Hdr10MetadataTypeDef",
     "F4vSettingsTypeDef",
     "M3u8SettingsTypeDef",
     "MovSettingsTypeDef",
     "Mp4SettingsTypeDef",
     "MpdSettingsTypeDef",
     "HopDestinationTypeDef",
-    "ResponseMetadataTypeDef",
     "ReservationPlanSettingsTypeDef",
     "DashAdditionalManifestTypeDef",
     "SpekeKeyProviderTypeDef",
     "DashIsoImageBasedTrickPlaySettingsTypeDef",
     "DeinterlacerTypeDef",
     "DeleteJobTemplateRequestRequestTypeDef",
     "DeletePresetRequestRequestTypeDef",
     "DeleteQueueRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
     "DescribeEndpointsRequestRequestTypeDef",
     "EndpointTypeDef",
     "DisassociateCertificateRequestRequestTypeDef",
     "DolbyVisionLevel6MetadataTypeDef",
     "DvbNitSettingsTypeDef",
     "DvbSdtSettingsTypeDef",
     "DvbTdtSettingsTypeDef",
@@ -524,33 +529,40 @@
     "JobMessagesTypeDef",
     "KantarWatermarkSettingsTypeDef",
     "NielsenConfigurationTypeDef",
     "NielsenNonLinearWatermarkSettingsTypeDef",
     "TimecodeConfigTypeDef",
     "QueueTransitionTypeDef",
     "TimingTypeDef",
+    "WarningGroupTypeDef",
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
+    "ListPresetsRequestListPresetsPaginateTypeDef",
     "ListPresetsRequestRequestTypeDef",
+    "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListQueuesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ResourceTagsTypeDef",
     "M2tsScte35EsamTypeDef",
     "MotionImageInsertionFramerateTypeDef",
     "MotionImageInsertionOffsetTypeDef",
     "Mpeg2SettingsTypeDef",
     "MsSmoothAdditionalManifestTypeDef",
     "MxfXavcProfileSettingsTypeDef",
     "NexGuardFileMarkerSettingsTypeDef",
     "NoiseReducerFilterSettingsTypeDef",
     "NoiseReducerSpatialFilterSettingsTypeDef",
     "NoiseReducerTemporalFilterSettingsTypeDef",
     "VideoDetailTypeDef",
+    "PaginatorConfigTypeDef",
     "ProresSettingsTypeDef",
     "ReservationPlanTypeDef",
+    "ResponseMetadataTypeDef",
     "S3DestinationAccessControlTypeDef",
     "S3EncryptionSettingsTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TimecodeBurninTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "Vc3SettingsTypeDef",
     "Vp8SettingsTypeDef",
@@ -571,19 +583,14 @@
     "ColorCorrectorTypeDef",
     "VideoSelectorTypeDef",
     "CreateQueueRequestRequestTypeDef",
     "UpdateQueueRequestRequestTypeDef",
     "DashIsoEncryptionSettingsTypeDef",
     "HlsEncryptionSettingsTypeDef",
     "MsSmoothEncryptionSettingsTypeDef",
-    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
-    "ListPresetsRequestListPresetsPaginateTypeDef",
-    "ListQueuesRequestListQueuesPaginateTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "DolbyVisionTypeDef",
     "EsamSettingsTypeDef",
     "GetPolicyResponseTypeDef",
     "PutPolicyRequestRequestTypeDef",
     "PutPolicyResponseTypeDef",
     "H264SettingsTypeDef",
@@ -690,14 +697,23 @@
 AccelerationSettingsTypeDef = TypedDict(
     "AccelerationSettingsTypeDef",
     {
         "Mode": AccelerationModeType,
     },
 )
 
+AdvancedInputFilterSettingsTypeDef = TypedDict(
+    "AdvancedInputFilterSettingsTypeDef",
+    {
+        "AddTexture": AdvancedInputFilterAddTextureType,
+        "Sharpening": AdvancedInputFilterSharpenType,
+    },
+    total=False,
+)
+
 AiffSettingsTypeDef = TypedDict(
     "AiffSettingsTypeDef",
     {
         "BitDepth": int,
         "Channels": int,
         "SampleRate": int,
     },
@@ -1308,25 +1324,14 @@
         "Priority": int,
         "Queue": str,
         "WaitMinutes": int,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 ReservationPlanSettingsTypeDef = TypedDict(
     "ReservationPlanSettingsTypeDef",
     {
         "Commitment": Literal["ONE_YEAR"],
         "RenewalType": RenewalTypeType,
         "ReservedSlots": int,
     },
@@ -1392,20 +1397,19 @@
 DeleteQueueRequestRequestTypeDef = TypedDict(
     "DeleteQueueRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef = TypedDict(
+    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Mode": DescribeEndpointsModeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeEndpointsRequestRequestTypeDef = TypedDict(
     "DescribeEndpointsRequestRequestTypeDef",
     {
@@ -1768,50 +1772,101 @@
         "FinishTime": datetime,
         "StartTime": datetime,
         "SubmitTime": datetime,
     },
     total=False,
 )
 
+WarningGroupTypeDef = TypedDict(
+    "WarningGroupTypeDef",
+    {
+        "Code": int,
+        "Count": int,
+    },
+)
+
+ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    {
+        "Category": str,
+        "ListBy": JobTemplateListByType,
+        "Order": OrderType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListJobTemplatesRequestRequestTypeDef = TypedDict(
     "ListJobTemplatesRequestRequestTypeDef",
     {
         "Category": str,
         "ListBy": JobTemplateListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
     },
     total=False,
 )
 
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "Order": OrderType,
+        "Queue": str,
+        "Status": JobStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
         "Queue": str,
         "Status": JobStatusType,
     },
     total=False,
 )
 
+ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
+    "ListPresetsRequestListPresetsPaginateTypeDef",
+    {
+        "Category": str,
+        "ListBy": PresetListByType,
+        "Order": OrderType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPresetsRequestRequestTypeDef = TypedDict(
     "ListPresetsRequestRequestTypeDef",
     {
         "Category": str,
         "ListBy": PresetListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
     },
     total=False,
 )
 
+ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
+    "ListQueuesRequestListQueuesPaginateTypeDef",
+    {
+        "ListBy": QueueListByType,
+        "Order": OrderType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListQueuesRequestRequestTypeDef = TypedDict(
     "ListQueuesRequestRequestTypeDef",
     {
         "ListBy": QueueListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
@@ -1965,14 +2020,24 @@
     {
         "HeightInPx": int,
         "WidthInPx": int,
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 ProresSettingsTypeDef = TypedDict(
     "ProresSettingsTypeDef",
     {
         "ChromaSampling": ProresChromaSamplingType,
         "CodecProfile": ProresCodecProfileType,
         "FramerateControl": ProresFramerateControlType,
         "FramerateConversionAlgorithm": ProresFramerateConversionAlgorithmType,
@@ -1998,14 +2063,25 @@
         "RenewalType": RenewalTypeType,
         "ReservedSlots": int,
         "Status": ReservationPlanStatusType,
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 S3DestinationAccessControlTypeDef = TypedDict(
     "S3DestinationAccessControlTypeDef",
     {
         "CannedAcl": S3ObjectCannedAclType,
     },
     total=False,
 )
@@ -2254,14 +2330,15 @@
     total=False,
 )
 
 FileSourceSettingsTypeDef = TypedDict(
     "FileSourceSettingsTypeDef",
     {
         "Convert608To708": FileSourceConvert608To708Type,
+        "ConvertPaintToPop": CaptionSourceConvertPaintOnToPopOnType,
         "Framerate": CaptionSourceFramerateTypeDef,
         "SourceFile": str,
         "TimeDelta": int,
         "TimeDeltaUnits": FileSourceTimeDeltaUnitsType,
     },
     total=False,
 )
@@ -2396,72 +2473,20 @@
     "MsSmoothEncryptionSettingsTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
     total=False,
 )
 
-DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef = TypedDict(
-    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
-    {
-        "Mode": DescribeEndpointsModeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
-    {
-        "Category": str,
-        "ListBy": JobTemplateListByType,
-        "Order": OrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "Order": OrderType,
-        "Queue": str,
-        "Status": JobStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
-    "ListPresetsRequestListPresetsPaginateTypeDef",
-    {
-        "Category": str,
-        "ListBy": PresetListByType,
-        "Order": OrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
-    "ListQueuesRequestListQueuesPaginateTypeDef",
-    {
-        "ListBy": QueueListByType,
-        "Order": OrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DolbyVisionTypeDef = TypedDict(
     "DolbyVisionTypeDef",
     {
         "L6Metadata": DolbyVisionLevel6MetadataTypeDef,
@@ -2482,30 +2507,30 @@
     total=False,
 )
 
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutPolicyRequestRequestTypeDef = TypedDict(
     "PutPolicyRequestRequestTypeDef",
     {
         "Policy": PolicyTypeDef,
     },
 )
 
 PutPolicyResponseTypeDef = TypedDict(
     "PutPolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 H264SettingsTypeDef = TypedDict(
     "H264SettingsTypeDef",
     {
         "AdaptiveQuantization": H264AdaptiveQuantizationType,
@@ -2555,14 +2580,15 @@
 )
 
 H265SettingsTypeDef = TypedDict(
     "H265SettingsTypeDef",
     {
         "AdaptiveQuantization": H265AdaptiveQuantizationType,
         "AlternateTransferFunctionSei": H265AlternateTransferFunctionSeiType,
+        "BandwidthReductionFilter": BandwidthReductionFilterTypeDef,
         "Bitrate": int,
         "CodecLevel": H265CodecLevelType,
         "CodecProfile": H265CodecProfileType,
         "DynamicSubGop": H265DynamicSubGopType,
         "FlickerAdaptiveQuantization": H265FlickerAdaptiveQuantizationType,
         "FramerateControl": H265FramerateControlType,
         "FramerateConversionAlgorithm": H265FramerateConversionAlgorithmType,
@@ -2627,15 +2653,15 @@
     total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceTags": ResourceTagsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 M2tsSettingsTypeDef = TypedDict(
     "M2tsSettingsTypeDef",
     {
         "AudioBufferModel": M2tsAudioBufferModelType,
@@ -2890,40 +2916,40 @@
     total=False,
 )
 
 CreateQueueResponseTypeDef = TypedDict(
     "CreateQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetQueueResponseTypeDef = TypedDict(
     "GetQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListQueuesResponseTypeDef = TypedDict(
     "ListQueuesResponseTypeDef",
     {
         "NextToken": str,
         "Queues": List[QueueTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateQueueResponseTypeDef = TypedDict(
     "UpdateQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DestinationSettingsTypeDef = TypedDict(
     "DestinationSettingsTypeDef",
     {
         "S3Settings": S3DestinationSettingsTypeDef,
@@ -3097,14 +3123,15 @@
         "ManifestCompression": HlsManifestCompressionType,
         "ManifestDurationFormat": HlsManifestDurationFormatType,
         "MinFinalSegmentLength": float,
         "MinSegmentLength": int,
         "OutputSelection": HlsOutputSelectionType,
         "ProgramDateTime": HlsProgramDateTimeType,
         "ProgramDateTimePeriod": int,
+        "ProgressiveWriteHlsManifest": HlsProgressiveWriteHlsManifestType,
         "SegmentControl": HlsSegmentControlType,
         "SegmentLength": int,
         "SegmentLengthControl": HlsSegmentLengthControlType,
         "SegmentsPerSubdirectory": int,
         "StreamInfResolution": HlsStreamInfResolutionType,
         "TargetDurationCompatibilityMode": HlsTargetDurationCompatibilityModeType,
         "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
@@ -3150,14 +3177,16 @@
     },
     total=False,
 )
 
 InputTemplateTypeDef = TypedDict(
     "InputTemplateTypeDef",
     {
+        "AdvancedInputFilter": AdvancedInputFilterType,
+        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
         "AudioSelectorGroups": Mapping[str, AudioSelectorGroupTypeDef],
         "AudioSelectors": Mapping[str, AudioSelectorTypeDef],
         "CaptionSelectors": Mapping[str, CaptionSelectorTypeDef],
         "Crop": RectangleTypeDef,
         "DeblockFilter": InputDeblockFilterType,
         "DenoiseFilter": InputDenoiseFilterType,
         "DolbyVisionMetadataXml": str,
@@ -3175,14 +3204,16 @@
     },
     total=False,
 )
 
 InputTypeDef = TypedDict(
     "InputTypeDef",
     {
+        "AdvancedInputFilter": AdvancedInputFilterType,
+        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
         "AudioSelectorGroups": Mapping[str, AudioSelectorGroupTypeDef],
         "AudioSelectors": Mapping[str, AudioSelectorTypeDef],
         "CaptionSelectors": Mapping[str, CaptionSelectorTypeDef],
         "Crop": RectangleTypeDef,
         "DeblockFilter": InputDeblockFilterType,
         "DecryptionSettings": InputDecryptionSettingsTypeDef,
         "DenoiseFilter": InputDenoiseFilterType,
@@ -3366,40 +3397,40 @@
     total=False,
 )
 
 CreatePresetResponseTypeDef = TypedDict(
     "CreatePresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPresetResponseTypeDef = TypedDict(
     "GetPresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPresetsResponseTypeDef = TypedDict(
     "ListPresetsResponseTypeDef",
     {
         "NextToken": str,
         "Presets": List[PresetTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePresetResponseTypeDef = TypedDict(
     "UpdatePresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "Role": str,
@@ -3441,14 +3472,15 @@
 _OptionalJobTypeDef = TypedDict(
     "_OptionalJobTypeDef",
     {
         "AccelerationSettings": AccelerationSettingsTypeDef,
         "AccelerationStatus": AccelerationStatusType,
         "Arn": str,
         "BillingTagsSource": BillingTagsSourceType,
+        "ClientRequestToken": str,
         "CreatedAt": datetime,
         "CurrentPhase": JobPhaseType,
         "ErrorCode": int,
         "ErrorMessage": str,
         "HopDestinations": List[HopDestinationTypeDef],
         "Id": str,
         "JobPercentComplete": int,
@@ -3460,14 +3492,15 @@
         "QueueTransitions": List[QueueTransitionTypeDef],
         "RetryCount": int,
         "SimulateReservedQueue": SimulateReservedQueueType,
         "Status": JobStatusType,
         "StatusUpdateInterval": StatusUpdateIntervalType,
         "Timing": TimingTypeDef,
         "UserMetadata": Dict[str, str],
+        "Warnings": List[WarningGroupTypeDef],
     },
     total=False,
 )
 
 
 class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
     pass
@@ -3560,60 +3593,60 @@
     pass
 
 
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJobResponseTypeDef = TypedDict(
     "GetJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateJobTemplateResponseTypeDef = TypedDict(
     "CreateJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJobTemplateResponseTypeDef = TypedDict(
     "GetJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJobTemplatesResponseTypeDef = TypedDict(
     "ListJobTemplatesResponseTypeDef",
     {
         "JobTemplates": List[JobTemplateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateJobTemplateResponseTypeDef = TypedDict(
     "UpdateJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert/type_defs.pyi` & `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,17 @@
     Ac3DynamicRangeCompressionLineType,
     Ac3DynamicRangeCompressionProfileType,
     Ac3DynamicRangeCompressionRfType,
     Ac3LfeFilterType,
     Ac3MetadataControlType,
     AccelerationModeType,
     AccelerationStatusType,
+    AdvancedInputFilterAddTextureType,
+    AdvancedInputFilterSharpenType,
+    AdvancedInputFilterType,
     AfdSignalingType,
     AlphaBehaviorType,
     AncillaryConvert608To708Type,
     AncillaryTerminateCaptionsType,
     AntiAliasType,
     AudioChannelTagType,
     AudioCodecType,
@@ -70,14 +73,15 @@
     BurninSubtitleFallbackFontType,
     BurninSubtitleFontColorType,
     BurninSubtitleOutlineColorType,
     BurninSubtitleShadowColorType,
     BurnInSubtitleStylePassthroughType,
     BurninSubtitleTeletextSpacingType,
     CaptionDestinationTypeType,
+    CaptionSourceConvertPaintOnToPopOnType,
     CaptionSourceTypeType,
     CmafClientCacheType,
     CmafCodecSpecificationType,
     CmafEncryptionTypeType,
     CmafImageBasedTrickPlayType,
     CmafInitializationVectorInManifestType,
     CmafIntervalCadenceType,
@@ -241,14 +245,15 @@
     HlsIntervalCadenceType,
     HlsKeyProviderTypeType,
     HlsManifestCompressionType,
     HlsManifestDurationFormatType,
     HlsOfflineEncryptedType,
     HlsOutputSelectionType,
     HlsProgramDateTimeType,
+    HlsProgressiveWriteHlsManifestType,
     HlsSegmentControlType,
     HlsSegmentLengthControlType,
     HlsStreamInfResolutionType,
     HlsTargetDurationCompatibilityModeType,
     HlsTimedMetadataId3FrameType,
     ImscAccessibilitySubsType,
     ImscStylePassthroughType,
@@ -425,14 +430,15 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AacSettingsTypeDef",
     "Ac3SettingsTypeDef",
     "AccelerationSettingsTypeDef",
+    "AdvancedInputFilterSettingsTypeDef",
     "AiffSettingsTypeDef",
     "AllowedRenditionSizeTypeDef",
     "AncillarySourceSettingsTypeDef",
     "AssociateCertificateRequestRequestTypeDef",
     "AudioChannelTaggingSettingsTypeDef",
     "Eac3AtmosSettingsTypeDef",
     "Eac3SettingsTypeDef",
@@ -477,24 +483,23 @@
     "Hdr10MetadataTypeDef",
     "F4vSettingsTypeDef",
     "M3u8SettingsTypeDef",
     "MovSettingsTypeDef",
     "Mp4SettingsTypeDef",
     "MpdSettingsTypeDef",
     "HopDestinationTypeDef",
-    "ResponseMetadataTypeDef",
     "ReservationPlanSettingsTypeDef",
     "DashAdditionalManifestTypeDef",
     "SpekeKeyProviderTypeDef",
     "DashIsoImageBasedTrickPlaySettingsTypeDef",
     "DeinterlacerTypeDef",
     "DeleteJobTemplateRequestRequestTypeDef",
     "DeletePresetRequestRequestTypeDef",
     "DeleteQueueRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
     "DescribeEndpointsRequestRequestTypeDef",
     "EndpointTypeDef",
     "DisassociateCertificateRequestRequestTypeDef",
     "DolbyVisionLevel6MetadataTypeDef",
     "DvbNitSettingsTypeDef",
     "DvbSdtSettingsTypeDef",
     "DvbTdtSettingsTypeDef",
@@ -523,33 +528,40 @@
     "JobMessagesTypeDef",
     "KantarWatermarkSettingsTypeDef",
     "NielsenConfigurationTypeDef",
     "NielsenNonLinearWatermarkSettingsTypeDef",
     "TimecodeConfigTypeDef",
     "QueueTransitionTypeDef",
     "TimingTypeDef",
+    "WarningGroupTypeDef",
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
+    "ListPresetsRequestListPresetsPaginateTypeDef",
     "ListPresetsRequestRequestTypeDef",
+    "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListQueuesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ResourceTagsTypeDef",
     "M2tsScte35EsamTypeDef",
     "MotionImageInsertionFramerateTypeDef",
     "MotionImageInsertionOffsetTypeDef",
     "Mpeg2SettingsTypeDef",
     "MsSmoothAdditionalManifestTypeDef",
     "MxfXavcProfileSettingsTypeDef",
     "NexGuardFileMarkerSettingsTypeDef",
     "NoiseReducerFilterSettingsTypeDef",
     "NoiseReducerSpatialFilterSettingsTypeDef",
     "NoiseReducerTemporalFilterSettingsTypeDef",
     "VideoDetailTypeDef",
+    "PaginatorConfigTypeDef",
     "ProresSettingsTypeDef",
     "ReservationPlanTypeDef",
+    "ResponseMetadataTypeDef",
     "S3DestinationAccessControlTypeDef",
     "S3EncryptionSettingsTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TimecodeBurninTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "Vc3SettingsTypeDef",
     "Vp8SettingsTypeDef",
@@ -570,19 +582,14 @@
     "ColorCorrectorTypeDef",
     "VideoSelectorTypeDef",
     "CreateQueueRequestRequestTypeDef",
     "UpdateQueueRequestRequestTypeDef",
     "DashIsoEncryptionSettingsTypeDef",
     "HlsEncryptionSettingsTypeDef",
     "MsSmoothEncryptionSettingsTypeDef",
-    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
-    "ListPresetsRequestListPresetsPaginateTypeDef",
-    "ListQueuesRequestListQueuesPaginateTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "DolbyVisionTypeDef",
     "EsamSettingsTypeDef",
     "GetPolicyResponseTypeDef",
     "PutPolicyRequestRequestTypeDef",
     "PutPolicyResponseTypeDef",
     "H264SettingsTypeDef",
@@ -689,14 +696,23 @@
 AccelerationSettingsTypeDef = TypedDict(
     "AccelerationSettingsTypeDef",
     {
         "Mode": AccelerationModeType,
     },
 )
 
+AdvancedInputFilterSettingsTypeDef = TypedDict(
+    "AdvancedInputFilterSettingsTypeDef",
+    {
+        "AddTexture": AdvancedInputFilterAddTextureType,
+        "Sharpening": AdvancedInputFilterSharpenType,
+    },
+    total=False,
+)
+
 AiffSettingsTypeDef = TypedDict(
     "AiffSettingsTypeDef",
     {
         "BitDepth": int,
         "Channels": int,
         "SampleRate": int,
     },
@@ -1307,25 +1323,14 @@
         "Priority": int,
         "Queue": str,
         "WaitMinutes": int,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 ReservationPlanSettingsTypeDef = TypedDict(
     "ReservationPlanSettingsTypeDef",
     {
         "Commitment": Literal["ONE_YEAR"],
         "RenewalType": RenewalTypeType,
         "ReservedSlots": int,
     },
@@ -1391,20 +1396,19 @@
 DeleteQueueRequestRequestTypeDef = TypedDict(
     "DeleteQueueRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef = TypedDict(
+    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Mode": DescribeEndpointsModeType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeEndpointsRequestRequestTypeDef = TypedDict(
     "DescribeEndpointsRequestRequestTypeDef",
     {
@@ -1767,50 +1771,101 @@
         "FinishTime": datetime,
         "StartTime": datetime,
         "SubmitTime": datetime,
     },
     total=False,
 )
 
+WarningGroupTypeDef = TypedDict(
+    "WarningGroupTypeDef",
+    {
+        "Code": int,
+        "Count": int,
+    },
+)
+
+ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    {
+        "Category": str,
+        "ListBy": JobTemplateListByType,
+        "Order": OrderType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListJobTemplatesRequestRequestTypeDef = TypedDict(
     "ListJobTemplatesRequestRequestTypeDef",
     {
         "Category": str,
         "ListBy": JobTemplateListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
     },
     total=False,
 )
 
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "Order": OrderType,
+        "Queue": str,
+        "Status": JobStatusType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
         "Queue": str,
         "Status": JobStatusType,
     },
     total=False,
 )
 
+ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
+    "ListPresetsRequestListPresetsPaginateTypeDef",
+    {
+        "Category": str,
+        "ListBy": PresetListByType,
+        "Order": OrderType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListPresetsRequestRequestTypeDef = TypedDict(
     "ListPresetsRequestRequestTypeDef",
     {
         "Category": str,
         "ListBy": PresetListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
     },
     total=False,
 )
 
+ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
+    "ListQueuesRequestListQueuesPaginateTypeDef",
+    {
+        "ListBy": QueueListByType,
+        "Order": OrderType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListQueuesRequestRequestTypeDef = TypedDict(
     "ListQueuesRequestRequestTypeDef",
     {
         "ListBy": QueueListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
@@ -1964,14 +2019,24 @@
     {
         "HeightInPx": int,
         "WidthInPx": int,
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 ProresSettingsTypeDef = TypedDict(
     "ProresSettingsTypeDef",
     {
         "ChromaSampling": ProresChromaSamplingType,
         "CodecProfile": ProresCodecProfileType,
         "FramerateControl": ProresFramerateControlType,
         "FramerateConversionAlgorithm": ProresFramerateConversionAlgorithmType,
@@ -1997,14 +2062,25 @@
         "RenewalType": RenewalTypeType,
         "ReservedSlots": int,
         "Status": ReservationPlanStatusType,
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 S3DestinationAccessControlTypeDef = TypedDict(
     "S3DestinationAccessControlTypeDef",
     {
         "CannedAcl": S3ObjectCannedAclType,
     },
     total=False,
 )
@@ -2251,14 +2327,15 @@
     total=False,
 )
 
 FileSourceSettingsTypeDef = TypedDict(
     "FileSourceSettingsTypeDef",
     {
         "Convert608To708": FileSourceConvert608To708Type,
+        "ConvertPaintToPop": CaptionSourceConvertPaintOnToPopOnType,
         "Framerate": CaptionSourceFramerateTypeDef,
         "SourceFile": str,
         "TimeDelta": int,
         "TimeDeltaUnits": FileSourceTimeDeltaUnitsType,
     },
     total=False,
 )
@@ -2389,72 +2466,20 @@
     "MsSmoothEncryptionSettingsTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
     total=False,
 )
 
-DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef = TypedDict(
-    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
-    {
-        "Mode": DescribeEndpointsModeType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
-    {
-        "Category": str,
-        "ListBy": JobTemplateListByType,
-        "Order": OrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "Order": OrderType,
-        "Queue": str,
-        "Status": JobStatusType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
-    "ListPresetsRequestListPresetsPaginateTypeDef",
-    {
-        "Category": str,
-        "ListBy": PresetListByType,
-        "Order": OrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
-    "ListQueuesRequestListQueuesPaginateTypeDef",
-    {
-        "ListBy": QueueListByType,
-        "Order": OrderType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DolbyVisionTypeDef = TypedDict(
     "DolbyVisionTypeDef",
     {
         "L6Metadata": DolbyVisionLevel6MetadataTypeDef,
@@ -2475,30 +2500,30 @@
     total=False,
 )
 
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutPolicyRequestRequestTypeDef = TypedDict(
     "PutPolicyRequestRequestTypeDef",
     {
         "Policy": PolicyTypeDef,
     },
 )
 
 PutPolicyResponseTypeDef = TypedDict(
     "PutPolicyResponseTypeDef",
     {
         "Policy": PolicyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 H264SettingsTypeDef = TypedDict(
     "H264SettingsTypeDef",
     {
         "AdaptiveQuantization": H264AdaptiveQuantizationType,
@@ -2548,14 +2573,15 @@
 )
 
 H265SettingsTypeDef = TypedDict(
     "H265SettingsTypeDef",
     {
         "AdaptiveQuantization": H265AdaptiveQuantizationType,
         "AlternateTransferFunctionSei": H265AlternateTransferFunctionSeiType,
+        "BandwidthReductionFilter": BandwidthReductionFilterTypeDef,
         "Bitrate": int,
         "CodecLevel": H265CodecLevelType,
         "CodecProfile": H265CodecProfileType,
         "DynamicSubGop": H265DynamicSubGopType,
         "FlickerAdaptiveQuantization": H265FlickerAdaptiveQuantizationType,
         "FramerateControl": H265FramerateControlType,
         "FramerateConversionAlgorithm": H265FramerateConversionAlgorithmType,
@@ -2620,15 +2646,15 @@
     total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceTags": ResourceTagsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 M2tsSettingsTypeDef = TypedDict(
     "M2tsSettingsTypeDef",
     {
         "AudioBufferModel": M2tsAudioBufferModelType,
@@ -2881,40 +2907,40 @@
     total=False,
 )
 
 CreateQueueResponseTypeDef = TypedDict(
     "CreateQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetQueueResponseTypeDef = TypedDict(
     "GetQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListQueuesResponseTypeDef = TypedDict(
     "ListQueuesResponseTypeDef",
     {
         "NextToken": str,
         "Queues": List[QueueTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateQueueResponseTypeDef = TypedDict(
     "UpdateQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DestinationSettingsTypeDef = TypedDict(
     "DestinationSettingsTypeDef",
     {
         "S3Settings": S3DestinationSettingsTypeDef,
@@ -3088,14 +3114,15 @@
         "ManifestCompression": HlsManifestCompressionType,
         "ManifestDurationFormat": HlsManifestDurationFormatType,
         "MinFinalSegmentLength": float,
         "MinSegmentLength": int,
         "OutputSelection": HlsOutputSelectionType,
         "ProgramDateTime": HlsProgramDateTimeType,
         "ProgramDateTimePeriod": int,
+        "ProgressiveWriteHlsManifest": HlsProgressiveWriteHlsManifestType,
         "SegmentControl": HlsSegmentControlType,
         "SegmentLength": int,
         "SegmentLengthControl": HlsSegmentLengthControlType,
         "SegmentsPerSubdirectory": int,
         "StreamInfResolution": HlsStreamInfResolutionType,
         "TargetDurationCompatibilityMode": HlsTargetDurationCompatibilityModeType,
         "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
@@ -3141,14 +3168,16 @@
     },
     total=False,
 )
 
 InputTemplateTypeDef = TypedDict(
     "InputTemplateTypeDef",
     {
+        "AdvancedInputFilter": AdvancedInputFilterType,
+        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
         "AudioSelectorGroups": Mapping[str, AudioSelectorGroupTypeDef],
         "AudioSelectors": Mapping[str, AudioSelectorTypeDef],
         "CaptionSelectors": Mapping[str, CaptionSelectorTypeDef],
         "Crop": RectangleTypeDef,
         "DeblockFilter": InputDeblockFilterType,
         "DenoiseFilter": InputDenoiseFilterType,
         "DolbyVisionMetadataXml": str,
@@ -3166,14 +3195,16 @@
     },
     total=False,
 )
 
 InputTypeDef = TypedDict(
     "InputTypeDef",
     {
+        "AdvancedInputFilter": AdvancedInputFilterType,
+        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
         "AudioSelectorGroups": Mapping[str, AudioSelectorGroupTypeDef],
         "AudioSelectors": Mapping[str, AudioSelectorTypeDef],
         "CaptionSelectors": Mapping[str, CaptionSelectorTypeDef],
         "Crop": RectangleTypeDef,
         "DeblockFilter": InputDeblockFilterType,
         "DecryptionSettings": InputDecryptionSettingsTypeDef,
         "DenoiseFilter": InputDenoiseFilterType,
@@ -3351,40 +3382,40 @@
     total=False,
 )
 
 CreatePresetResponseTypeDef = TypedDict(
     "CreatePresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetPresetResponseTypeDef = TypedDict(
     "GetPresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPresetsResponseTypeDef = TypedDict(
     "ListPresetsResponseTypeDef",
     {
         "NextToken": str,
         "Presets": List[PresetTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdatePresetResponseTypeDef = TypedDict(
     "UpdatePresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "Role": str,
@@ -3424,14 +3455,15 @@
 _OptionalJobTypeDef = TypedDict(
     "_OptionalJobTypeDef",
     {
         "AccelerationSettings": AccelerationSettingsTypeDef,
         "AccelerationStatus": AccelerationStatusType,
         "Arn": str,
         "BillingTagsSource": BillingTagsSourceType,
+        "ClientRequestToken": str,
         "CreatedAt": datetime,
         "CurrentPhase": JobPhaseType,
         "ErrorCode": int,
         "ErrorMessage": str,
         "HopDestinations": List[HopDestinationTypeDef],
         "Id": str,
         "JobPercentComplete": int,
@@ -3443,14 +3475,15 @@
         "QueueTransitions": List[QueueTransitionTypeDef],
         "RetryCount": int,
         "SimulateReservedQueue": SimulateReservedQueueType,
         "Status": JobStatusType,
         "StatusUpdateInterval": StatusUpdateIntervalType,
         "Timing": TimingTypeDef,
         "UserMetadata": Dict[str, str],
+        "Warnings": List[WarningGroupTypeDef],
     },
     total=False,
 )
 
 class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
     pass
 
@@ -3535,60 +3568,60 @@
 ):
     pass
 
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJobResponseTypeDef = TypedDict(
     "GetJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateJobTemplateResponseTypeDef = TypedDict(
     "CreateJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetJobTemplateResponseTypeDef = TypedDict(
     "GetJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListJobTemplatesResponseTypeDef = TypedDict(
     "ListJobTemplatesResponseTypeDef",
     {
         "JobTemplates": List[JobTemplateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateJobTemplateResponseTypeDef = TypedDict(
     "UpdateJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert.egg-info/PKG-INFO` & `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediaconvert
-Version: 1.26.98
-Summary: Type annotations for boto3.MediaConvert 1.26.98 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.MediaConvert 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-mediaconvert"></a>
 
 # mypy-boto3-mediaconvert
 
 [![PyPI - mypy-boto3-mediaconvert](https://img.shields.io/pypi/v/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconvert?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConvert 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[boto3.MediaConvert 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mediaconvert docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,14 +325,17 @@
     Ac3DynamicRangeCompressionLineType,
     Ac3DynamicRangeCompressionProfileType,
     Ac3DynamicRangeCompressionRfType,
     Ac3LfeFilterType,
     Ac3MetadataControlType,
     AccelerationModeType,
     AccelerationStatusType,
+    AdvancedInputFilterAddTextureType,
+    AdvancedInputFilterSharpenType,
+    AdvancedInputFilterType,
     AfdSignalingType,
     AlphaBehaviorType,
     AncillaryConvert608To708Type,
     AncillaryTerminateCaptionsType,
     AntiAliasType,
     AudioChannelTagType,
     AudioCodecType,
@@ -368,14 +371,15 @@
     BurninSubtitleBackgroundColorType,
     BurninSubtitleFallbackFontType,
     BurninSubtitleFontColorType,
     BurninSubtitleOutlineColorType,
     BurninSubtitleShadowColorType,
     BurninSubtitleTeletextSpacingType,
     CaptionDestinationTypeType,
+    CaptionSourceConvertPaintOnToPopOnType,
     CaptionSourceTypeType,
     CmafClientCacheType,
     CmafCodecSpecificationType,
     CmafEncryptionTypeType,
     CmafImageBasedTrickPlayType,
     CmafInitializationVectorInManifestType,
     CmafIntervalCadenceType,
@@ -542,14 +546,15 @@
     HlsIntervalCadenceType,
     HlsKeyProviderTypeType,
     HlsManifestCompressionType,
     HlsManifestDurationFormatType,
     HlsOfflineEncryptedType,
     HlsOutputSelectionType,
     HlsProgramDateTimeType,
+    HlsProgressiveWriteHlsManifestType,
     HlsSegmentControlType,
     HlsSegmentLengthControlType,
     HlsStreamInfResolutionType,
     HlsTargetDurationCompatibilityModeType,
     HlsTimedMetadataId3FrameType,
     ImscAccessibilitySubsType,
     ImscStylePassthroughType,
@@ -741,14 +746,15 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediaconvert.type_defs import (
     AacSettingsTypeDef,
     Ac3SettingsTypeDef,
     AccelerationSettingsTypeDef,
+    AdvancedInputFilterSettingsTypeDef,
     AiffSettingsTypeDef,
     AllowedRenditionSizeTypeDef,
     AncillarySourceSettingsTypeDef,
     AssociateCertificateRequestRequestTypeDef,
     AudioChannelTaggingSettingsTypeDef,
     Eac3AtmosSettingsTypeDef,
     Eac3SettingsTypeDef,
@@ -793,24 +799,23 @@
     Hdr10MetadataTypeDef,
     F4vSettingsTypeDef,
     M3u8SettingsTypeDef,
     MovSettingsTypeDef,
     Mp4SettingsTypeDef,
     MpdSettingsTypeDef,
     HopDestinationTypeDef,
-    ResponseMetadataTypeDef,
     ReservationPlanSettingsTypeDef,
     DashAdditionalManifestTypeDef,
     SpekeKeyProviderTypeDef,
     DashIsoImageBasedTrickPlaySettingsTypeDef,
     DeinterlacerTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
     DescribeEndpointsRequestRequestTypeDef,
     EndpointTypeDef,
     DisassociateCertificateRequestRequestTypeDef,
     DolbyVisionLevel6MetadataTypeDef,
     DvbNitSettingsTypeDef,
     DvbSdtSettingsTypeDef,
     DvbTdtSettingsTypeDef,
@@ -839,33 +844,40 @@
     JobMessagesTypeDef,
     KantarWatermarkSettingsTypeDef,
     NielsenConfigurationTypeDef,
     NielsenNonLinearWatermarkSettingsTypeDef,
     TimecodeConfigTypeDef,
     QueueTransitionTypeDef,
     TimingTypeDef,
+    WarningGroupTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ResourceTagsTypeDef,
     M2tsScte35EsamTypeDef,
     MotionImageInsertionFramerateTypeDef,
     MotionImageInsertionOffsetTypeDef,
     Mpeg2SettingsTypeDef,
     MsSmoothAdditionalManifestTypeDef,
     MxfXavcProfileSettingsTypeDef,
     NexGuardFileMarkerSettingsTypeDef,
     NoiseReducerFilterSettingsTypeDef,
     NoiseReducerSpatialFilterSettingsTypeDef,
     NoiseReducerTemporalFilterSettingsTypeDef,
     VideoDetailTypeDef,
+    PaginatorConfigTypeDef,
     ProresSettingsTypeDef,
     ReservationPlanTypeDef,
+    ResponseMetadataTypeDef,
     S3DestinationAccessControlTypeDef,
     S3EncryptionSettingsTypeDef,
     TagResourceRequestRequestTypeDef,
     TimecodeBurninTypeDef,
     UntagResourceRequestRequestTypeDef,
     Vc3SettingsTypeDef,
     Vp8SettingsTypeDef,
@@ -886,19 +898,14 @@
     ColorCorrectorTypeDef,
     VideoSelectorTypeDef,
     CreateQueueRequestRequestTypeDef,
     UpdateQueueRequestRequestTypeDef,
     DashIsoEncryptionSettingsTypeDef,
     HlsEncryptionSettingsTypeDef,
     MsSmoothEncryptionSettingsTypeDef,
-    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
-    ListPresetsRequestListPresetsPaginateTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
     DescribeEndpointsResponseTypeDef,
     DolbyVisionTypeDef,
     EsamSettingsTypeDef,
     GetPolicyResponseTypeDef,
     PutPolicyRequestRequestTypeDef,
     PutPolicyResponseTypeDef,
     H264SettingsTypeDef,
```

### Comparing `mypy-boto3-mediaconvert-1.26.98/mypy_boto3_mediaconvert.egg-info/SOURCES.txt` & `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.26.98/setup.py` & `mypy-boto3-mediaconvert-1.27.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediaconvert",
-    version="1.26.98",
+    version="1.27.0",
     packages=["mypy_boto3_mediaconvert"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaConvert 1.26.98 service generated with mypy-boto3-builder"
-        " 7.14.2"
+        "Type annotations for boto3.MediaConvert 1.27.0 service generated with mypy-boto3-builder"
+        " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

