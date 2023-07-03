# Comparing `tmp/aliyun-python-sdk-ocr-1.0.8.tar.gz` & `tmp/aliyun-python-sdk-ocr-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-ocr-1.0.8.tar", last modified: Tue Aug  4 08:26:39 2020, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-ocr-1.0.9.tar", last modified: Fri Nov 13 06:20:24 2020, max compression
```

## Comparing `aliyun-python-sdk-ocr-1.0.8.tar` & `aliyun-python-sdk-ocr-1.0.9.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/
--rw-rw-r--   0 admin     (1017) admin     (1017)       21 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/__init__.py
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/
--rw-rw-r--   0 admin     (1017) admin     (1017)     1438 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeAccountPageRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1580 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeDrivingLicenseRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1578 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeDriverLicenseRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1438 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizePassportMRZRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1448 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeVerificationcodeRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1440 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeLicensePlateRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)        0 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/__init__.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1440 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeTakeoutOrderRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2358 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeTableRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1576 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeIdentityCardRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1748 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/TrimDocumentRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1438 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeTrainTicketRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1814 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeCharacterRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1442 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeChinapassportRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1440 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeBusinessCardRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1430 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeVINCodeRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1426 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeStampRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1446 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeBusinessLicenseRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1563 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeQrCodeRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1414 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/GetAsyncJobResultRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1590 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeVATInvoiceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1432 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeBankCardRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1438 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeTaxiInvoiceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)        0 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/__init__.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1088 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/endpoint.py
--rw-rw-r--   0 admin     (1017) admin     (1017)        0 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/MANIFEST.in
--rw-rw-r--   0 admin     (1017) admin     (1017)       38 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/setup.cfg
--rw-rw-r--   0 admin     (1017) admin     (1017)      527 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/README.rst
--rw-rw-r--   0 admin     (1017) admin     (1017)     1537 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/PKG-INFO
--rw-rw-r--   0 admin     (1017) admin     (1017)     2452 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/setup.py
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyun_python_sdk_ocr.egg-info/
--rw-rw-r--   0 admin     (1017) admin     (1017)        1 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyun_python_sdk_ocr.egg-info/dependency_links.txt
--rw-rw-r--   0 admin     (1017) admin     (1017)       13 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyun_python_sdk_ocr.egg-info/top_level.txt
--rw-rw-r--   0 admin     (1017) admin     (1017)       31 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyun_python_sdk_ocr.egg-info/requires.txt
--rw-rw-r--   0 admin     (1017) admin     (1017)     1727 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyun_python_sdk_ocr.egg-info/SOURCES.txt
--rw-rw-r--   0 admin     (1017) admin     (1017)     1537 2020-08-04 08:26:39.000000 aliyun-python-sdk-ocr-1.0.8/aliyun_python_sdk_ocr.egg-info/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1537 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyun_python_sdk_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1537 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyun_python_sdk_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1847 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyun_python_sdk_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyun_python_sdk_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyun_python_sdk_ocr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyun_python_sdk_ocr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/
+-rw-r--r--   0 root         (0) root         (0)       21 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/
+-rw-r--r--   0 root         (0) root         (0)     1438 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/DetectCardScreenshotRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1414 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/GetAsyncJobResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeAccountPageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1432 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeBankCardRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeBusinessCardRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1446 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeBusinessLicenseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeCharacterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeChinapassportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeDriverLicenseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1580 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeDrivingLicenseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeIdentityCardRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeLicensePlateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizePassportMRZRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizePoiNameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1562 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeQrCodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeStampRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeTableRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeTakeoutOrderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeTaxiInvoiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeTrainTicketRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeVATInvoiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeVINCodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeVerificationcodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/TrimDocumentRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2452 2020-11-13 06:20:24.000000 aliyun-python-sdk-ocr-1.0.9/setup.py
```

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeAccountPageRequest.py` & `aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeAccountPageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeDrivingLicenseRequest.py` & `aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeDrivingLicenseRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeDriverLicenseRequest.py` & `aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeDriverLicenseRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizePassportMRZRequest.py` & `aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizePassportMRZRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeVerificationcodeRequest.py` & `aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeVerificationcodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeLicensePlateRequest.py` & `aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeLicensePlateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeTakeoutOrderRequest.py` & `aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeTakeoutOrderRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeTableRequest.py` & `aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeTableRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeIdentityCardRequest.py` & `aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeIdentityCardRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/TrimDocumentRequest.py` & `aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/TrimDocumentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeTrainTicketRequest.py` & `aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeTrainTicketRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeCharacterRequest.py` & `aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeCharacterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeChinapassportRequest.py` & `aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeChinapassportRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeBusinessCardRequest.py` & `aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeBusinessCardRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeVINCodeRequest.py` & `aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeVINCodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeStampRequest.py` & `aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeStampRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeBusinessLicenseRequest.py` & `aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeBusinessLicenseRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeQrCodeRequest.py` & `aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeQrCodeRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,13 +28,13 @@
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_Taskss(self):
-		return self.get_body_params().get('Taskss')
+		return self.get_body_params().get('Tasks')
 
 	def set_Taskss(self, Taskss):
 		for depth1 in range(len(Taskss)):
 			if Taskss[depth1].get('ImageURL') is not None:
 				self.add_body_params('Tasks.' + str(depth1 + 1) + '.ImageURL', Taskss[depth1].get('ImageURL'))
```

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/GetAsyncJobResultRequest.py` & `aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/GetAsyncJobResultRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeVATInvoiceRequest.py` & `aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeVATInvoiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeBankCardRequest.py` & `aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeBankCardRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/request/v20191230/RecognizeTaxiInvoiceRequest.py` & `aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/request/v20191230/RecognizeTaxiInvoiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyunsdkocr/endpoint.py` & `aliyun-python-sdk-ocr-1.0.9/aliyunsdkocr/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/README.rst` & `aliyun-python-sdk-ocr-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/PKG-INFO` & `aliyun-python-sdk-ocr-1.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-ocr
-Version: 1.0.8
+Version: 1.0.9
 Summary: The ocr module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-ocr
