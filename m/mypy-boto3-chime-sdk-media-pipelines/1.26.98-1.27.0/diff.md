# Comparing `tmp/mypy-boto3-chime-sdk-media-pipelines-1.26.98.tar.gz` & `tmp/mypy-boto3-chime-sdk-media-pipelines-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-media-pipelines-1.26.98.tar", last modified: Thu Mar 23 19:33:04 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-sdk-media-pipelines-1.27.0.tar", last modified: Mon Jul  3 19:50:27 2023, max compression
```

## Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.98.tar` & `mypy-boto3-chime-sdk-media-pipelines-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.399627 mypy-boto3-chime-sdk-media-pipelines-1.26.98/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17974 2023-03-23 19:33:04.395626 mypy-boto3-chime-sdk-media-pipelines-1.26.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16418 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.383626 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17691 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17665 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10930 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    38555 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38510 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.395626 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17974 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 19:33:04.399627 mypy-boto3-chime-sdk-media-pipelines-1.26.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-03-23 19:32:00.000000 mypy-boto3-chime-sdk-media-pipelines-1.26.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.202905 mypy-boto3-chime-sdk-media-pipelines-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:25.000000 mypy-boto3-chime-sdk-media-pipelines-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18002 2023-07-03 19:50:27.202905 mypy-boto3-chime-sdk-media-pipelines-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-07-03 19:33:25.000000 mypy-boto3-chime-sdk-media-pipelines-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.202905 mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-03 19:33:25.000000 mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-03 19:33:25.000000 mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-03 19:33:25.000000 mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17691 2023-07-03 19:33:25.000000 mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17665 2023-07-03 19:33:25.000000 mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-07-03 19:33:25.000000 mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-03 19:33:25.000000 mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:25.000000 mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    38639 2023-07-03 19:33:26.000000 mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38594 2023-07-03 19:33:26.000000 mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:25.000000 mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.202905 mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18002 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-03 19:50:27.000000 mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:27.202905 mypy-boto3-chime-sdk-media-pipelines-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-03 19:33:24.000000 mypy-boto3-chime-sdk-media-pipelines-1.27.0/setup.py
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.98/LICENSE` & `mypy-boto3-chime-sdk-media-pipelines-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.98/PKG-INFO` & `mypy-boto3-chime-sdk-media-pipelines-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-media-pipelines
-Version: 1.26.98
-Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.26.98 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-chime-sdk-media-pipelines"></a>
 
 # mypy-boto3-chime-sdk-media-pipelines
 
 [![PyPI - mypy-boto3-chime-sdk-media-pipelines](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-media-pipelines?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMediaPipelines 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[boto3.ChimeSDKMediaPipelines 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
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
 [mypy-boto3-chime-sdk-media-pipelines docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,19 +345,19 @@
     VideoConcatenationConfigurationTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
     ChannelDefinitionTypeDef,
     S3BucketSinkConfigurationTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     DeleteMediaCapturePipelineRequestRequestTypeDef,
     DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     DeleteMediaPipelineRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     TimestampRangeTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     GetMediaPipelineRequestRequestTypeDef,
     PresenterOnlyConfigurationTypeDef,
     IssueDetectionConfigurationTypeDef,
     KeywordMatchConfigurationTypeDef,
@@ -373,24 +373,24 @@
     ListTagsForResourceRequestRequestTypeDef,
     LiveConnectorRTMPConfigurationTypeDef,
     S3RecordingSinkConfigurationTypeDef,
     SnsTopicSinkConfigurationTypeDef,
     SqsQueueSinkConfigurationTypeDef,
     VoiceAnalyticsProcessorConfigurationTypeDef,
     SentimentConfigurationTypeDef,
+    ResponseMetadataTypeDef,
     SelectedVideoStreamsTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMediaInsightsPipelineStatusRequestRequestTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
     ArtifactsConcatenationConfigurationTypeDef,
     StreamChannelDefinitionTypeDef,
     ConcatenationSinkTypeDef,
-    TagResourceRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     FragmentSelectorTypeDef,
     GridViewConfigurationTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
     LiveConnectorSinkConfigurationTypeDef,
     RealTimeAlertRuleTypeDef,
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.98/README.md` & `mypy-boto3-chime-sdk-media-pipelines-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-chime-sdk-media-pipelines"></a>
 
 # mypy-boto3-chime-sdk-media-pipelines
 
 [![PyPI - mypy-boto3-chime-sdk-media-pipelines](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-media-pipelines?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMediaPipelines 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[boto3.ChimeSDKMediaPipelines 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
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
 [mypy-boto3-chime-sdk-media-pipelines docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
 
@@ -313,19 +313,19 @@
     VideoConcatenationConfigurationTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
     ChannelDefinitionTypeDef,
     S3BucketSinkConfigurationTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     DeleteMediaCapturePipelineRequestRequestTypeDef,
     DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     DeleteMediaPipelineRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     TimestampRangeTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     GetMediaPipelineRequestRequestTypeDef,
     PresenterOnlyConfigurationTypeDef,
     IssueDetectionConfigurationTypeDef,
     KeywordMatchConfigurationTypeDef,
@@ -341,24 +341,24 @@
     ListTagsForResourceRequestRequestTypeDef,
     LiveConnectorRTMPConfigurationTypeDef,
     S3RecordingSinkConfigurationTypeDef,
     SnsTopicSinkConfigurationTypeDef,
     SqsQueueSinkConfigurationTypeDef,
     VoiceAnalyticsProcessorConfigurationTypeDef,
     SentimentConfigurationTypeDef,
+    ResponseMetadataTypeDef,
     SelectedVideoStreamsTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMediaInsightsPipelineStatusRequestRequestTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
     ArtifactsConcatenationConfigurationTypeDef,
     StreamChannelDefinitionTypeDef,
     ConcatenationSinkTypeDef,
-    TagResourceRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     FragmentSelectorTypeDef,
     GridViewConfigurationTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
     LiveConnectorSinkConfigurationTypeDef,
     RealTimeAlertRuleTypeDef,
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/__main__.py` & `mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ChimeSDKMediaPipelines 1.26.98\nVersion:        "
-        " 1.26.98\nBuilder version: 7.14.2\nDocs:           "
+        "Type annotations for boto3.ChimeSDKMediaPipelines 1.27.0\nVersion:         1.27.0\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines\nOther"
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

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/client.py` & `mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/client.pyi` & `mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/literals.py` & `mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,15 @@
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
@@ -165,14 +166,15 @@
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
@@ -314,14 +316,15 @@
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
@@ -340,16 +343,19 @@
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
@@ -433,15 +439,17 @@
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

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/literals.pyi` & `mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
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
@@ -163,14 +164,15 @@
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
@@ -312,14 +314,15 @@
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
@@ -338,16 +341,19 @@
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
@@ -431,15 +437,17 @@
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

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/type_defs.py` & `mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,19 +60,19 @@
     "VideoConcatenationConfigurationTypeDef",
     "AudioArtifactsConfigurationTypeDef",
     "ContentArtifactsConfigurationTypeDef",
     "VideoArtifactsConfigurationTypeDef",
     "ChannelDefinitionTypeDef",
     "S3BucketSinkConfigurationTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     "DeleteMediaCapturePipelineRequestRequestTypeDef",
     "DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "DeleteMediaPipelineRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "TimestampRangeTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "GetMediaPipelineRequestRequestTypeDef",
     "PresenterOnlyConfigurationTypeDef",
     "IssueDetectionConfigurationTypeDef",
     "KeywordMatchConfigurationTypeDef",
@@ -88,24 +88,24 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "LiveConnectorRTMPConfigurationTypeDef",
     "S3RecordingSinkConfigurationTypeDef",
     "SnsTopicSinkConfigurationTypeDef",
     "SqsQueueSinkConfigurationTypeDef",
     "VoiceAnalyticsProcessorConfigurationTypeDef",
     "SentimentConfigurationTypeDef",
+    "ResponseMetadataTypeDef",
     "SelectedVideoStreamsTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMediaInsightsPipelineStatusRequestRequestTypeDef",
     "AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
     "ArtifactsConcatenationConfigurationTypeDef",
     "StreamChannelDefinitionTypeDef",
     "ConcatenationSinkTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "FragmentSelectorTypeDef",
     "GridViewConfigurationTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     "ListMediaPipelinesResponseTypeDef",
     "LiveConnectorSinkConfigurationTypeDef",
     "RealTimeAlertRuleTypeDef",
@@ -331,25 +331,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
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
 S3RecordingSinkRuntimeConfigurationTypeDef = TypedDict(
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
     },
 )
@@ -371,14 +360,21 @@
 DeleteMediaPipelineRequestRequestTypeDef = TypedDict(
     "DeleteMediaPipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TimestampRangeTypeDef = TypedDict(
     "TimestampRangeTypeDef",
     {
         "StartTimestamp": Union[datetime, str],
         "EndTimestamp": Union[datetime, str],
     },
 )
@@ -549,14 +545,15 @@
     pass
 
 
 S3RecordingSinkConfigurationTypeDef = TypedDict(
     "S3RecordingSinkConfigurationTypeDef",
     {
         "Destination": str,
+        "RecordingFileFormat": RecordingFileFormatType,
     },
     total=False,
 )
 
 SnsTopicSinkConfigurationTypeDef = TypedDict(
     "SnsTopicSinkConfigurationTypeDef",
     {
@@ -587,14 +584,25 @@
     {
         "RuleName": str,
         "SentimentType": Literal["NEGATIVE"],
         "TimePeriod": int,
     },
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
 SelectedVideoStreamsTypeDef = TypedDict(
     "SelectedVideoStreamsTypeDef",
     {
         "AttendeeIds": Sequence[str],
         "ExternalUserIds": Sequence[str],
     },
     total=False,
@@ -687,34 +695,27 @@
     "ConcatenationSinkTypeDef",
     {
         "Type": Literal["S3Bucket"],
         "S3BucketSinkConfiguration": S3BucketSinkConfigurationTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 FragmentSelectorTypeDef = TypedDict(
     "FragmentSelectorTypeDef",
     {
         "FragmentSelectorType": FragmentSelectorTypeType,
@@ -744,35 +745,35 @@
 
 
 ListMediaCapturePipelinesResponseTypeDef = TypedDict(
     "ListMediaCapturePipelinesResponseTypeDef",
     {
         "MediaCapturePipelines": List[MediaCapturePipelineSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMediaInsightsPipelineConfigurationsResponseTypeDef = TypedDict(
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     {
         "MediaInsightsPipelineConfigurations": List[
             MediaInsightsPipelineConfigurationSummaryTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMediaPipelinesResponseTypeDef = TypedDict(
     "ListMediaPipelinesResponseTypeDef",
     {
         "MediaPipelines": List[MediaPipelineSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LiveConnectorSinkConfigurationTypeDef = TypedDict(
     "LiveConnectorSinkConfigurationTypeDef",
     {
         "SinkType": Literal["RTMP"],
@@ -1118,31 +1119,31 @@
     },
 )
 
 CreateMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "CreateMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "GetMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "UpdateMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef",
     {
         "Sources": Sequence[ConcatenationSourceTypeDef],
@@ -1180,15 +1181,15 @@
     total=False,
 )
 
 CreateMediaInsightsPipelineResponseTypeDef = TypedDict(
     "CreateMediaInsightsPipelineResponseTypeDef",
     {
         "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
@@ -1270,39 +1271,39 @@
     total=False,
 )
 
 CreateMediaConcatenationPipelineResponseTypeDef = TypedDict(
     "CreateMediaConcatenationPipelineResponseTypeDef",
     {
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateMediaCapturePipelineResponseTypeDef = TypedDict(
     "CreateMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMediaCapturePipelineResponseTypeDef = TypedDict(
     "GetMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateMediaLiveConnectorPipelineResponseTypeDef = TypedDict(
     "CreateMediaLiveConnectorPipelineResponseTypeDef",
     {
         "MediaLiveConnectorPipeline": MediaLiveConnectorPipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MediaPipelineTypeDef = TypedDict(
     "MediaPipelineTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
@@ -1313,10 +1314,10 @@
     total=False,
 )
 
 GetMediaPipelineResponseTypeDef = TypedDict(
     "GetMediaPipelineResponseTypeDef",
     {
         "MediaPipeline": MediaPipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi` & `mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -59,19 +59,19 @@
     "VideoConcatenationConfigurationTypeDef",
     "AudioArtifactsConfigurationTypeDef",
     "ContentArtifactsConfigurationTypeDef",
     "VideoArtifactsConfigurationTypeDef",
     "ChannelDefinitionTypeDef",
     "S3BucketSinkConfigurationTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     "DeleteMediaCapturePipelineRequestRequestTypeDef",
     "DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "DeleteMediaPipelineRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "TimestampRangeTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "GetMediaPipelineRequestRequestTypeDef",
     "PresenterOnlyConfigurationTypeDef",
     "IssueDetectionConfigurationTypeDef",
     "KeywordMatchConfigurationTypeDef",
@@ -87,24 +87,24 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "LiveConnectorRTMPConfigurationTypeDef",
     "S3RecordingSinkConfigurationTypeDef",
     "SnsTopicSinkConfigurationTypeDef",
     "SqsQueueSinkConfigurationTypeDef",
     "VoiceAnalyticsProcessorConfigurationTypeDef",
     "SentimentConfigurationTypeDef",
+    "ResponseMetadataTypeDef",
     "SelectedVideoStreamsTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMediaInsightsPipelineStatusRequestRequestTypeDef",
     "AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
     "ArtifactsConcatenationConfigurationTypeDef",
     "StreamChannelDefinitionTypeDef",
     "ConcatenationSinkTypeDef",
-    "TagResourceRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "FragmentSelectorTypeDef",
     "GridViewConfigurationTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     "ListMediaPipelinesResponseTypeDef",
     "LiveConnectorSinkConfigurationTypeDef",
     "RealTimeAlertRuleTypeDef",
@@ -320,25 +320,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
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
 S3RecordingSinkRuntimeConfigurationTypeDef = TypedDict(
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     {
         "Destination": str,
         "RecordingFileFormat": RecordingFileFormatType,
     },
 )
@@ -360,14 +349,21 @@
 DeleteMediaPipelineRequestRequestTypeDef = TypedDict(
     "DeleteMediaPipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TimestampRangeTypeDef = TypedDict(
     "TimestampRangeTypeDef",
     {
         "StartTimestamp": Union[datetime, str],
         "EndTimestamp": Union[datetime, str],
     },
 )
@@ -534,14 +530,15 @@
 ):
     pass
 
 S3RecordingSinkConfigurationTypeDef = TypedDict(
     "S3RecordingSinkConfigurationTypeDef",
     {
         "Destination": str,
+        "RecordingFileFormat": RecordingFileFormatType,
     },
     total=False,
 )
 
 SnsTopicSinkConfigurationTypeDef = TypedDict(
     "SnsTopicSinkConfigurationTypeDef",
     {
@@ -572,14 +569,25 @@
     {
         "RuleName": str,
         "SentimentType": Literal["NEGATIVE"],
         "TimePeriod": int,
     },
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
 SelectedVideoStreamsTypeDef = TypedDict(
     "SelectedVideoStreamsTypeDef",
     {
         "AttendeeIds": Sequence[str],
         "ExternalUserIds": Sequence[str],
     },
     total=False,
@@ -668,34 +676,27 @@
     "ConcatenationSinkTypeDef",
     {
         "Type": Literal["S3Bucket"],
         "S3BucketSinkConfiguration": S3BucketSinkConfigurationTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 FragmentSelectorTypeDef = TypedDict(
     "FragmentSelectorTypeDef",
     {
         "FragmentSelectorType": FragmentSelectorTypeType,
@@ -723,35 +724,35 @@
     pass
 
 ListMediaCapturePipelinesResponseTypeDef = TypedDict(
     "ListMediaCapturePipelinesResponseTypeDef",
     {
         "MediaCapturePipelines": List[MediaCapturePipelineSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMediaInsightsPipelineConfigurationsResponseTypeDef = TypedDict(
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     {
         "MediaInsightsPipelineConfigurations": List[
             MediaInsightsPipelineConfigurationSummaryTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListMediaPipelinesResponseTypeDef = TypedDict(
     "ListMediaPipelinesResponseTypeDef",
     {
         "MediaPipelines": List[MediaPipelineSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LiveConnectorSinkConfigurationTypeDef = TypedDict(
     "LiveConnectorSinkConfigurationTypeDef",
     {
         "SinkType": Literal["RTMP"],
@@ -1079,31 +1080,31 @@
     },
 )
 
 CreateMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "CreateMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "GetMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateMediaInsightsPipelineConfigurationResponseTypeDef = TypedDict(
     "UpdateMediaInsightsPipelineConfigurationResponseTypeDef",
     {
         "MediaInsightsPipelineConfiguration": MediaInsightsPipelineConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef",
     {
         "Sources": Sequence[ConcatenationSourceTypeDef],
@@ -1139,15 +1140,15 @@
     total=False,
 )
 
 CreateMediaInsightsPipelineResponseTypeDef = TypedDict(
     "CreateMediaInsightsPipelineResponseTypeDef",
     {
         "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
@@ -1225,39 +1226,39 @@
     total=False,
 )
 
 CreateMediaConcatenationPipelineResponseTypeDef = TypedDict(
     "CreateMediaConcatenationPipelineResponseTypeDef",
     {
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateMediaCapturePipelineResponseTypeDef = TypedDict(
     "CreateMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMediaCapturePipelineResponseTypeDef = TypedDict(
     "GetMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateMediaLiveConnectorPipelineResponseTypeDef = TypedDict(
     "CreateMediaLiveConnectorPipelineResponseTypeDef",
     {
         "MediaLiveConnectorPipeline": MediaLiveConnectorPipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MediaPipelineTypeDef = TypedDict(
     "MediaPipelineTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
@@ -1268,10 +1269,10 @@
     total=False,
 )
 
 GetMediaPipelineResponseTypeDef = TypedDict(
     "GetMediaPipelineResponseTypeDef",
     {
         "MediaPipeline": MediaPipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO` & `mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-media-pipelines
-Version: 1.26.98
-Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.26.98 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.ChimeSDKMediaPipelines 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-chime-sdk-media-pipelines"></a>
 
 # mypy-boto3-chime-sdk-media-pipelines
 
 [![PyPI - mypy-boto3-chime-sdk-media-pipelines](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-media-pipelines.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-media-pipelines)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-media-pipelines?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-media-pipelines)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMediaPipelines 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
+[boto3.ChimeSDKMediaPipelines 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
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
 [mypy-boto3-chime-sdk-media-pipelines docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_media_pipelines/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,19 +345,19 @@
     VideoConcatenationConfigurationTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
     ChannelDefinitionTypeDef,
     S3BucketSinkConfigurationTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     DeleteMediaCapturePipelineRequestRequestTypeDef,
     DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     DeleteMediaPipelineRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     TimestampRangeTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     GetMediaPipelineRequestRequestTypeDef,
     PresenterOnlyConfigurationTypeDef,
     IssueDetectionConfigurationTypeDef,
     KeywordMatchConfigurationTypeDef,
@@ -373,24 +373,24 @@
     ListTagsForResourceRequestRequestTypeDef,
     LiveConnectorRTMPConfigurationTypeDef,
     S3RecordingSinkConfigurationTypeDef,
     SnsTopicSinkConfigurationTypeDef,
     SqsQueueSinkConfigurationTypeDef,
     VoiceAnalyticsProcessorConfigurationTypeDef,
     SentimentConfigurationTypeDef,
+    ResponseMetadataTypeDef,
     SelectedVideoStreamsTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMediaInsightsPipelineStatusRequestRequestTypeDef,
     AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef,
     ArtifactsConcatenationConfigurationTypeDef,
     StreamChannelDefinitionTypeDef,
     ConcatenationSinkTypeDef,
-    TagResourceRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     FragmentSelectorTypeDef,
     GridViewConfigurationTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
     LiveConnectorSinkConfigurationTypeDef,
     RealTimeAlertRuleTypeDef,
```

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.98/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt` & `mypy-boto3-chime-sdk-media-pipelines-1.27.0/mypy_boto3_chime_sdk_media_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-media-pipelines-1.26.98/setup.py` & `mypy-boto3-chime-sdk-media-pipelines-1.27.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime-sdk-media-pipelines",
-    version="1.26.98",
+    version="1.27.0",
     packages=["mypy_boto3_chime_sdk_media_pipelines"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ChimeSDKMediaPipelines 1.26.98 service generated with"
-        " mypy-boto3-builder 7.14.2"
+        "Type annotations for boto3.ChimeSDKMediaPipelines 1.27.0 service generated with"
+        " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

