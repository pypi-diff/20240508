# Comparing `tmp/pcffont-0.0.7.tar.gz` & `tmp/pcffont-0.0.8.tar.gz`

## Comparing `pcffont-0.0.7.tar` & `pcffont-0.0.8.tar`

### file list

```diff
@@ -1,51 +1,59 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pcffont-0.0.7/requirements.txt
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pcffont-0.0.7/.github/workflows/publish.yml
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 pcffont-0.0.7/.github/workflows/test.yml
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/demo/README.md
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/demo/demo-lsbyte-lsbit-p2-u4.pcf
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/demo/demo-lsbyte-lsbit-p4-u2.pcf
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/demo/demo-lsbyte-msbit-p2-u4.pcf
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/demo/demo-lsbyte-msbit-p4-u2.pcf
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/demo/demo-msbyte-lsbit-p2-u4.pcf
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/demo/demo-msbyte-lsbit-p4-u2.pcf
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/demo/demo-msbyte-msbit-p2-u4.pcf
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/demo/demo-msbyte-msbit-p4-u2.pcf
--rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/demo/demo.bdf
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/spleen/LICENSE
--rw-r--r--   0        0        0   230552 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/spleen/spleen-12x24.pcf
--rw-r--r--   0        0        0   268184 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/spleen/spleen-16x32.pcf
--rw-r--r--   0        0        0   392216 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/spleen/spleen-32x64.pcf
--rw-r--r--   0        0        0   145220 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/spleen/spleen-5x8.pcf
--rw-r--r--   0        0        0   158776 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/spleen/spleen-6x12.pcf
--rw-r--r--   0        0        0   206164 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/spleen/spleen-8x16.pcf
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/unifont/OFL.txt
--rw-r--r--   0        0        0  5155808 2020-02-02 00:00:00.000000 pcffont-0.0.7/assets/unifont/unifont-15.1.05.pcf
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pcffont-0.0.7/examples/__init__.py
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 pcffont-0.0.7/examples/create.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 pcffont-0.0.7/examples/load.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/__init__.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/error.py
--rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/font.py
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/format.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/header.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/metric.py
--rw-r--r--   0        0        0     5864 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/t_accelerators.py
--rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/t_bitmaps.py
--rw-r--r--   0        0        0     4577 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/t_encodings.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/t_glyph_names.py
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/t_metrics.py
--rw-r--r--   0        0        0    12050 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/t_properties.py
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/t_scalable_widths.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/table.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/internal/__init__.py
--rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 pcffont-0.0.7/src/pcffont/internal/buffer.py
--rw-r--r--   0        0        0     8169 2020-02-02 00:00:00.000000 pcffont-0.0.7/tests/test_buffer.py
--rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 pcffont-0.0.7/tests/test_demo.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pcffont-0.0.7/tests/test_example.py
--rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 pcffont-0.0.7/tests/test_load_save.py
--rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 pcffont-0.0.7/tests/test_reload.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 pcffont-0.0.7/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pcffont-0.0.7/LICENSE
--rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 pcffont-0.0.7/README.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pcffont-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pcffont-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pcffont-0.0.8/requirements.txt
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pcffont-0.0.8/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 pcffont-0.0.8/.github/workflows/test.yml
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/README.md
+-rw-r--r--   0        0        0    16275 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo-2.bdf
+-rw-r--r--   0        0        0   123960 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo-2.pcf
+-rw-r--r--   0        0        0   154104 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo-lsbyte-lsbit-p2-u4.pcf
+-rw-r--r--   0        0        0   165624 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo-lsbyte-lsbit-p4-u2.pcf
+-rw-r--r--   0        0        0   154104 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo-lsbyte-msbit-p2-u4.pcf
+-rw-r--r--   0        0        0   165624 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo-lsbyte-msbit-p4-u2.pcf
+-rw-r--r--   0        0        0   154104 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo-msbyte-lsbit-p2-u4.pcf
+-rw-r--r--   0        0        0   165624 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo-msbyte-lsbit-p4-u2.pcf
+-rw-r--r--   0        0        0   154104 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo-msbyte-msbit-p2-u4.pcf
+-rw-r--r--   0        0        0   165624 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo-msbyte-msbit-p4-u2.pcf
+-rw-r--r--   0        0        0    84057 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo.bdf
+-rw-r--r--   0        0        0   165624 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo.pcf
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/spleen/LICENSE
+-rw-r--r--   0        0        0   230552 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/spleen/spleen-12x24.pcf
+-rw-r--r--   0        0        0   268184 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/spleen/spleen-16x32.pcf
+-rw-r--r--   0        0        0   392216 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/spleen/spleen-32x64.pcf
+-rw-r--r--   0        0        0   145220 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/spleen/spleen-5x8.pcf
+-rw-r--r--   0        0        0   158776 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/spleen/spleen-6x12.pcf
+-rw-r--r--   0        0        0   206164 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/spleen/spleen-8x16.pcf
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/unifont/OFL.txt
+-rw-r--r--   0        0        0  9385540 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/unifont/unifont-15.1.05.bdf
+-rw-r--r--   0        0        0  5155808 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/unifont/unifont-15.1.05.pcf
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pcffont-0.0.8/examples/__init__.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 pcffont-0.0.8/examples/create.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 pcffont-0.0.8/examples/load.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/__init__.py
+-rw-r--r--   0        0        0     5890 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/builder.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/error.py
+-rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/font.py
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/format.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/glyph.py
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/header.py
+-rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/metric.py
+-rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/t_accelerators.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/t_bitmaps.py
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/t_encodings.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/t_glyph_names.py
+-rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/t_metrics.py
+-rw-r--r--   0        0        0    12296 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/t_properties.py
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/t_scalable_widths.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/table.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/internal/__init__.py
+-rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/internal/buffer.py
+-rw-r--r--   0        0        0     8169 2020-02-02 00:00:00.000000 pcffont-0.0.8/tests/test_buffer.py
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 pcffont-0.0.8/tests/test_builder.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pcffont-0.0.8/tests/test_example.py
+-rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pcffont-0.0.8/tests/test_load_save.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 pcffont-0.0.8/tests/test_no_compat.py
+-rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 pcffont-0.0.8/tests/test_type.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 pcffont-0.0.8/tests/test_validity.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 pcffont-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pcffont-0.0.8/LICENSE
+-rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 pcffont-0.0.8/README.md
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pcffont-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 pcffont-0.0.8/PKG-INFO
```

