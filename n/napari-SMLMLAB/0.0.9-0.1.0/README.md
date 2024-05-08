# Comparing `tmp/napari_smlmlab-0.0.9.tar.gz` & `tmp/napari_smlmlab-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\turnerp\PycharmProjects\napari-SMLMLAB\dist\.tmp-ara6p5wv\napari_smlmlab-0.0.9.tar", last modified: Tue Apr 30 13:09:44 2024, max compression
+gzip compressed data, was "C:\Users\turnerp\PycharmProjects\napari-SMLMLAB\dist\.tmp-mqpxpvd3\napari_smlmlab-0.1.0.tar", last modified: Wed May  8 14:34:50 2024, max compression
```

## Comparing `napari_smlmlab-0.0.9.tar` & `napari_smlmlab-0.1.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 13:09:44.848864 napari_smlmlab-0.0.9/
--rw-rw-rw-   0        0        0     1515 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      101 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     4645 2024-04-30 13:09:44.848864 napari_smlmlab-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     2854 2024-04-25 14:22:00.000000 napari_smlmlab-0.0.9/README.md
--rw-rw-rw-   0        0        0     1243 2024-04-24 10:36:49.000000 napari_smlmlab-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0     1819 2024-04-30 13:09:44.859080 napari_smlmlab-0.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-30 13:09:44.769051 napari_smlmlab-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-30 13:09:44.848864 napari_smlmlab-0.0.9/src/napari_SMLMLAB.egg-info/
--rw-rw-rw-   0        0        0     4645 2024-04-30 13:09:44.000000 napari_smlmlab-0.0.9/src/napari_SMLMLAB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      731 2024-04-30 13:09:44.000000 napari_smlmlab-0.0.9/src/napari_SMLMLAB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 13:09:44.000000 napari_smlmlab-0.0.9/src/napari_SMLMLAB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-30 13:09:44.000000 napari_smlmlab-0.0.9/src/napari_SMLMLAB.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      148 2024-04-30 13:09:44.000000 napari_smlmlab-0.0.9/src/napari_SMLMLAB.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-30 13:09:44.000000 napari_smlmlab-0.0.9/src/napari_SMLMLAB.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-30 13:09:44.809130 napari_smlmlab-0.0.9/src/smlmlab/
--rw-rw-rw-   0        0        0      102 2024-04-30 13:09:31.000000 napari_smlmlab-0.0.9/src/smlmlab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 13:09:44.819657 napari_smlmlab-0.0.9/src/smlmlab/_tests/
--rw-rw-rw-   0        0        0        0 2024-04-24 10:36:50.000000 napari_smlmlab-0.0.9/src/smlmlab/_tests/__init__.py
--rw-rw-rw-   0        0        0     2176 2024-04-25 13:50:35.000000 napari_smlmlab-0.0.9/src/smlmlab/_tests/test_widget.py
--rw-rw-rw-   0        0        0    14371 2024-04-30 11:06:04.000000 napari_smlmlab-0.0.9/src/smlmlab/_widget.py
--rw-rw-rw-   0        0        0    36584 2024-04-29 11:00:01.000000 napari_smlmlab-0.0.9/src/smlmlab/gui.py
--rw-rw-rw-   0        0        0      502 2024-04-25 13:52:37.000000 napari_smlmlab-0.0.9/src/smlmlab/napari.yaml
-drwxrwxrwx   0        0        0        0 2024-04-30 13:09:44.848864 napari_smlmlab-0.0.9/src/smlmlab/utils/
--rw-rw-rw-   0        0        0        0 2024-04-24 11:59:46.000000 napari_smlmlab-0.0.9/src/smlmlab/utils/__init__.py
--rw-rw-rw-   0        0        0     9793 2024-04-25 12:48:07.000000 napari_smlmlab-0.0.9/src/smlmlab/utils/compute_utils.py
--rw-rw-rw-   0        0        0    29078 2024-04-30 10:33:27.000000 napari_smlmlab-0.0.9/src/smlmlab/utils/events_utils.py
--rw-rw-rw-   0        0        0    21257 2024-04-30 08:13:50.000000 napari_smlmlab-0.0.9/src/smlmlab/utils/import_utils.py
--rw-rw-rw-   0        0        0    31463 2024-04-26 16:23:10.000000 napari_smlmlab-0.0.9/src/smlmlab/utils/loc_utils.py
--rw-rw-rw-   0        0        0    24786 2024-04-26 20:50:24.000000 napari_smlmlab-0.0.9/src/smlmlab/utils/picasso_utils.py
--rw-rw-rw-   0        0        0     9607 2024-04-29 10:09:03.000000 napari_smlmlab-0.0.9/src/smlmlab/utils/undrift_utils.py
--rw-rw-rw-   0        0        0     8197 2024-04-26 20:55:11.000000 napari_smlmlab-0.0.9/src/smlmlab/utils/viewer_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:34:50.085157 napari_smlmlab-0.1.0/
+-rw-rw-rw-   0        0        0     1515 2024-04-24 10:36:49.000000 napari_smlmlab-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-04-24 10:36:49.000000 napari_smlmlab-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4669 2024-05-08 14:34:50.085157 napari_smlmlab-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2854 2024-04-25 14:22:00.000000 napari_smlmlab-0.1.0/README.md
+-rw-rw-rw-   0        0        0     1243 2024-04-24 10:36:49.000000 napari_smlmlab-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1829 2024-05-08 14:34:50.089107 napari_smlmlab-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 14:34:50.011745 napari_smlmlab-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-08 14:34:50.082153 napari_smlmlab-0.1.0/src/napari_SMLMLAB.egg-info/
+-rw-rw-rw-   0        0        0     4669 2024-05-08 14:34:49.000000 napari_smlmlab-0.1.0/src/napari_SMLMLAB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      763 2024-05-08 14:34:50.000000 napari_smlmlab-0.1.0/src/napari_SMLMLAB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 14:34:49.000000 napari_smlmlab-0.1.0/src/napari_SMLMLAB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-08 14:34:49.000000 napari_smlmlab-0.1.0/src/napari_SMLMLAB.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      156 2024-05-08 14:34:49.000000 napari_smlmlab-0.1.0/src/napari_SMLMLAB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-08 14:34:49.000000 napari_smlmlab-0.1.0/src/napari_SMLMLAB.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 14:34:50.049198 napari_smlmlab-0.1.0/src/smlmlab/
+-rw-rw-rw-   0        0        0      102 2024-05-08 14:33:29.000000 napari_smlmlab-0.1.0/src/smlmlab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:34:50.053205 napari_smlmlab-0.1.0/src/smlmlab/_tests/
+-rw-rw-rw-   0        0        0        0 2024-04-24 10:36:50.000000 napari_smlmlab-0.1.0/src/smlmlab/_tests/__init__.py
+-rw-rw-rw-   0        0        0     2176 2024-04-25 13:50:35.000000 napari_smlmlab-0.1.0/src/smlmlab/_tests/test_widget.py
+-rw-rw-rw-   0        0        0    12689 2024-05-08 14:33:46.000000 napari_smlmlab-0.1.0/src/smlmlab/_widget.py
+-rw-rw-rw-   0        0        0    43726 2024-05-08 13:37:00.000000 napari_smlmlab-0.1.0/src/smlmlab/gui.py
+-rw-rw-rw-   0        0        0      502 2024-04-25 13:52:37.000000 napari_smlmlab-0.1.0/src/smlmlab/napari.yaml
+drwxrwxrwx   0        0        0        0 2024-05-08 14:34:50.079163 napari_smlmlab-0.1.0/src/smlmlab/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-24 11:59:46.000000 napari_smlmlab-0.1.0/src/smlmlab/utils/__init__.py
+-rw-rw-rw-   0        0        0     9793 2024-04-25 12:48:07.000000 napari_smlmlab-0.1.0/src/smlmlab/utils/compute_utils.py
+-rw-rw-rw-   0        0        0    29165 2024-05-08 11:10:02.000000 napari_smlmlab-0.1.0/src/smlmlab/utils/events_utils.py
+-rw-rw-rw-   0        0        0    21490 2024-05-08 11:10:02.000000 napari_smlmlab-0.1.0/src/smlmlab/utils/import_utils.py
+-rw-rw-rw-   0        0        0    31463 2024-04-26 16:23:10.000000 napari_smlmlab-0.1.0/src/smlmlab/utils/loc_utils.py
+-rw-rw-rw-   0        0        0    24786 2024-04-26 20:50:24.000000 napari_smlmlab-0.1.0/src/smlmlab/utils/picasso_utils.py
+-rw-rw-rw-   0        0        0    12393 2024-05-08 12:05:51.000000 napari_smlmlab-0.1.0/src/smlmlab/utils/plot_utils.py
+-rw-rw-rw-   0        0        0     9607 2024-04-29 10:09:03.000000 napari_smlmlab-0.1.0/src/smlmlab/utils/undrift_utils.py
+-rw-rw-rw-   0        0        0     8199 2024-05-07 14:43:51.000000 napari_smlmlab-0.1.0/src/smlmlab/utils/viewer_utils.py
```

### Comparing `napari_smlmlab-0.0.9/LICENSE` & `napari_smlmlab-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.9/PKG-INFO` & `napari_smlmlab-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-SMLMLAB
-Version: 0.0.9
+Version: 0.1.0
 Summary: Napari widget for BP04 Practical
 Home-page: https://github.com/piedrro/napari-SMLMLAB
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-SMLMLAB/issues
 Project-URL: Documentation, https://github.com/piedrro/napari-SMLMLAB#README.md
