# Comparing `tmp/basictdf-0.1.4.tar.gz` & `tmp/basictdf-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basictdf-0.1.4.tar", max compression
+gzip compressed data, was "basictdf-0.1.5.tar", max compression
```

## Comparing `basictdf-0.1.4.tar` & `basictdf-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      179 2023-07-02 04:13:20.905305 basictdf-0.1.4/README.md
--rw-r--r--   0        0        0      537 2023-07-02 04:13:20.909305 basictdf-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2920 2023-07-02 04:13:20.909305 basictdf-0.1.4/src/basictdf/__init__.py
--rw-r--r--   0        0        0    17567 2023-07-02 04:13:20.909305 basictdf-0.1.4/src/basictdf/basictdf.py
--rw-r--r--   0        0        0     3440 2023-07-02 04:13:20.909305 basictdf-0.1.4/src/basictdf/tdfBlock.py
--rw-r--r--   0        0        0    12064 2023-07-02 04:13:20.909305 basictdf-0.1.4/src/basictdf/tdfCalibrationData.py
--rw-r--r--   0        0        0    12413 2023-07-02 04:13:20.909305 basictdf-0.1.4/src/basictdf/tdfData3D.py
--rw-r--r--   0        0        0     6909 2023-07-02 04:13:20.909305 basictdf-0.1.4/src/basictdf/tdfEMG.py
--rw-r--r--   0        0        0     3938 2023-07-02 04:13:20.909305 basictdf-0.1.4/src/basictdf/tdfEvents.py
--rw-r--r--   0        0        0    10720 2023-07-02 04:13:20.909305 basictdf-0.1.4/src/basictdf/tdfForce3D.py
--rw-r--r--   0        0        0     5627 2023-07-02 04:13:20.909305 basictdf-0.1.4/src/basictdf/tdfOpticalSystem.py
--rw-r--r--   0        0        0     6494 2023-07-02 04:13:20.909305 basictdf-0.1.4/src/basictdf/tdfTypes.py
--rw-r--r--   0        0        0     1434 2023-07-02 04:13:20.909305 basictdf-0.1.4/src/basictdf/tdfUtils.py
--rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 basictdf-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      321 2023-07-03 21:05:53.181489 basictdf-0.1.5/README.md
+-rw-r--r--   0        0        0      579 2023-07-03 21:05:53.185489 basictdf-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2956 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/__init__.py
+-rw-r--r--   0        0        0    17639 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/basictdf.py
+-rw-r--r--   0        0        0     3499 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/tdfBlock.py
+-rw-r--r--   0        0        0    12235 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/tdfCalibrationData.py
+-rw-r--r--   0        0        0    12413 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/tdfData3D.py
+-rw-r--r--   0        0        0     6907 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/tdfEMG.py
+-rw-r--r--   0        0        0     3938 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/tdfEvents.py
+-rw-r--r--   0        0        0    10735 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/tdfForce3D.py
+-rw-r--r--   0        0        0     7743 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/tdfForcePlatformsCalibration.py
+-rw-r--r--   0        0        0     5627 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/tdfOpticalSystem.py
+-rw-r--r--   0        0        0     6587 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/tdfTypes.py
+-rw-r--r--   0        0        0     1434 2023-07-03 21:05:53.185489 basictdf-0.1.5/src/basictdf/tdfUtils.py
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 basictdf-0.1.5/PKG-INFO
```

### Comparing `basictdf-0.1.4/src/basictdf/__init__.py` & `basictdf-0.1.5/src/basictdf/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,7 +108,8 @@
     "EMGTrack",
 ]
 
 
 __pdoc__ = {}
 __pdoc__["basictdf.tdfUtils"] = False
 __pdoc__["basictdf.tdfTypes"] = False
+__pdoc__["collections.ABC"] = False
```

### Comparing `basictdf-0.1.4/src/basictdf/basictdf.py` & `basictdf-0.1.5/src/basictdf/basictdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from basictdf.tdfBlock import (
     AnalogData,
     AnthropometricData,
     Block,
     BlockType,
     CalibrationData2D,
     Data2D,
-    ForcePlatformsCalibrationData,
     ForcePlatformsCalibrationData2D,
     ForcePlatformsData,
     GeneralCalibrationData,
     NotDefinedBlock,
     UnusedBlock,
     VolumetricData,
 )
@@ -25,14 +24,15 @@
 from basictdf.tdfOpticalSystem import OpticalSetupBlock
 from basictdf.tdfTypes import BTSDate, BTSString, i32, u32
 from basictdf.tdfUtils import (
     provide_context_if_needed,
     raise_if_outside_context,
     raise_if_outside_write_context,
 )
