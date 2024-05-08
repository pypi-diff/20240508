# Comparing `tmp/eclean_kernel-2.99.7.tar.gz` & `tmp/eclean_kernel-2.99.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eclean_kernel-2.99.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "eclean_kernel-2.99.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `eclean_kernel-2.99.7.tar` & `eclean_kernel-2.99.8.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0     1300 2021-04-07 09:16:05.131500 eclean_kernel-2.99.7/COPYING
--rw-r--r--   0        0        0     4234 2021-04-07 09:16:05.131500 eclean_kernel-2.99.7/README.rst
--rw-r--r--   0        0        0      193 2023-12-05 17:14:38.131193 eclean_kernel-2.99.7/ecleankernel/__init__.py
--rw-r--r--   0        0        0    15059 2023-12-04 18:35:01.815804 eclean_kernel-2.99.7/ecleankernel/__main__.py
--rw-r--r--   0        0        0      640 2021-04-07 09:16:05.131500 eclean_kernel-2.99.7/ecleankernel/bootloader/__init__.py
--rw-r--r--   0        0        0      784 2021-04-07 09:16:05.131500 eclean_kernel-2.99.7/ecleankernel/bootloader/grub.py
--rw-r--r--   0        0        0     1287 2021-04-07 09:16:05.131500 eclean_kernel-2.99.7/ecleankernel/bootloader/grub2.py
--rw-r--r--   0        0        0     1539 2021-04-07 09:16:05.131500 eclean_kernel-2.99.7/ecleankernel/bootloader/lilo.py
--rw-r--r--   0        0        0      522 2021-04-07 09:16:05.131500 eclean_kernel-2.99.7/ecleankernel/bootloader/symlinks.py
--rw-r--r--   0        0        0      258 2021-04-07 09:16:05.131500 eclean_kernel-2.99.7/ecleankernel/bootloader/yaboot.py
--rw-r--r--   0        0        0    10651 2023-12-05 17:14:14.874121 eclean_kernel-2.99.7/ecleankernel/file.py
--rw-r--r--   0        0        0     2418 2023-07-12 18:19:10.822326 eclean_kernel-2.99.7/ecleankernel/kernel.py
--rw-r--r--   0        0        0     1144 2021-04-07 09:16:05.131500 eclean_kernel-2.99.7/ecleankernel/layout/__init__.py
--rw-r--r--   0        0        0     5948 2023-12-04 18:34:24.208067 eclean_kernel-2.99.7/ecleankernel/layout/blspec.py
--rw-r--r--   0        0        0     1864 2021-04-07 09:16:05.131500 eclean_kernel-2.99.7/ecleankernel/layout/moduledir.py
--rw-r--r--   0        0        0     4624 2021-04-07 09:16:05.131500 eclean_kernel-2.99.7/ecleankernel/layout/std.py
--rw-r--r--   0        0        0     4538 2023-08-21 02:09:58.604904 eclean_kernel-2.99.7/ecleankernel/process.py
--rw-r--r--   0        0        0     1496 2021-04-07 09:16:05.131500 eclean_kernel-2.99.7/ecleankernel/sort.py
--rw-r--r--   0        0        0     1118 2023-03-21 14:59:38.314280 eclean_kernel-2.99.7/pyproject.toml
--rw-r--r--   0        0        0      127 2021-04-07 09:16:05.131500 eclean_kernel-2.99.7/test/__init__.py
--rw-r--r--   0        0        0     7931 2023-12-05 17:13:09.406290 eclean_kernel-2.99.7/test/test_file.py
--rw-r--r--   0        0        0    24204 2023-07-12 18:19:20.285932 eclean_kernel-2.99.7/test/test_layout_blspec.py
--rw-r--r--   0        0        0    17653 2023-07-12 18:19:10.822326 eclean_kernel-2.99.7/test/test_layout_std.py
--rw-r--r--   0        0        0     7020 2023-08-21 02:07:16.184640 eclean_kernel-2.99.7/test/test_process.py
--rw-r--r--   0        0        0     2323 2021-04-07 09:16:05.131500 eclean_kernel-2.99.7/test/test_sort.py
--rw-r--r--   0        0        0      522 2023-08-21 02:22:06.995715 eclean_kernel-2.99.7/tox.ini
--rw-r--r--   0        0        0     4895 1970-01-01 00:00:00.000000 eclean_kernel-2.99.7/PKG-INFO
+-rw-r--r--   0        0        0     4234 2021-04-07 09:16:05.131500 eclean_kernel-2.99.8/README.rst
+-rw-r--r--   0        0        0      156 2024-05-08 09:04:39.103218 eclean_kernel-2.99.8/ecleankernel/__init__.py
+-rw-r--r--   0        0        0    15022 2024-05-08 08:58:32.913916 eclean_kernel-2.99.8/ecleankernel/__main__.py
+-rw-r--r--   0        0        0      603 2024-05-08 08:58:32.897249 eclean_kernel-2.99.8/ecleankernel/bootloader/__init__.py
+-rw-r--r--   0        0        0      747 2024-05-08 08:58:32.900583 eclean_kernel-2.99.8/ecleankernel/bootloader/grub.py
+-rw-r--r--   0        0        0     1250 2024-05-08 08:58:32.900583 eclean_kernel-2.99.8/ecleankernel/bootloader/grub2.py
+-rw-r--r--   0        0        0     1502 2024-05-08 08:58:32.900583 eclean_kernel-2.99.8/ecleankernel/bootloader/lilo.py
+-rw-r--r--   0        0        0      485 2024-05-08 08:58:32.903916 eclean_kernel-2.99.8/ecleankernel/bootloader/symlinks.py
+-rw-r--r--   0        0        0      221 2024-05-08 08:58:32.903916 eclean_kernel-2.99.8/ecleankernel/bootloader/yaboot.py
+-rw-r--r--   0        0        0    10614 2024-05-08 08:58:32.917250 eclean_kernel-2.99.8/ecleankernel/file.py
+-rw-r--r--   0        0        0     2381 2024-05-08 08:58:32.913916 eclean_kernel-2.99.8/ecleankernel/kernel.py
+-rw-r--r--   0        0        0     1107 2024-05-08 08:58:32.907250 eclean_kernel-2.99.8/ecleankernel/layout/__init__.py
+-rw-r--r--   0        0        0     6461 2024-05-08 08:58:32.907250 eclean_kernel-2.99.8/ecleankernel/layout/blspec.py
+-rw-r--r--   0        0        0     1827 2024-05-08 08:58:32.907250 eclean_kernel-2.99.8/ecleankernel/layout/moduledir.py
+-rw-r--r--   0        0        0     5199 2024-05-08 08:58:32.910583 eclean_kernel-2.99.8/ecleankernel/layout/std.py
+-rw-r--r--   0        0        0     4501 2024-05-08 08:58:32.913916 eclean_kernel-2.99.8/ecleankernel/process.py
+-rw-r--r--   0        0        0     1459 2024-05-08 08:58:32.910583 eclean_kernel-2.99.8/ecleankernel/sort.py
+-rw-r--r--   0        0        0     1195 2024-05-08 08:59:13.554809 eclean_kernel-2.99.8/pyproject.toml
+-rw-r--r--   0        0        0       90 2024-05-08 08:58:32.920583 eclean_kernel-2.99.8/test/__init__.py
+-rw-r--r--   0        0        0     7894 2024-05-08 08:58:32.923916 eclean_kernel-2.99.8/test/test_file.py
+-rw-r--r--   0        0        0    24786 2024-05-08 08:58:32.927250 eclean_kernel-2.99.8/test/test_layout_blspec.py
+-rw-r--r--   0        0        0    21612 2024-05-08 08:58:32.927250 eclean_kernel-2.99.8/test/test_layout_std.py
+-rw-r--r--   0        0        0     6983 2024-05-08 08:58:32.923916 eclean_kernel-2.99.8/test/test_process.py
+-rw-r--r--   0        0        0     2286 2024-05-08 08:58:32.920583 eclean_kernel-2.99.8/test/test_sort.py
+-rw-r--r--   0        0        0      524 2024-05-08 08:55:36.556699 eclean_kernel-2.99.8/tox.ini
+-rw-r--r--   0        0        0     4953 1970-01-01 00:00:00.000000 eclean_kernel-2.99.8/PKG-INFO
```

### Comparing `eclean_kernel-2.99.7/README.rst` & `eclean_kernel-2.99.8/README.rst`

 * *Files identical despite different names*

### Comparing `eclean_kernel-2.99.7/ecleankernel/__main__.py` & `eclean_kernel-2.99.8/ecleankernel/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# vim:fileencoding=utf-8
 # (c) 2011-2020 Michał Górny <mgorny@gentoo.org>