@@ -32,14 +32,15 @@
 Requires-Dist: scipy
 Requires-Dist: pyqtgraph
 Requires-Dist: picassosr
 Requires-Dist: matplotlib
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Requires-Dist: pyqt5-tools
+Requires-Dist: trackpy
 Provides-Extra: testing
 Requires-Dist: tox; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-qt; extra == "testing"
 Requires-Dist: napari; extra == "testing"
 Requires-Dist: pyqt5; extra == "testing"
```

### Comparing `napari_smlmlab-0.0.9/README.md` & `napari_smlmlab-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.9/pyproject.toml` & `napari_smlmlab-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.9/setup.cfg` & `napari_smlmlab-0.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -74,41 +74,42 @@
 00000490: 7569 7265 7320 3d20 0d0a 096e 6170 6172  uires = ...napar
 000004a0: 695b 616c 6c5d 0d0a 096e 756d 7079 0d0a  i[all]...numpy..
 000004b0: 096d 6167 6963 6775 690d 0a09 7174 7079  .magicgui...qtpy
 000004c0: 0d0a 0973 6369 7079 0d0a 0970 7971 7467  ...scipy...pyqtg
 000004d0: 7261 7068 0d0a 0970 6963 6173 736f 7372  raph...picassosr
 000004e0: 0d0a 096d 6174 706c 6f74 6c69 620d 0a09  ...matplotlib...
 000004f0: 7363 6970 790d 0a09 7471 646d 0d0a 0970  scipy...tqdm...p