+from basictdf.tdfForcePlatformsCalibration import ForcePlatformsCalibrationDataBlock
 
 
 def _get_block_class(block_type: BlockType) -> Type[Block]:
     if block_type == BlockType.unusedSlot:
         return UnusedBlock
     elif block_type == BlockType.notDefined:
         return NotDefinedBlock
@@ -43,15 +43,15 @@
     elif block_type == BlockType.data2D:
         return Data2D
     elif block_type == BlockType.data3D:
         return Data3D
     elif block_type == BlockType.opticalSystemConfiguration:
         return OpticalSetupBlock
     elif block_type == BlockType.forcePlatformsCalibrationData:
-        return ForcePlatformsCalibrationData
+        return ForcePlatformsCalibrationDataBlock
     elif block_type == BlockType.forcePlatformsCalibrationData2D:
         return ForcePlatformsCalibrationData2D
     elif block_type == BlockType.forcePlatformsData:
         return ForcePlatformsData
     elif block_type == BlockType.anthropometricData:
         return AnthropometricData
     elif block_type == BlockType.electromyographicData:
@@ -90,15 +90,15 @@
         self.size = size
         self.creation_date = creation_date
         self.last_modification_date = last_modification_date
         self.last_access_date = last_access_date
         self.comment = comment
         self.nBytes = 8 * 4 + 256
 
-    def _write(self, file):
+    def _write(self, file) -> None:
         u32.bwrite(file, self.type.value)
         u32.bwrite(file, self.format)
         i32.bwrite(file, self.offset)
         i32.bwrite(file, self.size)
         BTSDate.bwrite(file, self.creation_date)
         BTSDate.bwrite(file, self.last_modification_date)
         BTSDate.bwrite(file, self.last_access_date)
@@ -144,15 +144,15 @@
 
         if not self.filePath.exists():
             raise FileNotFoundError(f"File {self.filePath} not found")
 
         self._mode = "rb"
         self._inside_context = False
 
-    def allow_write(self):
+    def allow_write(self) -> "Tdf":
         """Allow writing to the file."""
         self._mode = "r+b"
         return self
 
     def __enter__(self) -> "Tdf":
         self._inside_context = True
         self.handler: IO[bytes] = self.filePath.open(self._mode)
```

### Comparing `basictdf-0.1.4/src/basictdf/tdfBlock.py` & `basictdf-0.1.5/src/basictdf/tdfBlock.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,18 @@
     volumetricData = 13  # TDF_DATABLOCK_VOLUME
     analogData = 14  # TDF_DATABLOCK_GENPURPOSE
     generalCalibrationData = 15  # TDF_DATABLOCK_CALGENPURP
     temporalEventsData = 16  # TDF_DATABLOCK_EVENTS
 
 
 class Block(ABC):