-# Released under the terms of the 2-clause BSD license.
+# SPDX-License-Identifier: GPL-2.0-or-later
 
 import argparse
 import logging
 import os
 import os.path
 import shlex
 import subprocess
```

### Comparing `eclean_kernel-2.99.7/ecleankernel/bootloader/grub.py` & `eclean_kernel-2.99.8/ecleankernel/bootloader/grub.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# vim:fileencoding=utf-8
 # (c) 2011-2020 Michał Górny <mgorny@gentoo.org>
-# Released under the terms of the 2-clause BSD license.
+# SPDX-License-Identifier: GPL-2.0-or-later
 
 import logging
 import os.path
 import typing
 
 from ecleankernel.bootloader.lilo import LILO
```

### Comparing `eclean_kernel-2.99.7/ecleankernel/bootloader/grub2.py` & `eclean_kernel-2.99.8/ecleankernel/bootloader/grub2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# vim:fileencoding=utf-8
 # (c) 2011-2020 Michał Górny <mgorny@gentoo.org>
-# Released under the terms of the 2-clause BSD license.
+# SPDX-License-Identifier: GPL-2.0-or-later
 
 import logging
 import subprocess
 import typing
 
 from ecleankernel.bootloader.grub import GRUB
```

### Comparing `eclean_kernel-2.99.7/ecleankernel/bootloader/lilo.py` & `eclean_kernel-2.99.8/ecleankernel/bootloader/lilo.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# vim:fileencoding=utf-8
 # (c) 2011-2020 Michał Górny <mgorny@gentoo.org>
-# Released under the terms of the 2-clause BSD license.
+# SPDX-License-Identifier: GPL-2.0-or-later
 
 import logging
 import re
 import typing
 
 from ecleankernel.bootloader import Bootloader, BootloaderNotFound
```

### Comparing `eclean_kernel-2.99.7/ecleankernel/file.py` & `eclean_kernel-2.99.8/ecleankernel/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# vim:fileencoding=utf-8
 # (c) 2011-2023 Michał Górny <mgorny@gentoo.org>
-# Released under the terms of the 2-clause BSD license.
+# SPDX-License-Identifier: GPL-2.0-or-later
 
 import contextlib
 import enum
 import errno
 import importlib
 import logging
 import os
```

### Comparing `eclean_kernel-2.99.7/ecleankernel/kernel.py` & `eclean_kernel-2.99.8/ecleankernel/kernel.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# vim:fileencoding=utf-8
 # (c) 2011-2020 Michał Górny <mgorny@gentoo.org>
-# Released under the terms of the 2-clause BSD license.
+# SPDX-License-Identifier: GPL-2.0-or-later
 
 import os
 import os.path
 import typing
 
 from pathlib import Path
```

### Comparing `eclean_kernel-2.99.7/ecleankernel/layout/blspec.py` & `eclean_kernel-2.99.8/ecleankernel/layout/blspec.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# vim:fileencoding=utf-8
 # (c) 2020-2023 Michał Górny <mgorny@gentoo.org>
-# Released under the terms of the 2-clause BSD license.
+# (c) 2024 Andrew Ammerlaan <andrewammerlaan@gentoo.org>
+# SPDX-License-Identifier: GPL-2.0-or-later
 