### Comparing `pcffont-0.0.7/.github/workflows/publish.yml` & `pcffont-0.0.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.7/.github/workflows/test.yml` & `pcffont-0.0.8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.7/assets/demo/README.md` & `pcffont-0.0.8/assets/demo/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,8 +9,11 @@
 bdftopcf demo.bdf -o demo-msbyte-lsbit-p4-u2.pcf -l -p4 -u2
 bdftopcf demo.bdf -o demo-msbyte-msbit-p4-u2.pcf -p4 -u2
 
 bdftopcf demo.bdf -o demo-lsbyte-lsbit-p2-u4.pcf -L -l -p2 -u4
 bdftopcf demo.bdf -o demo-lsbyte-msbit-p2-u4.pcf -L -p2 -u4
 bdftopcf demo.bdf -o demo-msbyte-lsbit-p2-u4.pcf -l -p2 -u4
 bdftopcf demo.bdf -o demo-msbyte-msbit-p2-u4.pcf -p2 -u4
+
+bdftopcf demo.bdf -o demo.pcf
+bdftopcf demo-2.bdf -o demo-2.pcf
 ```
```

### Comparing `pcffont-0.0.7/assets/spleen/LICENSE` & `pcffont-0.0.8/assets/spleen/LICENSE`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.7/assets/spleen/spleen-12x24.pcf` & `pcffont-0.0.8/assets/spleen/spleen-12x24.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.7/assets/spleen/spleen-16x32.pcf` & `pcffont-0.0.8/assets/spleen/spleen-16x32.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.7/assets/spleen/spleen-32x64.pcf` & `pcffont-0.0.8/assets/spleen/spleen-32x64.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.7/assets/spleen/spleen-5x8.pcf` & `pcffont-0.0.8/assets/spleen/spleen-5x8.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.7/assets/spleen/spleen-6x12.pcf` & `pcffont-0.0.8/assets/spleen/spleen-6x12.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.7/assets/spleen/spleen-8x16.pcf` & `pcffont-0.0.8/assets/spleen/spleen-8x16.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.7/assets/unifont/OFL.txt` & `pcffont-0.0.8/assets/unifont/OFL.txt`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.7/assets/unifont/unifont-15.1.05.pcf` & `pcffont-0.0.8/assets/unifont/unifont-15.1.05.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.7/examples/load.py` & `pcffont-0.0.8/examples/load.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     for code_point, glyph_index in sorted(font.bdf_encodings.items()):
         glyph_name = font.glyph_names[glyph_index]
         metric = font.metrics[glyph_index]
         bitmap = font.bitmaps[glyph_index]
         print(f'char: {chr(code_point)} ({code_point:04X})')
         print(f'glyph_name: {glyph_name}')
         print(f'advance_width: {metric.character_width}')
