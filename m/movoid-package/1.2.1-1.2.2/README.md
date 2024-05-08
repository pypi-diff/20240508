# Comparing `tmp/movoid_package-1.2.1.tar.gz` & `tmp/movoid_package-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_package-1.2.1.tar", last modified: Sat Apr 20 15:52:45 2024, max compression
+gzip compressed data, was "movoid_package-1.2.2.tar", last modified: Wed May  8 15:56:46 2024, max compression
```

## Comparing `movoid_package-1.2.1.tar` & `movoid_package-1.2.2.tar`

### file list

```diff
@@ -1,20 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 15:52:45.345510 movoid_package-1.2.1/
--rw-rw-rw-   0        0        0      212 2024-04-20 15:52:45.344513 movoid_package-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_package-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 15:52:45.328946 movoid_package-1.2.1/movoid_package/
--rw-rw-rw-   0        0        0      253 2024-03-04 17:02:37.000000 movoid_package-1.2.1/movoid_package/__init__.py
--rw-rw-rw-   0        0        0     2902 2024-03-04 15:17:35.000000 movoid_package-1.2.1/movoid_package/for_import.py
--rw-rw-rw-   0        0        0    13774 2024-04-20 15:50:56.000000 movoid_package-1.2.1/movoid_package/stub.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:52:45.343516 movoid_package-1.2.1/movoid_package.egg-info/
--rw-rw-rw-   0        0        0      212 2024-04-20 15:52:45.000000 movoid_package-1.2.1/movoid_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-04-20 15:52:45.000000 movoid_package-1.2.1/movoid_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 15:52:45.000000 movoid_package-1.2.1/movoid_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-20 15:52:45.000000 movoid_package-1.2.1/movoid_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 15:52:45.345510 movoid_package-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      461 2024-04-20 15:51:43.000000 movoid_package-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:52:45.342520 movoid_package-1.2.1/test/
--rw-rw-rw-   0        0        0     1617 2024-03-03 15:42:19.000000 movoid_package-1.2.1/test/__init__.py
--rw-rw-rw-   0        0        0      732 2024-03-04 16:41:42.000000 movoid_package-1.2.1/test/test1.py
--rw-rw-rw-   0        0        0      573 2024-03-04 16:52:19.000000 movoid_package-1.2.1/test/test1.pyi
--rw-rw-rw-   0        0        0      245 2024-03-04 16:29:14.000000 movoid_package-1.2.1/test/test2.py
--rw-rw-rw-   0        0        0      396 2024-04-20 15:19:33.000000 movoid_package-1.2.1/test/test3.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:56:46.110339 movoid_package-1.2.2/
+-rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_package-1.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      212 2024-05-08 15:56:46.109342 movoid_package-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_package-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 15:56:46.098195 movoid_package-1.2.2/movoid_package/
+-rw-rw-rw-   0        0        0      253 2024-03-04 17:02:37.000000 movoid_package-1.2.2/movoid_package/__init__.py
+-rw-rw-rw-   0        0        0     2902 2024-03-04 15:17:35.000000 movoid_package-1.2.2/movoid_package/for_import.py
+-rw-rw-rw-   0        0        0    13862 2024-05-08 15:41:29.000000 movoid_package-1.2.2/movoid_package/stub.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:56:46.103240 movoid_package-1.2.2/movoid_package.egg-info/
+-rw-rw-rw-   0        0        0      212 2024-05-08 15:56:46.000000 movoid_package-1.2.2/movoid_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2024-05-08 15:56:46.000000 movoid_package-1.2.2/movoid_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 15:56:46.000000 movoid_package-1.2.2/movoid_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-08 15:56:46.000000 movoid_package-1.2.2/movoid_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 15:56:46.110339 movoid_package-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      461 2024-05-08 15:56:12.000000 movoid_package-1.2.2/setup.py
```

### Comparing `movoid_package-1.2.1/movoid_package/for_import.py` & `movoid_package-1.2.2/movoid_package/for_import.py`

 * *Files identical despite different names*

### Comparing `movoid_package-1.2.1/movoid_package/stub.py` & `movoid_package-1.2.2/movoid_package/stub.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,20 +203,22 @@
 
     def _read_class_init_variable(self):
         with self._file_path.open(mode='r', encoding=self._encoding) as file:
             file_text = file.read()
             class_text = re.findall(r'\nclass (.*?)(\(|:)((.|\s)*?)(\n\S|$)', file_text)
             for class_one in class_text:
                 class_name = class_one[0]
-                init_text = re.search(r'\n(\t| {4})def __init__((.|\s)*?)(\n(\t| {4})\S|$)', class_one[2]).group(2)
-                super_text = re.search(r'\n(\t| {4}){2}(super.*)', init_text).group(2)
-                self_text = [list(_) for _ in re.findall(r'\n(\t| {4}){2}(self\..*?):(.*?)=(.*)', init_text)]
-                for _i in self_text:
-                    _i[2] = _i[2].strip(' ')
-                self._class_init_variable[class_name] = {'super': super_text, 'self': self_text}
+                init_re = re.search(r'\n(\t| {4})def __init__((.|\s)*?)(\n(\t| {4})\S|$)', class_one[2])
+                if init_re:
+                    init_text = init_re.group(2)
+                    super_text = re.search(r'\n(\t| {4}){2}(super.*)', init_text).group(2)
+                    self_text = [list(_) for _ in re.findall(r'\n(\t| {4}){2}(self\..*?):(.*?)=(.*)', init_text)]
+                    for _i in self_text:
+                        _i[2] = _i[2].strip(' ')
+                    self._class_init_variable[class_name] = {'super': super_text, 'self': self_text}
 
     def _exploit_annotation(self, anno: Any, starting: str = ': ') -> str:
         annotation_string = ''
         if anno != inspect.Parameter.empty:
             annotation_string += starting + self._get_element_name_with_module(anno)
         return annotation_string
```

