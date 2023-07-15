# Comparing `tmp/structio-1.3.3.tar.gz` & `tmp/structio-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structio-1.3.3.tar", last modified: Thu May 18 02:05:00 2023, max compression
+gzip compressed data, was "structio-1.3.4.tar", last modified: Sat Jul 15 00:11:42 2023, max compression
```

## Comparing `structio-1.3.3.tar` & `structio-1.3.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:05:00.852738 structio-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-05-18 02:05:00.852738 structio-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-05-18 02:04:43.000000 structio-1.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-18 02:04:43.000000 structio-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 02:05:00.852738 structio-1.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 02:05:00.852738 structio-1.3.3/structio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-05-18 02:05:00.000000 structio-1.3.3/structio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-18 02:05:00.000000 structio-1.3.3/structio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 02:05:00.000000 structio-1.3.3/structio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 02:05:00.000000 structio-1.3.3/structio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-05-18 02:04:43.000000 structio-1.3.3/structio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:11:42.979097 structio-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-07-15 00:11:42.979097 structio-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13544 2023-07-15 00:11:23.000000 structio-1.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-15 00:11:23.000000 structio-1.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 00:11:42.979097 structio-1.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:11:42.979097 structio-1.3.4/structio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-07-15 00:11:42.000000 structio-1.3.4/structio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-15 00:11:42.000000 structio-1.3.4/structio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 00:11:42.000000 structio-1.3.4/structio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-15 00:11:42.000000 structio-1.3.4/structio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12130 2023-07-15 00:11:23.000000 structio-1.3.4/structio.py
```

### Comparing `structio-1.3.3/PKG-INFO` & `structio-1.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structio
-Version: 1.3.3
+Version: 1.3.4
 Summary: A Library for unparsing, parsing, and editing binary files
 Project-URL: Homepage, https://github.com/lingeringwillx/StructIO
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 
 A small Python library based on the BytesIO object from the standard library, designed to make parsing and editing binary files easier.
 
@@ -17,15 +17,15 @@
 ```
 
 ### Example
 
 Writing to a stream:
 
 ```python
->>> from structio import StructIO
+>>> from structio import *
 >>> stream = StructIO()
 >>> stream.write_int(10, 2)
 2
 >>> stream.write_float(3.14, 4)
 4
 >>> stream.write_cstr('Hello')
 6
@@ -140,27 +140,31 @@
 
 ### StructIO
 
 File-like object stored in memory. Extends *io.BytesIO* from the standard library, which means that it has all of the basic methods of file-like objects, including *read*, *write*, *seek*, *tell*, and *truncate*.
 
 ### Attributes
 
-**buffer**: the current content of the object.
+**buffer**: the current content of the object (read only).
 
-**endian**: specifies the default endian that would be used by the object, can either be *'little'* or *'big'*.
+**pos**: the current position in the object.
 
-**encoding**: specifies the default encoding used by string methods.
+**end**: the length of the object (read only).
 