-        print(f'offset: ({metric.left_side_bearing}, {-metric.descent})')
+        print(f'dimensions: {metric.dimensions}')
+        print(f'origin: {metric.origin}')
         for bitmap_row in bitmap:
             text = ''.join(map(str, bitmap_row)).replace('0', '  ').replace('1', '██')
             print(f'{text}*')
         print()
     font.save(os.path.join(outputs_dir, 'unifont-15.1.05.pcf'))
```

### Comparing `pcffont-0.0.7/src/pcffont/error.py` & `pcffont-0.0.8/src/pcffont/error.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.7/src/pcffont/font.py` & `pcffont-0.0.8/src/pcffont/font.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.7/src/pcffont/header.py` & `pcffont-0.0.8/src/pcffont/header.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from enum import IntEnum
+from typing import Any
 
 from pcffont.error import PcfParseError
 from pcffont.format import PcfTableFormat
 from pcffont.internal.buffer import Buffer
 
 _FILE_VERSION = b'\x01fcp'
 
@@ -65,13 +66,21 @@
 
     def __init__(self, table_type: PcfTableType, table_format: PcfTableFormat, table_size: int, table_offset: int):
         self.table_type = table_type
         self.table_format = table_format
         self.table_size = table_size
         self.table_offset = table_offset
 
+    def __eq__(self, other: Any) -> bool:
+        if not isinstance(other, PcfHeader):
+            return False
+        return (self.table_type == other.table_type and
+                self.table_format == other.table_format and
+                self.table_size == other.table_size and
+                self.table_offset == other.table_offset)
+
     def read_and_check_table_format(self, buffer: Buffer, strict_level: int) -> 'PcfTableFormat':
         buffer.seek(self.table_offset)
         value = buffer.read_uint32()
         if value != self.table_format.value and strict_level >= 2:
             raise PcfParseError(f"The table format definition is inconsistent with the header: type '{self.table_type.name}', offset {self.table_offset}")
         return self.table_format
```

### Comparing `pcffont-0.0.7/src/pcffont/t_accelerators.py` & `pcffont-0.0.8/src/pcffont/t_accelerators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Any
+
 import pcffont
 from pcffont.format import PcfTableFormat
 from pcffont.header import PcfHeader
 from pcffont.internal.buffer import Buffer
 from pcffont.metric import PcfMetric
 from pcffont.table import PcfTable
 
