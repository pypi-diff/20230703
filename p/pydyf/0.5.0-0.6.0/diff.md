# Comparing `tmp/pydyf-0.5.0.tar.gz` & `tmp/pydyf-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydyf-0.5.0.tar", last modified: Tue Oct 11 14:12:34 2022, max compression
+gzip compressed data, was "pydyf-0.6.0.tar", last modified: Wed Mar 29 19:48:55 2023, max compression
```

## Comparing `pydyf-0.5.0.tar` & `pydyf-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1521 2020-10-23 10:08:11.789280 pydyf-0.5.0/LICENSE
--rw-r--r--   0        0        0      866 2022-04-24 06:04:00.881657 pydyf-0.5.0/README.rst
--rw-r--r--   0        0        0      224 2020-12-06 18:47:25.896394 pydyf-0.5.0/docs/api_reference.rst
--rw-r--r--   0        0        0     4760 2022-10-11 14:06:24.923553 pydyf-0.5.0/docs/changelog.rst
--rw-r--r--   0        0        0     4355 2020-12-06 18:47:25.896394 pydyf-0.5.0/docs/common_use_cases.rst
--rw-r--r--   0        0        0     2660 2021-12-27 12:07:06.627084 pydyf-0.5.0/docs/conf.py
--rw-r--r--   0        0        0     2086 2022-09-19 07:09:14.775515 pydyf-0.5.0/docs/contribute.rst
--rw-r--r--   0        0        0      758 2020-12-06 18:47:25.897394 pydyf-0.5.0/docs/first_steps.rst
--rw-r--r--   0        0        0     1032 2022-04-25 11:13:06.410209 pydyf-0.5.0/docs/going_further.rst
--rw-r--r--   0        0        0      296 2020-12-06 18:47:25.897394 pydyf-0.5.0/docs/index.rst
--rw-r--r--   0        0        0      884 2020-12-06 18:47:25.897394 pydyf-0.5.0/docs/support.rst
--rwxr-xr-x   0        0        0    17386 2022-10-11 14:03:43.788010 pydyf-0.5.0/pydyf/__init__.py
--rw-r--r--   0        0        0     1826 2022-09-19 08:20:58.063255 pydyf-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2945 2022-04-23 22:14:02.282916 pydyf-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0    15742 2022-05-22 16:50:31.356023 pydyf-0.5.0/tests/test_pydyf.py
--rw-r--r--   0        0        0     2500 1970-01-01 00:00:00.000000 pydyf-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1521 2020-10-23 10:08:11.789280 pydyf-0.6.0/LICENSE
+-rw-r--r--   0        0        0      866 2022-04-24 06:04:00.881657 pydyf-0.6.0/README.rst
+-rw-r--r--   0        0        0      312 2023-03-29 18:08:19.213027 pydyf-0.6.0/docs/api_reference.rst
+-rw-r--r--   0        0        0     5293 2023-03-29 19:47:15.466918 pydyf-0.6.0/docs/changelog.rst
+-rw-r--r--   0        0        0     4389 2023-03-29 18:08:19.214027 pydyf-0.6.0/docs/common_use_cases.rst
+-rw-r--r--   0        0        0     2660 2021-12-27 12:07:06.627084 pydyf-0.6.0/docs/conf.py
+-rw-r--r--   0        0        0     2086 2022-09-19 07:09:14.775515 pydyf-0.6.0/docs/contribute.rst
+-rw-r--r--   0        0        0      758 2020-12-06 18:47:25.897394 pydyf-0.6.0/docs/first_steps.rst
+-rw-r--r--   0        0        0     1032 2022-04-25 11:13:06.410209 pydyf-0.6.0/docs/going_further.rst
+-rw-r--r--   0        0        0      296 2020-12-06 18:47:25.897394 pydyf-0.6.0/docs/index.rst
+-rw-r--r--   0        0        0      884 2020-12-06 18:47:25.897394 pydyf-0.6.0/docs/support.rst
+-rwxr-xr-x   0        0        0    20915 2023-03-29 19:31:01.352578 pydyf-0.6.0/pydyf/__init__.py
+-rw-r--r--   0        0        0     1826 2022-09-19 08:20:58.063255 pydyf-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2945 2022-04-23 22:14:02.282916 pydyf-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0    15742 2022-05-22 16:50:31.356023 pydyf-0.6.0/tests/test_pydyf.py
+-rw-r--r--   0        0        0     2500 1970-01-01 00:00:00.000000 pydyf-0.6.0/PKG-INFO
```

### Comparing `pydyf-0.5.0/LICENSE` & `pydyf-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydyf-0.5.0/README.rst` & `pydyf-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `pydyf-0.5.0/docs/changelog.rst` & `pydyf-0.6.0/docs/changelog.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,54 @@
 Changelog
 =========
 
 
+Version 0.6.0
+-------------
+
+Released on 2023-03-29.
+
+New features:
+
+* Add an option to use compressed object streams for PDF 1.5+, with financial support from Code & Co.
+* Add new text operators
+* Clean and fix documentation
+
+Backers and sponsors:
+
+* Kobalt
+* Grip Angebotssoftware
+* Spacinov
+* Crisp BV
+* Castedo Ellerman
+* Manuel Barkhau
+* SimonSoft
+* Menutech
+* KontextWork
+* NCC Group
+* René Fritz
+* Moritz Mahringer
+* Yanal-Yvez Fargialla
+* Piotr Horzycki
+* Healthchecks.io
+* Hammerbacher
+* TrainingSparkle
+* Synapsium
+
+
+
 Version 0.5.0
 -------------
 
 Released on 2022-10-11.
 
 New features:
 
 * Add the PDF.page_references property
-* Revert the PDF.pages['Kids'] behavior to be retro-compatible with version 0.3.0
+* Revert the PDF.pages['Kids'] behavior to be backwards compatible with version 0.3.0
 
 Backers and sponsors:
 
 * Grip Angebotssoftware
 * Manuel Barkhau
 * Crisp BV
 * SimonSoft
```