-00000500: 7971 7435 2d74 6f6f 6c73 0d0a 7079 7468  yqt5-tools..pyth
-00000510: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-00000520: 332e 390d 0a69 6e63 6c75 6465 5f70 6163  3.9..include_pac
-00000530: 6b61 6765 5f64 6174 6120 3d20 5472 7565  kage_data = True
-00000540: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
-00000550: 0d0a 093d 7372 630d 0a0d 0a5b 6f70 7469  ...=src....[opti
-00000560: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
-00000570: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
-00000580: 0a0d 0a5b 6f70 7469 6f6e 732e 656e 7472  ...[options.entr
-00000590: 795f 706f 696e 7473 5d0d 0a6e 6170 6172  y_points]..napar
-000005a0: 692e 6d61 6e69 6665 7374 203d 200d 0a09  i.manifest = ...
-000005b0: 6e61 7061 7269 2d53 4d4c 4d4c 4142 203d  napari-SMLMLAB =
-000005c0: 2073 6d6c 6d6c 6162 3a6e 6170 6172 692e   smlmlab:napari.
-000005d0: 7961 6d6c 0d0a 0d0a 5b6f 7074 696f 6e73  yaml....[options
-000005e0: 2e65 7874 7261 735f 7265 7175 6972 655d  .extras_require]
-000005f0: 0d0a 7465 7374 696e 6720 3d20 0d0a 0974  ..testing = ...t
-00000600: 6f78 0d0a 0970 7974 6573 7420 2023 2068  ox...pytest  # h
-00000610: 7474 7073 3a2f 2f64 6f63 732e 7079 7465  ttps://docs.pyte
-00000620: 7374 2e6f 7267 2f65 6e2f 6c61 7465 7374  st.org/en/latest
-00000630: 2f63 6f6e 7465 6e74 732e 6874 6d6c 0d0a  /contents.html..
-00000640: 0970 7974 6573 742d 636f 7620 2023 2068  .pytest-cov  # h
-00000650: 7474 7073 3a2f 2f70 7974 6573 742d 636f  ttps://pytest-co
-00000660: 762e 7265 6164 7468 6564 6f63 732e 696f  v.readthedocs.io
-00000670: 2f65 6e2f 6c61 7465 7374 2f0d 0a09 7079  /en/latest/...py
-00000680: 7465 7374 2d71 7420 2023 2068 7474 7073  test-qt  # https
-00000690: 3a2f 2f70 7974 6573 742d 7174 2e72 6561  ://pytest-qt.rea
-000006a0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-000006b0: 6174 6573 742f 0d0a 096e 6170 6172 690d  atest/...napari.
-000006c0: 0a09 7079 7174 350d 0a0d 0a5b 6f70 7469  ..pyqt5....[opti
-000006d0: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
-000006e0: 5d0d 0a2a 203d 202a 2e79 616d 6c0d 0a0d  ]..* = *.yaml...
-000006f0: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-00000700: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-00000710: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000500: 7971 7435 2d74 6f6f 6c73 0d0a 0974 7261  yqt5-tools...tra
+00000510: 636b 7079 0d0a 7079 7468 6f6e 5f72 6571  ckpy..python_req
+00000520: 7569 7265 7320 3d20 3e3d 332e 390d 0a69  uires = >=3.9..i
+00000530: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
+00000540: 6174 6120 3d20 5472 7565 0d0a 7061 636b  ata = True..pack
+00000550: 6167 655f 6469 7220 3d20 0d0a 093d 7372  age_dir = ...=sr
+00000560: 630d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  c....[options.pa
+00000570: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
+00000580: 6572 6520 3d20 7372 630d 0a0d 0a5b 6f70  ere = src....[op
+00000590: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
+000005a0: 7473 5d0d 0a6e 6170 6172 692e 6d61 6e69  ts]..napari.mani
+000005b0: 6665 7374 203d 200d 0a09 6e61 7061 7269  fest = ...napari
+000005c0: 2d53 4d4c 4d4c 4142 203d 2073 6d6c 6d6c  -SMLMLAB = smlml
+000005d0: 6162 3a6e 6170 6172 692e 7961 6d6c 0d0a  ab:napari.yaml..
+000005e0: 0d0a 5b6f 7074 696f 6e73 2e65 7874 7261  ..[options.extra
+000005f0: 735f 7265 7175 6972 655d 0d0a 7465 7374  s_require]..test
+00000600: 696e 6720 3d20 0d0a 0974 6f78 0d0a 0970  ing = ...tox...p
+00000610: 7974 6573 7420 2023 2068 7474 7073 3a2f  ytest  # https:/
+00000620: 2f64 6f63 732e 7079 7465 7374 2e6f 7267  /docs.pytest.org
+00000630: 2f65 6e2f 6c61 7465 7374 2f63 6f6e 7465  /en/latest/conte
+00000640: 6e74 732e 6874 6d6c 0d0a 0970 7974 6573  nts.html...pytes
+00000650: 742d 636f 7620 2023 2068 7474 7073 3a2f  t-cov  # https:/
+00000660: 2f70 7974 6573 742d 636f 762e 7265 6164  /pytest-cov.read
+00000670: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00000680: 7465 7374 2f0d 0a09 7079 7465 7374 2d71  test/...pytest-q
+00000690: 7420 2023 2068 7474 7073 3a2f 2f70 7974  t  # https://pyt
+000006a0: 6573 742d 7174 2e72 6561 6474 6865 646f  est-qt.readthedo
+000006b0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+000006c0: 0d0a 096e 6170 6172 690d 0a09 7079 7174  ...napari...pyqt
+000006d0: 350d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  5....[options.pa
+000006e0: 636b 6167 655f 6461 7461 5d0d 0a2a 203d  ckage_data]..* =
+000006f0: 202a 2e79 616d 6c0d 0a0d 0a5b 6567 675f   *.yaml....[egg_
+00000700: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+00000710: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+00000720: 300d 0a0d 0a                             0....
```

### Comparing `napari_smlmlab-0.0.9/src/napari_SMLMLAB.egg-info/PKG-INFO` & `napari_smlmlab-0.1.0/src/napari_SMLMLAB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-SMLMLAB
-Version: 0.0.9
+Version: 0.1.0
 Summary: Napari widget for BP04 Practical
 Home-page: https://github.com/piedrro/napari-SMLMLAB
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-SMLMLAB/issues
 Project-URL: Documentation, https://github.com/piedrro/napari-SMLMLAB#README.md
@@ -32,14 +32,15 @@
 Requires-Dist: scipy
 Requires-Dist: pyqtgraph
 Requires-Dist: picassosr
 Requires-Dist: matplotlib
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Requires-Dist: pyqt5-tools
+Requires-Dist: trackpy
 Provides-Extra: testing
 Requires-Dist: tox; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-qt; extra == "testing"
 Requires-Dist: napari; extra == "testing"
 Requires-Dist: pyqt5; extra == "testing"
```

### Comparing `napari_smlmlab-0.0.9/src/napari_SMLMLAB.egg-info/SOURCES.txt` & `napari_smlmlab-0.1.0/src/napari_SMLMLAB.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,9 +17,10 @@
 src/smlmlab/_tests/test_widget.py
 src/smlmlab/utils/__init__.py
 src/smlmlab/utils/compute_utils.py
 src/smlmlab/utils/events_utils.py
 src/smlmlab/utils/import_utils.py
 src/smlmlab/utils/loc_utils.py
 src/smlmlab/utils/picasso_utils.py
+src/smlmlab/utils/plot_utils.py
 src/smlmlab/utils/undrift_utils.py
 src/smlmlab/utils/viewer_utils.py
```

### Comparing `napari_smlmlab-0.0.9/src/smlmlab/_tests/test_widget.py` & `napari_smlmlab-0.1.0/src/smlmlab/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.9/src/smlmlab/_widget.py` & `napari_smlmlab-0.1.0/src/smlmlab/utils/plot_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,125 +1,77 @@
-import traceback
-from functools import partial
-from multiprocessing import Manager
-from typing import TYPE_CHECKING
-
-import matplotlib.colors as mcolors
-import matplotlib.pyplot as plt
 import numpy as np
 import pyqtgraph as pg
-from qtpy.QtCore import QThreadPool
-from qtpy.QtWidgets import (QVBoxLayout, QWidget, )
+import  traceback
 from scipy.ndimage import map_coordinates
+import matplotlib.pyplot as plt
+from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
+from matplotlib.figure import Figure
+from PyQt5.QtWidgets import QVBoxLayout, QWidget
 
-if TYPE_CHECKING:
-    import napari
-
-from smlmlab.gui import Ui_Frame as gui
-from smlmlab.utils.compute_utils import _utils_compute
-from smlmlab.utils.events_utils import _events_utils
-from smlmlab.utils.import_utils import _import_utils
-from smlmlab.utils.loc_utils import _loc_utils
-from smlmlab.utils.picasso_utils import _picasso_detect_utils
-from smlmlab.utils.viewer_utils import _viewer_utils
-from smlmlab.utils.undrift_utils import _undrift_utils
-
-
-class smlmlabWidget(QWidget, gui,
-    _import_utils, _events_utils,
-    _picasso_detect_utils, _loc_utils,
-    _viewer_utils, _utils_compute,
-    _undrift_utils):
-
-    def __init__(self, viewer: "napari.viewer.Viewer"):
-        super().__init__()
-        self.viewer = viewer
-
-        self.gui = gui()
-        self.gui.setupUi(self)
-
-        # create pyqt graph container
-        self.graph_container = self.gui.graph_container
-        self.graph_container.setLayout(QVBoxLayout())
-
-        self.graph_canvas = pg.GraphicsLayoutWidget()
-        self.graph_container.layout().addWidget(self.graph_canvas)
-
-        self.gui.import_data.clicked.connect(self.import_image_data)
-
-        self.viewer.dims.events.current_step.connect(partial(self.draw_molecules, update_vis=False))
-
-        self.gui.picasso_detect.clicked.connect(partial(self.pixseq_picasso, detect=True, fit=False))
-        self.gui.picasso_fit.clicked.connect(partial(self.pixseq_picasso, detect=False, fit=True))
-        self.gui.picasso_detectfit.clicked.connect(partial(self.pixseq_picasso, detect=True, fit=True))
-        self.gui.picasso_render.clicked.connect(self.picasso_render)
-        self.gui.export_locs.clicked.connect(self.initialise_export_locs)
-
-        self.gui.picasso_undrift.clicked.connect(self.initialise_undrift)
+class _plot_utils:
 
-        self.gui.picasso_vis_mode.currentIndexChanged.connect(partial(self.draw_molecules, update_vis=True))
-        self.gui.picasso_vis_mode.currentIndexChanged.connect(partial(self.draw_bounding_boxes, update_vis=True))
-        self.gui.picasso_vis_size.currentIndexChanged.connect(partial(self.draw_molecules, update_vis=True))
-        self.gui.picasso_vis_size.currentIndexChanged.connect(partial(self.draw_bounding_boxes, update_vis=True))
-        self.gui.picasso_vis_opacity.currentIndexChanged.connect(partial(self.draw_molecules, update_vis=True))
-        self.gui.picasso_vis_opacity.currentIndexChanged.connect(partial(self.draw_bounding_boxes, update_vis=True))
-        self.gui.picasso_vis_edge_width.currentIndexChanged.connect(partial(self.draw_molecules, update_vis=True))
-        self.gui.picasso_vis_edge_width.currentIndexChanged.connect(partial(self.draw_bounding_boxes, update_vis=True))
+    def update_plot_channel(self):
 
-        self.gui.picasso_dataset.currentIndexChanged.connect(lambda: self.update_channel_selector(dataset_selector="picasso_dataset", channel_selector="picasso_channel", ))
-        self.gui.picasso_render_dataset.currentIndexChanged.connect(lambda: self.update_channel_selector(dataset_selector="picasso_render_dataset", channel_selector="picasso_render_channel", ))
-        self.gui.plot_dataset.currentIndexChanged.connect(lambda: self.update_channel_selector(dataset_selector="plot_dataset", channel_selector="plot_channel", efficiency=True, ))
-        self.gui.locs_export_dataset.currentIndexChanged.connect(lambda: self.update_channel_selector(dataset_selector="locs_export_dataset", channel_selector="locs_export_channel", ))
-        self.gui.picasso_undrift_dataset.currentIndexChanged.connect(lambda: self.update_channel_selector(dataset_selector="picasso_undrift_dataset", channel_selector="picasso_undrift_channel", ))
+        plot_mode = self.gui.plot_mode.currentIndex()
+        plot_channel = self.gui.plot_channel.currentText()
+        plot_dataset = self.gui.plot_dataset.currentText()
 
-        self.gui.plot_mode.currentIndexChanged.connect(self.draw_line_plot)
-        self.gui.plot_dataset.currentIndexChanged.connect(self.draw_line_plot)
-        self.gui.plot_channel.currentIndexChanged.connect(self.draw_line_plot)
+        plot_channels = list(self.dataset_dict[plot_dataset].keys())
 
-        self.gui.dataset_selector.currentIndexChanged.connect(partial(self.update_active_image,
-            dataset = self.gui.dataset_selector.currentText()))
+        plot_channels = [channel.capitalize() for channel in plot_channels]
 
-        self.verbose = False
+        if plot_mode in [2, 3]:
+            if set(["Donor", "Acceptor"]).issubset(plot_channels):
+                plot_channels.extend(["FRET Data", "FRET Efficiency"])
 
-        self.dataset_dict = {}
-        self.localisation_dict = {"bounding_boxes": {}, "molecules": {}}
-        self.traces_dict = {}
-        self.plot_dict = {}
-        self.contrast_dict = {}
+        self.gui.plot_channel.blockSignals(True)
+        self.gui.plot_channel.clear()
+        self.gui.plot_channel.addItems(plot_channels)
 
-        self.active_dataset = None
-        self.active_channel = None
+        if plot_channel in plot_channels:
+            index = plot_channels.index(plot_channel)
+            self.gui.plot_channel.setCurrentIndex(index)
 
-        self.threadpool = QThreadPool()
+        self.gui.plot_channel.blockSignals(False)
 
-        manager = Manager()
-        self.stop_event = manager.Event()
+        self.draw_line_plot()
 
-        self.worker = None
-        self.multiprocessing_active = False
+    def draw_shapes(self, mode="line"):
 
-        self.viewer.layers.events.inserted.connect(self.on_add_layer)
+        try:
 
-    def on_add_layer(self, event):
-        if event.value.name == "Shapes":
-            self.shapes_layer = self.viewer.layers["Shapes"]
+            self.shapes_layer = self.get_shapes_layer()
 
-            self.shapes_layer.events.data.connect(self.shapes_layer_updated)
+            if mode == "line":
+                self.shapes_layer.mode = 'add_line'
+                self.shapes_layer.current_edge_color = "red"
+                self.shapes_layer.current_properties = {"mode": "line"}
+            elif mode == "box":
+                self.shapes_layer.mode = 'add_rectangle'
+                self.shapes_layer.current_edge_color = "green"
+                self.shapes_layer.current_properties = {"mode": "box"}
+            elif mode == "background":
+                self.shapes_layer.mode = 'add_rectangle'
+                self.shapes_layer.current_edge_color = "white"
+                self.shapes_layer.current_properties = {"mode": "background"}
 
-            self.shapes_layer.current_edge_color = list(mcolors.to_rgb("green"))
             self.shapes_layer.current_face_color = [0, 0, 0, 0]
-            self.shapes_layer.current_edge_width = 1
+            self.shapes_layer.current_edge_width = 2
+
+        except:
+            print(traceback.format_exc())
 
     def shapes_layer_updated(self, event):
         try:
-            if event.action in ["added", "changed", "removed"]:
+            if event.action in ["added"]:
 
                 shapes_layer = self.viewer.layers["Shapes"]
                 shapes = shapes_layer.data
                 shape_types = shapes_layer.shape_type
+                shape_properties = shapes_layer.properties
 
                 if len(shapes) > 0:
                     shape_type = shapes_layer.shape_type[-1]
 
                     if shapes_layer.ndim == 3:
                         if self.verbose:
                             print("reformatting shapes to ndim=2")
@@ -128,184 +80,208 @@
                         shapes = [shape[:, -2:] for shape in shapes]
                         shapes_layer.data = []
                         shapes_layer.add(shapes, shape_type=shape_type)
 
                     if event.action == "added":
                         n_shapes = len(shapes)
                         if n_shapes > 1:
-                            shapes = shapes_layer.data.copy()
-                            shape_types = shapes_layer.shape_type.copy()
-                            shapes_layer.data = []
-                            shapes_layer.add(shapes[-1], shape_type=shape_types[-1])
+
+                            shape_modes = shape_properties["mode"]
+
+                            delete_list = []
+
+                            for mode in np.unique(shape_modes):
+
+                                delete_indices = np.where(shape_modes == mode)[0][:-1]
+                                delete_list.extend(delete_indices)
+
+                            shapes_layer.selected_data = set(delete_list)
+                            shapes_layer.remove_selected()
 
                     if shape_type == "line":
                         self.gui.plot_mode.setCurrentIndex(0)
 
                     if shape_type == "rectangle":
                         self.gui.plot_mode.setCurrentIndex(2)
 
 
+            if event.action in ["added", "changed", "removed"]:
                 self.draw_line_plot()
 
         except:
             print(traceback.format_exc())
 
+    def get_box_profile(self, box, dataset, channel):
+
+        x1, y1, x2, y2 = (box[0, 1], box[0, 0], box[2, 1], box[2, 0],)
+        x1, y1 = int(x1), int(y1)
+        x2, y2 = int(x2), int(y2)
+
+        img = self.dataset_dict[dataset][channel]["data"]
+
+        box_data = img[:, y1:y2, x1:x2]
+
+        box_profile = np.mean(box_data, axis=(1, 2))
+
+        return box_profile
+
+    def get_line_profile(self, line, dataset, channel, current_frame):
+
+        [[x1, y1], [x2, y2]] = line
+
+        x1, y1 = int(x1), int(y1)
+        x2, y2 = int(x2), int(y2)
+
+        num = int(np.hypot(x2 - x1, y2 - y1))
+
+        img = self.dataset_dict[dataset][channel]["data"][current_frame]
+
+        x, y = np.linspace(x1, x2, num), np.linspace(y1, y2, num)
+        coords = np.vstack((x, y))
+
+        line_profile = map_coordinates(img, coords, order=1, mode="nearest")
+
+        return line_profile
+
     def get_plot_data(self):
-        plot_dataset = {}
+
+        plot_data = {}
 
         try:
             layer_names = [layer.name for layer in self.viewer.layers]
 
             if "Shapes" in layer_names:
                 shapes_layer = self.viewer.layers["Shapes"]
                 shapes = shapes_layer.data.copy()
                 shape_types = shapes_layer.shape_type.copy()
+                shape_modes = shapes_layer.properties["mode"].tolist()
 
                 plot_mode = self.gui.plot_mode.currentIndex()
+                plot_channel = self.gui.plot_channel.currentText()
                 dataset = self.gui.plot_dataset.currentText()
-
+                subtract_background = self.gui.subtract_background.isChecked()
                 current_frame = self.viewer.dims.current_step[0]
 
-                for channel in self.dataset_dict[dataset].keys():
-                    if channel not in plot_dataset:
-                        plot_dataset[channel] = {}
-
-                    for shape_index, (shape, shape_type) in enumerate(zip(shapes, shape_types)):
-                        if shape_type == "line" and plot_mode in [0, 1]:
-                            if shape.shape[-1] == 3:
-                                dat = shape[:, 1:]
-                            else:
-                                dat = shape
+                if plot_channel.lower() in ["donor", "acceptor"]:
+                    plot_channels = [plot_channel.lower()]
+                else:
+                    plot_channels = ["donor", "acceptor"]
 
-                            [[x1, y1], [x2, y2]] = dat
+                for channel in plot_channels:
 
-                            x1, y1 = int(x1), int(y1)
-                            x2, y2 = int(x2), int(y2)
+                    if plot_mode in [0, 1]:
 
-                            num = int(np.hypot(x2 - x1, y2 - y1))
+                        dat = [shape for mode, shape in zip(shape_modes, shapes) if mode == "line"]
 
-                            img = self.dataset_dict[dataset][channel]["data"][current_frame]
+                        if len(dat) > 0:
 
-                            x, y = np.linspace(x1, x2, num), np.linspace(y1, y2, num)
-                            coords = np.vstack((x, y))
+                            line_profile = self.get_line_profile(dat[0], dataset, channel, current_frame)
 
-                            line_profile = map_coordinates(img, coords, order=1, mode="nearest")
-
-                            plot_dataset[channel] = {channel.capitalize(): line_profile}
-
-                        if shape_type == "rectangle" and plot_mode == 2:
-                            if shape.shape[-1] == 3:
-                                dat = shape[:, 1:]
-                            else:
-                                dat = shape
+                            plot_data[channel.capitalize()] = line_profile
 
-                            x1, y1, x2, y2 = (dat[0, 1], dat[0, 0], dat[2, 1], dat[2, 0],)
-                            x1, y1 = int(x1), int(y1)
-                            x2, y2 = int(x2), int(y2)
+                    if plot_mode == 2:
 
-                            img = self.dataset_dict[dataset][channel]["data"]
+                        box = [shape for mode, shape in zip(shape_modes, shapes) if mode == "box"]
+                        background = [shape for mode, shape in zip(shape_modes, shapes) if mode == "background"]
 
-                            box_data = img[:, y1:y2, x1:x2]
+                        if len(box) == 1:
 
-                            box_profile = np.mean(box_data, axis=(1, 2))
+                            box_profile = self.get_box_profile(box[0], dataset, channel)
 
-                            plot_dataset[channel] = {channel.capitalize(): box_profile}
+                            if len(background) == 1 and subtract_background == True:
+                                background_profile = self.get_box_profile(background[0], dataset, channel)
+                                plot_data[channel.capitalize()] = box_profile - background_profile
+                            else:
+                                plot_data[channel.capitalize()] = box_profile
 
-                if set(["donor", "acceptor"]).issubset(plot_dataset.keys()):
-                    plot_dataset = self.calculate_fret(plot_dataset)
-                    try:
-                        plot_dataset["fret data"] = {"Donor": plot_dataset["donor"]["Donor"],
-                                                     "Acceptor": plot_dataset["acceptor"]["Acceptor"]}#
-                    except:
-                        pass
+                if set(["Donor", "Acceptor"]).issubset(plot_data.keys()) and plot_mode in [2, 3]:
+                    if plot_channel.lower() == "fret efficiency":
+                        plot_data = self.calculate_fret(plot_data)
+                        plot_data.pop("Donor")
+                        plot_data.pop("Acceptor")
 
         except:
             print(traceback.format_exc())
 
-        return plot_dataset
+        return plot_data
 
-    def calculate_fret(self, plot_dataset):
+    def calculate_fret(self, plot_data):
         try:
-            donor_data = plot_dataset["donor"]
-            acceptor_data = plot_dataset["acceptor"]
-
-            for shape_index, (donor, acceptor) in enumerate(zip(donor_data.values(), acceptor_data.values())):
-                if "fret efficiency" not in plot_dataset.keys():
-                    plot_dataset["fret efficiency"] = {}
+            donor = plot_data["Donor"]
+            acceptor = plot_data["Acceptor"]
 
-                fret = acceptor / (donor + acceptor)
-                plot_dataset["fret efficiency"] = {"FRET Efficiency": fret}
+            fret = acceptor / (donor + acceptor)
+            plot_data["FRET Efficiency"] = fret
 
         except:
             print(traceback.format_exc())
 
-        return plot_dataset
+        return plot_data
 
     def draw_line_plot(self):
         try:
             plot_mode = self.gui.plot_mode.currentIndex()
-            plot_channel = self.gui.plot_channel.currentText()
-
-            plot_dataset = self.get_plot_data()
+            plot_data = self.get_plot_data()
 
             self.graph_canvas.clear()
 
-            if plot_channel.lower() in plot_dataset.keys():
-                plot_data = plot_dataset[plot_channel.lower()]
+            if plot_mode == 0:
+                plot_title = "Line profile(s)"
+            if plot_mode == 1:
+                plot_title = "Line profile(s)"
+            if plot_mode in [2, 3]:
+                plot_title = "Single Molecule Time Series"
+
+            ax = self.graph_canvas.addPlot(title=plot_title)
+
+            legend = pg.LegendItem(offset=(-50, 20),brush=(255, 255, 255, 50))
+            legend.setParentItem(ax.graphicsItem())
+
+            for label, data in plot_data.items():
+
+                y_data  = np.array(data)
+                x_data = np.arange(len(y_data))
+
+                if label.lower() == "donor":
+                    colour = (255, 0, 0)
+                if label.lower() == "acceptor":
+                    colour = (0, 255, 0)
+                if label.lower() == "fret efficiency":
+                    colour = (0, 0, 255)
+
+                if plot_mode in [0, 1]:
+                    line = ax.plot(x_data, y_data, pen=colour,
+                        symbol="o", symbolPen=(255, 255, 255),name=label)
+                    legend.addItem(line, label)
+                else:
+                    line = ax.plot(x_data, y_data, pen=colour, name=label)
+                    legend.addItem(line, label)
 
-                if plot_data != {}:
+                if plot_mode == 1:
 
-                    if plot_mode == 0:
-                        plot_title = "Line profile(s)"
-                    if plot_mode == 1:
-                        plot_title = "Line profile(s)"
-                    if plot_mode == 2:
-                        plot_title = "Single Molecule Time Series"
+                    try:
+                        fitX, fitY, peak_width = self.fit_custom_gaussian(x_data, y_data)
+                        ax.plot(fitX, fitY, pen=(0, 255, 0), name="Gaussian fit")
+                        text = pg.TextItem(f"Peak FWHM {peak_width:.2f}", color=(200, 200, 200))
+                        ax.addItem(text)
+
+                        x_min, x_max = ax.viewRange()[0]
+                        y_min, y_max = ax.viewRange()[1]
+                        offset_x = 0.05 * (x_max - x_min)
+                        offset_y = 0.05 * (y_max - y_min)
 
-                    ax = self.graph_canvas.addPlot(title=plot_title)
-                    #add legend
-                    ax.addLegend()
-
-                    for label, data in plot_data.items():
-
-                        y_data  = np.array(data)
-                        x_data = np.arange(len(y_data))
-
-                        if label.lower() == "donor":
-                            colour = (255, 0, 0)
-                        if label.lower() == "acceptor":
-                            colour = (0, 255, 0)
-                        if label.lower() == "fret efficiency":
-                            colour = (0, 0, 255)
-
-                        if plot_mode in [0, 1]:
-                            ax.plot(x_data, y_data, pen=colour, symbol="o", symbolPen=(255, 255, 255))
-                        else:
-                            ax.plot(x_data, y_data, pen=colour)
-
-                        if plot_mode == 1:
-                            try:
-                                fitX, fitY, peak_width = self.fit_custom_gaussian(x_data, y_data)
-                                ax.plot(fitX, fitY, pen=(0, 255, 0))
-                                text = pg.TextItem(f"Peak FWHM {peak_width:.2f}", color=(200, 200, 200))
-                                ax.addItem(text)
-
-                                x_min, x_max = ax.viewRange()[0]
-                                y_min, y_max = ax.viewRange()[1]
-                                offset_x = 0.05 * (x_max - x_min)
-                                offset_y = 0.05 * (y_max - y_min)
-
-                                text.setPos(x_min + offset_x, y_max - offset_y)
-                            except:
-                                pass
+                        text.setPos(x_min + offset_x, y_max - offset_y)
+                    except:
+                        pass
 
-                    plt.show()
+            plt.show()
 
         except:
             print(traceback.format_exc())
+            print(plot_data)
 
     def custom_gaussian(self, x, a, b, c, d):
         """ Custom Gaussian model with baseline and peak height parameters. """
         return a + (b - a) * np.exp(-(x - c) ** 2 / (2 * d ** 2))
 
     def fit_custom_gaussian(self, x_data, y_data):
         """ Fit the custom Gaussian model to 1D data. """
@@ -330,8 +306,34 @@
         fitX = np.linspace(start = min(x_data), stop = max(x_data), num = 1000)
 
         # Generate the fitted curve
         fitY = self.custom_gaussian(fitX, *popt)
 
         width = 2 * np.sqrt(2 * np.log(2)) * popt[3]
 
-        return fitX, fitY, width
+        return fitX, fitY, width
+
+
+class CustomMatplotlibWidget(QWidget):
+    def __init__(self, parent=None):
+        super().__init__(parent)
+
+        # Initialize matplotlib figure
+        self.figure = Figure()
+        self.canvas = FigureCanvas(self.figure)
+        self.axes = self.figure.add_subplot(111)
+
+        # Setup layout
+        layout = QVBoxLayout()
+        layout.addWidget(self.canvas)
+        self.setLayout(layout)
+
+    def mousePressEvent(self, event):
+        # Handle mouse press event
+        if event.modifiers():  # Check for any specific modifiers you need
+            click_position = event.pos()
+            # Convert click position to axes coordinates
+            axes_coord = self.axes.transData.inverted().transform((click_position.x(), click_position.y()))
+            print("Clicked at:", axes_coord)
+            # You can add your logic here
+
+        super().mousePressEvent(event)
```

### Comparing `napari_smlmlab-0.0.9/src/smlmlab/gui.py` & `napari_smlmlab-0.1.0/src/smlmlab/gui.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
 class Ui_Frame(object):
     def setupUi(self, Frame):
         Frame.setObjectName("Frame")
-        Frame.resize(482, 556)
+        Frame.resize(482, 710)
         self.verticalLayout = QtWidgets.QVBoxLayout(Frame)
         self.verticalLayout.setObjectName("verticalLayout")
         self.tabWidget = QtWidgets.QTabWidget(Frame)
         self.tabWidget.setObjectName("tabWidget")
         self.tab = QtWidgets.QWidget()
         self.tab.setObjectName("tab")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout(self.tab)
@@ -377,14 +377,42 @@
         spacerItem6 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_3.addItem(spacerItem6)
         self.tabWidget.addTab(self.tab_2, "")
         self.tab_6 = QtWidgets.QWidget()
         self.tab_6.setObjectName("tab_6")
         self.verticalLayout_7 = QtWidgets.QVBoxLayout(self.tab_6)
         self.verticalLayout_7.setObjectName("verticalLayout_7")
+        self.label_22 = QtWidgets.QLabel(self.tab_6)
+        font = QtGui.QFont()
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_22.setFont(font)
+        self.label_22.setObjectName("label_22")
+        self.verticalLayout_7.addWidget(self.label_22)
+        self.gridLayout_2 = QtWidgets.QGridLayout()
+        self.gridLayout_2.setObjectName("gridLayout_2")
+        self.add_line = QtWidgets.QPushButton(self.tab_6)
+        self.add_line.setObjectName("add_line")
+        self.gridLayout_2.addWidget(self.add_line, 0, 0, 1, 1)
+        self.add_box = QtWidgets.QPushButton(self.tab_6)
+        self.add_box.setObjectName("add_box")
+        self.gridLayout_2.addWidget(self.add_box, 0, 1, 1, 1)
+        self.add_background = QtWidgets.QPushButton(self.tab_6)
+        self.add_background.setObjectName("add_background")
+        self.gridLayout_2.addWidget(self.add_background, 0, 2, 1, 1)
+        self.verticalLayout_7.addLayout(self.gridLayout_2)
+        spacerItem7 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Minimum)
+        self.verticalLayout_7.addItem(spacerItem7)
+        self.label_23 = QtWidgets.QLabel(self.tab_6)
+        font = QtGui.QFont()
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_23.setFont(font)
+        self.label_23.setObjectName("label_23")
+        self.verticalLayout_7.addWidget(self.label_23)
         self.formLayout_5 = QtWidgets.QFormLayout()
         self.formLayout_5.setObjectName("formLayout_5")
         self.label_16 = QtWidgets.QLabel(self.tab_6)
         self.label_16.setObjectName("label_16")
         self.formLayout_5.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_16)
         self.plot_mode = QtWidgets.QComboBox(self.tab_6)
         self.plot_mode.setObjectName("plot_mode")
@@ -401,25 +429,97 @@
         self.label_18 = QtWidgets.QLabel(self.tab_6)
         self.label_18.setObjectName("label_18")
         self.formLayout_5.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_18)
         self.plot_channel = QtWidgets.QComboBox(self.tab_6)
         self.plot_channel.setObjectName("plot_channel")
         self.formLayout_5.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.plot_channel)
         self.verticalLayout_7.addLayout(self.formLayout_5)