+    """
+    A class to represent a TDF block.
+    """
+
     type = BlockType.notDefined
 
     def __init__(
         self,
         creation_date: Optional[datetime] = None,
         last_modification_date: Optional[datetime] = None,
         last_access_date: Optional[datetime] = None,
@@ -66,15 +70,15 @@
 
 class NotImplementedBlock(Block):
     type = BlockType.notDefined
 
     @classmethod
     def _build(cls, *args, **kwargs):
         raise NotImplementedError(
-            f"Buidling blocks of type {cls.type} is yet implemented"
+            f"Buidling blocks of type {cls.type} is not implemented yet"
         )
 
     def _write(self, *args, **kwargs):
         raise NotImplementedError(
             f"Writing blocks type {self.type} is not implemented yet."
         )
```

### Comparing `basictdf-0.1.4/src/basictdf/tdfCalibrationData.py` & `basictdf-0.1.5/src/basictdf/tdfCalibrationData.py`

 * *Files 3% similar despite different names*

```diff
@@ -240,14 +240,20 @@
 
     Unknown = 0
     Seelab1 = 1
     BTS = 2
 
 
 class CalibrationDataBlock(Block):
+    """
+    A class representing the Calibration Data block. This block holds
+    the calibration data for the cameras, as well as the calibration
+    volume data.
+    """
+
     type = BlockType.calibrationData
 
     def __init__(
         self,
         distorsion_model: DistorsionModel,
         calibration_volume_size: np.ndarray,
         calibration_volume_rotation_matrix: np.ndarray,
@@ -359,9 +365,9 @@
         return (
             i32.btype.itemsize  # nCams
             + i32.btype.itemsize  # DistorsionModel
             + VEC3F.btype.itemsize  # calibration_volume
             + MAT3X3F.btype.itemsize  # rotation matrix
             + VEC3F.btype.itemsize  # translation_vector
             + i16.btype.itemsize * len(self.cam_data)  # calibration map
-            + sum([cam.nBytes for cam in self.cam_data])  # calibration data
+            + sum(cam.nBytes for cam in self.cam_data)  # calibration data
         )
```

### Comparing `basictdf-0.1.4/src/basictdf/tdfData3D.py` & `basictdf-0.1.5/src/basictdf/tdfData3D.py`

 * *Files identical despite different names*

### Comparing `basictdf-0.1.4/src/basictdf/tdfEMG.py` & `basictdf-0.1.5/src/basictdf/tdfEMG.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class EMGBlockFormat(Enum):
     unknownFormat = 0
     byTrack = 1
     byFrame = 2
 
 
 class EMGTrack:
-    def __init__(self, label: str, trackData: np.ndarray):
+    def __init__(self, label: str, trackData: np.ndarray) -> None:
         self.label = label
         self.data = trackData
 
     @property
     def nSamples(self) -> int:
         """
         Returns:
@@ -33,26 +33,26 @@
 
     @property
     def _segments(self):
         maskedTrackData = np.ma.masked_invalid(self.data)
         return np.ma.clump_unmasked(maskedTrackData.T)
 
     @staticmethod
-    def build(stream, nSamples):
+    def build(stream, nSamples) -> "EMGTrack":
         label = BTSString.bread(stream, 256)
         nSegments = i32.bread(stream)
         i32.skip(stream)  # padding
         segmentData = SegmentData.bread(stream, nSegments)
         trackData = np.empty(nSamples, dtype="<f4")
         trackData[:] = np.nan
         for startFrame, nFrames in segmentData:
             trackData[startFrame : startFrame + nFrames] = f32.bread(stream, nFrames)
         return EMGTrack(label, trackData)
 
-    def write(self, file):
+    def write(self, file) -> None:
         # label
         BTSString.bwrite(file, 256, self.label)
 
         segments = self._segments
 
         # nSegments
         i32.bwrite(file, len(segments))
@@ -76,54 +76,53 @@
         for segment in self._segments:
             base += 4 + 4 + (segment.stop - segment.start) * f32.btype.itemsize
         return base
 
     def __eq__(self, other):
         return self.label == other.label and np.all(self.data == other.data)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (
             f"EMGTrack(label={self.label}, nSamples={self.nSamples},"
             f"segments={len(self._segments)})"
         )
 
 
 class EMG(Block):
     """Electromyography data block"""
 
     type = BlockType.electromyographicData
 
-    def __init__(self, frequency, nSamples, startTime=0.0):
+    def __init__(self, frequency, nSamples, startTime=0.0) -> None:
         super().__init__()
         self.frequency = frequency
         self.startTime = startTime
         self.nSamples = nSamples
         self._signals = []
         self._emgMap = []
 
     @staticmethod
-    def _build(stream, format):
+    def _build(stream, format) -> "EMG":
         format = EMGBlockFormat(format)
         nSignals = i32.bread(stream)
         frequency = i32.bread(stream)
         startTime = f32.bread(stream)
         nSamples = i32.bread(stream) + 49  # Why 49??? Whyyyy????
         emgMap = i16.bread(stream, n=nSignals)
 
         d = EMG(frequency, nSamples, startTime)
         if format == EMGBlockFormat.byTrack:
-            # d._signals = [EMGTrack.build(stream, nSamples) for _ in range(nSignals)]
             for n in range(nSignals):
                 emgSignal = EMGTrack.build(stream, nSamples)
                 d.addSignal(emgSignal, channel=emgMap[n])
         else:
             raise NotImplementedError(f"EMG format {format} not implemented yet")
         return d
 
-    def _write(self, file):
+    def _write(self, file) -> None:
         if self.format != EMGBlockFormat.byTrack:
             raise NotImplementedError(f"EMG format {self.format} not implemented yet")
 
         # nSignals
         i32.bwrite(file, len(self._signals))
 
         # frequency
@@ -168,15 +167,15 @@
     def __eq__(self, other) -> bool:
         buff1 = BytesIO()
         buff2 = BytesIO()
         self.write(buff1)
         other.write(buff2)
         return buff1.getvalue() == buff2.getvalue()
 
-    def addSignal(self, signal: EMGTrack, channel=None):
+    def addSignal(self, signal: EMGTrack, channel=None) -> None:
         """
         adds a signal to the EMG block. If the channel is not specified,
         it is set to the next one  available
         """
         if not isinstance(signal, EMGTrack):
             raise TypeError(f"Can only add EMGTrack objects, got {type(signal)}")
         if signal.nSamples != self.nSamples:
@@ -195,15 +194,15 @@
             self._emgMap.append(next_channel)
         else:
             if channel in self._emgMap:
                 raise ValueError(f"Channel {channel} already in use")
             self._emgMap.append(channel)
         self._signals.append(signal)
 
-    def removeSignal(self, label: str):
+    def removeSignal(self, label: str) -> None:
         try:
             pos = next(i for i, v in enumerate(self._signals) if v == label)
         except StopIteration:
             raise KeyError(f"EMG signal with label {label} not found")
 
         del self._signals[pos]
         del self._emgMap[pos]
@@ -215,12 +214,12 @@
             base += signal.nBytes
         return base
 
     @property
     def nSignals(self) -> int:
         return len(self._signals)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (
             f"EMGBlock(frequency={self.frequency}, nSamples={self.nSamples}, "
             f"nSignals={self.nSignals}, startTime={self.startTime},)"
         )
```

### Comparing `basictdf-0.1.4/src/basictdf/tdfEvents.py` & `basictdf-0.1.5/src/basictdf/tdfEvents.py`

 * *Files identical despite different names*

### Comparing `basictdf-0.1.4/src/basictdf/tdfForce3D.py` & `basictdf-0.1.5/src/basictdf/tdfForce3D.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,15 +316,15 @@
             + VEC3F.btype.itemsize
             + 4
         )
         for track in self._tracks:
             base += track.nBytes
         return base
 
-    def _write(self, file):
+    def _write(self, file) -> None:
         if self.format != ForceTorque3DBlockFormat.byTrack:
             raise NotImplementedError(
                 f"Force3D format {self.format} not implemented yet"
             )
         # nFrames
         i32.bwrite(file, self.nFrames)
 
@@ -344,12 +344,12 @@
 
         # padding
         i32.bpad(file)
 
         for track in self._tracks:
             track._write(file)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (
             f"<ForceTorque3D: {self.nFrames} frames, {self.frequency} Hz, "
             f"{self.nTracks} tracks, tracks={[i.label for i in self._tracks]}>"
         )
```

### Comparing `basictdf-0.1.4/src/basictdf/tdfOpticalSystem.py` & `basictdf-0.1.5/src/basictdf/tdfOpticalSystem.py`

 * *Files identical despite different names*

### Comparing `basictdf-0.1.4/src/basictdf/tdfTypes.py` & `basictdf-0.1.5/src/basictdf/tdfTypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,17 @@
             return la.decode(encoding)
 
     @staticmethod
     def write(size: int, data: str) -> bytes:
         dat = data.encode("windows-1252") + b"\x00"
         padding = b"\x00" * (size - len(dat))
         if len(dat) > size:
-            raise ValueError(f"data is too long for {size}")
+            raise ValueError(
+                f"The string is too long: max {size} chars, got {len(dat)}"
+            )
         return dat + padding
 
     @staticmethod
     def bwrite(file: BinaryIO, size: int, data: str) -> None:
         file.write(BTSString.write(size, data))
 
     @staticmethod
@@ -142,14 +144,15 @@
 
 Volume = TdfType(np.dtype("3<f4"))
 
 VEC3F = TdfType(np.dtype("3<f4"))
 VEC3D = TdfType(np.dtype("3<f8"))
 
 VEC2I = TdfType(np.dtype("2<i4"))
+VEC2F = TdfType(np.dtype("2<f4"))
 VEC2D = TdfType(np.dtype("2<f8"))
 
 MAT3X3F = TdfType(np.dtype("(3,3)<f4"))
 MAT3X3D = TdfType(np.dtype("(3,3)<f8"))
 
 i32 = TdfType(np.dtype("<i4"))
 i16 = TdfType(np.dtype("<i2"))
```

### Comparing `basictdf-0.1.4/src/basictdf/tdfUtils.py` & `basictdf-0.1.5/src/basictdf/tdfUtils.py`

 * *Files identical despite different names*

### Comparing `basictdf-0.1.4/PKG-INFO` & `basictdf-0.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basictdf
-Version: 0.1.4
+Version: 0.1.5
 Summary: A basic TDF parser
 Author: Marcos A. Núñez
 Author-email: silver94@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -13,10 +13,11 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.20,<2.0)
 Description-Content-Type: text/markdown
 
 # basictdf
 
 ![example workflow](https://github.com/marnunez/basictdf/actions/workflows/test.yml/badge.svg)
+[![codecov](https://codecov.io/gh/marnunez/basictdf/branch/master/graph/badge.svg?token=7BP5TOHNBF)](https://codecov.io/gh/marnunez/basictdf)
 
 A read/write binary parser for the BTS Bioengineering TDF data format.
```