```

### Comparing `aliyun-python-sdk-ocr-1.0.8/setup.py` & `aliyun-python-sdk-ocr-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyun_python_sdk_ocr.egg-info/SOURCES.txt` & `aliyun-python-sdk-ocr-1.0.9/aliyun_python_sdk_ocr.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,26 +5,28 @@
 aliyun_python_sdk_ocr.egg-info/SOURCES.txt
 aliyun_python_sdk_ocr.egg-info/dependency_links.txt
 aliyun_python_sdk_ocr.egg-info/requires.txt
 aliyun_python_sdk_ocr.egg-info/top_level.txt
 aliyunsdkocr/__init__.py
 aliyunsdkocr/endpoint.py
 aliyunsdkocr/request/__init__.py
+aliyunsdkocr/request/v20191230/DetectCardScreenshotRequest.py
 aliyunsdkocr/request/v20191230/GetAsyncJobResultRequest.py
 aliyunsdkocr/request/v20191230/RecognizeAccountPageRequest.py
 aliyunsdkocr/request/v20191230/RecognizeBankCardRequest.py
 aliyunsdkocr/request/v20191230/RecognizeBusinessCardRequest.py
 aliyunsdkocr/request/v20191230/RecognizeBusinessLicenseRequest.py
 aliyunsdkocr/request/v20191230/RecognizeCharacterRequest.py
 aliyunsdkocr/request/v20191230/RecognizeChinapassportRequest.py
 aliyunsdkocr/request/v20191230/RecognizeDriverLicenseRequest.py
 aliyunsdkocr/request/v20191230/RecognizeDrivingLicenseRequest.py
 aliyunsdkocr/request/v20191230/RecognizeIdentityCardRequest.py
 aliyunsdkocr/request/v20191230/RecognizeLicensePlateRequest.py
 aliyunsdkocr/request/v20191230/RecognizePassportMRZRequest.py
+aliyunsdkocr/request/v20191230/RecognizePoiNameRequest.py
 aliyunsdkocr/request/v20191230/RecognizeQrCodeRequest.py
 aliyunsdkocr/request/v20191230/RecognizeStampRequest.py
 aliyunsdkocr/request/v20191230/RecognizeTableRequest.py
 aliyunsdkocr/request/v20191230/RecognizeTakeoutOrderRequest.py
 aliyunsdkocr/request/v20191230/RecognizeTaxiInvoiceRequest.py
 aliyunsdkocr/request/v20191230/RecognizeTrainTicketRequest.py
 aliyunsdkocr/request/v20191230/RecognizeVATInvoiceRequest.py
```

### Comparing `aliyun-python-sdk-ocr-1.0.8/aliyun_python_sdk_ocr.egg-info/PKG-INFO` & `aliyun-python-sdk-ocr-1.0.9/aliyun_python_sdk_ocr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-ocr
-Version: 1.0.8
+Version: 1.0.9
 Summary: The ocr module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-ocr
```