+        self.subtract_background = QtWidgets.QCheckBox(self.tab_6)
+        self.subtract_background.setObjectName("subtract_background")
+        self.verticalLayout_7.addWidget(self.subtract_background)
         self.graph_container = QtWidgets.QWidget(self.tab_6)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.MinimumExpanding, QtWidgets.QSizePolicy.MinimumExpanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.graph_container.sizePolicy().hasHeightForWidth())
         self.graph_container.setSizePolicy(sizePolicy)
         self.graph_container.setMinimumSize(QtCore.QSize(50, 0))
         self.graph_container.setToolTipDuration(0)
         self.graph_container.setObjectName("graph_container")
         self.verticalLayout_7.addWidget(self.graph_container)
         self.tabWidget.addTab(self.tab_6, "")
+        self.tab_9 = QtWidgets.QWidget()
+        self.tab_9.setObjectName("tab_9")
+        self.verticalLayout_10 = QtWidgets.QVBoxLayout(self.tab_9)
+        self.verticalLayout_10.setObjectName("verticalLayout_10")
+        self.label_24 = QtWidgets.QLabel(self.tab_9)
+        font = QtGui.QFont()
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_24.setFont(font)
+        self.label_24.setObjectName("label_24")
+        self.verticalLayout_10.addWidget(self.label_24)
+        self.formLayout_7 = QtWidgets.QFormLayout()
+        self.formLayout_7.setObjectName("formLayout_7")
+        self.label_25 = QtWidgets.QLabel(self.tab_9)
+        self.label_25.setObjectName("label_25")
+        self.formLayout_7.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_25)
+        self.lifetimes_dataset = QtWidgets.QComboBox(self.tab_9)
+        self.lifetimes_dataset.setObjectName("lifetimes_dataset")
+        self.formLayout_7.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.lifetimes_dataset)
+        self.label_26 = QtWidgets.QLabel(self.tab_9)
+        self.label_26.setObjectName("label_26")
+        self.formLayout_7.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_26)
+        self.lifetimes_channel = QtWidgets.QComboBox(self.tab_9)
+        self.lifetimes_channel.setObjectName("lifetimes_channel")
+        self.formLayout_7.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.lifetimes_channel)
+        self.label_29 = QtWidgets.QLabel(self.tab_9)
+        self.label_29.setObjectName("label_29")
+        self.formLayout_7.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_29)
+        self.lifetime_bins = QtWidgets.QSpinBox(self.tab_9)
+        self.lifetime_bins.setMinimum(10)
+        self.lifetime_bins.setMaximum(200)
+        self.lifetime_bins.setProperty("value", 30)
+        self.lifetime_bins.setObjectName("lifetime_bins")
+        self.formLayout_7.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.lifetime_bins)
+        self.label_33 = QtWidgets.QLabel(self.tab_9)
+        self.label_33.setObjectName("label_33")
+        self.formLayout_7.setWidget(3, QtWidgets.QFormLayout.LabelRole, self.label_33)
+        self.min_lifetime = QtWidgets.QSpinBox(self.tab_9)
+        self.min_lifetime.setMaximum(1000)
+        self.min_lifetime.setProperty("value", 5)
+        self.min_lifetime.setObjectName("min_lifetime")
+        self.formLayout_7.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.min_lifetime)
+        self.label_34 = QtWidgets.QLabel(self.tab_9)
+        self.label_34.setObjectName("label_34")
+        self.formLayout_7.setWidget(4, QtWidgets.QFormLayout.LabelRole, self.label_34)
+        self.max_lifetime = QtWidgets.QSpinBox(self.tab_9)
+        self.max_lifetime.setMaximum(1000)
+        self.max_lifetime.setProperty("value", 100)
+        self.max_lifetime.setObjectName("max_lifetime")
+        self.formLayout_7.setWidget(4, QtWidgets.QFormLayout.FieldRole, self.max_lifetime)
+        self.verticalLayout_10.addLayout(self.formLayout_7)
+        self.fit_exponential = QtWidgets.QCheckBox(self.tab_9)
+        self.fit_exponential.setObjectName("fit_exponential")
+        self.verticalLayout_10.addWidget(self.fit_exponential)
+        self.plot_lifetime_hist = QtWidgets.QPushButton(self.tab_9)
+        self.plot_lifetime_hist.setObjectName("plot_lifetime_hist")
+        self.verticalLayout_10.addWidget(self.plot_lifetime_hist)
+        self.lifetime_graph = QtWidgets.QWidget(self.tab_9)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.lifetime_graph.sizePolicy().hasHeightForWidth())
+        self.lifetime_graph.setSizePolicy(sizePolicy)
+        self.lifetime_graph.setObjectName("lifetime_graph")
+        self.verticalLayout_10.addWidget(self.lifetime_graph)
+        self.export_lifetime_data = QtWidgets.QPushButton(self.tab_9)
+        self.export_lifetime_data.setObjectName("export_lifetime_data")
+        self.verticalLayout_10.addWidget(self.export_lifetime_data)
+        self.tabWidget.addTab(self.tab_9, "")
         self.verticalLayout.addWidget(self.tabWidget)
         self.label_12 = QtWidgets.QLabel(Frame)
         font = QtGui.QFont()
         font.setBold(True)
         font.setWeight(75)
         self.label_12.setFont(font)
         self.label_12.setObjectName("label_12")
