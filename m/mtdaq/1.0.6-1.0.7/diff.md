# Comparing `tmp/mtdaq-1.0.6-py3-none-any.whl.zip` & `tmp/mtdaq-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3840 bytes, number of entries: 7
+Zip file size: 3755 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat      106 b- defN 23-Mar-09 02:34 mtdaq/__init__.py
--rw-rw-rw-  2.0 fat     8840 b- defN 23-Apr-03 03:17 mtdaq/mtdaq.py
--rw-rw-rw-  2.0 fat      192 b- defN 23-Apr-03 03:22 mtdaq-1.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-03 03:22 mtdaq-1.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-03 03:22 mtdaq-1.0.6.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Feb-21 07:19 mtdaq-1.0.6.dist-info/zip-safe
-?rw-rw-r--  2.0 fat      516 b- defN 23-Apr-03 03:22 mtdaq-1.0.6.dist-info/RECORD
-7 files, 9754 bytes uncompressed, 2924 bytes compressed:  70.0%
+-rw-rw-rw-  2.0 fat     8654 b- defN 23-Jul-03 07:17 mtdaq/mtdaq.py
+-rw-rw-rw-  2.0 fat      192 b- defN 23-Jul-03 07:20 mtdaq-1.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-03 07:20 mtdaq-1.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Jul-03 07:20 mtdaq-1.0.7.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Feb-21 07:19 mtdaq-1.0.7.dist-info/zip-safe
+?rw-rw-r--  2.0 fat      516 b- defN 23-Jul-03 07:20 mtdaq-1.0.7.dist-info/RECORD
+7 files, 9568 bytes uncompressed, 2839 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: mtdaq/__init__.py
 Comment: 
 
 Filename: mtdaq/mtdaq.py
 Comment: 
 
-Filename: mtdaq-1.0.6.dist-info/METADATA
+Filename: mtdaq-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: mtdaq-1.0.6.dist-info/WHEEL
+Filename: mtdaq-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: mtdaq-1.0.6.dist-info/top_level.txt
+Filename: mtdaq-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: mtdaq-1.0.6.dist-info/zip-safe
+Filename: mtdaq-1.0.7.dist-info/zip-safe
 Comment: 
 
-Filename: mtdaq-1.0.6.dist-info/RECORD
+Filename: mtdaq-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mtdaq/mtdaq.py