+import distro
 import logging
 import os
 import typing
 
 from pathlib import Path
 
 from ecleankernel.file import (
@@ -49,22 +50,25 @@
                 break
             except FileNotFoundError:
                 pass
         else:
             raise LayoutNotFound("/etc/machine-id not found")
 
         for d in self.potential_dirs:
+            # Present if type 1
             bootloaderdir = root / d / "loader"
-            if bootloaderdir.is_dir():
+            # Present if type 2
+            ukidir = root / d / "EFI" / "Linux"
+            if bootloaderdir.is_dir() or ukidir.is_dir():
                 # Type 1 entries (linux+initrd) are in
                 # $BOOT/ENTRY-TOKEN/KERNEL-VERSION/
                 self.blsdir = root / d / self.kernel_id
                 # Type 2 entries (uki's) are in
                 # $BOOT/EFI/Linux/ENTRY-TOKEN-KERNEL-VERSION.efi
-                self.ukidir = root / d / "EFI" / "Linux"
+                self.ukidir = ukidir
                 return
         else:
             raise LayoutNotFound("/boot/[EFI/]loader not found")
 
     def append_kernel_files(self,
                             ftype: KernelFileType,
                             path: Path,
@@ -124,32 +128,40 @@
                         k, ver, module_dict, exclusions)
                 kernels[(ver, "bls")].all_files.append(
                     EmptyDirectory(dir_path))
 
         # collect from ESP/Linux
         if self.ukidir.is_dir():
             for file in os.listdir(self.ukidir):
-                if not file.endswith(".efi"):
+                basename = file.removesuffix(".efi")
+                if file == basename:
                     # Not an UKI
                     continue
 
-                ver = file.removeprefix(f"{self.kernel_id}-"
-                                        ).removeprefix("gentoo-")
-                if file == ver:
+                distro_id = distro.id() or "linux"
+
+                ver = basename.removeprefix(f"{self.kernel_id}-"
+                                            ).removeprefix(f"{distro_id}-")
+                if basename == ver:
                     # Not our UKI
                     continue
-                ver = ver.removesuffix(".efi")
 
                 kernels[(ver, "uki")] = self.append_kernel_files(
                         KernelFileType.KERNEL,
                         self.ukidir / file,
                         Kernel(ver, layout="uki"),
                         ver, module_dict,
                         exclusions)
 
+                uki_icon = self.ukidir / f"{basename}.png"
+                if (KernelFileType.MISC not in exclusions and
+                        os.path.isfile(uki_icon)):
+                    kernels[(ver, "uki")].all_files.append(GenericFile(
+                        uki_icon, KernelFileType.MISC))
+
         # merge unassociated modules into kernel groups
         for mkv, fobjs in module_dict.items():
             if any(mkv == k.real_kv for k in kernels.values()):
                 continue
             # this mkv does not have a corresponding kernel
             # with same real_kv in kernels
             match_found = False
```

### Comparing `eclean_kernel-2.99.7/ecleankernel/layout/moduledir.py` & `eclean_kernel-2.99.8/ecleankernel/layout/moduledir.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# vim:fileencoding=utf-8
 # (c) 2011-2020 Michał Górny <mgorny@gentoo.org>
-# Released under the terms of the 2-clause BSD license.
+# SPDX-License-Identifier: GPL-2.0-or-later
 
 import os
 import typing
 
 from pathlib import Path
 
 from ecleankernel.file import (
```

### Comparing `eclean_kernel-2.99.7/ecleankernel/layout/std.py` & `eclean_kernel-2.99.8/ecleankernel/layout/std.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# vim:fileencoding=utf-8
 # (c) 2011-2020 Michał Górny <mgorny@gentoo.org>
-# Released under the terms of the 2-clause BSD license.
+# (c) 2024 Andrew Ammerlaan <andrewammerlaan@gentoo.org>
+# SPDX-License-Identifier: GPL-2.0-or-later
 
+import distro
 import itertools
 import os
 import os.path
 import typing
 
 from ecleankernel.file import (
     KernelFileType,
@@ -43,14 +44,20 @@
         '.img',
 
         # config
         '.bz2',
         '.gz',
         '.lz',
         '.xz',
+
+        # refind
+        ".png",
+
+        # efistub
+        '.efi',
     ]
 
     def find_kernels(self,
                      exclusions: typing.Container[KernelFileType] = [],
                      ) -> typing.List[Kernel]:
         # this would wreak havok all around the place
         assert KernelFileType.KERNEL not in exclusions
@@ -59,62 +66,74 @@
         module_dict = self.get_module_dict(
             exclusions=exclusions,
             module_directory=self.root / 'lib/modules')
 
         # collect from /boot
         kernels: typing.Dict[str, typing.Dict[str, Kernel]] = {}
         other_files: typing.List[typing.Tuple[GenericFile, str]] = []
-        boot_directory = self.root / 'boot'
-        try:
-            diter = os.listdir(boot_directory)
-        except FileNotFoundError:
-            pass
-        else:
-            for fn in diter:
-                # skip hidden and GRUB signature files
-                if fn.startswith('.') or fn.endswith('.sig'):
-                    continue
-                path = boot_directory / fn
-                if path.is_symlink() or not path.is_file():
-                    continue
-                # skip unversioned files
-                ver = fn.partition('-')[2]
-                if not ver:
-                    continue
-
-                # strip suffix from filename to get the correct version
-                for suffix in self.suffixes:
-                    if ver.endswith(suffix):
-                        ver = ver[:-len(suffix)]
-                        break
-                    elif ver.endswith(suffix + '.old'):
-                        ver = ver[:-len(suffix)-4] + '.old'
 
-                # try recognizing kernel image via magic
+        distro_name = distro.name() or "Linux"
+
+        def find_std_files() -> typing.Iterator:
+            for directory in (self.root / 'boot',
+                              self.root / f"boot/EFI/EFI/{distro_name}",
+                              self.root / f"boot/efi/EFI/{distro_name}",
+                              self.root / f"boot/EFI/{distro_name}",
+                              self.root / f"efi/EFI/{distro_name}"):
                 try:
-                    kobj = KernelImage(path)
-                except UnrecognizedKernelError:
-                    # fall back to filename
-                    for ftype, prefix in self.prefixes:
-                        if ftype not in exclusions:
-                            if fn.startswith(prefix):
-                                other_files.append(
-                                    (GenericFile(path, ftype), ver))
-                                break
-                    continue
-
-                # the following is done only for kernel images
-                assert isinstance(kobj, KernelImage)
-                kg = kernels.setdefault(ver, {})
-                k = kg.setdefault(kobj.internal_version, Kernel(ver))
-                k.all_files.append(kobj)
-
-                # associate the module directory
-                k.all_files.extend(
-                    module_dict.get(kobj.internal_version, []))
+                    for file in os.listdir(directory):
+                        yield directory / file
+                except FileNotFoundError:
+                    pass
+
+        for path in find_std_files():
+            fn = path.name
+            # skip hidden and GRUB signature files
+            if fn.startswith('.') or fn.endswith('.sig'):
+                continue
+            if path.is_symlink() or not path.is_file():
+                continue
+            # skip unversioned files
+            ver = fn.partition('-')[2]
+            if not ver:
+                continue
+
+            # strip suffix from filename to get the correct version
+            for suffix in self.suffixes:
+                if ver.endswith(suffix):
+                    ver = ver[:-len(suffix)]
+                    break
+                elif ver.endswith(suffix + '.old'):
+                    ver = ver[:-len(suffix)-4] + '.old'
+
+            # try recognizing kernel image via magic
+            try:
+                kobj = KernelImage(path)
+            except UnrecognizedKernelError:
+                # fall back to filename
+                for ftype, prefix in self.prefixes:
+                    # kernel refind icon has same name as kernel +'.png'
+                    if fn.endswith(".png"):
+                        ftype = KernelFileType.MISC
+                    if ftype not in exclusions:
+                        if fn.startswith(prefix):
+                            other_files.append(
+                                (GenericFile(path, ftype), ver))
+                            break
+                continue
+
+            # the following is done only for kernel images
+            assert isinstance(kobj, KernelImage)
+            kg = kernels.setdefault(ver, {})
+            k = kg.setdefault(kobj.internal_version, Kernel(ver))
+            k.all_files.append(kobj)
+
+            # associate the module directory
+            k.all_files.extend(
+                module_dict.get(kobj.internal_version, []))
 
         # merge other files into kernel groups
         for fobj, ver in other_files:
             kg = kernels.setdefault(ver, {})
             # if we had some images with matching apparent version,
             # append to all of their Kernels; if we had none, create
             # a single Kernel object
```

### Comparing `eclean_kernel-2.99.7/ecleankernel/process.py` & `eclean_kernel-2.99.8/ecleankernel/process.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# vim:fileencoding=utf-8
 # (c) 2011-2020 Michał Górny <mgorny@gentoo.org>
-# Released under the terms of the 2-clause BSD license.
+# SPDX-License-Identifier: GPL-2.0-or-later
 
 import itertools
 import logging
 import os
 import os.path
 import typing
```

### Comparing `eclean_kernel-2.99.7/ecleankernel/sort.py` & `eclean_kernel-2.99.8/ecleankernel/sort.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# vim:fileencoding=utf-8
 # (c) 2020 Michał Górny <mgorny@gentoo.org>
-# Released under the terms of the 2-clause BSD license.
+# SPDX-License-Identifier: GPL-2.0-or-later
 
 import abc
 import re
 import typing
 
 from ecleankernel.kernel import Kernel
```

### Comparing `eclean_kernel-2.99.7/pyproject.toml` & `eclean_kernel-2.99.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "eclean-kernel"
 authors = [{name = "Michał Górny", email = "mgorny@gentoo.org"}]
-license = {file = "COPYING"}
+license = {text = "GPL-2.0-or-later"}
 readme = "README.rst"
 dynamic = ["version", "description"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: System Administrators",
-    "License :: OSI Approved :: BSD License",
+    "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
     "Operating System :: POSIX",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: System :: Installation/Setup"
 ]
 requires-python = ">=3.9"
+dependencies = [
+    "distro"
+]
 
 [project.optional-dependencies]
 test = ["pytest"]
 
 [project.urls]
 Homepage = "https://github.com/projg2/eclean-kernel/"
```

### Comparing `eclean_kernel-2.99.7/test/test_file.py` & `eclean_kernel-2.99.8/test/test_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# vim:fileencoding=utf-8
 # (c) 2020-2023 Michał Górny <mgorny@gentoo.org>
-# Released under the terms of the 2-clause BSD license.
+# SPDX-License-Identifier: GPL-2.0-or-later
 
 import gzip
 import hashlib
 import os
 import tempfile
 import unittest
```

### Comparing `eclean_kernel-2.99.7/test/test_layout_blspec.py` & `eclean_kernel-2.99.8/test/test_layout_blspec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# vim:fileencoding=utf-8
 # (c) 2020 Michał Górny <mgorny@gentoo.org>
-# Released under the terms of the 2-clause BSD license.
+# (c) 2024 Andrew Ammerlaan <andrewammerlaan@gentoo.org>
+# SPDX-License-Identifier: GPL-2.0-or-later
 
+import distro
 import os
 import tempfile
 import unittest
 
 from pathlib import Path
 
 from ecleankernel.__main__ import main
@@ -18,14 +19,16 @@
     )
 from ecleankernel.layout import LayoutNotFound
 from ecleankernel.layout.blspec import BlSpecLayout
 
 from test.test_file import write_bzImage
 from test.test_layout_std import make_test_files, kernel_paths
 
+distro_id = distro.id() or "linux"
+
 
 class BlSpecLayoutTests(unittest.TestCase):
     maxDiff = None
 
     machine_id = '0123456789abcdef0123456789abcdef'
     entry_token = "testsys"
 
@@ -38,15 +41,16 @@
                       efi_subdir: bool = False,
                       entry_token: bool = False,
                       ) -> tempfile.TemporaryDirectory:
         subdir = 'EFI/' if efi_subdir else ''
         entry = self.entry_token if entry_token else self.machine_id
         test_spec = [
             f"boot/{subdir}/EFI/Linux/{entry}-1.2.6.efi",
-            f"boot/{subdir}/EFI/Linux/{entry}-1.2.5.efi",
+            f"boot/{subdir}/EFI/Linux/{entry}-1.2.6.png",
+            f"boot/{subdir}/EFI/Linux/{distro_id}-1.2.5.efi",
             f"boot/{subdir}/{entry}/1.2.5/initrd",
             f"boot/{subdir}/{entry}/1.2.5/linux",
             f"boot/{subdir}/{entry}/1.2.4/initrd",
             f"boot/{subdir}/{entry}/1.2.3/initrd",
             f"boot/{subdir}/{entry}/1.2.3/linux",
             f"boot/{subdir}/{entry}/1.2.3/misc",
             f"boot/{subdir}/{entry}/1.2.2/initrd",
@@ -75,15 +79,16 @@
 
         with open(path / 'etc/machine-id', 'w') as f:
             f.write(f'{self.machine_id}\n')
         if entry_token:
             with open(path / "etc/kernel/entry-token", "w") as f:
                 f.write(f"{self.entry_token}\n")
         write_bzImage(bootsub / f"EFI/Linux/{entry}-1.2.6.efi", b'1.2.6 test')
-        write_bzImage(bootsub / f"EFI/Linux/{entry}-1.2.5.efi", b'1.2.5 test')
+        write_bzImage(bootsub / f"EFI/Linux/{distro_id}-1.2.5.efi",
+                      b'1.2.5 test')
         write_bzImage(bootsub / f"{entry}/1.2.5/linux", b'1.2.5 test')
         write_bzImage(bootsub / f"{entry}/1.2.3/linux", b'1.2.3 test')
         write_bzImage(bootsub / f"{entry}/1.2.2/linux", b'1.2.2 test')
         write_bzImage(bootsub / f"{entry}/1.2.1/linux", b'1.2.1 test')
         os.symlink('../../../usr/src/linux', modules / '1.2.6/build')
         os.symlink('../../../usr/src/linux', modules / '1.2.5/build')
         os.symlink('../../../usr/src/linux', modules / '1.2.3/build')
@@ -101,15 +106,15 @@
                        k122: bool = True,
                        k121: bool = True
                        ) -> None:
         """Assert whether specified kernels were removed or kept"""
         subdir = 'EFI/' if efi_subdir else ''
         files = {
             f'boot/{subdir}/EFI/Linux/{self.machine_id}-1.2.6.efi': k126,
-            f'boot/{subdir}/EFI/Linux/{self.machine_id}-1.2.5.efi': k125,
+            f'boot/{subdir}/EFI/Linux/{distro_id}-1.2.5.efi': k125,
             f'boot/{subdir}{self.machine_id}/1.2.5/initrd': k125,
             f'boot/{subdir}{self.machine_id}/1.2.5/linux': k125,
             f'boot/{subdir}{self.machine_id}/1.2.5': k125,
             f'boot/{subdir}{self.machine_id}/1.2.4/initrd': k124,
             f'boot/{subdir}{self.machine_id}/1.2.4': k124,
             f'boot/{subdir}{self.machine_id}/1.2.3/initrd': k123,
             f'boot/{subdir}{self.machine_id}/1.2.3/linux': k123,
@@ -230,22 +235,24 @@
                    KernelImage(blspath / '1.2.5/linux'),
                    ModuleDirectory(modules / '1.2.5'),
                    GenericFile(modules / '1.2.5/../../../usr/src/linux',
                                KFT.BUILD),
                    ],
                   '1.2.5'),
                  ('1.2.5',
-                  [KernelImage(ukipath / f"{self.machine_id}-1.2.5.efi"),
+                  [KernelImage(ukipath / f"{distro_id}-1.2.5.efi"),
                    ModuleDirectory(modules / '1.2.5'),
                    GenericFile(modules / '1.2.5/../../../usr/src/linux',
                                KFT.BUILD),
                    ],
                   '1.2.5'),
                  ('1.2.6',
                   [KernelImage(ukipath / f"{self.machine_id}-1.2.6.efi"),
+                   GenericFile(ukipath / f"{self.machine_id}-1.2.6.png",
+                               KFT.MISC),
                    ModuleDirectory(modules / '1.2.6'),
                    GenericFile(modules / '1.2.6/../../../usr/src/linux',
                                KFT.BUILD),
                    ],
                   '1.2.6'),
                  ])
 