@@ -569,16 +669,32 @@
         self.picasso_vis_edge_width.setItemText(5, _translate("Frame", "0.6"))
         self.picasso_vis_edge_width.setItemText(6, _translate("Frame", "0.7"))
         self.picasso_vis_edge_width.setItemText(7, _translate("Frame", "0.8"))
         self.picasso_vis_edge_width.setItemText(8, _translate("Frame", "0.9"))
         self.picasso_vis_edge_width.setItemText(9, _translate("Frame", "1.0"))
         self.tabWidget_2.setTabText(self.tabWidget_2.indexOf(self.tab_4), _translate("Frame", "Visualisation Settings"))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_2), _translate("Frame", "SMLM"))
+        self.label_22.setText(_translate("Frame", "Add Shapes"))
+        self.add_line.setText(_translate("Frame", "Add Line Profile"))
+        self.add_box.setText(_translate("Frame", "Add Box Profile"))
+        self.add_background.setText(_translate("Frame", "Add Background Box"))
+        self.label_23.setText(_translate("Frame", "Plot Settings"))
         self.label_16.setText(_translate("Frame", "Plot Mode"))
         self.plot_mode.setItemText(0, _translate("Frame", "Line Profiles"))
         self.plot_mode.setItemText(1, _translate("Frame", "Line Profiles With Gaussian Fit"))
         self.plot_mode.setItemText(2, _translate("Frame", "Single Molecule Time Series"))
         self.label_17.setText(_translate("Frame", "Plot Dataset"))
         self.label_18.setText(_translate("Frame", "Plot Channel"))