@@ -22,15 +24,15 @@
         font_ascent = buffer.read_int32(table_format.ms_byte_first)
         font_descent = buffer.read_int32(table_format.ms_byte_first)
         max_overlap = buffer.read_int32(table_format.ms_byte_first)
 
         min_bounds = PcfMetric.parse(buffer, table_format.ms_byte_first, False)
         max_bounds = PcfMetric.parse(buffer, table_format.ms_byte_first, False)
 
-        if table_format.has_ink_bounds:
+        if table_format.ink_or_compressed_metrics:
             ink_min_bounds = PcfMetric.parse(buffer, table_format.ms_byte_first, False)
             ink_max_bounds = PcfMetric.parse(buffer, table_format.ms_byte_first, False)
         else:
             ink_min_bounds = None
             ink_max_bounds = None
 
         # Compat
@@ -99,14 +101,34 @@
         self.max_overlap = max_overlap
         self.min_bounds = min_bounds
         self.max_bounds = max_bounds
         self.ink_min_bounds = ink_min_bounds
         self.ink_max_bounds = ink_max_bounds
         self._compat_info: tuple[int, int, bytes] | None = None
 
+    def __eq__(self, other: Any) -> bool:
+        if not isinstance(other, PcfAccelerators):
+            return False
+        return (self.table_format == other.table_format and
+                self.no_overlap == other.no_overlap and
+                self.constant_metrics == other.constant_metrics and
+                self.terminal_font == other.terminal_font and
+                self.constant_width == other.constant_width and
+                self.ink_inside == other.ink_inside and
+                self.ink_metrics == other.ink_metrics and
+                self.draw_right_to_left == other.draw_right_to_left and
+                self.font_ascent == other.font_ascent and
+                self.font_descent == other.font_descent and
+                self.max_overlap == other.max_overlap and
+                self.min_bounds == other.min_bounds and
+                self.max_bounds == other.max_bounds and
+                self.ink_min_bounds == other.ink_min_bounds and
+                self.ink_max_bounds == other.ink_max_bounds and
+                self._compat_info == other._compat_info)
+
     def _dump(self, buffer: Buffer, _font: 'pcffont.PcfFont', table_offset: int) -> int:
         buffer.seek(table_offset)
         buffer.write_uint32(self.table_format.value)
         buffer.write_bool(self.no_overlap)
         buffer.write_bool(self.constant_metrics)
         buffer.write_bool(self.terminal_font)
         buffer.write_bool(self.constant_width)
@@ -117,15 +139,15 @@
         buffer.write_int32(self.font_ascent, self.table_format.ms_byte_first)
         buffer.write_int32(self.font_descent, self.table_format.ms_byte_first)
         buffer.write_int32(self.max_overlap, self.table_format.ms_byte_first)
 
         self.min_bounds.dump(buffer, self.table_format.ms_byte_first, False)
         self.max_bounds.dump(buffer, self.table_format.ms_byte_first, False)
 
-        if self.table_format.has_ink_bounds:
+        if self.table_format.ink_or_compressed_metrics:
             self.ink_min_bounds.dump(buffer, self.table_format.ms_byte_first, False)
             self.ink_max_bounds.dump(buffer, self.table_format.ms_byte_first, False)
 
         table_size = buffer.tell() - table_offset
 
         # Compat
         if self._compat_info is not None:
```

### Comparing `pcffont-0.0.7/src/pcffont/t_bitmaps.py` & `pcffont-0.0.8/src/pcffont/t_bitmaps.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import math
 from collections import UserList
+from typing import Any
 
 import pcffont
 from pcffont.format import PcfTableFormat
 from pcffont.header import PcfHeader
 from pcffont.internal.buffer import Buffer
 from pcffont.table import PcfTable
 
@@ -30,26 +31,26 @@
         bitmaps_sizes = buffer.read_uint32_list(4, table_format.ms_byte_first)
         bitmaps_start = buffer.tell()
 
         bitmaps = PcfBitmaps(table_format)
         for glyph_index, bitmap_offset in enumerate(bitmap_offsets):
             buffer.seek(bitmaps_start + bitmap_offset)
             metric = font.metrics[glyph_index]
