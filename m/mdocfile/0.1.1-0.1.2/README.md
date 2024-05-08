# Comparing `tmp/mdocfile-0.1.1.tar.gz` & `tmp/mdocfile-0.1.2.tar.gz`

## Comparing `mdocfile-0.1.1.tar` & `mdocfile-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 mdocfile-0.1.1/.github_changelog_generator
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 mdocfile-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 mdocfile-0.1.1/MANIFEST.in
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 mdocfile-0.1.1/mkdocs.yml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 mdocfile-0.1.1/tox.ini
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 mdocfile-0.1.1/.github/workflows/build-and-deploy-docs.yml
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 mdocfile-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 mdocfile-0.1.1/docs/index.md
--rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 mdocfile-0.1.1/docs/writing.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mdocfile-0.1.1/src/mdocfile/__init__.py
--rw-r--r--   0        0        0     6768 2020-02-02 00:00:00.000000 mdocfile-0.1.1/src/mdocfile/data_models.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 mdocfile-0.1.1/src/mdocfile/functions.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 mdocfile-0.1.1/src/mdocfile/utils.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 mdocfile-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 mdocfile-0.1.1/tests/test_data_models.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 mdocfile-0.1.1/tests/test_functions.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 mdocfile-0.1.1/tests/test_data/frame_set_multiple.mdoc
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 mdocfile-0.1.1/tests/test_data/frame_set_single.mdoc
--rw-r--r--   0        0        0    43777 2020-02-02 00:00:00.000000 mdocfile-0.1.1/tests/test_data/montage_section.mdoc
--rw-r--r--   0        0        0    68940 2020-02-02 00:00:00.000000 mdocfile-0.1.1/tests/test_data/montage_section_multiple.mdoc
--rw-r--r--   0        0        0    20443 2020-02-02 00:00:00.000000 mdocfile-0.1.1/tests/test_data/tilt_series.mdoc
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 mdocfile-0.1.1/.gitignore
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 mdocfile-0.1.1/LICENSE
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 mdocfile-0.1.1/README.md
--rw-r--r--   0        0        0     4295 2020-02-02 00:00:00.000000 mdocfile-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 mdocfile-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 mdocfile-0.1.2/.github_changelog_generator
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 mdocfile-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 mdocfile-0.1.2/MANIFEST.in
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 mdocfile-0.1.2/mkdocs.yml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 mdocfile-0.1.2/tox.ini
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 mdocfile-0.1.2/.github/workflows/build-and-deploy-docs.yml
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 mdocfile-0.1.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 mdocfile-0.1.2/docs/index.md
+-rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 mdocfile-0.1.2/docs/writing.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mdocfile-0.1.2/src/mdocfile/__init__.py
+-rw-r--r--   0        0        0     6781 2020-02-02 00:00:00.000000 mdocfile-0.1.2/src/mdocfile/data_models.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 mdocfile-0.1.2/src/mdocfile/functions.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 mdocfile-0.1.2/src/mdocfile/utils.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 mdocfile-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 mdocfile-0.1.2/tests/test_data_models.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 mdocfile-0.1.2/tests/test_functions.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 mdocfile-0.1.2/tests/test_data/frame_set_multiple.mdoc
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 mdocfile-0.1.2/tests/test_data/frame_set_single.mdoc
+-rw-r--r--   0        0        0    43777 2020-02-02 00:00:00.000000 mdocfile-0.1.2/tests/test_data/montage_section.mdoc
+-rw-r--r--   0        0        0    68940 2020-02-02 00:00:00.000000 mdocfile-0.1.2/tests/test_data/montage_section_multiple.mdoc
+-rw-r--r--   0        0        0    20443 2020-02-02 00:00:00.000000 mdocfile-0.1.2/tests/test_data/tilt_series.mdoc
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 mdocfile-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 mdocfile-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 mdocfile-0.1.2/README.md
+-rw-r--r--   0        0        0     4295 2020-02-02 00:00:00.000000 mdocfile-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 mdocfile-0.1.2/PKG-INFO
```

### Comparing `mdocfile-0.1.1/.pre-commit-config.yaml` & `mdocfile-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mdocfile-0.1.1/mkdocs.yml` & `mdocfile-0.1.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mdocfile-0.1.1/.github/workflows/build-and-deploy-docs.yml` & `mdocfile-0.1.2/.github/workflows/build-and-deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `mdocfile-0.1.1/.github/workflows/ci.yml` & `mdocfile-0.1.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `mdocfile-0.1.1/docs/index.md` & `mdocfile-0.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `mdocfile-0.1.1/docs/writing.md` & `mdocfile-0.1.2/docs/writing.md`

 * *Files identical despite different names*