### Comparing `pydyf-0.5.0/docs/common_use_cases.rst` & `pydyf-0.6.0/docs/common_use_cases.rst`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
 .. code-block:: python
 
    import pydyf
 
    document = pydyf.PDF()
 
-   extra = Dictionary({
+   extra = pydyf.Dictionary({
        'Type': '/XObject',
        'Subtype': '/Image',
        'Width': 197,
        'Height': 101,
        'ColorSpace': '/DeviceRGB',
        'BitsPerComponent': 8,
        'Filter': '/DCTDecode',
@@ -154,17 +154,17 @@
   document.add_object(font)
 
   # Set the font use for the text
   # Move to where to display the text
   # And display it
   text = pydyf.Stream()
   text.begin_text()
-  text.set_font_size('F1', 24)
+  text.set_font_size('F1', 20)
   text.text_matrix(1, 0, 0, 1, 10, 90)
-  text.show_text(pydyf.String('Hello World'))
+  text.show_text(pydyf.String('Bœuf grillé & café'.encode('macroman')))
   text.end_text()
 
   document.add_object(text)
 
   # Put the font in the resources of the PDF
   document.add_page(pydyf.Dictionary({
       'Type': '/Page',
@@ -175,8 +175,7 @@
           'ProcSet': pydyf.Array(['/PDF', '/Text']),
           'Font': pydyf.Dictionary({'F1': font.reference}),
       })
   }))
 
   with open('document.pdf', 'wb') as f:
       document.write(f)
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pydyf-0.5.0/docs/conf.py` & `pydyf-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pydyf-0.5.0/docs/contribute.rst` & `pydyf-0.6.0/docs/contribute.rst`

 * *Files identical despite different names*

### Comparing `pydyf-0.5.0/docs/first_steps.rst` & `pydyf-0.6.0/docs/first_steps.rst`

 * *Files identical despite different names*

### Comparing `pydyf-0.5.0/docs/going_further.rst` & `pydyf-0.6.0/docs/going_further.rst`

 * *Files identical despite different names*

### Comparing `pydyf-0.5.0/docs/support.rst` & `pydyf-0.6.0/docs/support.rst`

 * *Files identical despite different names*

### Comparing `pydyf-0.5.0/pydyf/__init__.py` & `pydyf-0.6.0/pydyf/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 
 """
 
 import re
 import zlib
 from codecs import BOM_UTF16_BE
 from hashlib import md5
+from math import ceil, log
 
-VERSION = __version__ = '0.5.0'
+VERSION = __version__ = '0.6.0'
 
 
 def _to_bytes(item):
     """Convert item to bytes."""
     if isinstance(item, bytes):
         return item
     elif isinstance(item, Object):
         return item.data
     elif isinstance(item, float):
         if item.is_integer():
             return f'{int(item):d}'.encode('ascii')
         else:
-            return f'{item:f}'.encode('ascii')
+            return f'{item:f}'.rstrip('0').encode('ascii')
     elif isinstance(item, int):
         return f'{item:d}'.encode('ascii')
     return str(item).encode('ascii')
 
 
 class Object:
     """Base class for PDF objects."""
@@ -39,59 +40,49 @@
         #: Indicate if an object is used (``'n'``), or has been deleted
         #: and therefore is free (``'f'``).
         self.free = 'n'
 
     @property
     def indirect(self):
         """Indirect representation of an object."""
-        return b'\n'.join((
-            str(self.number).encode() + b' ' +
-            str(self.generation).encode() + b' obj',
-            self.data,
-            b'endobj',
-        ))
+        header = f'{self.number} {self.generation} obj\n'.encode()
+        return header + self.data + b'\nendobj'
 
     @property
     def reference(self):
         """Object identifier."""
-        return (
-            str(self.number).encode() + b' ' +
-            str(self.generation).encode() + b' R')
+        return f'{self.number} {self.generation} R'.encode()
 
     @property
     def data(self):
         """Data contained in the object. Shall be defined in each subclass."""
         raise NotImplementedError()
 
+    @property
+    def compressible(self):
+        """Whether the object can be included in an object stream."""
+        return not self.generation and not isinstance(self, Stream)
 
-class Dictionary(Object, dict):
-    """PDF Dictionary object.
-
-    Inherits from :class:`Object` and Python :obj:`dict`.
 
-    """
+class Dictionary(Object, dict):
+    """PDF Dictionary object."""
     def __init__(self, values=None):
         Object.__init__(self)
         dict.__init__(self, values or {})
 
     @property
     def data(self):
-        result = [b'<<']
-        for key, value in self.items():
-            result.append(b'/' + _to_bytes(key) + b' ' + _to_bytes(value))
-        result.append(b'>>')
-        return b'\n'.join(result)
+        result = [
+            b'/' + _to_bytes(key) + b' ' + _to_bytes(value)
+            for key, value in self.items()]
+        return b'<<' + b''.join(result) + b'>>'
 
 
 class Stream(Object):
-    """PDF Stream object.
-
-    Inherits from :class:`Object`.
-
-    """
+    """PDF Stream object."""
     def __init__(self, stream=None, extra=None, compress=False):
         super().__init__()
         #: Python array of data composing stream.
         self.stream = stream or []
         #: Metadata containing at least the length of the Stream.
         self.extra = extra or {}
         #: Compress the stream data if set to ``True``. Default is ``False``.
@@ -217,14 +208,18 @@
         """Add line from current point to point ``(x, y)``."""
         self.stream.append(b' '.join((_to_bytes(x), _to_bytes(y), b'l')))
 
     def move_to(self, x, y):
         """Begin new subpath by moving current point to ``(x, y)``."""
         self.stream.append(b' '.join((_to_bytes(x), _to_bytes(y), b'm')))
 
+    def move_text_to(self, x, y):
+        """Move text to next line at ``(x, y)`` distance from previous line."""
+        self.stream.append(b' '.join((_to_bytes(x), _to_bytes(y), b'Td')))
+
     def shading(self, name):
         """Paint shape and color shading using shading dictionary ``name``."""
         self.stream.append(b'/' + _to_bytes(name) + b' sh')
 
     def pop_state(self):
         """Restore graphic state."""
         self.stream.append(b'Q')
@@ -306,17 +301,21 @@
 
         :param state_name: Name of the graphic state.
 
         """
         self.stream.append(b'/' + _to_bytes(state_name) + b' gs')
 
     def show_text(self, text):
-        """Show text."""
+        """Show text strings with individual glyph positioning."""
         self.stream.append(b'[' + _to_bytes(text) + b'] TJ')
 
+    def show_text_string(self, text):
+        """Show single text string."""
+        self.stream.append(String(text).data + b' Tj')
+
     def stroke(self):
         """Stroke path."""
         self.stream.append(b'S')
 
     def stroke_and_close(self):
         """Stroke and close path."""
         self.stream.append(b's')
@@ -365,27 +364,23 @@
 
     @property
     def data(self):
         stream = b'\n'.join(_to_bytes(item) for item in self.stream)
         extra = Dictionary(self.extra.copy())
         if self.compress:
             extra['Filter'] = '/FlateDecode'
-            compressobj = zlib.compressobj()
+            compressobj = zlib.compressobj(level=9)
             stream = compressobj.compress(stream)
             stream += compressobj.flush()
         extra['Length'] = len(stream)
         return b'\n'.join((extra.data, b'stream', stream, b'endstream'))
 
 
 class String(Object):
-    """PDF String object.
-
-    Inherits from :class:`Object`.
-
-    """
+    """PDF String object."""
     def __init__(self, string=''):
         super().__init__()
         #: Unicode string.
         self.string = string
 
     @property
     def data(self):
@@ -398,30 +393,22 @@
             return b'(' + escaped + b')'
         except UnicodeEncodeError:
             encoded = BOM_UTF16_BE + str(self.string).encode('utf-16-be')
             return b'<' + encoded.hex().encode() + b'>'
 
 
 class Array(Object, list):
-    """PDF Array object.
-
-    Inherits from :class:`Object` and Python :obj:`list`.
-
-    """
+    """PDF Array object."""
     def __init__(self, array=None):
         Object.__init__(self)
         list.__init__(self, array or [])
 
     @property
     def data(self):
-        result = [b'[']
-        for child in self:
-            result.append(_to_bytes(child))
-        result.append(b']')
-        return b' '.join(result)
+        return b'[' + b' '.join(_to_bytes(child) for child in self) + b']'
 
 
 class PDF:
     """PDF document."""
     def __init__(self, version=b'1.7', identifier=None):
         """Create a PDF document.
 
@@ -496,56 +483,131 @@
         :param output: Output stream.
         :type output: binary :term:`file object`
 
         """
         self.current_position += len(content) + 1
         output.write(content + b'\n')
 
-    def write(self, output, version=None, identifier=None):
+    def write(self, output, version=None, identifier=None, compress=False):
         """Write PDF to output.
 
         :param output: Output stream.
         :type output: binary :term:`file object`
         :param bytes version: PDF version.
         :param bytes identifier: PDF file identifier.
+        :param bool compress: whether the PDF uses a compressed object stream.
 
         """
         version = self.version if version is None else _to_bytes(version)
         identifier = self.identifier if identifier is None else identifier
 
         # Write header
         self.write_line(b'%PDF-' + version, output)
         self.write_line(b'%\xf0\x9f\x96\xa4', output)
 
-        # Write all non-free PDF objects
-        for object_ in self.objects:
-            if object_.free == 'f':
-                continue
-            object_.offset = self.current_position
-            self.write_line(object_.indirect, output)
-
-        # Write cross reference table
-        self.xref_position = self.current_position
-        self.write_line(b'xref', output)
-        self.write_line(f'0 {len(self.objects)}'.encode(), output)
-        for object_ in self.objects:
-            self.write_line(
-                (f'{object_.offset:010} {object_.generation:05} '
-                 f'{object_.free} ').encode(), output)
-
-        # Write trailer
-        self.write_line(b'trailer', output)
-        self.write_line(b'<<', output)
-        self.write_line(f'/Size {len(self.objects)}'.encode(), output)
-        self.write_line(b'/Root ' + self.catalog.reference, output)
-        self.write_line(b'/Info ' + self.info.reference, output)
-        if identifier is not None:
-            data = b''.join(
-                obj.data for obj in self.objects if obj.free != 'f')
-            data_hash = md5(data).hexdigest().encode()
-            self.write_line(
-                b'/ID [' + String(identifier).data + b' ' +
-                String(data_hash).data + b']', output)
-        self.write_line(b'>>', output)
+        if version >= b'1.5' and compress:
+            # Store compressed objects for later and write other ones in PDF
+            compressed_objects = []
+            for object_ in self.objects:
+                if object_.free == 'f':
+                    continue
+                if object_.compressible:
+                    compressed_objects.append(object_)
+                else:
+                    object_.offset = self.current_position
+                    self.write_line(object_.indirect, output)
+
+            # Write compressed objects in object stream
+            stream = [[]]
+            position = 0
+            for i, object_ in enumerate(compressed_objects):
+                data = object_.data
+                stream.append(data)
+                stream[0].append(object_.number)
+                stream[0].append(position)
+                position += len(data) + 1
+            stream[0] = ' '.join(str(i) for i in stream[0])
+            extra = {
+                'Type': '/ObjStm',
+                'N': len(compressed_objects),
+                'First': len(stream[0]) + 1,
+            }
+            object_stream = Stream(stream, extra, compress)
+            object_stream.offset = self.current_position
+            self.add_object(object_stream)
+            self.write_line(object_stream.indirect, output)
+
+            # Write cross-reference stream
+            xref = []
+            dict_index = 0
+            for object_ in self.objects:
+                if object_.compressible:
+                    xref.append((2, object_stream.number, dict_index))
+                    dict_index += 1
+                else:
+                    xref.append((
+                        bool(object_.number), object_.offset,
+                        object_.generation))
+            xref.append((1, self.current_position, 0))
+
+            field2_size = ceil(log(self.current_position, 8))
+            max_generation = max(
+                object_.generation for object_ in self.objects)
+            field3_size = ceil(log(
+                max(max_generation, len(compressed_objects)), 8))
+            xref_lengths = (1, field2_size, field3_size)
+            xref_stream = b''.join(
+                value.to_bytes(length, 'big')
+                for line in xref for length, value in zip(xref_lengths, line))
+            extra = {
+                'Type': '/XRef',
+                'Index': Array((0, len(self.objects) + 1)),
+                'W': Array(xref_lengths),
+                'Size': len(self.objects) + 1,
+                'Root': self.catalog.reference,
+                'Info': self.info.reference,
+            }
+            if identifier is not None:
+                data = b''.join(
+                    obj.data for obj in self.objects if obj.free != 'f')
+                data_hash = md5(data).hexdigest().encode()
+                extra['ID'] = Array((
+                    String(identifier).data, String(data_hash).data))
+            dict_stream = Stream([xref_stream], extra, compress)
+            self.xref_position = dict_stream.offset = self.current_position
+            self.add_object(dict_stream)
+            self.write_line(dict_stream.indirect, output)
+        else:
+            # Write all non-free PDF objects
+            for object_ in self.objects:
+                if object_.free == 'f':
+                    continue
+                object_.offset = self.current_position
+                self.write_line(object_.indirect, output)
+
+            # Write cross-reference table
+            self.xref_position = self.current_position
+            self.write_line(b'xref', output)
+            self.write_line(f'0 {len(self.objects)}'.encode(), output)
+            for object_ in self.objects:
+                self.write_line(
+                    (f'{object_.offset:010} {object_.generation:05} '
+                     f'{object_.free} ').encode(), output)
+
+            # Write trailer
+            self.write_line(b'trailer', output)
+            self.write_line(b'<<', output)
+            self.write_line(f'/Size {len(self.objects)}'.encode(), output)
+            self.write_line(b'/Root ' + self.catalog.reference, output)
+            self.write_line(b'/Info ' + self.info.reference, output)
+            if identifier is not None:
+                data = b''.join(
+                    obj.data for obj in self.objects if obj.free != 'f')
+                data_hash = md5(data).hexdigest().encode()
+                self.write_line(
+                    b'/ID [' + String(identifier).data + b' ' +
+                    String(data_hash).data + b']', output)
+            self.write_line(b'>>', output)
+
         self.write_line(b'startxref', output)
         self.write_line(f'{self.xref_position}'.encode(), output)
         self.write_line(b'%%EOF', output)
```

### Comparing `pydyf-0.5.0/pyproject.toml` & `pydyf-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydyf-0.5.0/tests/__init__.py` & `pydyf-0.6.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pydyf-0.5.0/tests/test_pydyf.py` & `pydyf-0.6.0/tests/test_pydyf.py`

 * *Files identical despite different names*

### Comparing `pydyf-0.5.0/PKG-INFO` & `pydyf-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydyf
-Version: 0.5.0
+Version: 0.6.0
 Summary: A low-level PDF generator.
 Keywords: pdf,generator
 Author-email: CourtBouillon <contact@courtbouillon.org>
 Maintainer-email: CourtBouillon <contact@courtbouillon.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
```

