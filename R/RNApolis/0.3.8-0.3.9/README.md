# Comparing `tmp/RNApolis-0.3.8.tar.gz` & `tmp/RNApolis-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RNApolis-0.3.8.tar", last modified: Wed Mar 13 12:13:57 2024, max compression
+gzip compressed data, was "RNApolis-0.3.9.tar", last modified: Tue Mar 19 11:46:31 2024, max compression
```

## Comparing `RNApolis-0.3.8.tar` & `RNApolis-0.3.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2024-03-13 12:13:57.511131 RNApolis-0.3.8/
--rw-r--r--   0 tzok      (1000) tzok      (1000)     1066 2023-04-04 15:11:51.000000 RNApolis-0.3.8/LICENSE
--rw-r--r--   0 tzok      (1000) tzok      (1000)    54300 2024-03-13 12:13:57.511131 RNApolis-0.3.8/PKG-INFO
--rw-r--r--   0 tzok      (1000) tzok      (1000)    53344 2023-12-22 13:09:36.000000 RNApolis-0.3.8/README.md
--rw-r--r--   0 tzok      (1000) tzok      (1000)       86 2023-04-04 15:11:51.000000 RNApolis-0.3.8/pyproject.toml
--rw-r--r--   0 tzok      (1000) tzok      (1000)       38 2024-03-13 12:13:57.511131 RNApolis-0.3.8/setup.cfg
--rw-r--r--   0 tzok      (1000) tzok      (1000)     1617 2024-03-13 12:13:43.000000 RNApolis-0.3.8/setup.py
-drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2024-03-13 12:13:57.507797 RNApolis-0.3.8/src/
-drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2024-03-13 12:13:57.511131 RNApolis-0.3.8/src/RNApolis.egg-info/
--rw-r--r--   0 tzok      (1000) tzok      (1000)    54300 2024-03-13 12:13:57.000000 RNApolis-0.3.8/src/RNApolis.egg-info/PKG-INFO
--rw-r--r--   0 tzok      (1000) tzok      (1000)      742 2024-03-13 12:13:57.000000 RNApolis-0.3.8/src/RNApolis.egg-info/SOURCES.txt
--rw-r--r--   0 tzok      (1000) tzok      (1000)        1 2024-03-13 12:13:57.000000 RNApolis-0.3.8/src/RNApolis.egg-info/dependency_links.txt
--rw-r--r--   0 tzok      (1000) tzok      (1000)      308 2024-03-13 12:13:57.000000 RNApolis-0.3.8/src/RNApolis.egg-info/entry_points.txt
--rw-r--r--   0 tzok      (1000) tzok      (1000)       78 2024-03-13 12:13:57.000000 RNApolis-0.3.8/src/RNApolis.egg-info/requires.txt
--rw-r--r--   0 tzok      (1000) tzok      (1000)        9 2024-03-13 12:13:57.000000 RNApolis-0.3.8/src/RNApolis.egg-info/top_level.txt
-drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2024-03-13 12:13:57.511131 RNApolis-0.3.8/src/rnapolis/
--rw-r--r--   0 tzok      (1000) tzok      (1000)    21364 2024-02-01 12:47:07.000000 RNApolis-0.3.8/src/rnapolis/annotator.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)     8514 2023-04-04 15:11:51.000000 RNApolis-0.3.8/src/rnapolis/clashfinder.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)    26440 2023-11-09 14:41:44.000000 RNApolis-0.3.8/src/rnapolis/common.py
--rwxr-xr-x   0 tzok      (1000) tzok      (1000)     1683 2023-04-04 15:11:51.000000 RNApolis-0.3.8/src/rnapolis/metareader.py
--rwxr-xr-x   0 tzok      (1000) tzok      (1000)     6918 2023-11-23 10:44:00.000000 RNApolis-0.3.8/src/rnapolis/molecule_filter.py
--rwxr-xr-x   0 tzok      (1000) tzok      (1000)      774 2023-11-09 14:41:44.000000 RNApolis-0.3.8/src/rnapolis/motif_extractor.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)    11905 2023-04-04 15:11:51.000000 RNApolis-0.3.8/src/rnapolis/parser.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)    11112 2024-03-13 12:13:43.000000 RNApolis-0.3.8/src/rnapolis/rfam_folder.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)    18957 2023-11-09 14:41:44.000000 RNApolis-0.3.8/src/rnapolis/tertiary.py
--rwxr-xr-x   0 tzok      (1000) tzok      (1000)     1817 2023-04-04 15:11:51.000000 RNApolis-0.3.8/src/rnapolis/transformer.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)      543 2023-04-04 15:11:51.000000 RNApolis-0.3.8/src/rnapolis/util.py
-drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2024-03-13 12:13:57.511131 RNApolis-0.3.8/tests/
--rw-r--r--   0 tzok      (1000) tzok      (1000)     1510 2023-11-09 14:41:44.000000 RNApolis-0.3.8/tests/test_annotator.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)     2698 2023-11-09 14:41:44.000000 RNApolis-0.3.8/tests/test_bugfixes.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)     3578 2023-11-09 14:41:44.000000 RNApolis-0.3.8/tests/test_common.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)     1145 2023-04-04 15:11:51.000000 RNApolis-0.3.8/tests/test_metareader.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)      383 2023-04-04 15:11:51.000000 RNApolis-0.3.8/tests/test_parser.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)    15733 2023-11-09 14:41:44.000000 RNApolis-0.3.8/tests/test_quadruplexes.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)     1117 2024-03-13 12:13:43.000000 RNApolis-0.3.8/tests/test_rfam_folder.py
--rw-r--r--   0 tzok      (1000) tzok      (1000)      906 2023-08-17 14:21:58.000000 RNApolis-0.3.8/tests/test_tertiary.py
+drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2024-03-19 11:46:31.368431 RNApolis-0.3.9/
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     1066 2023-04-04 15:11:51.000000 RNApolis-0.3.9/LICENSE
+-rw-r--r--   0 tzok      (1000) tzok      (1000)    54300 2024-03-19 11:46:31.368431 RNApolis-0.3.9/PKG-INFO
+-rw-r--r--   0 tzok      (1000) tzok      (1000)    53344 2023-12-22 13:09:36.000000 RNApolis-0.3.9/README.md
+-rw-r--r--   0 tzok      (1000) tzok      (1000)       86 2023-04-04 15:11:51.000000 RNApolis-0.3.9/pyproject.toml
+-rw-r--r--   0 tzok      (1000) tzok      (1000)       38 2024-03-19 11:46:31.368431 RNApolis-0.3.9/setup.cfg
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     1617 2024-03-19 11:46:17.000000 RNApolis-0.3.9/setup.py
+drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2024-03-19 11:46:31.365098 RNApolis-0.3.9/src/
+drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2024-03-19 11:46:31.368431 RNApolis-0.3.9/src/RNApolis.egg-info/
+-rw-r--r--   0 tzok      (1000) tzok      (1000)    54300 2024-03-19 11:46:31.000000 RNApolis-0.3.9/src/RNApolis.egg-info/PKG-INFO
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      742 2024-03-19 11:46:31.000000 RNApolis-0.3.9/src/RNApolis.egg-info/SOURCES.txt
+-rw-r--r--   0 tzok      (1000) tzok      (1000)        1 2024-03-19 11:46:31.000000 RNApolis-0.3.9/src/RNApolis.egg-info/dependency_links.txt
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      308 2024-03-19 11:46:31.000000 RNApolis-0.3.9/src/RNApolis.egg-info/entry_points.txt
+-rw-r--r--   0 tzok      (1000) tzok      (1000)       78 2024-03-19 11:46:31.000000 RNApolis-0.3.9/src/RNApolis.egg-info/requires.txt
+-rw-r--r--   0 tzok      (1000) tzok      (1000)        9 2024-03-19 11:46:31.000000 RNApolis-0.3.9/src/RNApolis.egg-info/top_level.txt
+drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2024-03-19 11:46:31.368431 RNApolis-0.3.9/src/rnapolis/
+-rw-r--r--   0 tzok      (1000) tzok      (1000)    21481 2024-03-19 11:46:17.000000 RNApolis-0.3.9/src/rnapolis/annotator.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     8514 2023-04-04 15:11:51.000000 RNApolis-0.3.9/src/rnapolis/clashfinder.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)    26440 2023-11-09 14:41:44.000000 RNApolis-0.3.9/src/rnapolis/common.py
+-rwxr-xr-x   0 tzok      (1000) tzok      (1000)     1683 2023-04-04 15:11:51.000000 RNApolis-0.3.9/src/rnapolis/metareader.py
+-rwxr-xr-x   0 tzok      (1000) tzok      (1000)     6918 2023-11-23 10:44:00.000000 RNApolis-0.3.9/src/rnapolis/molecule_filter.py
+-rwxr-xr-x   0 tzok      (1000) tzok      (1000)      774 2023-11-09 14:41:44.000000 RNApolis-0.3.9/src/rnapolis/motif_extractor.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)    11948 2024-03-19 11:46:17.000000 RNApolis-0.3.9/src/rnapolis/parser.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)    11112 2024-03-13 12:13:43.000000 RNApolis-0.3.9/src/rnapolis/rfam_folder.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)    18957 2023-11-09 14:41:44.000000 RNApolis-0.3.9/src/rnapolis/tertiary.py
+-rwxr-xr-x   0 tzok      (1000) tzok      (1000)     1817 2023-04-04 15:11:51.000000 RNApolis-0.3.9/src/rnapolis/transformer.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      543 2023-04-04 15:11:51.000000 RNApolis-0.3.9/src/rnapolis/util.py
+drwxr-xr-x   0 tzok      (1000) tzok      (1000)        0 2024-03-19 11:46:31.368431 RNApolis-0.3.9/tests/
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     1510 2023-11-09 14:41:44.000000 RNApolis-0.3.9/tests/test_annotator.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     2698 2023-11-09 14:41:44.000000 RNApolis-0.3.9/tests/test_bugfixes.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     3578 2023-11-09 14:41:44.000000 RNApolis-0.3.9/tests/test_common.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     1145 2023-04-04 15:11:51.000000 RNApolis-0.3.9/tests/test_metareader.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      383 2023-04-04 15:11:51.000000 RNApolis-0.3.9/tests/test_parser.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)    15733 2023-11-09 14:41:44.000000 RNApolis-0.3.9/tests/test_quadruplexes.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)     1117 2024-03-13 12:13:43.000000 RNApolis-0.3.9/tests/test_rfam_folder.py
+-rw-r--r--   0 tzok      (1000) tzok      (1000)      906 2023-08-17 14:21:58.000000 RNApolis-0.3.9/tests/test_tertiary.py
```

### Comparing `RNApolis-0.3.8/LICENSE` & `RNApolis-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `RNApolis-0.3.8/PKG-INFO` & `RNApolis-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RNApolis
-Version: 0.3.8
+Version: 0.3.9
 Summary: A Python library containing RNA-related bioinformatics functions and classes
 Home-page: https://github.com/tzok/rnapolis-py
 Author: Tomasz Zok
 Author-email: tomasz.zok@cs.put.poznan.pl
 Project-URL: Bug Tracker, https://github.com/tzok/rnapolis-py/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `RNApolis-0.3.8/README.md` & `RNApolis-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `RNApolis-0.3.8/setup.py` & `RNApolis-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="RNApolis",
-    version="0.3.8",
+    version="0.3.9",
     packages=["rnapolis"],
     package_dir={"": "src"},
     author="Tomasz Zok",
     author_email="tomasz.zok@cs.put.poznan.pl",
     description="A Python library containing RNA-related bioinformatics functions and classes",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `RNApolis-0.3.8/src/RNApolis.egg-info/PKG-INFO` & `RNApolis-0.3.9/src/RNApolis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RNApolis