@@ -298,15 +305,15 @@
                    KernelImage(blspath / '1.2.5/linux'),
                    ModuleDirectory(modules / '1.2.5'),
                    GenericFile(modules / '1.2.5/../../../usr/src/linux',
                                KFT.BUILD),
                    ],
                   '1.2.5'),
                  ('1.2.5',
-                  [KernelImage(ukipath / f"{self.machine_id}-1.2.5.efi"),
+                  [KernelImage(ukipath / f"{distro_id}-1.2.5.efi"),
                    ModuleDirectory(modules / '1.2.5'),
                    GenericFile(modules / '1.2.5/../../../usr/src/linux',
                                KFT.BUILD),
                    ],
                   '1.2.5'),
                  ('1.2.6',
                   [KernelImage(ukipath / f"{self.machine_id}-1.2.6.efi"),
@@ -362,21 +369,23 @@
                    GenericFile(blspath / '1.2.5/initrd', KFT.INITRAMFS),
                    KernelImage(blspath / '1.2.5/linux'),
                    GenericFile(modules / '1.2.5/../../../usr/src/linux',
                                KFT.BUILD),
                    ],
                   '1.2.5'),
                  ('1.2.5',
-                  [KernelImage(ukipath / f"{self.machine_id}-1.2.5.efi"),
+                  [KernelImage(ukipath / f"{distro_id}-1.2.5.efi"),
                    GenericFile(modules / '1.2.5/../../../usr/src/linux',
                                KFT.BUILD),
                    ],
                   '1.2.5'),
                  ('1.2.6',
                   [KernelImage(ukipath / f"{self.machine_id}-1.2.6.efi"),
+                   GenericFile(ukipath / f"{self.machine_id}-1.2.6.png",
+                               KFT.MISC),
                    GenericFile(modules / '1.2.6/../../../usr/src/linux',
                                KFT.BUILD),
                    ],
                   '1.2.6'),
                  ])
 
     def test_exclude_build(self) -> None:
@@ -423,20 +432,22 @@
                   [EmptyDirectory(blspath / '1.2.5'),
                    GenericFile(blspath / '1.2.5/initrd', KFT.INITRAMFS),
                    KernelImage(blspath / '1.2.5/linux'),
                    ModuleDirectory(modules / '1.2.5'),
                    ],
                   '1.2.5'),
                  ('1.2.5',
-                  [KernelImage(ukipath / f"{self.machine_id}-1.2.5.efi"),
+                  [KernelImage(ukipath / f"{distro_id}-1.2.5.efi"),
                    ModuleDirectory(modules / '1.2.5'),
                    ],
                   '1.2.5'),
                  ('1.2.6',
                   [KernelImage(ukipath / f"{self.machine_id}-1.2.6.efi"),
+                   GenericFile(ukipath / f"{self.machine_id}-1.2.6.png",
+                               KFT.MISC),
                    ModuleDirectory(modules / '1.2.6'),
                    ],
                   '1.2.6'),
                  ])
 
     def test_find_modules_EFI(self) -> None:
         with self.create_layout(efi_subdir=True) as td:
@@ -487,22 +498,24 @@
                    KernelImage(blspath / '1.2.5/linux'),
                    ModuleDirectory(modules / '1.2.5'),
                    GenericFile(modules / '1.2.5/../../../usr/src/linux',
                                KFT.BUILD),
                    ],
                   '1.2.5'),
                  ('1.2.5',
-                  [KernelImage(ukipath / f"{self.machine_id}-1.2.5.efi"),
+                  [KernelImage(ukipath / f"{distro_id}-1.2.5.efi"),
                    ModuleDirectory(modules / '1.2.5'),
                    GenericFile(modules / '1.2.5/../../../usr/src/linux',
                                KFT.BUILD),
                    ],
                   '1.2.5'),
                  ('1.2.6',
                   [KernelImage(ukipath / f"{self.machine_id}-1.2.6.efi"),
+                   GenericFile(ukipath / f"{self.machine_id}-1.2.6.png",
+                               KFT.MISC),
                    ModuleDirectory(modules / '1.2.6'),
                    GenericFile(modules / '1.2.6/../../../usr/src/linux',
                                KFT.BUILD),
                    ],
                   '1.2.6'),
                  ])