### Comparing `mdocfile-0.1.1/src/mdocfile/data_models.py` & `mdocfile-0.1.2/src/mdocfile/data_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     YedgeDxy: Optional[Tuple[float, float]] = None
     XedgeDxyVS: Optional[Union[Tuple[float, float], Tuple[float, float, float]]] = None
     YedgeDxyVS: Optional[Union[Tuple[float, float], Tuple[float, float, float]]] = None
     StageOffsets: Optional[Tuple[float, float]] = None
     AlignedPieceCoords: Optional[Union[Tuple[float, float], Tuple[float, float, float]]] = None
     AlignedPieceCoordsVS: Optional[
         Union[Tuple[float, float], Tuple[float, float, float]]] = None
-    SubFramePath: Optional[PureWindowsPath] = None
+    SubFramePath: Optional[Union[PureWindowsPath, Path]] = None
     NumSubFrames: Optional[int] = None
     FrameDosesAndNumbers: Optional[Sequence[Tuple[float, int]]] = None
     DateTime: Optional[str] = None
     NavigatorLabel: Optional[str] = None
     FilterSlitAndLoss: Optional[Tuple[float, float]] = None
     ChannelName: Optional[str] = None
     MultiShotHoleAndPosition: Optional[Union[Tuple[int, int], Tuple[int, int, int]]] = None
```

### Comparing `mdocfile-0.1.1/src/mdocfile/functions.py` & `mdocfile-0.1.2/src/mdocfile/functions.py`

 * *Files identical despite different names*

### Comparing `mdocfile-0.1.1/src/mdocfile/utils.py` & `mdocfile-0.1.2/src/mdocfile/utils.py`

 * *Files identical despite different names*

### Comparing `mdocfile-0.1.1/tests/conftest.py` & `mdocfile-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mdocfile-0.1.1/tests/test_data_models.py` & `mdocfile-0.1.2/tests/test_data_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,7 +85,10 @@
         tmp.write(mdoc.to_string().encode())
         mdoc2 = Mdoc.from_file(tmp.name)
     mdoc_dict = mdoc.section_data[0].model_dump()
     mdoc2_dict = mdoc2.section_data[0].model_dump()
     for (k1, v1), (k2, v2) in zip(mdoc_dict.items(), mdoc2_dict.items()):
         assert v1 == v2
         assert k1 == k2
+
+def test_section_data_from_path():
+    section = MdocSectionData(SubFramePath=Path('bla.tif'))
```

### Comparing `mdocfile-0.1.1/tests/test_functions.py` & `mdocfile-0.1.2/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `mdocfile-0.1.1/tests/test_data/frame_set_multiple.mdoc` & `mdocfile-0.1.2/tests/test_data/frame_set_multiple.mdoc`

 * *Files identical despite different names*

### Comparing `mdocfile-0.1.1/tests/test_data/frame_set_single.mdoc` & `mdocfile-0.1.2/tests/test_data/frame_set_single.mdoc`

 * *Files identical despite different names*

### Comparing `mdocfile-0.1.1/tests/test_data/montage_section.mdoc` & `mdocfile-0.1.2/tests/test_data/montage_section.mdoc`

 * *Files identical despite different names*

### Comparing `mdocfile-0.1.1/tests/test_data/montage_section_multiple.mdoc` & `mdocfile-0.1.2/tests/test_data/montage_section_multiple.mdoc`

 * *Files identical despite different names*

### Comparing `mdocfile-0.1.1/tests/test_data/tilt_series.mdoc` & `mdocfile-0.1.2/tests/test_data/tilt_series.mdoc`

 * *Files identical despite different names*

### Comparing `mdocfile-0.1.1/.gitignore` & `mdocfile-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mdocfile-0.1.1/LICENSE` & `mdocfile-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mdocfile-0.1.1/README.md` & `mdocfile-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mdocfile-0.1.1/pyproject.toml` & `mdocfile-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mdocfile-0.1.1/PKG-INFO` & `mdocfile-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: mdocfile
-Version: 0.1.1
+Version: 0.1.2
 Summary: SerialEM mdoc files as pandas dataframes.
 Project-URL: homepage, https://github.com/teamtomo/mdocfile
 Project-URL: repository, https://github.com/teamtomo/mdocfile
 Author-email: Alister Burt <alisterburt@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