-**errors**: specifies default error handling behavior when encoding or decoding strings. More information could be found in [Python's documentation](https://docs.python.org/3/library/codecs.html#error-handlers).
+**endian**: the default endian that would be used by the object (read only).
+
+**encoding**: the default encoding used by string methods (read only).
+
+**errors**: the default error handling behavior when encoding or decoding strings (read only).
 
 ### Methods
 
-**StructIO(b=b'', endian='little', encoding='utf-8', errors='ignore', struct=Struct)**
+**StructIO(b=b'', struct=structio._struct)**
 
-Take bytes object *b* and returns a *StructIO* instance containing *b*. The *endian* argument specifies the default endian that would be used by the object, should either be *'little'* or *'big'*. *struct* is the class used for unpacking and packing, should either be [Struct](#Struct) or a class implementing the same methods..
+Take bytes object *b* and returns a *StructIO* instance containing *b*. *struct* is the object used for unpacking and packing, should either be [Struct](#Struct) or an object implementing the same methods. The default Struct object used has endian *'little'* and encoding *'utf-8'* and error handler *'ignore'*.
 
 **\_\_len\_\_()**
 
 Returns the size/length of the file.
 
 **\_\_eq\_\_(other)**
 
@@ -365,29 +369,40 @@
         b = self.pack_str(string)
         return self.pack_7bint(len(b)) + b
 ```
 
 As well as the stream object:
 
 ```python
+extended_struct = ExtendedStruct()
+
 class ExtendedStructIO(StructIO):
-    def __init__(self, b=b'', endian='little', struct=ExtendedStruct):
-        super().__init__(b, endian, struct=struct)
+    def __init__(self, b=b'', struct=extended_struct):
+        super().__init__(b, struct)
+        
+    def copy(self):
+        return ExtendedStructIO(self.getvalue(), self._struct)
+        
+    def _get_7bstr_len(self):
+        return self._struct._get_7bstr_len(self.getvalue(), start=self.tell())
         
     def read_7bstr(self):
-        return self._read(self._struct.unpack_7bstr, ())
+        value, length = self._struct.unpack_7bstr(self.getvalue(), start=self.tell())
+        self.seek(length, 1)
+        return value
         
     def write_7bstr(self, string):
         return self.write(self._struct.pack_7bstr(string))
         
     def append_7bstr(self, string):
         return self.append(self._struct.pack_7bstr(string))
         
     def overwrite_7bstr(self, string):
-        return self._overwrite(self._struct._get_7bstr_len, (), self._struct.pack_7bstr, (string,))
-		 
+        start = self.tell()
+        return self.overwrite(start, start + self._get_7bstr_len(), self._struct.pack_7bstr(string))
+        
     def skip_7bstr(self):
-        return self._skip(self._struct._get_7bstr_len, ())
+        return self.seek(self._get_7bstr_len(), 1)
         
     def delete_7bstr(self):
-        return self._delete(self._struct._get_7bstr_len, ())
+        return self.delete(self._get_7bstr_len())
 ```
```

### Comparing `structio-1.3.3/README.md` & `structio-1.3.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ```
 
 ### Example
 
 Writing to a stream:
 
 ```python
->>> from structio import StructIO
+>>> from structio import *
 >>> stream = StructIO()
 >>> stream.write_int(10, 2)
 2
 >>> stream.write_float(3.14, 4)
 4
 >>> stream.write_cstr('Hello')
 6
@@ -132,27 +132,31 @@
 
 ### StructIO
 
 File-like object stored in memory. Extends *io.BytesIO* from the standard library, which means that it has all of the basic methods of file-like objects, including *read*, *write*, *seek*, *tell*, and *truncate*.
 
 ### Attributes
 
-**buffer**: the current content of the object.
+**buffer**: the current content of the object (read only).
 
-**endian**: specifies the default endian that would be used by the object, can either be *'little'* or *'big'*.
+**pos**: the current position in the object.
 
-**encoding**: specifies the default encoding used by string methods.
+**end**: the length of the object (read only).
 
-**errors**: specifies default error handling behavior when encoding or decoding strings. More information could be found in [Python's documentation](https://docs.python.org/3/library/codecs.html#error-handlers).
+**endian**: the default endian that would be used by the object (read only).
+
+**encoding**: the default encoding used by string methods (read only).
+
+**errors**: the default error handling behavior when encoding or decoding strings (read only).
 
 ### Methods
 
-**StructIO(b=b'', endian='little', encoding='utf-8', errors='ignore', struct=Struct)**
+**StructIO(b=b'', struct=structio._struct)**
 
-Take bytes object *b* and returns a *StructIO* instance containing *b*. The *endian* argument specifies the default endian that would be used by the object, should either be *'little'* or *'big'*. *struct* is the class used for unpacking and packing, should either be [Struct](#Struct) or a class implementing the same methods..
+Take bytes object *b* and returns a *StructIO* instance containing *b*. *struct* is the object used for unpacking and packing, should either be [Struct](#Struct) or an object implementing the same methods. The default Struct object used has endian *'little'* and encoding *'utf-8'* and error handler *'ignore'*.
 
 **\_\_len\_\_()**
 
 Returns the size/length of the file.
 
 **\_\_eq\_\_(other)**
 
@@ -357,29 +361,40 @@
         b = self.pack_str(string)
         return self.pack_7bint(len(b)) + b
 ```
 
 As well as the stream object:
 
 ```python
+extended_struct = ExtendedStruct()
+
 class ExtendedStructIO(StructIO):
-    def __init__(self, b=b'', endian='little', struct=ExtendedStruct):
-        super().__init__(b, endian, struct=struct)
+    def __init__(self, b=b'', struct=extended_struct):
+        super().__init__(b, struct)
+        
+    def copy(self):
+        return ExtendedStructIO(self.getvalue(), self._struct)
+        
+    def _get_7bstr_len(self):
+        return self._struct._get_7bstr_len(self.getvalue(), start=self.tell())
         
     def read_7bstr(self):
-        return self._read(self._struct.unpack_7bstr, ())
+        value, length = self._struct.unpack_7bstr(self.getvalue(), start=self.tell())
+        self.seek(length, 1)
+        return value
         
     def write_7bstr(self, string):
         return self.write(self._struct.pack_7bstr(string))
         
     def append_7bstr(self, string):
         return self.append(self._struct.pack_7bstr(string))
         
     def overwrite_7bstr(self, string):
-        return self._overwrite(self._struct._get_7bstr_len, (), self._struct.pack_7bstr, (string,))
-		 
+        start = self.tell()
+        return self.overwrite(start, start + self._get_7bstr_len(), self._struct.pack_7bstr(string))
+        
     def skip_7bstr(self):
-        return self._skip(self._struct._get_7bstr_len, ())
+        return self.seek(self._get_7bstr_len(), 1)
         
     def delete_7bstr(self):
-        return self._delete(self._struct._get_7bstr_len, ())
+        return self.delete(self._get_7bstr_len())
 ```
```

### Comparing `structio-1.3.3/structio.egg-info/PKG-INFO` & `structio-1.3.4/structio.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structio
-Version: 1.3.3
+Version: 1.3.4
 Summary: A Library for unparsing, parsing, and editing binary files
 Project-URL: Homepage, https://github.com/lingeringwillx/StructIO
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 
 A small Python library based on the BytesIO object from the standard library, designed to make parsing and editing binary files easier.
 
@@ -17,15 +17,15 @@
 ```
 
 ### Example
 
 Writing to a stream:
 
 ```python
->>> from structio import StructIO
+>>> from structio import *
 >>> stream = StructIO()
 >>> stream.write_int(10, 2)
 2
 >>> stream.write_float(3.14, 4)
 4
 >>> stream.write_cstr('Hello')
 6
@@ -140,27 +140,31 @@
 
 ### StructIO
 
 File-like object stored in memory. Extends *io.BytesIO* from the standard library, which means that it has all of the basic methods of file-like objects, including *read*, *write*, *seek*, *tell*, and *truncate*.
 
 ### Attributes
 
-**buffer**: the current content of the object.
+**buffer**: the current content of the object (read only).
 
-**endian**: specifies the default endian that would be used by the object, can either be *'little'* or *'big'*.
+**pos**: the current position in the object.
 
-**encoding**: specifies the default encoding used by string methods.
+**end**: the length of the object (read only).
 
-**errors**: specifies default error handling behavior when encoding or decoding strings. More information could be found in [Python's documentation](https://docs.python.org/3/library/codecs.html#error-handlers).
+**endian**: the default endian that would be used by the object (read only).
+
+**encoding**: the default encoding used by string methods (read only).
+
+**errors**: the default error handling behavior when encoding or decoding strings (read only).
 
 ### Methods
 
-**StructIO(b=b'', endian='little', encoding='utf-8', errors='ignore', struct=Struct)**
+**StructIO(b=b'', struct=structio._struct)**
 
-Take bytes object *b* and returns a *StructIO* instance containing *b*. The *endian* argument specifies the default endian that would be used by the object, should either be *'little'* or *'big'*. *struct* is the class used for unpacking and packing, should either be [Struct](#Struct) or a class implementing the same methods..
+Take bytes object *b* and returns a *StructIO* instance containing *b*. *struct* is the object used for unpacking and packing, should either be [Struct](#Struct) or an object implementing the same methods. The default Struct object used has endian *'little'* and encoding *'utf-8'* and error handler *'ignore'*.
 
 **\_\_len\_\_()**
 
 Returns the size/length of the file.
 
 **\_\_eq\_\_(other)**
 
@@ -365,29 +369,40 @@
         b = self.pack_str(string)
         return self.pack_7bint(len(b)) + b
 ```
 
 As well as the stream object:
 
 ```python
+extended_struct = ExtendedStruct()
+
 class ExtendedStructIO(StructIO):
-    def __init__(self, b=b'', endian='little', struct=ExtendedStruct):
-        super().__init__(b, endian, struct=struct)
+    def __init__(self, b=b'', struct=extended_struct):
+        super().__init__(b, struct)
+        
+    def copy(self):
+        return ExtendedStructIO(self.getvalue(), self._struct)
+        
+    def _get_7bstr_len(self):
+        return self._struct._get_7bstr_len(self.getvalue(), start=self.tell())
         
     def read_7bstr(self):
-        return self._read(self._struct.unpack_7bstr, ())
+        value, length = self._struct.unpack_7bstr(self.getvalue(), start=self.tell())
+        self.seek(length, 1)
+        return value
         
     def write_7bstr(self, string):
         return self.write(self._struct.pack_7bstr(string))
         
     def append_7bstr(self, string):
         return self.append(self._struct.pack_7bstr(string))
         
     def overwrite_7bstr(self, string):
-        return self._overwrite(self._struct._get_7bstr_len, (), self._struct.pack_7bstr, (string,))
-		 
+        start = self.tell()
+        return self.overwrite(start, start + self._get_7bstr_len(), self._struct.pack_7bstr(string))
+        
     def skip_7bstr(self):
-        return self._skip(self._struct._get_7bstr_len, ())
+        return self.seek(self._get_7bstr_len(), 1)
         
     def delete_7bstr(self):
-        return self._delete(self._struct._get_7bstr_len, ())
+        return self.delete(self._get_7bstr_len())
 ```
```

### Comparing `structio-1.3.3/structio.py` & `structio-1.3.4/structio.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import io
 import struct
 
-_endians = {'big': '>', 'little': '<'}
-_float_formats = {2: 'e', 4: 'f', 8: 'd'} 
-
 class Struct:
+    _endians = {'big': '>', 'little': '<'}
+    _float_formats = {2: 'e', 4: 'f', 8: 'd'}
+    
     def __init__(self, endian='little', encoding='utf-8', errors='ignore'):
         self.endian = endian
         self.encoding = encoding
         self.errors = errors
         
     def _get_endian(self, endian):
         if endian is None:
@@ -46,21 +46,21 @@
     def unpack_int(self, b, endian=None, signed=False):
         return int.from_bytes(b, self._get_endian(endian), signed=signed)
         
     def pack_int(self, number, numbytes, endian=None, signed=False):
         return number.to_bytes(numbytes, self._get_endian(endian), signed=signed)
         
     def _get_format(self, numbytes, endian=None):
-        if numbytes not in _float_formats:
+        if numbytes not in self._float_formats:
             raise ValueError("float size '{}' not supported".format(numbytes))
             
-        if endian not in _endians:
+        if endian not in self._endians:
             raise ValueError("endian '{}' is not recognized".format(endian))
             
-        return _endians[endian] + _float_formats[numbytes]
+        return self._endians[endian] + self._float_formats[numbytes]
         
     def unpack_float(self, b, numbytes, endian=None):
         return struct.unpack(self._get_format(numbytes, self._get_endian(endian)), b)[0]
         
     def pack_float(self, number, numbytes, endian=None):
         return struct.pack(self._get_format(numbytes, self._get_endian(endian)), number)
         
@@ -107,82 +107,84 @@
         
     def unpack_7bint(self, b, start=0):
         number = 0
         i = 0
         
         byte = b[start]
         while byte > 127:
-            number |= (byte & 0b01111111) << (7 * i)
+            number += (byte & 0b01111111) << (7 * i)
             i += 1
             
             byte = b[start + i]
             
-        number |= byte << (7 * i)
+        number += byte << (7 * i)
         length = i + 1
         
         return number, length
         
     def pack_7bint(self, number):
         b = b''
         
         while number > 127:
             b += self.pack_int(number & 0b01111111 | 0b10000000, 1) 
             number >>= 7
             
         b += self.pack_int(number, 1)
         return b
         
+_struct = Struct()
+
 class StructIO(io.BytesIO):
-    def __init__(self, b=b'', endian='little', encoding='utf-8', errors='ignore', struct=Struct):
+    def __init__(self, b=b'', struct=_struct):
         super().__init__(b)
-        self._struct = struct(endian, encoding, errors)
+        self._struct = struct
         
     @property
     def buffer(self):
         return self.getvalue()
         
     @property
+    def pos(self):
+        return self.tell()
+        
+    @pos.setter
+    def pos(self, value):
+        self.seek(value)
+        
+    @property
+    def end(self):
+        return len(self.getvalue())
+        
+    @property
     def endian(self):
         return self._struct.endian
         
-    @endian.setter
-    def endian(self, value):
-        self._struct.endian = value
-        
     @property
     def encoding(self):
         return self._struct.encoding
         
-    @encoding.setter
-    def encoding(self, value):
-        self._struct.encoding = value
-        
     @property
     def errors(self):
         return self._struct.errors
         
-    @errors.setter
-    def errors(self, value):
-        self._struct.errors = value
-        
     def __len__(self):
         return len(self.getvalue())
         
     def __eq__(self, other):
         return self.getvalue() == other.getvalue()
         
     def is_eof(self):
         if self.read(1) == b'':
             return True
         else:
             self.seek(-1, 1)
             return False
             
     def copy(self):
-        return StructIO(self.getvalue(), self._struct.endian, self._struct.encoding, self._struct.errors)
+        return StructIO(self.getvalue(), self._struct)
         
     def read_all(self):
         self.seek(0)
         return self.getvalue()
         
     def write_all(self, buffer):
         self.seek(0)
@@ -236,30 +238,14 @@
         location = self.find(bytes_sequence, n)
         
         if location == -1:
             raise ValueError('{} not found'.format(bytes_sequence))
             
         return location
         
-    def _read(self, unpack_func, unpack_args):
-        value, length = unpack_func(self.getvalue(), *unpack_args, start=self.tell())
-        self.seek(length, 1)
-        return value
-        
-    def _overwrite(self, len_func, len_args, pack_func, pack_args):
-        start = self.tell()
-        length = len_func(self.getvalue(), *len_args, start=start)
-        return self.overwrite(start, start + length, pack_func(*pack_args))
-        
-    def _skip(self, len_func, len_args):
-        return self.seek(len_func(self.getvalue(), *len_args, start=self.tell()), 1)
-        
-    def _delete(self, len_func, len_args):
-        return self.delete(len_func(self.getvalue(), *len_args, start=self.tell()))
-        
     def read_bool(self):
         return self._struct.unpack_bool(self.read(1))
         
     def write_bool(self, boolean):
         return self.write(self._struct.pack_bool(boolean))
         
     def append_bool(self, boolean):
@@ -301,60 +287,78 @@
     def append_str(self, string):
         return self.append(self._struct.pack_str(string))
         
     def overwrite_str(self, string, length):
         start = self.tell()
         return self.overwrite(start, start + length, self._struct.pack_str(string))
         
+    def _get_cstr_len(self):
+        return self._struct._get_cstr_len(self.getvalue(), start=self.tell())
+        
     def read_cstr(self):
-        return self._read(self._struct.unpack_cstr, ())
+        value, length = self._struct.unpack_cstr(self.getvalue(), start=self.tell())
+        self.seek(length, 1)
+        return value
         
     def write_cstr(self, string):
         return self.write(self._struct.pack_cstr(string))
         
     def append_cstr(self, string):
         return self.append(self._struct.pack_cstr(string))
         
     def overwrite_cstr(self, string):
-        return self._overwrite(self._struct._get_cstr_len, (), self._struct.pack_cstr, (string,))
+        start = self.tell()
+        return self.overwrite(start, start + self._get_cstr_len(), self._struct.pack_cstr(string))
         
     def skip_cstr(self):
-        return self._skip(self._struct._get_cstr_len, ())
+        return self.seek(self._get_cstr_len(), 1)
         
     def delete_cstr(self):
-        return self._delete(self._struct._get_cstr_len, ())
+        return self.delete(self._get_cstr_len())
+        
+    def _get_pstr_len(self, numbytes, endian=None):
+        return self._struct._get_pstr_len(self.getvalue(), numbytes, endian, start=self.tell())
         
     def read_pstr(self, numbytes, endian=None):
-        return self._read(self._struct.unpack_pstr, (numbytes, endian))
+        value, length = self._struct.unpack_pstr(self.getvalue(), numbytes, endian, start=self.tell())
+        self.seek(length, 1)
+        return value
         
     def write_pstr(self, string, numbytes, endian=None):
         return self.write(self._struct.pack_pstr(string, numbytes, endian))
         
     def append_pstr(self, string, numbytes, endian=None):
         return self.append(self._struct.pack_pstr(string, numbytes, endian))
         
     def overwrite_pstr(self, string, numbytes, endian=None):
-        return self._overwrite(self._struct._get_pstr_len, (numbytes, endian), self._struct.pack_pstr, (string, numbytes, endian))
+        start = self.tell()
+        return self.overwrite(start, start + self._get_pstr_len(numbytes, endian), self._struct.pack_pstr(string, numbytes, endian))
         
     def skip_pstr(self, numbytes, endian=None):
-        return self._skip(self._struct._get_pstr_len, (numbytes, endian))
+        return self.seek(self._get_pstr_len(numbytes, endian), 1)
         
     def delete_pstr(self, numbytes, endian=None):
-        return self._delete(self._struct._get_pstr_len, (numbytes, endian))
+        return self.delete(self._get_pstr_len(numbytes, endian))
+        
+    def _get_7bint_len(self):
+        return self._struct._get_7bint_len(self.getvalue(), start=self.tell())
         
     def read_7bint(self):
-        return self._read(self._struct.unpack_7bint, ())
+        value, length = self._struct.unpack_7bint(self.getvalue(), start=self.tell())
+        self.seek(length, 1)
+        return value
         
     def write_7bint(self, number):
         return self.write(self._struct.pack_7bint(number))
         
     def append_7bint(self, number):
         return self.append(self._struct.pack_7bint(number))
         
     def overwrite_7bint(self, number):
-        return self._overwrite(self._struct._get_7bint_len, (), self._struct.pack_7bint, (number,))
+        start = self.tell()
+        return self.overwrite(start, start + self._get_7bint_len(), self._struct.pack_7bint(number))
         
     def skip_7bint(self):
-        return self._skip(self._struct._get_7bint_len, ())
+        return self.seek(self._get_7bint_len(), 1)
         
     def delete_7bint(self):
-        return self._delete(self._struct._get_7bint_len, ())
+        return self.delete(self._get_7bint_len())
```