-            glyph_row_pad = math.ceil(metric.glyph_width / (glyph_pad * 8)) * glyph_pad
+            glyph_row_pad = math.ceil(metric.width / (glyph_pad * 8)) * glyph_pad
 
-            fragments = buffer.read_binary_list(glyph_row_pad * metric.glyph_height, table_format.ms_bit_first)
+            fragments = buffer.read_binary_list(glyph_row_pad * metric.height, table_format.ms_bit_first)
             if table_format.ms_byte_first != table_format.ms_bit_first:
                 _swap_fragments(fragments, scan_unit)
 
             bitmap = []
-            for _ in range(metric.glyph_height):
+            for _ in range(metric.height):
                 bitmap_row = []
                 for _ in range(glyph_row_pad):
                     bitmap_row.extend(fragments.pop(0))
-                bitmap_row = bitmap_row[:metric.glyph_width]
+                bitmap_row = bitmap_row[:metric.width]
                 bitmap.append(bitmap_row)
             bitmaps.append(bitmap)
 
         # Compat
         bitmaps._compat_info = bitmaps_sizes
 
         return bitmaps
@@ -61,28 +62,35 @@
     ):
         if table_format is None:
             table_format = PcfTableFormat()
         PcfTable.__init__(self, table_format)
         UserList.__init__(self, bitmaps)
         self._compat_info: list[int] | None = None
 
+    def __eq__(self, other: Any) -> bool:
+        if not isinstance(other, PcfBitmaps):
+            return False
+        return (self.table_format == other.table_format and
+                self._compat_info == other._compat_info and
+                UserList.__eq__(self, other))
+
     def _dump(self, buffer: Buffer, font: 'pcffont.PcfFont', table_offset: int) -> int:
         glyph_pad = [1, 2, 4, 8][self.table_format.glyph_pad_index]
         scan_unit = [1, 2, 4][self.table_format.scan_unit_index]
 
         glyphs_count = len(self)
 
         bitmaps_start = table_offset + 4 + 4 + 4 * glyphs_count + 4 * 4
         bitmaps_size = 0
         bitmap_offsets = []
         buffer.seek(bitmaps_start)
         for glyph_index, bitmap in enumerate(self):
             bitmap_offsets.append(bitmaps_size)
             metric = font.metrics[glyph_index]
-            bitmap_row_width = math.ceil(metric.glyph_width / (glyph_pad * 8)) * glyph_pad * 8
+            bitmap_row_width = math.ceil(metric.width / (glyph_pad * 8)) * glyph_pad * 8
 
             fragments = []
             for bitmap_row in bitmap:
                 if len(bitmap_row) < bitmap_row_width:
                     bitmap_row = bitmap_row + [0] * (bitmap_row_width - len(bitmap_row))
                 elif len(bitmap_row) > bitmap_row_width:
                     bitmap_row = bitmap_row[:bitmap_row_width]
```

### Comparing `pcffont-0.0.7/src/pcffont/t_encodings.py` & `pcffont-0.0.8/src/pcffont/t_encodings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from collections import UserDict
+from typing import Final, Any
 
 import pcffont
 from pcffont.error import PcfOutOfRangeError
 from pcffont.format import PcfTableFormat
 from pcffont.header import PcfHeader
 from pcffont.internal.buffer import Buffer
 from pcffont.table import PcfTable
 
-_MAX_CODE_POINT = 0xFFFF
-_NO_GLYPH_INDEX = 0xFFFF
-
 
 class PcfBdfEncodings(PcfTable, UserDict[int, int]):
     """
     code_point -> glyph_index
     """
 