-Version: 0.3.8
+Version: 0.3.9
 Summary: A Python library containing RNA-related bioinformatics functions and classes
 Home-page: https://github.com/tzok/rnapolis-py
 Author: Tomasz Zok
 Author-email: tomasz.zok@cs.put.poznan.pl
 Project-URL: Bug Tracker, https://github.com/tzok/rnapolis-py/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `RNApolis-0.3.8/src/RNApolis.egg-info/SOURCES.txt` & `RNApolis-0.3.9/src/RNApolis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RNApolis-0.3.8/src/rnapolis/annotator.py` & `RNApolis-0.3.9/src/rnapolis/annotator.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,23 +171,23 @@
     for key, bphs_brs in bph_br_map.items():
         if len(bphs_brs) > 1:
             bph_br_map[key] = OrderedSet([bphs_brs[0]])
     return bph_br_map
 
 
 def find_pairs(
-    structure: Structure3D, model: int = 1
+    structure: Structure3D, model: Optional[int] = None
 ) -> Tuple[List[BasePair], List[BasePhosphate], List[BaseRibose]]:
     # put all donors and acceptors into a KDTree
     coordinates = []
     coordinates_atom_map: Dict[Tuple[float, float, float], Atom] = {}
     coordinates_type_map: Dict[Tuple[float, float, float], str] = {}
     coordinates_residue_map: Dict[Tuple[float, float, float], Residue3D] = {}
     for residue in structure.residues:
-        if residue.model != model:
+        if model is not None and residue.model != model:
             continue
         acceptors = (
             BASE_ACCEPTORS.get(residue.one_letter_name, [])
             + RIBOSE_ACCEPTORS
             + PHOSPHATE_ACCEPTORS
         )
         donors = BASE_DONORS.get(residue.one_letter_name, [])
@@ -392,20 +392,22 @@
                     BR[f"_{br}"],
                 )
             )
 
     return base_pairs, base_phosphates, base_riboses
 
 
-def find_stackings(structure: Structure3D, model: int = 1) -> List[Stacking]:
+def find_stackings(
+    structure: Structure3D, model: Optional[int] = None
+) -> List[Stacking]:
     # put all nitrogen ring centers into a KDTree
     coordinates = []
     coordinates_residue_map: Dict[Tuple[float, float, float], Residue3D] = {}
     for residue in structure.residues:
-        if residue.model != model:
+        if model is not None and residue.model != model:
             continue
         base_atoms = BASE_ATOMS.get(residue.one_letter_name, [])
         xs, ys, zs = [], [], []
         for atom_name in base_atoms:
             atom = residue.find_atom(atom_name)
             if atom is not None:
                 xs.append(atom.x)
@@ -469,23 +471,25 @@
         nt2 = Residue(residue_j.label, residue_j.auth)
         stackings.append(Stacking(nt1, nt2, StackingTopology[topology]))
 
     return stackings
 
 
 def extract_base_interactions(
-    tertiary_structure: Structure3D, model: int = 1
+    tertiary_structure: Structure3D, model: Optional[int] = None
 ) -> BaseInteractions:
     base_pairs, base_phosphate, base_ribose = find_pairs(tertiary_structure, model)
     stackings = find_stackings(tertiary_structure, model)
     return BaseInteractions(base_pairs, stackings, base_ribose, base_phosphate, [])
 
 
 def extract_secondary_structure(
-    tertiary_structure: Structure3D, model: int = 1, find_gaps: bool = False
+    tertiary_structure: Structure3D,
+    model: Optional[int] = None,
+    find_gaps: bool = False,
 ) -> BaseInteractions:
     base_interactions = extract_base_interactions(tertiary_structure, model)
     mapping = Mapping2D3D(
         tertiary_structure,
         base_interactions.basePairs,
         base_interactions.stackings,
         find_gaps,
@@ -593,16 +597,16 @@
         help="(optional) if set, the program will detect gaps and break the PDB chain into two or more strands; "
         f"the gap is defined as O3'-P distance greater then {1.5 * AVERAGE_OXYGEN_PHOSPHORUS_DISTANCE_COVALENT}",
     )
     parser.add_argument("--dot", help="(optional) path to output DOT file")
     args = parser.parse_args()
 
     file = handle_input_file(args.input)