```diff
@@ -1,22 +1,20 @@
 # -*- coding: utf-8 -*-
 
 from ctypes import *
 import platform
 import os
-from itertools import chain
-
 
 system = platform.system()
 bit = platform.architecture()
 if system == 'Windows': #Win
     if bit[0] == '32bit':
-        dllpath = os.getenv('SystemDrive')+r'\ProgramData\MangoTree\DLL\x86\MTDAQ_x86.dll'
+        dllpath = os.getenv('SystemDrive') + r'\ProgramData\MangoTree\DLL\x86\MTDAQ_x86.dll'
     elif bit[0] == '64bit':
-        dllpath = os.getenv('SystemDrive')+r'\ProgramData\MangoTree\DLL\x64\MTDAQ_x64.dll'
+        dllpath = os.getenv('SystemDrive') + r'\ProgramData\MangoTree\DLL\x64\MTDAQ_x64.dll'
 elif system == 'Darwin': #MacOS
     if bit[0] == '64bit':
         dllpath = r'/Library/Application Support/MangoTree/DLL/MTDAQ.framework/MTDAQ'
     else:
         raise Exception("Python 64-bit Required on MacOS.")
 elif system == "Linux": #Linux
     if bit[0] == '64bit':
@@ -94,42 +92,35 @@
     
 def _data_ci(task, samples, timeout):
     ctype_ci = c_float * samples
     dll.MTDAQ_ReadCI.argtypes = [c_char_p, c_uint32, c_int32, ctype_ci, c_int32]
     c_cidata = ctype_ci()
     dll.MTDAQ_ReadCI(task, c_uint32(samples), timeout, c_cidata, samples)
     return c_cidata    
-    
-def _data_pwm(task, pwmconfig):
-    _pwmconfig = list(chain.from_iterable(pwmconfig))
-    _len = len(_pwmconfig)
-    if _len % 3 != 0:
-        raise Exception("PWM Config Error.")
-    chnum = _len // 3
-    ctype_pwm = c_float * chnum
-    dll.MTDAQ_WritePWM.argtypes = [c_char_p, ctype_pwm, ctype_pwm, ctype_pwm, c_int32]
-    c_frequency = ctype_pwm(_pwmconfig[0::3])
-    c_dutycircle = ctype_pwm(_pwmconfig[1::3])
-    c_count = ctype_pwm(_pwmconfig[2::3])
-    dll.MTDAQ_WritePWM(task, c_frequency, c_dutycircle, c_count, chnum)
+#todo    
+def _data_pwm(task, count):
+    ctype_pwm = c_float * count
+    dll.MTDAQ_WritePWM.argtypes = [c_char_p, c_float]
+    dll.MTDAQ_WritePWM(task, c_float(count))
     
 def _data_encoder(task, samples, channel_num, timeout):
     datalen = samples * channel_num * 2
     ctype_encoder = c_int32 * datalen
     dll.MTDAQ_ReadEncoder.argtypes = [c_char_p, c_uint32, c_int32, ctype_encoder, c_int32]
     c_encoderdata = ctype_encoder()
     dll.MTDAQ_ReadEncoder(task, c_uint32(datalen), timeout, c_encoderdata, datalen)
     return c_encoderdata
     
-def _data_rtd(task, channel_num):
-    ctype_rtd = c_doule * channel_num
-    dll.MTDAQ_ReadRTD.argtypes = [c_char_p, ctype_rtd, c_int32]
-    c_rtd = ctype_rtd()
-    dll.MTDAQ_ReadRTD(task, c_rtd, channel_num)
-    return c_rtd
+def _data_temperature(task, channel_num):
+    ctype_temp = c_doule * channel_num 
+    dll.MTDAQ_ReadTemp.argtypes = [c_char_p, ctype_temp, POINTER(c_float), c_int32]
+    c_temp = ctype_temp()
+    c_cjc = c_float()
+    dll.MTDAQ_ReadTemp(task, c_temp, pointer(c_cjc), channel_num)
+    return c_temp, c_cjc
     
 def _get_channel_num(task, channel_name):
     chnnel_num_dict = {
         "AI": 0,
         "AO": 1,
         "HSDI": 2,
         "HSDO": 3,
@@ -197,51 +188,85 @@
         self._run = True
         
     def close(self):
         _dev_close(self._task)
         self._run = False
     
     @is_running
-    def ai(self, samples, timeout=2500):
+    def analogRead(self, samples, timeout=2500):
         if "AI" not in self._chnum.keys():
             self._chnum["AI"] = _get_channel_num(self._task, "AI")
         return _data_ai(self._task, samples, self._chnum["AI"], timeout)
     
     @is_running
-    def ao(self, aodata, timeout=2500):
-        return _data_ao(self._task, aodata, timeout)
+    def analogWrite(self, aodata, timeout=2500):
+        _data_ao(self._task, aodata, timeout)
     
     @is_running
-    def lowspeed_di(self):
+    def digitalRead(self):
         return _data_ldi(self._task)
     
     @is_running
-    def lowspeed_do(self, ldodata):
-        return _data_ldo(self._task, ldodata)
+    def digitalWrite(self, dodata):
+        _data_ldo(self._task, dodata)
     
     @is_running
-    def highspeed_di(self, samples, timeout=2500):
+    def digitalWaveformRead(self, samples, timeout=2500):
         return _data_hdi(self._task, samples, timeout)
     
     @is_running
-    def highspeed_do(self, hdodata, timeout=2500):
-        return _data_hdo(self._task, hdodata, timeout)
+    def digitalWaveformWrite(self, dodata, timeout=2500):
+        _data_hdo(self._task, dodata, timeout)
         
     @is_running
-    def ci(self, samples, timeout=2500):
+    def counterRead(self, samples, timeout=2500):
         return _data_ci(self._task, samples, timeout)
     
     @is_running
-    def pwm(self, pwmconfig):
-        return _data_pwm(self._task, pwmconfig)
+    def pwmWrite(self, count):
+        return _data_pwm(self._task, count)
     
     @is_running
-    def encoder(self, samples, timeout=2500):
+    def encoderRead(self, samples, timeout=2500):
         if "Encoder" not in self._chnum.keys():
             self._chnum["Encoder"] = _get_channel_num(self._task, "Encoder")
         return _data_ai(self._task, samples, self._chnum["Encoder"])
     
     @is_running
-    def rtd(self):
+    def temperatureRead(self):
         if "AI" not in self._chnum.keys():
             self._chnum["AI"] = _get_channel_num(self._task, "AI")
-        return _data_rtd(self._task, self._chnum["AI"])
+        return _data_temperature(self._task, self._chnum["AI"])
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+    
+    
+    
+    
+    
+    
+
```

## Comparing `mtdaq-1.0.6.dist-info/RECORD` & `mtdaq-1.0.7.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 mtdaq/__init__.py,sha256=RJj86tAfgKB2nBXrmMyUKbNEPRtxMUjJzHwKRL8HdbU,106
-mtdaq/mtdaq.py,sha256=OOqw44FCQR9yRy2-3iuSiruvvaNcAUaNk574bvPSPdo,8840
-mtdaq-1.0.6.dist-info/METADATA,sha256=cwhvenWx9AbqVF5Ji34skkVsiP6ow5Qx6NviPw4w50g,192
-mtdaq-1.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mtdaq-1.0.6.dist-info/top_level.txt,sha256=Bd3sAd8aoKE6GZpMmtu8pFnacN7MS9HO-IJStPxyUHw,6
-mtdaq-1.0.6.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-mtdaq-1.0.6.dist-info/RECORD,,
+mtdaq/mtdaq.py,sha256=FiKkPKXdgx7Rn1F80iNU4e_KklOpXnNXKXgQ_gOdfVk,8654
+mtdaq-1.0.7.dist-info/METADATA,sha256=sAiLkv_cxGU9XS1ohgm7CCGFRA9k1Be66DuLjwkhu48,192
+mtdaq-1.0.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+mtdaq-1.0.7.dist-info/top_level.txt,sha256=Bd3sAd8aoKE6GZpMmtu8pFnacN7MS9HO-IJStPxyUHw,6
+mtdaq-1.0.7.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+mtdaq-1.0.7.dist-info/RECORD,,
```