+    MAX_CODE_POINT: Final[int] = 0xFFFF
+    NO_GLYPH_INDEX: Final[int] = 0xFFFF
+
     @staticmethod
     def parse(buffer: Buffer, _font: 'pcffont.PcfFont', header: PcfHeader, strict_level: int) -> 'PcfBdfEncodings':
         table_format = header.read_and_check_table_format(buffer, strict_level)
 
         min_byte_2 = buffer.read_uint16(table_format.ms_byte_first)
         max_byte_2 = buffer.read_uint16(table_format.ms_byte_first)
         min_byte_1 = buffer.read_uint16(table_format.ms_byte_first)
@@ -41,34 +42,41 @@
                     glyph_index = glyph_indices[(byte_1 - min_byte_1) * (max_byte_2 - min_byte_2 + 1) + byte_2 - min_byte_2]
                     encodings[code_point] = glyph_index
         return encodings
 
     def __init__(
             self,
             table_format: PcfTableFormat = None,
-            default_char: int = _NO_GLYPH_INDEX,
+            default_char: int = NO_GLYPH_INDEX,
             encodings: dict[int, int] = None,
     ):
         if table_format is None:
             table_format = PcfTableFormat()
         PcfTable.__init__(self, table_format)
         UserDict.__init__(self, encodings)
         self.default_char = default_char
 
     def __setitem__(self, code_point: int, glyph_index: int | None):
-        if code_point < 0 or code_point > _MAX_CODE_POINT:
-            raise PcfOutOfRangeError(f'Code point must between [0, {_MAX_CODE_POINT}]')
-        if glyph_index < 0 or glyph_index > _NO_GLYPH_INDEX:
-            raise PcfOutOfRangeError(f'Glyph index must between [0, {_NO_GLYPH_INDEX}]')
+        if code_point < 0 or code_point > PcfBdfEncodings.MAX_CODE_POINT:
+            raise PcfOutOfRangeError(f'Code point must between [0, {PcfBdfEncodings.MAX_CODE_POINT}]')
+        if glyph_index < 0 or glyph_index > PcfBdfEncodings.NO_GLYPH_INDEX:
+            raise PcfOutOfRangeError(f'Glyph index must between [0, {PcfBdfEncodings.NO_GLYPH_INDEX}]')
 
-        if glyph_index is None or glyph_index == _NO_GLYPH_INDEX:
+        if glyph_index is None or glyph_index == PcfBdfEncodings.NO_GLYPH_INDEX:
             self.pop(code_point, None)
         else:
             super().__setitem__(code_point, glyph_index)
 
+    def __eq__(self, other: Any) -> bool:
+        if not isinstance(other, PcfBdfEncodings):
+            return False
+        return (self.table_format == other.table_format and
+                self.default_char == other.default_char and
+                UserDict.__eq__(self, other))
+
     def _dump(self, buffer: Buffer, _font: 'pcffont.PcfFont', table_offset: int) -> int:
         min_byte_2 = 0xFF
         max_byte_2 = 0
         min_byte_1 = 0xFF
         max_byte_1 = 0
         for code_point in self:
             bs = code_point.to_bytes(2, 'big')
@@ -89,18 +97,18 @@
         buffer.write_uint16(max_byte_2, self.table_format.ms_byte_first)
         buffer.write_uint16(min_byte_1, self.table_format.ms_byte_first)
         buffer.write_uint16(max_byte_1, self.table_format.ms_byte_first)
         buffer.write_uint16(self.default_char, self.table_format.ms_byte_first)
 
         if min_byte_1 == max_byte_1 == 0:
             for code_point in range(min_byte_2, max_byte_2 + 1):
-                glyph_index = self.get(code_point, _NO_GLYPH_INDEX)
+                glyph_index = self.get(code_point, PcfBdfEncodings.NO_GLYPH_INDEX)
                 buffer.write_uint16(glyph_index, self.table_format.ms_byte_first)
         else:
             for byte_1 in range(min_byte_1, max_byte_1 + 1):
                 for byte_2 in range(min_byte_2, max_byte_2 + 1):
                     code_point = int.from_bytes(bytes([byte_1, byte_2]), 'big')