-    structure3d = read_3d_structure(file, 1)
-    structure2d = extract_secondary_structure(structure3d, 1, args.find_gaps)
+    structure3d = read_3d_structure(file, None)
+    structure2d = extract_secondary_structure(structure3d, None, args.find_gaps)
 
     if args.csv:
         write_csv(args.csv, structure2d)
 
     if args.json:
         write_json(args.json, structure2d)
```

### Comparing `RNApolis-0.3.8/src/rnapolis/clashfinder.py` & `RNApolis-0.3.9/src/rnapolis/clashfinder.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.3.8/src/rnapolis/common.py` & `RNApolis-0.3.9/src/rnapolis/common.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.3.8/src/rnapolis/metareader.py` & `RNApolis-0.3.9/src/rnapolis/metareader.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.3.8/src/rnapolis/molecule_filter.py` & `RNApolis-0.3.9/src/rnapolis/molecule_filter.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.3.8/src/rnapolis/motif_extractor.py` & `RNApolis-0.3.9/src/rnapolis/motif_extractor.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.3.8/src/rnapolis/parser.py` & `RNApolis-0.3.9/src/rnapolis/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 from mmcif.io.IoAdapterPy import IoAdapterPy
 
 from rnapolis.common import ResidueAuth, ResidueLabel
 from rnapolis.tertiary import BASE_ATOMS, Atom, Residue3D, Structure3D
 
 
 def read_3d_structure(
-    cif_or_pdb: IO[str], model: int = 1, nucleic_acid_only: bool = False
+    cif_or_pdb: IO[str], model: Optional[int] = None, nucleic_acid_only: bool = False
 ) -> Structure3D:
     atoms, modified, sequence = (
         parse_cif(cif_or_pdb) if is_cif(cif_or_pdb) else parse_pdb(cif_or_pdb)
     )