-        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_6), _translate("Frame", "Plots"))
+        self.subtract_background.setText(_translate("Frame", "Subtract Background (Single Molecule Time Series)"))
+        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_6), _translate("Frame", "Plot Profiles"))
+        self.label_24.setText(_translate("Frame", "Lifetime Histogram Settings"))
+        self.label_25.setText(_translate("Frame", "Dataset"))
+        self.label_26.setText(_translate("Frame", "Channel"))
+        self.label_29.setText(_translate("Frame", "Histogram N Bins"))
+        self.label_33.setText(_translate("Frame", "Min Lifetime"))
+        self.label_34.setText(_translate("Frame", "Max Lifetime"))
+        self.fit_exponential.setText(_translate("Frame", "Fit Exponential"))
+        self.plot_lifetime_hist.setText(_translate("Frame", "Plot Lifetime Histogram"))
+        self.export_lifetime_data.setText(_translate("Frame", "Export Lifetime Data"))
+        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_9), _translate("Frame", "Plot Lifetimes"))
         self.label_12.setText(_translate("Frame", "Display Mode"))
         self.label_14.setText(_translate("Frame", "Dataset [PageUp/PageDown]"))
```

### Comparing `napari_smlmlab-0.0.9/src/smlmlab/utils/compute_utils.py` & `napari_smlmlab-0.1.0/src/smlmlab/utils/compute_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.9/src/smlmlab/utils/events_utils.py` & `napari_smlmlab-0.1.0/src/smlmlab/utils/events_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,15 +281,17 @@
 
                 self.active_dataset = None
                 self.active_channel = None
 
             layer_names = [layer.name for layer in self.viewer.layers]
 
             if "Shapes" not in layer_names:
-                self.shapes_layer = self.viewer.add_shapes(name="Shapes", face_color="transparent", edge_color="red", edge_width=0.1, ndim=2, scale=scale, )
+                properties = {"mode": [], "ndim": 2}
+                self.shapes_layer = self.viewer.add_shapes(name="Shapes", face_color="transparent",
+                    edge_color="red", edge_width=0.1, ndim=2, scale=scale, properties=properties)
 
             self.draw_molecules(update_vis=True)
             self.update_overlay_text()
 
         except:
             print(traceback.format_exc())
 
@@ -374,17 +376,17 @@
     def populate_channel_selectors(self):
         try:
             if self.verbose:
                 print("Populating channel selectors")
 
             self.update_channel_selector(dataset_selector="picasso_dataset", channel_selector="picasso_channel", )
             self.update_channel_selector(dataset_selector="picasso_render_dataset", channel_selector="picasso_render_channel", )
-            self.update_channel_selector(dataset_selector="plot_dataset", channel_selector="plot_channel", efficiency=True, )
             self.update_channel_selector(dataset_selector="locs_export_dataset", channel_selector="locs_export_channel")
             self.update_channel_selector(dataset_selector="picasso_undrift_dataset", channel_selector="picasso_undrift_channel")
+            self.update_channel_selector(dataset_selector="lifetimes_dataset", channel_selector="lifetimes_channel")
 
         except:
             print(traceback.format_exc())
 
     def update_channel_select_buttons(self):
         try:
             datast_name = self.gui.dataset_selector.currentText()