-                    glyph_index = self.get(code_point, _NO_GLYPH_INDEX)
+                    glyph_index = self.get(code_point, PcfBdfEncodings.NO_GLYPH_INDEX)
                     buffer.write_uint16(glyph_index, self.table_format.ms_byte_first)
 
         table_size = buffer.tell() - table_offset
         return table_size
```

### Comparing `pcffont-0.0.7/src/pcffont/t_glyph_names.py` & `pcffont-0.0.8/src/pcffont/t_glyph_names.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from collections import UserList
+from typing import Any
 
 import pcffont
 from pcffont.format import PcfTableFormat
 from pcffont.header import PcfHeader
 from pcffont.internal.buffer import Buffer
 from pcffont.table import PcfTable
 
@@ -30,14 +31,20 @@
             names: list[str] = None,
     ):
         if table_format is None:
             table_format = PcfTableFormat()
         PcfTable.__init__(self, table_format)
         UserList.__init__(self, names)
 
+    def __eq__(self, other: Any) -> bool:
+        if not isinstance(other, PcfGlyphNames):
+            return False
+        return (self.table_format == other.table_format and
+                UserList.__eq__(self, other))
+
     def _dump(self, buffer: Buffer, _font: 'pcffont.PcfFont', table_offset: int) -> int:
         glyphs_count = len(self)
 
         strings_start = table_offset + 4 + 4 + 4 * glyphs_count + 4
         strings_size = 0
         name_offsets = []
         buffer.seek(strings_start)
```

### Comparing `pcffont-0.0.7/src/pcffont/t_metrics.py` & `pcffont-0.0.8/src/pcffont/t_scalable_widths.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 from collections import UserList
+from typing import Any
 
 import pcffont
 from pcffont.format import PcfTableFormat
 from pcffont.header import PcfHeader
 from pcffont.internal.buffer import Buffer
-from pcffont.metric import PcfMetric
 from pcffont.table import PcfTable
 
 
-class PcfMetrics(PcfTable, UserList[PcfMetric]):
+class PcfScalableWidths(PcfTable, UserList[int]):
     @staticmethod
-    def parse(buffer: Buffer, _font: 'pcffont.PcfFont', header: PcfHeader, strict_level: int) -> 'PcfMetrics':
+    def parse(buffer: Buffer, _font: 'pcffont.PcfFont', header: PcfHeader, strict_level: int) -> 'PcfScalableWidths':
         table_format = header.read_and_check_table_format(buffer, strict_level)
 
-        if table_format.is_compressed_metrics:
-            glyphs_count = buffer.read_uint16(table_format.ms_byte_first)
-        else:
-            glyphs_count = buffer.read_uint32(table_format.ms_byte_first)
-
-        metrics = PcfMetrics(table_format)
-        for _ in range(glyphs_count):
-            metric = PcfMetric.parse(buffer, table_format.ms_byte_first, table_format.is_compressed_metrics)
-            metrics.append(metric)
-        return metrics
+        glyphs_count = buffer.read_uint32(table_format.ms_byte_first)
+
+        scalable_widths = PcfScalableWidths(
+            table_format,
+            buffer.read_int32_list(glyphs_count, table_format.ms_byte_first),
+        )
+        return scalable_widths
 
     def __init__(
             self,
             table_format: PcfTableFormat = None,
-            metrics: list[PcfMetric] = None,
+            scalable_widths: list[int] = None,
     ):
         if table_format is None:
-            table_format = PcfTableFormat(is_compressed_metrics=True)
+            table_format = PcfTableFormat()
         PcfTable.__init__(self, table_format)
-        UserList.__init__(self, metrics)
+        UserList.__init__(self, scalable_widths)
+
+    def __eq__(self, other: Any) -> bool:
+        if not isinstance(other, PcfScalableWidths):
+            return False
+        return (self.table_format == other.table_format and
+                UserList.__eq__(self, other))
 
     def _dump(self, buffer: Buffer, _font: 'pcffont.PcfFont', table_offset: int) -> int:
         glyphs_count = len(self)
 
         buffer.seek(table_offset)
         buffer.write_uint32(self.table_format.value)