-    atoms = list(filter(lambda atom: atom.model == model, atoms))
+    if model is not None:
+        atoms = list(filter(lambda atom: atom.model == model, atoms))
     return group_atoms(atoms, modified, sequence, nucleic_acid_only)
 
 
 def is_cif(cif_or_pdb: IO[str]) -> bool:
     cif_or_pdb.seek(0)
     for line in cif_or_pdb.readlines():
         if line.startswith("_atom_site"):
```

### Comparing `RNApolis-0.3.8/src/rnapolis/rfam_folder.py` & `RNApolis-0.3.9/src/rnapolis/rfam_folder.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.3.8/src/rnapolis/tertiary.py` & `RNApolis-0.3.9/src/rnapolis/tertiary.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.3.8/src/rnapolis/transformer.py` & `RNApolis-0.3.9/src/rnapolis/transformer.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.3.8/src/rnapolis/util.py` & `RNApolis-0.3.9/src/rnapolis/util.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.3.8/tests/test_annotator.py` & `RNApolis-0.3.9/tests/test_annotator.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.3.8/tests/test_bugfixes.py` & `RNApolis-0.3.9/tests/test_bugfixes.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.3.8/tests/test_common.py` & `RNApolis-0.3.9/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.3.8/tests/test_metareader.py` & `RNApolis-0.3.9/tests/test_metareader.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.3.8/tests/test_quadruplexes.py` & `RNApolis-0.3.9/tests/test_quadruplexes.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.3.8/tests/test_rfam_folder.py` & `RNApolis-0.3.9/tests/test_rfam_folder.py`

 * *Files identical despite different names*

### Comparing `RNApolis-0.3.8/tests/test_tertiary.py` & `RNApolis-0.3.9/tests/test_tertiary.py`

 * *Files identical despite different names*