```

### Comparing `napari_smlmlab-0.0.9/src/smlmlab/utils/import_utils.py` & `napari_smlmlab-0.1.0/src/smlmlab/utils/import_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -437,14 +437,19 @@
             self.gui.locs_export_dataset.blockSignals(False)
 
             self.gui.picasso_undrift_dataset.blockSignals(True)
             self.gui.picasso_undrift_dataset.clear()
             self.gui.picasso_undrift_dataset.addItems(dataset_names)
             self.gui.picasso_undrift_dataset.blockSignals(False)
 
+            self.gui.lifetimes_dataset.blockSignals(True)
+            self.gui.lifetimes_dataset.clear()
+            self.gui.lifetimes_dataset.addItems(dataset_names)
+            self.gui.lifetimes_dataset.blockSignals(False)
+
         except:
             print(traceback.format_exc())
 
     def initialise_localisation_dict(self):
         if hasattr(self, "localisation_dict"):
             self.localisation_dict = {"bounding_boxes": {}, "molecules": {}}
```

### Comparing `napari_smlmlab-0.0.9/src/smlmlab/utils/loc_utils.py` & `napari_smlmlab-0.1.0/src/smlmlab/utils/loc_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.9/src/smlmlab/utils/picasso_utils.py` & `napari_smlmlab-0.1.0/src/smlmlab/utils/picasso_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.9/src/smlmlab/utils/undrift_utils.py` & `napari_smlmlab-0.1.0/src/smlmlab/utils/undrift_utils.py`

 * *Files identical despite different names*

### Comparing `napari_smlmlab-0.0.9/src/smlmlab/utils/viewer_utils.py` & `napari_smlmlab-0.1.0/src/smlmlab/utils/viewer_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import traceback
 
 
 class _viewer_utils:
 
     def draw_bounding_boxes(self, update_vis=False):
+
         if hasattr(self, "localisation_dict") and hasattr(self, "active_channel"):
             if hasattr(self, "bbox_layer"):
                 show_bboxes = self.bbox_layer.visible
             else:
                 show_bboxes = True
 
             if show_bboxes:
```