```

### Comparing `eclean_kernel-2.99.7/test/test_layout_std.py` & `eclean_kernel-2.99.8/test/test_layout_std.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-# vim:fileencoding=utf-8
 # (c) 2020 Michał Górny <mgorny@gentoo.org>
-# Released under the terms of the 2-clause BSD license.
+# (c) 2024 Andrew Ammerlaan <andrewammerlaan@gentoo.org>
+# SPDX-License-Identifier: GPL-2.0-or-later
 
 import io
+import distro
 import os
 import tempfile
 import typing
 import unittest
 
 from pathlib import Path
 from unittest.mock import patch
@@ -18,14 +19,16 @@
 from ecleankernel.layout.std import StdLayout
 
 from test.test_file import write_bzImage
 
 
 TEST_DATA_DIR = Path(__file__).parent / 'data'
 
+distro_name = distro.name() or "Linux"
+
 
 def kernel_paths(kd: typing.List[Kernel]
                  ) -> typing.Iterable[typing.Tuple[
                       str,
                       typing.List[GenericFile],
                       typing.Optional[str]]]:
     """Get iterable of tuples describing kernels"""
@@ -61,62 +64,82 @@
         test_spec = [
             'boot/vmlinuz-1.2.3',
             'boot/System.map-1.2.3',
             'boot/config-1.2.3',
             'boot/initrd-1.2.3.img',
         ]
         test_spec += [f'{x}.old' for x in test_spec]
+
+        """EFI Stub"""
+        test_spec += [
+            f"efi/EFI/{distro_name}/vmlinuz-1.2.1.efi",
+            f"efi/EFI/{distro_name}/vmlinuz-1.2.1.png",
+            f"efi/EFI/{distro_name}/System.map-1.2.1",
+            f"efi/EFI/{distro_name}/config-1.2.1",
+            f"efi/EFI/{distro_name}/initramfs-1.2.1.img",
+        ]
+
         test_spec += [
             'boot/config-1.2.4',
             'boot/vmlinuz-1.2.2',
             'boot/vmlinuz-1.2.2.sig',
             'boot/System.map-1.2.2',
+            'lib/modules/1.2.1/test.ko',
             'lib/modules/1.2.2/test.ko',
             'lib/modules/1.2.3/test.ko',
             'lib/modules/1.2.4/test.ko',
             'usr/src/linux/Makefile',
             # stray files
             'boot/System.map',
             'boot/config-',
         ]
 
         td = make_test_files(test_spec)
         path = Path(td.name)
         boot = path / 'boot'
+        efistub = path / f"efi/EFI/{distro_name}/"
         modules = path / 'lib/modules'
 
+        write_bzImage(efistub / 'vmlinuz-1.2.1.efi', b'1.2.1 test')
         write_bzImage(boot / 'vmlinuz-1.2.2', b'1.2.2 test')
         write_bzImage(boot / 'vmlinuz-1.2.3', b'1.2.3 test')
         write_bzImage(boot / 'vmlinuz-1.2.3.old', b'1.2.3 test')