-        if self.table_format.is_compressed_metrics:
-            buffer.write_uint16(glyphs_count, self.table_format.ms_byte_first)
-        else:
-            buffer.write_uint32(glyphs_count, self.table_format.ms_byte_first)
-        for metric in self:
-            metric.dump(buffer, self.table_format.ms_byte_first, self.table_format.is_compressed_metrics)
+        buffer.write_uint32(glyphs_count, self.table_format.ms_byte_first)
+        buffer.write_int32_list(self, self.table_format.ms_byte_first)
 
         table_size = buffer.tell() - table_offset
         return table_size
```

### Comparing `pcffont-0.0.7/src/pcffont/t_properties.py` & `pcffont-0.0.8/src/pcffont/t_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 from collections import UserDict
+from typing import Any
 
 import pcffont
 from pcffont.error import PcfError, PcfPropKeyError, PcfPropValueError, PcfXlfdError
 from pcffont.format import PcfTableFormat
 from pcffont.header import PcfHeader
 from pcffont.internal.buffer import Buffer
 from pcffont.table import PcfTable
@@ -169,14 +170,20 @@
         _check_key(key)
         if value is None:
             self.pop(key, None)
         else:
             _check_value(key, value)
             super().__setitem__(key, value)
 
+    def __eq__(self, other: Any) -> bool:
+        if not isinstance(other, PcfProperties):
+            return False
+        return (self.table_format == other.table_format and
+                UserDict.__eq__(self, other))
+
     @property
     def foundry(self) -> str | None:
         return self.get(_KEY_FOUNDRY, None)
 
     @foundry.setter
     def foundry(self, value: str | None):
         self[_KEY_FOUNDRY] = value
```

### Comparing `pcffont-0.0.7/src/pcffont/table.py` & `pcffont-0.0.8/src/pcffont/table.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.7/src/pcffont/internal/buffer.py` & `pcffont-0.0.8/src/pcffont/internal/buffer.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.7/tests/test_buffer.py` & `pcffont-0.0.8/tests/test_buffer.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.7/tests/test_load_save.py` & `pcffont-0.0.8/tests/test_load_save.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,7 +126,23 @@
 
 def test_demo_msbyte_msbit_p2_u4(tmp_path: Path):
     load_file_path = os.path.join(project_root_dir, 'assets', 'demo', 'demo-msbyte-msbit-p2-u4.pcf')
     save_file_path = os.path.join(tmp_path, 'demo-msbyte-msbit-p2-u4.pcf')
     font = PcfFont.load(load_file_path)
     font.save(save_file_path)
     assert _file_sha256(load_file_path) == _file_sha256(save_file_path)
+
+
+def test_demo(tmp_path: Path):
+    load_file_path = os.path.join(project_root_dir, 'assets', 'demo', 'demo.pcf')
+    save_file_path = os.path.join(tmp_path, 'demo.pcf')
+    font = PcfFont.load(load_file_path)
+    font.save(save_file_path)
+    assert _file_sha256(load_file_path) == _file_sha256(save_file_path)
+
+
+def test_demo_2(tmp_path: Path):
+    load_file_path = os.path.join(project_root_dir, 'assets', 'demo', 'demo-2.pcf')
+    save_file_path = os.path.join(tmp_path, 'demo-2.pcf')
+    font = PcfFont.load(load_file_path)
+    font.save(save_file_path)
+    assert _file_sha256(load_file_path) == _file_sha256(save_file_path)
```

### Comparing `pcffont-0.0.7/.gitignore` & `pcffont-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.7/LICENSE` & `pcffont-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.7/pyproject.toml` & `pcffont-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pcffont"
-version = "0.0.7"
+version = "0.0.8"
 description = "A library for manipulating Portable Compiled Format (PCF) Fonts."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
```