+        os.symlink('../../../usr/src/linux', modules / '1.2.1/build')
         os.symlink('../../../usr/src/linux', modules / '1.2.2/build')
         os.symlink('../../../usr/src/linux', modules / '1.2.3/build')
 
         return td
 
     def assert_kernels(self,
                        root: Path,
                        k124: bool = True,
                        k123: bool = True,
                        k123old: bool = True,
                        k122: bool = True,
+                       k121: bool = True,
                        stray: bool = True
                        ) -> None:
         """Assert whether specified kernels were removed or kept"""
         files = {
             'boot/vmlinuz-1.2.3': k123,
             'boot/System.map-1.2.3': k123,
             'boot/config-1.2.3': k123,
             'boot/initrd-1.2.3.img': k123,
             'boot/vmlinuz-1.2.3.old': k123old,
             'boot/System.map-1.2.3.old': k123old,
             'boot/config-1.2.3.old': k123old,
             'boot/initrd-1.2.3.img.old': k123old,
             'boot/vmlinuz-1.2.2': k122,
             'boot/System.map-1.2.2': k122,
+            f"efi/EFI/{distro_name}/vmlinuz-1.2.1.efi": k121,
+            f"efi/EFI/{distro_name}/System.map-1.2.1": k121,
+            f"efi/EFI/{distro_name}/config-1.2.1": k121,
+            f"efi/EFI/{distro_name}/initramfs-1.2.1.img": k121,
             'boot/config-1.2.4': k124,
+            'lib/modules/1.2.1/test.ko': k121,
             'lib/modules/1.2.2/test.ko': k122,
             'lib/modules/1.2.2': k122,
             'lib/modules/1.2.3/test.ko': k123 or k123old,
             'lib/modules/1.2.3': k123 or k123old,
             'lib/modules/1.2.4/test.ko': k124,
             'lib/modules/1.2.4': k124,
             'lib/modules': True,
@@ -131,20 +154,32 @@
         found_files = [f for f in files if (root / f).exists()]
         self.assertEqual(found_files, expected_files)
 
     def test_find_modules(self) -> None:
         with self.create_layout() as td:
             path = Path(td)
             boot = path / 'boot'
+            efistub = path / f"efi/EFI/{distro_name}/"
             modules = path / 'lib/modules'
 
             self.assertEqual(
                 sorted(kernel_paths(
                     StdLayout(root=path).find_kernels())),
-                [('1.2.2',
+                [('1.2.1',
+                  [GenericFile(efistub / 'System.map-1.2.1', KFT.SYSTEM_MAP),
+                   GenericFile(efistub / 'config-1.2.1', KFT.CONFIG),
+                   GenericFile(efistub / 'initramfs-1.2.1.img', KFT.INITRAMFS),
+                   KernelImage(efistub / 'vmlinuz-1.2.1.efi'),
+                   GenericFile(efistub / "vmlinuz-1.2.1.png", KFT.MISC),
+                   ModuleDirectory(modules / '1.2.1'),
+                   GenericFile(modules / '1.2.1/../../../usr/src/linux',
+                               KFT.BUILD),
+                   ],
+                  '1.2.1'),
+                 ('1.2.2',
                   [GenericFile(boot / 'System.map-1.2.2', KFT.SYSTEM_MAP),
                    KernelImage(boot / 'vmlinuz-1.2.2'),
                    ModuleDirectory(modules / '1.2.2'),
                    GenericFile(modules / '1.2.2/../../../usr/src/linux',
                                KFT.BUILD),
                    ],
                   '1.2.2'),
@@ -174,21 +209,32 @@
                    ],
                   None)])
 
     def test_exclude_config(self) -> None:
         with self.create_layout() as td:
             path = Path(td)
             boot = path / 'boot'
+            efistub = path / f"efi/EFI/{distro_name}/"
             modules = path / 'lib/modules'
 
             self.assertEqual(
                 sorted(kernel_paths(
                     StdLayout(root=path).find_kernels(
                         exclusions=[KFT.CONFIG]))),
-                [('1.2.2',
+                [('1.2.1',
+                  [GenericFile(efistub / 'System.map-1.2.1', KFT.SYSTEM_MAP),
+                   GenericFile(efistub / 'initramfs-1.2.1.img', KFT.INITRAMFS),
+                   KernelImage(efistub / 'vmlinuz-1.2.1.efi'),
+                   GenericFile(efistub / "vmlinuz-1.2.1.png", KFT.MISC),
+                   ModuleDirectory(modules / '1.2.1'),
+                   GenericFile(modules / '1.2.1/../../../usr/src/linux',
+                               KFT.BUILD),
+                   ],
+                  '1.2.1'),
+                 ('1.2.2',
                   [GenericFile(boot / 'System.map-1.2.2', KFT.SYSTEM_MAP),
                    KernelImage(boot / 'vmlinuz-1.2.2'),
                    ModuleDirectory(modules / '1.2.2'),
                    GenericFile(modules / '1.2.2/../../../usr/src/linux',
                                KFT.BUILD),
                    ],
                   '1.2.2'),
@@ -215,21 +261,32 @@
                    ],
                   None)])
 
     def test_exclude_modules(self) -> None:
         with self.create_layout() as td:
             path = Path(td)
             boot = path / 'boot'
+            efistub = path / f"efi/EFI/{distro_name}/"
             modules = path / 'lib/modules'
 
             self.assertEqual(
                 sorted(kernel_paths(
                     StdLayout(root=path).find_kernels(
                         exclusions=[KFT.MODULES]))),
-                [('1.2.2',
+                [('1.2.1',
+                  [GenericFile(efistub / 'System.map-1.2.1', KFT.SYSTEM_MAP),
+                   GenericFile(efistub / 'config-1.2.1', KFT.CONFIG),
+                   GenericFile(efistub / 'initramfs-1.2.1.img', KFT.INITRAMFS),
+                   KernelImage(efistub / 'vmlinuz-1.2.1.efi'),
+                   GenericFile(efistub / "vmlinuz-1.2.1.png", KFT.MISC),
+                   GenericFile(modules / '1.2.1/../../../usr/src/linux',
+                               KFT.BUILD),
+                   ],
+                  '1.2.1'),
+                 ('1.2.2',
                   [GenericFile(boot / 'System.map-1.2.2', KFT.SYSTEM_MAP),
                    KernelImage(boot / 'vmlinuz-1.2.2'),
                    GenericFile(modules / '1.2.2/../../../usr/src/linux',
                                KFT.BUILD),
                    ],
                   '1.2.2'),
                  ('1.2.3',
@@ -255,21 +312,31 @@
                    ],
                   None)])
 
     def test_exclude_build(self) -> None:
         with self.create_layout() as td:
             path = Path(td)
             boot = path / 'boot'
+            efistub = path / f"efi/EFI/{distro_name}/"
             modules = path / 'lib/modules'
 
             self.assertEqual(
                 sorted(kernel_paths(
                     StdLayout(root=path).find_kernels(
                         exclusions=[KFT.BUILD]))),
-                [('1.2.2',
+                [('1.2.1',
+                  [GenericFile(efistub / 'System.map-1.2.1', KFT.SYSTEM_MAP),
+                   GenericFile(efistub / 'config-1.2.1', KFT.CONFIG),
+                   GenericFile(efistub / 'initramfs-1.2.1.img', KFT.INITRAMFS),
+                   KernelImage(efistub / 'vmlinuz-1.2.1.efi'),
+                   GenericFile(efistub / "vmlinuz-1.2.1.png", KFT.MISC),
+                   ModuleDirectory(modules / '1.2.1'),
+                   ],
+                  '1.2.1'),
+                 ('1.2.2',
                   [GenericFile(boot / 'System.map-1.2.2', KFT.SYSTEM_MAP),
                    KernelImage(boot / 'vmlinuz-1.2.2'),
                    ModuleDirectory(modules / '1.2.2'),
                    ],
                   '1.2.2'),
                  ('1.2.3',
                   [GenericFile(boot / 'System.map-1.2.3', KFT.SYSTEM_MAP),
@@ -347,15 +414,23 @@
 - vmlinuz: {td}/boot/vmlinuz-1.2.3.old
 - modules: {td}/lib/modules/1.2.3
 - build: {td}/lib/modules/1.2.3/../../../usr/src/linux
 other 1.2.2 [1.2.2]
 - systemmap: {td}/boot/System.map-1.2.2
 - vmlinuz: {td}/boot/vmlinuz-1.2.2
 - modules: {td}/lib/modules/1.2.2
-- build: {td}/lib/modules/1.2.2/../../../usr/src/linux'''.lstrip())
+- build: {td}/lib/modules/1.2.2/../../../usr/src/linux
+other 1.2.1 [1.2.1]
+- systemmap: {td}/efi/EFI/{distro_name}/System.map-1.2.1
+- config: {td}/efi/EFI/{distro_name}/config-1.2.1
+- initramfs: {td}/efi/EFI/{distro_name}/initramfs-1.2.1.img
+- vmlinuz: {td}/efi/EFI/{distro_name}/vmlinuz-1.2.1.efi
+- misc: {td}/efi/EFI/{distro_name}/vmlinuz-1.2.1.png
+- modules: {td}/lib/modules/1.2.1
+- build: {td}/lib/modules/1.2.1/../../../usr/src/linux'''.lstrip())
             self.assert_kernels(Path(td))
 
     def test_main_remove(self) -> None:
         with self.create_layout() as td:
             self.assertEqual(
                 main(['--destructive',
                       '--root', td, '--debug', '--no-mount']),
@@ -374,14 +449,15 @@
     def test_main_remove_all(self) -> None:
         with self.create_layout() as td:
             self.assertEqual(
                 main(['--all', '--destructive',
                       '--root', td, '--debug', '--no-mount']),
                 0)
             self.assert_kernels(Path(td),
+                                k121=False,
                                 k122=False,
                                 k123=False,
                                 k123old=False,
                                 k124=False)
 
     def test_main_remove_all_pretend(self) -> None:
         with self.create_layout() as td:
@@ -394,14 +470,15 @@
     def test_main_remove_n2(self) -> None:
         with self.create_layout() as td:
             self.assertEqual(
                 main(['--destructive', '-n', '2',
                       '--root', td, '--debug', '--no-mount']),
                 0)
             self.assert_kernels(Path(td),
+                                k121=False,
                                 k122=False,
                                 k124=False)
 
     def test_main_remove_n2_pretend(self) -> None:
         with self.create_layout() as td:
             self.assertEqual(
                 main(['--destructive', '-n', '2', '--pretend',
@@ -424,14 +501,15 @@
             os.environ['XDG_CONFIG_DIRS'] += f':{td}'
 
             self.assertEqual(
                 main(['--destructive',
                       '--root', td, '--debug', '--no-mount']),
                 0)
             self.assert_kernels(Path(td),
+                                k121=False,
                                 k122=False,
                                 k124=False)
 
     def test_config_file_user(self) -> None:
         with self.create_layout() as td:
             path = Path(td)
             os.mkdir(path / 'system')
@@ -443,9 +521,10 @@
             os.environ['XDG_CONFIG_HOME'] = td
 
             self.assertEqual(
                 main(['--destructive',
                       '--root', td, '--debug', '--no-mount']),
                 0)
             self.assert_kernels(Path(td),
+                                k121=False,
                                 k122=False,
                                 k124=False)
```

### Comparing `eclean_kernel-2.99.7/test/test_process.py` & `eclean_kernel-2.99.8/test/test_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# vim:fileencoding=utf-8
 # (c) 2020 Michał Górny <mgorny@gentoo.org>
-# Released under the terms of the 2-clause BSD license.
+# SPDX-License-Identifier: GPL-2.0-or-later
 
 import os
 import tempfile
 import typing
 import unittest
 
 from pathlib import Path
```

### Comparing `eclean_kernel-2.99.7/test/test_sort.py` & `eclean_kernel-2.99.8/test/test_sort.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# vim:fileencoding=utf-8
 # (c) 2020 Michał Górny <mgorny@gentoo.org>
-# Released under the terms of the 2-clause BSD license.
+# SPDX-License-Identifier: GPL-2.0-or-later
 
 import os
 import tempfile
 import time
 import unittest
 
 from pathlib import Path
```

### Comparing `eclean_kernel-2.99.7/tox.ini` & `eclean_kernel-2.99.8/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tox]
-envlist = qa,py38,py39,py310,py311,py312,pypy3
+envlist = qa,py39,py310,py311,py312,pypy3
 skip_missing_interpreters = True
 isolated_build = True
 
 [testenv]
+deps =
+	mypy
 extras =
 	test
 commands =
 	pytest -vv {posargs:test}
+	mypy {posargs:ecleankernel test}
 
 [testenv:qa]
 basepython = python3
 ignore_errors = True
 skip_install = True
 deps =
-	mypy
 	pycodestyle
 	pyflakes
 commands =
-	mypy {posargs:ecleankernel test}
 	pyflakes {posargs:ecleankernel test}
 	pycodestyle {posargs:ecleankernel test}
 
 [testenv:upload]
 skip_install = True
 deps =
 	build
```

### Comparing `eclean_kernel-2.99.7/PKG-INFO` & `eclean_kernel-2.99.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: eclean-kernel
-Version: 2.99.7
+Version: 2.99.8
 Summary: Installed kernel cleanup tool
 Author-email: Michał Górny <mgorny@gentoo.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: System :: Installation/Setup
+Requires-Dist: distro
 Requires-Dist: pytest ; extra == "test"
 Project-URL: Homepage, https://github.com/projg2/eclean-kernel/
 Provides-Extra: test
 
 eclean-kernel
 =============
```

