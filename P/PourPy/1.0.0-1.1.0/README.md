# Comparing `tmp/PourPy-1.0.0.tar.gz` & `tmp/pourpy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PourPy-1.0.0.tar", last modified: Tue Jan 30 09:54:33 2024, max compression
+gzip compressed data, was "pourpy-1.1.0.tar", last modified: Wed May  8 20:55:04 2024, max compression
```

## Comparing `PourPy-1.0.0.tar` & `pourpy-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 mohit     (1000) mohit     (1000)        0 2024-01-30 09:54:33.512874 PourPy-1.0.0/
--rw-rw-r--   0 mohit     (1000) mohit     (1000)    35137 2023-12-31 20:05:01.000000 PourPy-1.0.0/LICENSE
--rw-r--r--   0 mohit     (1000) mohit     (1000)    43488 2024-01-30 09:54:33.512874 PourPy-1.0.0/PKG-INFO
-drwxrwxr-x   0 mohit     (1000) mohit     (1000)        0 2024-01-30 09:54:33.512874 PourPy-1.0.0/PourPy/
--rw-rw-r--   0 mohit     (1000) mohit     (1000)      277 2023-11-15 20:54:02.000000 PourPy-1.0.0/PourPy/__init__.py
--rw-rw-r--   0 mohit     (1000) mohit     (1000)      671 2023-12-05 21:14:07.000000 PourPy-1.0.0/PourPy/common.py
--rw-rw-r--   0 mohit     (1000) mohit     (1000)     3310 2024-01-01 14:29:37.000000 PourPy-1.0.0/PourPy/database.py
--rw-rw-r--   0 mohit     (1000) mohit     (1000)     4685 2024-01-02 14:01:51.000000 PourPy-1.0.0/PourPy/parser.py
--rw-rw-r--   0 mohit     (1000) mohit     (1000)    24331 2024-01-30 09:16:00.000000 PourPy-1.0.0/PourPy/pourbaix.py
--rw-rw-r--   0 mohit     (1000) mohit     (1000)     7948 2024-01-02 15:47:03.000000 PourPy-1.0.0/PourPy/reactant.py
--rw-rw-r--   0 mohit     (1000) mohit     (1000)    11944 2024-01-02 21:59:51.000000 PourPy-1.0.0/PourPy/reaction.py
--rw-rw-r--   0 mohit     (1000) mohit     (1000)    20598 2024-01-02 21:55:28.000000 PourPy-1.0.0/PourPy/system.py
-drwxrwxr-x   0 mohit     (1000) mohit     (1000)        0 2024-01-30 09:54:33.512874 PourPy-1.0.0/PourPy.egg-info/
--rw-r--r--   0 mohit     (1000) mohit     (1000)    43488 2024-01-30 09:54:33.000000 PourPy-1.0.0/PourPy.egg-info/PKG-INFO
--rw-rw-r--   0 mohit     (1000) mohit     (1000)      409 2024-01-30 09:54:33.000000 PourPy-1.0.0/PourPy.egg-info/SOURCES.txt
--rw-rw-r--   0 mohit     (1000) mohit     (1000)        1 2024-01-30 09:54:33.000000 PourPy-1.0.0/PourPy.egg-info/dependency_links.txt
--rw-rw-r--   0 mohit     (1000) mohit     (1000)        1 2024-01-30 09:48:52.000000 PourPy-1.0.0/PourPy.egg-info/not-zip-safe
--rw-rw-r--   0 mohit     (1000) mohit     (1000)      116 2024-01-30 09:54:33.000000 PourPy-1.0.0/PourPy.egg-info/requires.txt
--rw-rw-r--   0 mohit     (1000) mohit     (1000)        7 2024-01-30 09:54:33.000000 PourPy-1.0.0/PourPy.egg-info/top_level.txt
--rw-rw-r--   0 mohit     (1000) mohit     (1000)     2002 2024-01-30 09:43:54.000000 PourPy-1.0.0/README.md
--rw-rw-r--   0 mohit     (1000) mohit     (1000)     1025 2024-01-30 09:48:34.000000 PourPy-1.0.0/pyproject.toml
--rw-rw-r--   0 mohit     (1000) mohit     (1000)       38 2024-01-30 09:54:33.512874 PourPy-1.0.0/setup.cfg
--rw-rw-r--   0 mohit     (1000) mohit     (1000)      598 2024-01-30 09:47:22.000000 PourPy-1.0.0/setup.py
-drwxrwxr-x   0 mohit     (1000) mohit     (1000)        0 2024-01-30 09:54:33.512874 PourPy-1.0.0/tests/
--rw-rw-r--   0 mohit     (1000) mohit     (1000)      820 2024-01-30 09:51:05.000000 PourPy-1.0.0/tests/test_parser.py
--rw-rw-r--   0 mohit     (1000) mohit     (1000)     3347 2024-01-30 09:51:12.000000 PourPy-1.0.0/tests/test_pourbaix.py
+drwxrwxr-x   0 mohit     (1000) mohit     (1000)        0 2024-05-08 20:55:04.484177 pourpy-1.1.0/
+-rw-rw-r--   0 mohit     (1000) mohit     (1000)    35137 2023-12-31 20:05:01.000000 pourpy-1.1.0/LICENSE
+-rw-r--r--   0 mohit     (1000) mohit     (1000)    44207 2024-05-08 20:55:04.484177 pourpy-1.1.0/PKG-INFO
+drwxrwxr-x   0 mohit     (1000) mohit     (1000)        0 2024-05-08 20:55:04.484177 pourpy-1.1.0/PourPy/
+-rw-rw-r--   0 mohit     (1000) mohit     (1000)      277 2023-11-15 20:54:02.000000 pourpy-1.1.0/PourPy/__init__.py
+-rw-rw-r--   0 mohit     (1000) mohit     (1000)      671 2024-05-08 20:21:51.000000 pourpy-1.1.0/PourPy/common.py
+-rw-rw-r--   0 mohit     (1000) mohit     (1000)     3395 2024-05-08 20:21:51.000000 pourpy-1.1.0/PourPy/database.py
+-rw-rw-r--   0 mohit     (1000) mohit     (1000)     4685 2024-04-28 11:50:06.000000 pourpy-1.1.0/PourPy/parser.py
+-rw-rw-r--   0 mohit     (1000) mohit     (1000)    28635 2024-05-08 20:21:51.000000 pourpy-1.1.0/PourPy/pourbaix.py
+-rw-rw-r--   0 mohit     (1000) mohit     (1000)     7948 2024-01-02 15:47:03.000000 pourpy-1.1.0/PourPy/reactant.py
+-rw-rw-r--   0 mohit     (1000) mohit     (1000)    12106 2024-05-08 20:21:51.000000 pourpy-1.1.0/PourPy/reaction.py
+-rw-rw-r--   0 mohit     (1000) mohit     (1000)    20930 2024-05-08 20:21:51.000000 pourpy-1.1.0/PourPy/system.py
+drwxrwxr-x   0 mohit     (1000) mohit     (1000)        0 2024-05-08 20:55:04.484177 pourpy-1.1.0/PourPy.egg-info/
+-rw-r--r--   0 mohit     (1000) mohit     (1000)    44207 2024-05-08 20:55:04.000000 pourpy-1.1.0/PourPy.egg-info/PKG-INFO
+-rw-rw-r--   0 mohit     (1000) mohit     (1000)      409 2024-05-08 20:55:04.000000 pourpy-1.1.0/PourPy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mohit     (1000) mohit     (1000)        1 2024-05-08 20:55:04.000000 pourpy-1.1.0/PourPy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mohit     (1000) mohit     (1000)        1 2024-01-30 09:48:52.000000 pourpy-1.1.0/PourPy.egg-info/not-zip-safe
+-rw-rw-r--   0 mohit     (1000) mohit     (1000)      124 2024-05-08 20:55:04.000000 pourpy-1.1.0/PourPy.egg-info/requires.txt
+-rw-rw-r--   0 mohit     (1000) mohit     (1000)        7 2024-05-08 20:55:04.000000 pourpy-1.1.0/PourPy.egg-info/top_level.txt
+-rw-rw-r--   0 mohit     (1000) mohit     (1000)     2683 2024-05-08 20:20:30.000000 pourpy-1.1.0/README.md
+-rw-rw-r--   0 mohit     (1000) mohit     (1000)     1092 2024-05-08 20:54:47.000000 pourpy-1.1.0/pyproject.toml
+-rw-rw-r--   0 mohit     (1000) mohit     (1000)       38 2024-05-08 20:55:04.484177 pourpy-1.1.0/setup.cfg
+-rw-rw-r--   0 mohit     (1000) mohit     (1000)      600 2024-05-08 20:30:53.000000 pourpy-1.1.0/setup.py
+drwxrwxr-x   0 mohit     (1000) mohit     (1000)        0 2024-05-08 20:55:04.484177 pourpy-1.1.0/tests/
+-rw-rw-r--   0 mohit     (1000) mohit     (1000)      964 2024-03-03 08:47:13.000000 pourpy-1.1.0/tests/test_parser.py
+-rw-rw-r--   0 mohit     (1000) mohit     (1000)     1807 2024-03-03 13:50:52.000000 pourpy-1.1.0/tests/test_pourbaix.py
```

### Comparing `PourPy-1.0.0/LICENSE` & `pourpy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PourPy-1.0.0/PKG-INFO` & `pourpy-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PourPy
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python-based library to generate Pourbaix diagrams (potential/pH diagram)
 Home-page: https://gitlab.com/cmbm-ethz/pourbaix-diagrams
 Author: Fabio Furcas, Anja Korber, Mohit Pundir
 Author-email: Mohit Pundir <mpundir@ethz.ch>, "Fabio E. Furcas" <ffurcas@ethz.ch>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -685,22 +685,23 @@
 Keywords: potential-diagram,pourbaix,chemical
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argparse
-Requires-Dist: pytest
 Requires-Dist: bokeh
 Requires-Dist: matplotlib
 Requires-Dist: shapely
 Requires-Dist: nbsphinx
 Requires-Dist: sphinx-autoapi
 Requires-Dist: sphinx_rtd_theme
 Requires-Dist: tomli; python_version < "3.11"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 PourPy
 =============
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/cmbm-ethz%2Fpourbaix-diagrams/main?labpath=.%2Fexamples%2Fnotebooks%2Firon.ipynb)
 	
 A Python-based library to generate Pourbaix diagrams (potential/pH
 diagram). **PourPy** is an open-source python package,
@@ -729,26 +730,43 @@
 - nbsphinx
 - sphinx-autoapi
 - sphinx_rtd_theme
 
 
 Installation
 ===============
+Install the latest release from the Package repository:
+```
+pip install PourPy
+```
 
 Documentation
 =================
 The latest documentation is available on
 [readthedocs](https://readthedocs.org/). Please refer to the
 documentation on how to use the PourPy package:
 [pourbaix-diagrams.rtfd.io](https://pourbaix-diagrams.readthedocs.io/en/latest/)
 
+Webapp
+======
+PourPy is also available as a webapp with all the functionalities [PourPy Weabpp](https://pourpy-webapp.runmercury.com/app/pourpy-mercury)
+
 
 Examples
 ==========
-
 For live and interacting examples mentioned in the documentation, please check the following link:
 [Interactive examples](https://mybinder.org/v2/gl/cmbm-ethz%2Fpourbaix-diagrams/a20c113396cf23bf1b642c8ccdacc74124a3db5f?urlpath=lab%2Ftree%2Fexamples%2Fnotebooks%2Firon.ipynb)
 
+Contributing
+============
+Contributions to PourPy are welcome! Please follow the guidelines below.
+
+Report an issue
+If you have an account on [gitlab](https://gitlab.com/), you can submit an issue.
+
+Submit a patch / merge-request
+Follow this [guide](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html#new-merge-request-from-a-fork) to create a merge request on GitLab. Please target the repository's `main` branch.
+
 License
 =========
-PyPourbaix is distributed under the terms of [GNU LGPL v3](https://www.gnu.org/licenses/lgpl-3.0.en.html)
+PourPy is distributed under the terms of [GNU LGPL v3](https://www.gnu.org/licenses/lgpl-3.0.en.html)
```

### Comparing `PourPy-1.0.0/PourPy/common.py` & `pourpy-1.1.0/PourPy/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,14 @@
     STANDARD_PRESSURE = 1.0
 
 
 class Defaults(object):
     activity = 1.00
     maximum_electrode_potential = 2.0
     minimum_electrode_potenital = -2.0
-    maximum_pH_value = 14.0
+    maximum_pH_value = 16.0
     minimum_pH_value = 0.
     pressure = 1.
     temperature = 298.15
     reference_electrode_abbreviation = "SHE"
     reference_potential_difference = 0.0
     reference_electrodes = {"SHE": 0.000, "SCE":0.241, "CSE":0.314, "SCE":0.197}
```

### Comparing `PourPy-1.0.0/PourPy/database.py` & `pourpy-1.1.0/PourPy/database.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,77 +1,141 @@
 from .parser import DefaultParser
 
+
 class Database(object):
-    def __init__(self, species : list, elements : dict, parser=None):
+    def __init__(self, species: list, elements: dict, parser=None):
         self.elements = elements
         self.species = species
         self.parser = parser
 
     def __str__(self):
         padding = 8
         print(f"{'Database':{'-'}{'^'}{64}}")
-        print(f"{'Species':{padding}}\t{'dGf':>{padding}}\t{'dHf':>{padding}}\t{'Sm':>{padding}}")
-        print(f"{'':{'-'}{'^'}{64}}")      
+        print(
+            f"{'Species':{padding}}\t{'dGf':>{padding}}\t{'dHf':>{padding}}\t{'Sm':>{padding}}"
+        )
+        print(f"{'':{'-'}{'^'}{64}}")
         for species in self.species:
             print(species)
         return f"{'':{'-'}{'^'}{64}}"
 
     @classmethod
-    def from_default(cls, species : tuple):
-        """ Create database containing species and their chemical properties from a tuple of string
-        : param species : Species data as tuple of strings 
+    def from_default(cls, species: tuple):
+        """Create database containing species and their chemical properties from a tuple of string
+        : param species : Species data as tuple of strings
         : type species : tuple
         """
         elements = DefaultParser.parse_elements()
-        species  = DefaultParser.parse_species(species, elements)
+        species = DefaultParser.parse_species(species, elements)
         return cls(species, elements, DefaultParser)
 
     @classmethod
-    def from_file(cls, filename : str):
-        """ Create database containing species and their chemical properties from a txt file
-        : param filename : file containing species data 
+    def from_file(cls, filename: str):
+        """Create database containing species and their chemical properties from a txt file
+        : param filename : file containing species data
         : type filename : str
         """
 
-        with open(filename, 'r', encoding='utf-8') as f:
+        with open(filename, "r", encoding="utf-8") as f:
             lines = f.read().splitlines()
         return cls.from_default(tuple(lines))
 
     def add_reactions(self, reactions: tuple):
         parsed_reactions = self.parser.parse_reactions(reactions)
-        return self.associate_reactions_to_database(parsed_reactions)            
-    
-    def associate_reactions_to_database(self, reactions : list):
+        return self.associate_reactions_to_database(parsed_reactions)
+
+    def associate_reactions_to_database(self, reactions: list):
         complete = []
         for reac in reactions:
             dic = dict()
             for key, value in reac.items():
                 for react in self.species:
                     if key == react.formula:
                         dic[react] = value
             complete.append(dic)
         return complete
 
 
-
-elements = {'e': 0, 'La': 0, 'H': 1.0079, 'Xe': 131.3,
-            'He': 4.0026, 'Li': 6.941, 'Rf': 265.0, 'B': 10.81,
-            'Db': 268.0, 'Fe': 55.847, 'Sg': 271.0, 'Bh': 272.0,
-            'F': 18.998, 'Ag': 107.87, 'Mt': 276.0, 'Na': 22.99,
-            'Mg': 24.305, 'Cs': 132.91, 'Al': 26.982, 'Zr': 91.224,
-            'Si': 28.086, 'P': 30.974, 'S': 32.06, 'Cl': 35.453,
-            'Ar': 39.948, 'Ca': 40.08, 'N': 14.007, 'Sc': 44.955912,
-            'Hf': 178.49, 'Ti': 47.9, 'Hg': 200.59, 'V': 50.941,
-            'Cr': 51.996, 'Ta': 180.95, 'O': 15.999, 'Mn': 54.938,
-            'Be': 9.0122, 'Ba': 137.33, 'Co': 58.933, 'Fr': 223.0,
-            'Os': 190.2, 'Cu': 63.546, 'Ir': 192.22, 'Zn': 65.38,
-            'Pt': 195.09, 'Au': 196.97, 'Ga': 69.72, 'Ge': 72.59,
-            'C': 12.011, 'As': 74.922, 'W': 183.84, 'Tl': 204.37,
-            'Bi': 206.98, 'Br': 79.904, 'Rn': 222.0, 'At': 210.0,
-            'Kr': 83.8, 'Rb': 85.468, 'Sr': 87.62, 'Y': 88.906,
-            'Pb': 207.2, 'Nb': 92.906, 'Ni': 58.71, 'Ne': 20.179,
-            'Mo': 95.94, 'Tc': 97.0, 'Ra': 226.03, 'Ac': 227.0,
-            'Ru': 102.91, 'Po': 209.0, 'Re': 128.207, 'Pd': 106.4,
-            'K': 39.096, 'Cd': 112.41, 'In': 114.82, 'Sn': 118.69,
-            'Sb': 121.75, 'Se': 78.96, 'I': 126.9, 'Te': 127.6}
+elements = {
+    "e": 0,
+    "La": 0,
+    "H": 1.0079,
+    "Xe": 131.3,
+    "He": 4.0026,
+    "Li": 6.941,
+    "Rf": 265.0,
+    "B": 10.81,
+    "Db": 268.0,
+    "Fe": 55.847,
+    "Sg": 271.0,
+    "Bh": 272.0,
+    "F": 18.998,
+    "Ag": 107.87,
+    "Mt": 276.0,
+    "Na": 22.99,
+    "Mg": 24.305,
+    "Cs": 132.91,
+    "Al": 26.982,
+    "Zr": 91.224,
+    "Si": 28.086,
+    "P": 30.974,
+    "S": 32.06,
+    "Cl": 35.453,
+    "Ar": 39.948,
+    "Ca": 40.08,
+    "N": 14.007,
+    "Sc": 44.955912,
+    "Hf": 178.49,
+    "Ti": 47.9,
+    "Hg": 200.59,
+    "V": 50.941,
+    "Cr": 51.996,
+    "Ta": 180.95,
+    "O": 15.999,
+    "Mn": 54.938,
+    "Be": 9.0122,
+    "Ba": 137.33,
+    "Co": 58.933,
+    "Fr": 223.0,
+    "Os": 190.2,
+    "Cu": 63.546,
+    "Ir": 192.22,
+    "Zn": 65.38,
+    "Pt": 195.09,
+    "Au": 196.97,
+    "Ga": 69.72,
+    "Ge": 72.59,
+    "C": 12.011,
+    "As": 74.922,
+    "W": 183.84,
+    "Tl": 204.37,
+    "Bi": 206.98,
+    "Br": 79.904,
+    "Rn": 222.0,
+    "At": 210.0,
+    "Kr": 83.8,
+    "Rb": 85.468,
+    "Sr": 87.62,
+    "Y": 88.906,
+    "Pb": 207.2,
+    "Nb": 92.906,
+    "Ni": 58.71,
+    "Ne": 20.179,
+    "Mo": 95.94,
+    "Tc": 97.0,
+    "Ra": 226.03,
+    "Ac": 227.0,
+    "Ru": 102.91,
+    "Po": 209.0,
+    "Re": 128.207,
+    "Pd": 106.4,
+    "K": 39.096,
+    "Cd": 112.41,
+    "In": 114.82,
+    "Sn": 118.69,
+    "Sb": 121.75,
+    "Se": 78.96,
+    "I": 126.9,
+    "Te": 127.6,
+}
 
 element_list = list(elements.keys())
```

### Comparing `PourPy-1.0.0/PourPy/parser.py` & `pourpy-1.1.0/PourPy/parser.py`

 * *Files identical despite different names*

### Comparing `PourPy-1.0.0/PourPy/pourbaix.py` & `pourpy-1.1.0/PourPy/pourbaix.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,37 @@
- #!/usr/bin/env python3
+#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Sun May 14 11:01:46 2023
 
 @author: anjakorber
 """
 
-# Handhabung für H+ und e-?
-# jeweils H|+1| und e|-1?|
-
-
 import numpy as np
 import warnings
 import math
 import random
 
-from .reaction import Reaction
 from .parser import DefaultParser
 from .common import Defaults
 
 # Bokeh Moduls
 from bokeh import io, plotting, models, layouts
 from bokeh.palettes import Set3_12 as palette
 from colorsys import rgb_to_hsv, hsv_to_rgb
 import itertools
 
 # Matplotlib
 import matplotlib.pyplot as plt
 from matplotlib.collections import PatchCollection
 from matplotlib.patches import Polygon
-import shapely 
+import shapely
 
 
-class PourbaixDiagram(object): 
+class PourbaixDiagram(object):
     """
     PourbaixDiagram class that defines and plots a Pourbaix diagram.
 
     :param reactive_system: The reactive system for which the diagram is constructed.
     :type reactive_system: ReactiveSystem
 
     :param HER: Hydrogen Evolution Reaction.
@@ -58,190 +53,228 @@
 
         :param OER: The oxygen evolution reaction (OER).
         :type OER: Reaction, optional
         """
         self.system = reactive_system
         self.inspectorMode = line_inspection
         if HER is True:
-            self.HER    =  [self.system.pHmin, 0.000 - 0.059*self.system.pHmin, self.system.pHmax, 0.000 - 0.059*self.system.pHmax]
+            self.HER = [
+                Defaults.minimum_pH_value,
+                0.000 - 0.059 * Defaults.minimum_pH_value,
+                Defaults.maximum_pH_value,
+                0.000 - 0.059 * Defaults.maximum_pH_value,
+            ]
         else:
-            self.HER    =  None
+            self.HER = None
         if OER is True:
-            self.OER    =  [self.system.pHmin, 1.23 - 0.059*self.system.pHmin, self.system.pHmax, 1.23 - 0.059*self.system.pHmax]
+            self.OER = [
+                Defaults.minimum_pH_value,
+                1.23 - 0.059 * Defaults.minimum_pH_value,
+                Defaults.maximum_pH_value,
+                1.23 - 0.059 * Defaults.maximum_pH_value,
+            ]
         else:
-            self.OER    =  None
-        self.stable_regions = dict()        
-    
+            self.OER = None
+        self.stable_regions = dict()
+
     def solve(self):
         """
         Solve the Pourbaix diagram by computing the intersections of all Nernst equation reaction lines and the regions of stability enclosed between the lines.
         """
         self.system.initialize()
         if self.inspectorMode is False:
             self._compute_intersections(self._get_unique_constitutents())
             self._compute_boundary_lines(self.system)
             self._construct_stability_regions()
-        
-    def show(self, backend='bokeh', plot_regions=False, labelling=True):
+
+    def show(self, backend="bokeh", plot_regions=False, labelling=True):
         """
         Plots the Pourbaix diagram using the specified plotting backend.
 
         :param backend: The plotting backend to use (either 'bokeh' or 'matplotlib').
         :type backend: str
 
         :raises RuntimeError: If the specified backend is invalid.
         """
-        if backend == 'bokeh':
+        if backend == "bokeh":
             io.show(self._get_bokeh_plot(plot_regions, labelling))
-        elif backend == 'matplotlib':
+        elif backend == "matplotlib":
             self._get_matplotlib_plot(plot_regions, labelling)
         else:
-            raise RuntimeError('Invalid backend. Please specify either "bokeh" or "matplotlib".')
+            raise RuntimeError(
+                'Invalid backend. Please specify either "bokeh" or "matplotlib".'
+            )
 
     def _get_unique_constitutents(self):
         """
         Get a dictionary of unique constituents in the included in the reactive system.
         Species H+, e-, H2O(l), O2(g) and H2(g) are automatically excluded, as these species are unique constituents of the aqueous solvent bound by the HER and OER by default.
- 
+
         :return: A dictionary of unique constituents.
         :rtype: dict
         """
         if len(self.system.reactions) < 1:
-            raise ValueError("The physical system provided has no reactions to be plotted.")
+            raise ValueError(
+                "The physical system provided has no reactions to be plotted."
+            )
 
         unique_constituents = dict()
-        exclude = ['H|+1|', 'e|-1|', 'H2O', 'O2', 'H2', 'HCO3|-1|']
+        exclude = ["H|+1|", "e|-1|", "H2O", "O2", "H2", "HCO3|-1|"]
 
         for reaction in self.system.reactions:
             if reaction.pourbaix_line is None:
                 continue
 
             for constituent in reaction.constituents:
-                if constituent.formula not in exclude and constituent not in unique_constituents:
+                if (
+                    constituent.formula not in exclude
+                    and constituent not in unique_constituents
+                ):
                     associated_reactions = []
                     for k in self.system.reactions:
-                        if constituent in k.constituents and k.pourbaix_line is not None:
+                        if (
+                            constituent in k.constituents
+                            and k.pourbaix_line is not None
+                        ):
                             associated_reactions.append(k)
 
                     # only include constituents with two valid reactions
                     if len(associated_reactions) > 1:
                         unique_constituents.update({constituent: associated_reactions})
 
         return unique_constituents
 
-    @staticmethod
-    def _compute_intersections(unique_constituents : dict):
+    def check_pH(self, pH_to_check):
+        return self.system.pHmin <= pH_to_check <= self.system.pHmax
+
+    def _compute_intersections(self, unique_constituents: dict):
         """
         Compute intersections between the reactions marking the stablity region of each unique constituent.
 
         :param unique_constituents: A dictionary of unique constituents.
         :type unique_constituents: dict
         """
 
         tolerance = 1e-5
         for i in unique_constituents:
             if len(unique_constituents[i]) == 1:
                 continue
             for j in unique_constituents[i]:
                 for k in unique_constituents[i]:
                     if j != k:
-                        [x1, y1, x2, y2] = j.pourbaix_line
-                        [x3, y3, x4, y4] = k.pourbaix_line
-                        if j.echem_reaction and j.pH_reaction and k.echem_reaction and k.pH_reaction:
-                            k1 = (y2-y1)/(x2-x1)
-                            d1 = y1 - k1*x1
-                            k3 = (y4-y3)/(x4-x3)
-                            d3 = y3 - k3*x3
+                        [pH0, pot0, pH1, pot1] = j.pourbaix_line
+                        [pH2, pot2, pH3, pot3] = k.pourbaix_line
+
+                        if (
+                            j.echem_reaction
+                            and j.pH_reaction
+                            and k.echem_reaction
+                            and k.pH_reaction
+                        ):
+                            k1 = (pot1 - pot0) / (pH1 - pH0)
+                            d1 = pot0 - k1 * pH0
+                            k3 = (pot3 - pot2) / (pH3 - pH2)
+                            d3 = pot2 - k3 * pH2
                             if abs(k1 - k3) > tolerance:
-                                x = (d3-d1)/(k1-k3)
-                                j.intersections.append([x, k1*x + d1])
+                                x = (d3 - d1) / (k1 - k3)
+                                j.intersections.append([x, k1 * x + d1])
                                 j.intersecReac.append(k)
                         elif j.echem_reaction and j.pH_reaction and k.pH_reaction:
-                            k1 = (y2-y1)/(x2-x1)
-                            d1 = y1 - k1*x1
-                            j.intersections.append([x3, k1*x3+d1])
+                            k1 = (pot1 - pot0) / (pH1 - pH0)
+                            d1 = pot0 - k1 * pH0
+
+                            j.intersections.append([pH2, k1 * pH2 + d1])
                             j.intersecReac.append(k)
                         elif j.pH_reaction and k.echem_reaction and k.pH_reaction:
-                            k3 = (y4-y3)/(x4-x3)
-                            d3 = y3 - k3*x3
-                            j.intersections.append([x1, k3*x1+d3])
+                            k3 = (pot3 - pot2) / (pH3 - pH2)
+                            d3 = pot2 - k3 * pH2
+
+                            j.intersections.append([pH0, k3 * pH0 + d3])
                             j.intersecReac.append(k)
                         elif j.echem_reaction and j.pH_reaction and k.echem_reaction:
-                            k1 = (y2-y1)/(x2-x1)
-                            d1 = y1 - k1*x1
-                            j.intersections.append([(y3-d1)/k1, y3])
+                            k1 = (pot1 - pot0) / (pH1 - pH0)
+                            d1 = pot0 - k1 * pH0
+                            j.intersections.append([(pot2 - d1) / k1, pot2])
                             j.intersecReac.append(k)
                         elif j.echem_reaction and k.echem_reaction and k.pH_reaction:
-                            k3 = (y4-y3)/(x4-x3)
-                            d3 = y3 - k3*x3
-                            j.intersections.append([(y1-d3)/k3, y1])
+                            k3 = (pot3 - pot2) / (pH3 - pH2)
+                            d3 = pot2 - k3 * pH2
+
+                            j.intersections.append([(pot0 - d3) / k3, pot0])
                             j.intersecReac.append(k)
                         elif j.echem_reaction and k.pH_reaction:
-                            j.intersections.append([x3, y1])
+                            j.intersections.append([pH2, pot0])
                             j.intersecReac.append(k)
                         elif j.pH_reaction and k.echem_reaction:
-                            j.intersections.append([x1, y3])
+                            j.intersections.append([pH0, pot2])
                             j.intersecReac.append(k)
-        
+
     @staticmethod
     def _compute_boundary_lines(system):
         """
         Compute the boundary lines that actually enclose the stability region of each unique constituent.
 
         :param system: The reactive system.
         :type system: ReactiveSystem
         """
         tolerance = 1e-4
         for i in system.reactions:
-            
+
             if i.pourbaix_line is None:
                 continue
-            
+
             a = i.intersections
             b = i.intersecReac
 
             i.intersections = []
             i.intersecReac = []
             j = 0
             while j < len(a):
-                k = j+1
+                k = j + 1
                 while k < len(a):
-                    if abs(a[j][0]-a[k][0]) < tolerance and abs(a[j][1]-a[k][1]) < tolerance:
+                    if (
+                        abs(a[j][0] - a[k][0]) < tolerance
+                        and abs(a[j][1] - a[k][1]) < tolerance
+                    ):
                         i.intersections.append(a[j])
                         i.intersecReac.append(b[j])
                         a = [x for x in a if a[j] != x]
                         b = [x for x in b if b[j] != x]
                         j = 0
                         k = 0
                     k += 1
                 j += 1
 
-    
-                
             if len(i.intersections) == 1:
                 dummyReaction = i.intersecReac[0]
                 VZReactant = 0
                 VZe = 0
                 VZH = 0
                 for j in i.constituents:
                     for k in dummyReaction.constituents:
-                        if j == k and j.formula not in ['H|+1|', 'e|-1|', 'H2O', 'O2', 'H2', 'HCO3|-1|']:
+                        if j == k and j.formula not in [
+                            "H|+1|",
+                            "e|-1|",
+                            "H2O",
+                            "O2",
+                            "H2",
+                            "HCO3|-1|",
+                        ]:
                             VZReactant = dummyReaction.constituents[k][0]
-                        if k.formula == 'e|-1|':
+                        if k.formula == "e|-1|":
                             VZe = dummyReaction.constituents[k][0]
-                        if k.formula == 'H|+1|':
+                        if k.formula == "H|+1|":
                             VZH = dummyReaction.constituents[k][0]
-                            
-                            
+
                 if dummyReaction.pH_reaction and dummyReaction.echem_reaction:
                     if i.pH_reaction and i.echem_reaction:
-                        [x1, y1, x2, y2] = dummyReaction.pourbaix_line
-                        [x3, y3, x4, y4] = i.pourbaix_line
-                        k1 = (y2-y1)/(x2-x1)
-                        k3 = (y4-y3)/(x4-x3)
+                        [pH0, pot0, pH1, pot1] = dummyReaction.pourbaix_line
+                        [pH2, pot2, pH3, pot3] = i.pourbaix_line
+                        k1 = (pot1 - pot0) / (pH1 - pH0)
+                        k3 = (pot3 - pot2) / (pH3 - pH2)
                     if (VZReactant < 0 and VZe < 0) or (VZReactant > 0 and VZe > 0):
                         if i.pH_reaction and i.echem_reaction:
                             if k1 < k3:
                                 i.intersections.append(i.pourbaix_line[2:4])
                             else:
                                 i.intersections.append(i.pourbaix_line[0:2])
                         elif i.pH_reaction:
@@ -254,23 +287,21 @@
                                 i.intersections.append(i.pourbaix_line[0:2])
                             elif k1 > k3:
                                 i.intersections.append(i.pourbaix_line[2:4])
                         elif i.pH_reaction:
                             i.intersections.append(i.pourbaix_line[2:4])
                         elif i.echem_reaction:
                             i.intersections.append(i.pourbaix_line[0:2])
-                            
-                            
+
                 elif dummyReaction.pH_reaction:
                     if (VZReactant < 0 and VZH < 0) or (VZReactant > 0 and VZH > 0):
                         i.intersections.append(i.pourbaix_line[2:4])
                     elif (VZReactant < 0 and VZH > 0) or (VZReactant > 0 and VZH < 0):
                         i.intersections.append(i.pourbaix_line[0:2])
-                        
-                        
+
                 elif dummyReaction.echem_reaction:
                     if (VZReactant < 0 and VZe < 0) or (VZReactant > 0 and VZe > 0):
                         i.intersections.append(i.pourbaix_line[0:2])
                     elif (VZReactant < 0 and VZe > 0) or (VZReactant > 0 and VZe < 0):
                         i.intersections.append(i.pourbaix_line[2:4])
 
     def _construct_stability_regions(self):
@@ -279,52 +310,64 @@
 
         This method calculates stability regions for different constituents on the Pourbaix diagram
         and adds corner points where the computed intersection points are on the boundary of the diagram.
 
         :return: None
         :rtype: None
         """
+        coords = (
+            (self.system.pHmin, self.system.Emin),
+            (self.system.pHmax, self.system.Emin),
+            (self.system.pHmax, self.system.Emax),
+            (self.system.pHmin, self.system.Emax),
+        )
+        region_of_interest = shapely.Polygon(coords)
+
         unique_constituents = self._get_unique_constitutents()
         for i in unique_constituents:
             for j in self.system.reactions:
                 if i in j.constituents:
                     for k in j.intersections:
                         if k[0] not in i.intersectionsX or k[1] not in i.intersectionsY:
                             i.intersectionsX.append(k[0])
                             i.intersectionsY.append(k[1])
-                        if k[0] in i.intersectionsX and k[1] in i.intersectionsY and i.intersectionsX.index(k[0]) == i.intersectionsY.index(k[1]):
+                        if (
+                            k[0] in i.intersectionsX
+                            and k[1] in i.intersectionsY
+                            and i.intersectionsX.index(k[0])
+                            == i.intersectionsY.index(k[1])
+                        ):
                             pass
                         else:
                             i.intersectionsX.append(k[0])
                             i.intersectionsY.append(k[1])
 
-            try:
-                x_avg = sum(i.intersectionsX)/len(i.intersectionsX)
-                y_avg = sum(i.intersectionsY)/len(i.intersectionsY)
-            except ZeroDivisionError as e:
-                x_avg = 0
-                y_avg = 0
+            x_avg, y_avg = self._average_values(i)
 
             # Adding corner points where needed:
-            min_pH = self.system.pHmin
-            max_pH = self.system.pHmax
+            min_pH = Defaults.minimum_pH_value
+            max_pH = Defaults.maximum_pH_value
 
             if min_pH in i.intersectionsX:
                 indices = []
                 for idx, value in enumerate(i.intersectionsX):
                     if value == min_pH:
                         indices.append(idx)
                 if self.system.Emax in i.intersectionsY and len(indices) < 3:
                     i.intersectionsX.append(min_pH)
                     i.intersectionsY.append(self.system.Emax)
                 elif self.system.Emin in i.intersectionsY and len(indices) < 3:
                     i.intersectionsX.append(min_pH)
                     i.intersectionsY.append(self.system.Emin)
-                elif self.system.Emin not in i.intersectionsY and self.system.Emax not in i.intersectionsY and len(indices) < 3:
-                    del1 = abs(self.system.Emin - y_avg) 
+                elif (
+                    self.system.Emin not in i.intersectionsY
+                    and self.system.Emax not in i.intersectionsY
+                    and len(indices) < 3
+                ):
+                    del1 = abs(self.system.Emin - y_avg)
                     del2 = abs(self.system.Emax - y_avg)
                     if del2 > del1:
                         i.intersectionsX.append(min_pH)
                         i.intersectionsY.append(self.system.Emin)
                     else:
                         i.intersectionsX.append(min_pH)
                         i.intersectionsY.append(self.system.Emax)
@@ -333,50 +376,81 @@
                 if self.system.Emax in i.intersectionsY:
                     i.intersectionsX.append(max_pH)
                     i.intersectionsY.append(self.system.Emax)
                 if self.system.Emin in i.intersectionsY:
                     i.intersectionsX.append(max_pH)
                     i.intersectionsY.append(self.system.Emin)
 
-            def polar_angle(point, reference_point):
-                """
-                Calculate the polar angle of a point relative to a reference intersection point.
-
-                :param point: The point to calculate the angle for.
-                :type point: tuple
-                :param reference_point: The reference point with respect to which the angle is calculated.
-                :type reference_point: tuple
-
-                :return: The polar angle of the point relative to the reference point.
-                :rtype: float
-                """
-                dx = point[0] - reference_point[0]
-                dy = point[1] - reference_point[1]
-                return (math.atan2(dy, dx) + 2 * math.pi) % (2 * math.pi)
-
             # Sorting all intersection points according to the polar angle of a point relative to a reference point:
-            points = list(zip(i.intersectionsX, (y + self.system.deltaE for y in i.intersectionsY)))
+            points = list(
+                zip(
+                    i.intersectionsX, (y + self.system.deltaE for y in i.intersectionsY)
+                )
+            )
 
             # Recompute the x and y average after adding various corner points:
-            try:
-                x_avg = sum(i.intersectionsX)/len(i.intersectionsX)
-                y_avg = sum(i.intersectionsY)/len(i.intersectionsY)
-            except ZeroDivisionError as e:
-                x_avg = 0
-                y_avg = 0
-
-            sorted_points = sorted(points,
-                                   key =
-                                   lambda point:
-                                   polar_angle(point, [x_avg, y_avg]))
-
-            region = shapely.Polygon(tuple(sorted_points))
-            minx, miny, maxx, maxy = region.bounds
-
-            self.stable_regions[str(i.reactant_string)] = shapely.Polygon(tuple(sorted_points))
+            x_avg, y_avg = self._average_values(i)
+            sorted_points = sorted(
+                points, key=lambda point: self._polar_angle(point, [x_avg, y_avg])
+            )
+
+            polygon = shapely.Polygon(tuple(sorted_points))
+
+            # checking if the constructed polygon is valid or not
+            if not shapely.is_valid(polygon):
+                polygon = shapely.make_valid(polygon)
+                print(str(i.reactant_string))
+                print(polygon)
+
+                # if the valid geoemtrz is a collection of polygon and lines
+                if (
+                    shapely.get_type_id(polygon) == 7
+                ):  # shapely value for GEOMETRYCOLLECTION
+                    lines = []
+                    for _line in shapely.node(polygon).geoms:
+                        lines.append(_line)
+                    _polygon = shapely.polygonize(lines)
+                    polygon = _polygon.geoms[0]
+                    print(str(i.reactant_string))
+                    print(polygon)
+
+            # if the valid polygon lies entirly inside the region fo interest
+            if region_of_interest.contains_properly(polygon):
+                self.stable_regions[str(i.reactant_string)] = polygon
+
+            # if the valid polygon intersects the region fo interset
+            elif region_of_interest.intersects(polygon):
+                xmin, ymin, xmax, ymax = region_of_interest.bounds
+                clipped_polygon = shapely.clip_by_rect(polygon, xmin, ymin, xmax, ymax)
+                self.stable_regions[str(i.reactant_string)] = clipped_polygon
+
+    def _polar_angle(self, point, reference_point):
+        """
+        Calculate the polar angle of a point relative to a reference intersection point.
+
+        :param point: The point to calculate the angle for.
+        :type point: tuple
+        :param reference_point: The reference point with respect to which the angle is calculated.
+        :type reference_point: tuple
+
+        :return: The polar angle of the point relative to the reference point.
+        :rtype: float
+        """
+        dx = point[0] - reference_point[0]
+        dy = point[1] - reference_point[1]
+        return (math.atan2(dy, dx) + 2 * math.pi) % (2 * math.pi)
+
+    def _average_values(self, i):
+        try:
+            x_avg = sum(i.intersectionsX) / len(i.intersectionsX)
+            y_avg = sum(i.intersectionsY) / len(i.intersectionsY)
+        except ZeroDivisionError as e:
+            x_avg = 0
+            y_avg = 0
+        return x_avg, y_avg
 
     def get_stable_phases(self):
         """
         Get all stable phases within the created Pourbaix diagram.
 
         :return: A list of stable phases.
         :rtype: list
@@ -398,159 +472,253 @@
         :raises: warnings.warn if the point does not exist within the calculated range.
         """
         for key, value in self.stable_regions.items():
             if value.contains(shapely.Point(pH, potential)) is True:
                 return key
             else:
                 continue
-            
-        warnings.warn('Given point does not exist within the calculated range. Please modify the pH and potential limits of the diagram.')
+
+        warnings.warn(
+            "Given point does not exist within the calculated range. Please modify the pH and potential limits of the diagram."
+        )
         return 0
-            
+
     def _get_matplotlib_plot(self, plot_regions=False, labelling=True):
         """
         Display the created Pourbaix diagram using Matplotlib.
 
         :return: None
         :rtype: None
         """
         plt.figure(figsize=(8, 8))
         ax = plt.axes()
         if self.inspectorMode is True:
             for i in self.system.reactions:
                 xy = i.pourbaix_line
-                ax.plot([xy[0], xy[2]], [xy[1] + self.system.deltaE, xy[3] + self.system.deltaE], color='k', lw=0.6)
+                ax.plot(
+                    [xy[0], xy[2]],
+                    [xy[1] + self.system.deltaE, xy[3] + self.system.deltaE],
+                    color="k",
+                    lw=0.6,
+                )
         else:
             for i in self.system.reactions:
                 if i.pourbaix_line is None:
                     continue
                 if len(i.intersections) >= 2:
                     xy = i.intersections
-                    ax.plot([xy[0][0], xy[1][0]], [xy[0][1] + self.system.deltaE, xy[1][1] + self.system.deltaE],
-                            color='k', lw=0.6)
+                    ax.plot(
+                        [xy[0][0], xy[1][0]],
+                        [xy[0][1] + self.system.deltaE, xy[1][1] + self.system.deltaE],
+                        color="k",
+                        lw=0.6,
+                    )
 
         if self.HER != None:
-            ax.plot([self.HER[0], self.HER[2]], [self.HER[1] + self.system.deltaE, self.HER[3] + self.system.deltaE],
-                    color='blue', lw=0.6)
+            ax.plot(
+                [self.HER[0], self.HER[2]],
+                [self.HER[1] + self.system.deltaE, self.HER[3] + self.system.deltaE],
+                color="blue",
+                lw=0.6,
+            )
         if self.OER != None:
-            ax.plot([self.OER[0], self.OER[2]], [self.OER[1] + self.system.deltaE, self.OER[3] + self.system.deltaE],
-                    color='blue', lw=0.6)
+            ax.plot(
+                [self.OER[0], self.OER[2]],
+                [self.OER[1] + self.system.deltaE, self.OER[3] + self.system.deltaE],
+                color="blue",
+                lw=0.6,
+            )
 
         nb_regions = len(self.get_stable_phases())
         if labelling is True:
             patches = []
+
             for key, value in self.stable_regions.items():
-                polygon = Polygon(shapely.get_coordinates(value), closed=True, label=key)
+                print(key)
+                polygon = Polygon(
+                    shapely.get_coordinates(value), closed=True, label=key
+                )
                 patches.append(polygon)
-                ax.text(shapely.centroid(value).x, shapely.centroid(value).y, key,
-                        ha='center', va='center', transform=ax.transData)
+                ax.text(
+                    shapely.centroid(value).x,
+                    shapely.centroid(value).y,
+                    key,
+                    ha="center",
+                    va="center",
+                    transform=ax.transData,
+                )
             if plot_regions is True:
                 colors = 100 * np.arange(nb_regions)
                 p = PatchCollection(patches, alpha=0.2)
                 p.set_array(np.array(colors))
                 ax.add_collection(p)
-                
-        ax.set_ylim([self.system.Emin + self.system.deltaE, self.system.Emax + self.system.deltaE])
+
+        ax.set_ylim(
+            [
+                self.system.Emin + self.system.deltaE,
+                self.system.Emax + self.system.deltaE,
+            ]
+        )
         ax.set_xlim([self.system.pHmin, self.system.pHmax])
-  
-        ax.set_xlabel('pH', size=12)
-        ax.set_ylabel('Potential V vs. ' + self.system.reference_abbreviation, size=12)
+
+        ax.set_xlabel("pH", size=12)
+        ax.set_ylabel("Potential V vs. " + self.system.reference_abbreviation, size=12)
         plt.tight_layout()
         plt.show()
 
-    def _get_bokeh_plot(self, plot_regions=True,labelling=True):
+    def _get_bokeh_plot(self, plot_regions=True, labelling=True):
         """
         Display and return the created Pourbaix diagram using Bokeh.
 
         :return: Bokeh plot object.
         :rtype: Bokeh.plotting.figure
         """
         p = plotting.figure(
             title="POURBAIX DIAGRAM",
-            x_axis_label='pH',
-            y_axis_label='Potential V vs. ' + self.system.reference_abbreviation,
+            x_axis_label="pH",
+            y_axis_label="Potential V vs. " + self.system.reference_abbreviation,
             x_range=(self.system.pHmin, self.system.pHmax),
-            y_range=(self.system.Emin + self.system.deltaE,self.system.Emax + self.system.deltaE),
+            y_range=(
+                self.system.Emin + self.system.deltaE,
+                self.system.Emax + self.system.deltaE,
+            ),
             width=800,
-            height=800
+            height=800,
         )
 
         if self.inspectorMode is True:
             for i in self.system.reactions:
                 line_tooltip = [
                     ("pH, potential", "($x, $y)"),
-                    ("Reaction", str(i.reaction_string),)
+                    (
+                        "Reaction",
+                        str(i.reaction_string),
+                    ),
                 ]
-                p.line([i.pourbaix_line[0],i.pourbaix_line[2]],[i.pourbaix_line[1] + self.system.deltaE, i.pourbaix_line[3] + self.system.deltaE])
-                p.add_tools(models.HoverTool(renderers=[p.renderers[-1]], tooltips=line_tooltip))
+                p.line(
+                    [i.pourbaix_line[0], i.pourbaix_line[2]],
+                    [
+                        i.pourbaix_line[1] + self.system.deltaE,
+                        i.pourbaix_line[3] + self.system.deltaE,
+                    ],
+                )
+                p.add_tools(
+                    models.HoverTool(renderers=[p.renderers[-1]], tooltips=line_tooltip)
+                )
         else:
             for i in self.system.reactions:
                 if len(i.intersections) >= 2 and i.pourbaix_line is not None:
                     line_tooltip = [
-                    ("(pH, potential)", "($x, $y)"),
-                    ("Reaction", str(i.reaction_string)),
+                        ("(pH, potential)", "($x, $y)"),
+                        ("Reaction", str(i.reaction_string)),
                     ]
-                    p.line([i.intersections[0][0],i.intersections[1][0]],[i.intersections[0][1] + self.system.deltaE, i.intersections[1][1] + self.system.deltaE])
-                    p.add_tools(models.HoverTool(renderers=[p.renderers[-1]], tooltips=line_tooltip))
-
-
+                    p.line(
+                        [i.intersections[0][0], i.intersections[1][0]],
+                        [
+                            i.intersections[0][1] + self.system.deltaE,
+                            i.intersections[1][1] + self.system.deltaE,
+                        ],
+                    )
+                    p.add_tools(
+                        models.HoverTool(
+                            renderers=[p.renderers[-1]], tooltips=line_tooltip
+                        )
+                    )
 
             # Plotting HER and OER:
             if self.HER != None:
                 HER_tooltip = [
-                ("(pH, potential)", "($x, $y)"),
-                ("Component", "HER"),
+                    ("(pH, potential)", "($x, $y)"),
+                    ("Component", "HER"),
                 ]
-                p.line([self.HER[0], self.HER[2]],[self.HER[1] + self.system.deltaE, self.HER[3] + self.system.deltaE], line_dash='dashed',line_color='black')
-                p.add_tools(models.HoverTool(renderers=[p.renderers[-1]], tooltips=HER_tooltip))
+                p.line(
+                    [self.HER[0], self.HER[2]],
+                    [
+                        self.HER[1] + self.system.deltaE,
+                        self.HER[3] + self.system.deltaE,
+                    ],
+                    line_dash="dashed",
+                    line_color="black",
+                )
+                p.add_tools(
+                    models.HoverTool(renderers=[p.renderers[-1]], tooltips=HER_tooltip)
+                )
             if self.OER != None:
                 OER_tooltip = [
-                ("(pH, potential)", "($x, $y)"),
-                ("Reaction", "OER" ),
+                    ("(pH, potential)", "($x, $y)"),
+                    ("Reaction", "OER"),
                 ]
-                p.line([self.OER[0], self.OER[2]],[self.OER[1] + self.system.deltaE, self.OER[3] + self.system.deltaE], line_dash='dashed',line_color='black')
-                p.add_tools(models.HoverTool(renderers=[p.renderers[-1]], tooltips=OER_tooltip))
-
-            # Plotting regions of stability        
-            colors = itertools.cycle(palette)    
+                p.line(
+                    [self.OER[0], self.OER[2]],
+                    [
+                        self.OER[1] + self.system.deltaE,
+                        self.OER[3] + self.system.deltaE,
+                    ],
+                    line_dash="dashed",
+                    line_color="black",
+                )
+                p.add_tools(
+                    models.HoverTool(renderers=[p.renderers[-1]], tooltips=OER_tooltip)
+                )
 
+            # Plotting regions of stability
+            colors = itertools.cycle(palette)
 
         stability_regions = []
         if plot_regions is True:
             unique_const = self._get_unique_constitutents()
             for i, fill_color in zip(unique_const, colors):
-                if len(unique_const[i]) == 1:
+                if (
+                    len(unique_const[i]) == 1
+                    or str(i.reactant_string) not in self.stable_regions.keys()
+                ):
+                    continue
+                coords = shapely.get_coordinates(
+                    self.stable_regions[str(i.reactant_string)]
+                )
+                if len(coords) == 0:
                     continue
-                coords = shapely.get_coordinates(self.stable_regions[str(i.reactant_string)])
                 centroid = shapely.centroid(self.stable_regions[str(i.reactant_string)])
 
                 sorted_x = coords[:, 0]
                 sorted_y = coords[:, 1]
                 x_avg = centroid.x
                 y_avg = centroid.y
-                
-                stability_region = p.patch(sorted_x, sorted_y, fill_color=fill_color, alpha=0.5)
+
+                stability_region = p.patch(
+                    sorted_x, sorted_y, fill_color=fill_color, alpha=0.5
+                )
                 stability_regions.append(stability_region)
 
                 fill_tooltip = [
                     ("(pH, potential)", "($x, $y)"),
                     ("Component", str(i.reactant_string)),
                 ]
-                p.add_tools(models.HoverTool(renderers=[stability_region], tooltips=fill_tooltip))
+                p.add_tools(
+                    models.HoverTool(
+                        renderers=[stability_region], tooltips=fill_tooltip
+                    )
+                )
                 if labelling is True:
-                    stability_label =p.text(x_avg, y_avg, text=[str(i.reactant_string)], text_align="center", text_baseline="middle")
+                    stability_label = p.text(
+                        x_avg,
+                        y_avg,
+                        text=[str(i.reactant_string)],
+                        text_align="center",
+                        text_baseline="middle",
+                    )
 
         # pH range slider
         range_slider = models.RangeSlider(
             title="Adjust x-axis range",
             start=self.system.pHmin,
             end=self.system.pHmax,
             step=1,
             value=(p.x_range.start, p.x_range.end),
         )
         range_slider.js_link("value", p.x_range, "start", attr_selector=0)
         range_slider.js_link("value", p.x_range, "end", attr_selector=1)
 
         # Create Layout and Show Result
-        layout_standard = layouts.layout([[range_slider],[p]])
+        layout_standard = layouts.layout([[range_slider], [p]])
 
         return layout_standard
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `PourPy-1.0.0/PourPy/reactant.py` & `pourpy-1.1.0/PourPy/reactant.py`

 * *Files identical despite different names*

### Comparing `PourPy-1.0.0/PourPy/reaction.py` & `pourpy-1.1.0/PourPy/reaction.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,38 +7,38 @@
 """
 
 import numpy as np
 import json
 from .reactant import Reactant
 from .common import Constants, Defaults
 
+
 class Reaction(object):
-    """Reaction class featuring all reaction-specific parameters of the (electro)chemical reactions to be included in the Pourbaix diagram.
-    """
+    """Reaction class featuring all reaction-specific parameters of the (electro)chemical reactions to be included in the Pourbaix diagram."""
+
     def __init__(self, constituents, system):
         """Constructor method for Reaction class.
 
         :param constituents: A dictionary of reactants as keys and their corresponding stoichiometric coefficients and activities as values.
         :type constituents: dict
         :param system: The chemical system to which this reaction belongs.
         :type system: System
         """
         self.constituents = constituents
         self.system = system
         self.initialize()
-        
+
     def __str__(self):
         """Return the string representation of the reaction, where all reactants appear on the left hand side and all products appear on the right of the reacton arrow.
 
         :return: A string representation of the reaction, e.g., 'H2O ⇄ H2 + 0.5*O2'.
         :rtype: str
         """
         return self.reaction_string
 
-
     def initialize(self):
         """Initialize the Reaction object by calculating various reaction-specific properties.
 
         :return: None
         :rtype: None
         """
         for const in self.constituents:
@@ -49,277 +49,280 @@
         self.pH_reaction = self._get_pH_reaction()
         self.Hlimit = self._get_Hlimit()
         self.pourbaix_line = self._get_pourbaixLine()
         self.intersections = []
         self.lineBoundary = []
         self.intersecReac = []
 
-
     def _get_reaction_string(self):
         """Create the string representation of the reaction, where all reactants appear on the left hand side and all products appear on the right of the reacton arrow.
 
         Returns the string representation of the reaction, e.g., 'H2O ⇄ H2 + O2'.
 
         :return: A string representation of the reaction.
         :rtype: str
         """
-        arrow = ' ⇄ '
-        reactantStr = ''
-        productStr = ''
+        arrow = " ⇄ "
+        reactantStr = ""
+        productStr = ""
         for i in self.constituents:
             stoicCoeff = str(abs(self.constituents[i][0]))
-            if stoicCoeff == '1':
-                stoicCoeff = ''
+            if stoicCoeff == "1":
+                stoicCoeff = ""
             if self.constituents[i][0] < 0:
-                reactantStr += stoicCoeff + i.reactant_string + ' + '
+                reactantStr += stoicCoeff + i.reactant_string + " + "
             else:
-                productStr += stoicCoeff + i.reactant_string + ' + '
+                productStr += stoicCoeff + i.reactant_string + " + "
         reactantStr = reactantStr[0:-3]
         productStr = productStr[0:-3]
         return reactantStr + arrow + productStr
 
     def _get_echem_reaction(self):
         """Checks if the reaction is an electrochemical reaction, i.e. whether it contains electrons, and returns True if it's electrochemical, otherwise returns False.
 
         :return: True if the reaction is electrochemical, False otherwise.
         :rtype: bool
         """
 
         for i in self.constituents:
-            if i.formula == 'e|-1|':
+            if i.formula == "e|-1|":
                 return True
         return False
 
-
     def _get_pH_reaction(self):
         """Checks if the reaction is a pH-dependent reaction, i.e. whether it contains protons, and returns True if it's pH-dependent, otherwise returns False.
 
         :return: True if the reaction is pH-dependent, False otherwise.
         :rtype: bool
         """
 
         for i in self.constituents:
-            if i.formula == 'H|+1|': 
+            if i.formula == "H|+1|":
                 return True
         return False
 
     @property
     def dGr(self) -> float:
         """Calculate the standard Gibbs free energy change of the reaction from the standard molar Gibbs free energies of all reation costituents.
 
         :return: The standard Gibbs free energy change of the reaction in joules per mole.
         :rtype: float
         """
         dGr = 0.0
         for i in self.constituents:
-            dGr += self.constituents[i][0]*i.dGf
+            dGr += self.constituents[i][0] * i.dGf
         return dGr
-    
+
     @property
     def dHr(self) -> float:
         """Calculate the standard enthalpy change of the reaction from the standard molar enthalpies of all reation costituents.
 
         :return: The standard enthalpy change of the reaction in joules per mole.
         :rtype: float
         """
         dHr = 0.0
         for i in self.constituents:
-            dHr += self.constituents[i][0]*i.dHf
+            dHr += self.constituents[i][0] * i.dHf
         return dHr
 
     @property
     def dSr(self) -> float:
         """Calculate the standard entropy change of the reaction from the standard Gibbs free energy and enthalpy.
 
         :return: The standard entropy change of the reaction in joules per mole per degrees kelvin.
         :rtype: float
         """
 
-        return (self.dHr - self.dGr)/Constants.STANDARD_TEMPERATURE.value
+        return (self.dHr - self.dGr) / Constants.STANDARD_TEMPERATURE.value
 
     @property
     def K(self):
         """Calculate the equilibrium constant for the reaction from its standard Gibbs free energy.
 
         :return: The equilibrium constant K for the reaction.
         :rtype: float
         """
-    
-        return np.exp(-1*self.dGr/Constants.GAS.value/self.system.temperature)
+
+        return np.exp(-1 * self.dGr / Constants.GAS.value / self.system.temperature)
 
     @property
     def E0(self):
         """Calculate the standard electrode potential for the reaction in volts vs. SHE from its standard Gibbs gree energy.
 
         :return: The standard electrode potential E0 for the electrochemical reaction in volts vs. SHE, or 0 if the reaction is not an electrochemical reaction.
         :rtype: float
         """
         if not self.echem_reaction:
             return 0
         for i in self.constituents:
-            if i.formula == 'e|-1|':
-                return self.dGr/self.constituents[i][0]/Constants.FARADAY.value
+            if i.formula == "e|-1|":
+                return self.dGr / self.constituents[i][0] / Constants.FARADAY.value
 
     @property
     def nElectrons(self):
         """Retrieve the number of electrons involved in the reaction.
 
         :return: The number of electrons involved in the electrochemical reaction, or 0 if the reaction is not an electrochemical reaction.
         :rtype: float
         """
         if not self.echem_reaction:
             return 0
         for i in self.constituents:
-            if i.formula == 'e|-1|':
+            if i.formula == "e|-1|":
                 return self.constituents[i][0]
 
     @property
     def nProtons(self):
         """Retrieve the number of protons involved in the reaction.
 
         :return: The number of protons involved in the pH-dependent reaction, or 0 if the reaction is not pH-dependent.
         :rtype: float
         """
         if not self.pH_reaction:
             return 0
         for i in self.constituents:
-            if i.formula == 'H|+1|':
+            if i.formula == "H|+1|":
                 return self.constituents[i][0]
-                
-            
+
     def _get_Hlimit(self):
         """Retrieve the range of H+ activities corresponding to the pH limits of the Pourbaix diagram.
 
-        :return: An array of H+ activities. 
+        :return: An array of H+ activities.
         :rtype: numpy.ndarray
         """
-        return 10**(-np.linspace(self.system.pHmin, self.system.pHmax, 2))
-        
+        return 10 ** (
+            -np.linspace(Defaults.minimum_pH_value, Defaults.maximum_pH_value, 2)
+        )
+
     @property
     def Q(self) -> float:
         """Calculate the reaction quotient Q for the reaction.
 
         :return: The reaction quotient Q for the reaction.
         :rtype: float
         """
-        Q = 1.
+        Q = 1.0
         for i in self.constituents:
-            Q *= self.constituents[i][1]**self.constituents[i][0]
+            Q *= self.constituents[i][1] ** self.constituents[i][0]
         return Q
 
     @property
     def rQ(self) -> float:
         """Calculate the reduced reaction quotient rQ excluding the activity contribution of protons.
 
         :return: The reduced reaction quotient rQ for the reaction.
         :rtype: float
         """
-        rQ = 1.
+        rQ = 1.0
         for i in self.constituents:
-            if i.formula != 'H|+1|':
-                rQ *= self.constituents[i][1]**self.constituents[i][0]
+            if i.formula != "H|+1|":
+                rQ *= self.constituents[i][1] ** self.constituents[i][0]
         return rQ
 
     @property
     def QpH(self) -> list:
         """Calculate reaction quotient of the reaction at different H+ activities.
 
         :return: A list of reaction quotients at different H+ ion concentrations.
         :rtype: list
         """
         Q = []
         for i in range(len(self.Hlimit)):
             for j, value in self.constituents.items():
-                if j.formula == 'H|+1|':
+                if j.formula == "H|+1|":
                     value[1] = self.Hlimit[i]
             Q.append(self.Q)
         return Q
 
     def _get_pourbaixLine(self):
         """Calculate the Pourbaix line formulated by the reaction.
 
         :return: A list of coordinates defining the Pourbaix line, depending on whether the reaction is potential- and/or pH-dependent.
         :rtype: list
         :raises ValueError: If the reaction is neither potential- nor pH-dependent.
         """
-        if not(self.echem_reaction or self.pH_reaction):
-            raise ValueError("The reaction is neither pH nor potential\
-                             dependent and cannot be drawn.")
+        if not (self.echem_reaction or self.pH_reaction):
+            raise ValueError(
+                "The reaction is neither pH nor potential\
+                             dependent and cannot be drawn."
+            )
         elif self.echem_reaction and self.pH_reaction:
-            E = self.E0 + (Constants.GAS.value*self.system.temperature/Constants.FARADAY.value/self.nElectrons)*np.log(self.QpH)
-            return [self.system.pHmin, E[0], self.system.pHmax, E[-1]]
+            E = self.E0 + (
+                Constants.GAS.value
+                * self.system.temperature
+                / Constants.FARADAY.value
+                / self.nElectrons
+            ) * np.log(self.QpH)
+            return [Defaults.minimum_pH_value, E[0], Defaults.maximum_pH_value, E[-1]]
         elif self.pH_reaction:
-            pH = -np.log10((self.K/self.rQ)**(1./self.nProtons))
-            if pH < self.system.pHmin or pH > self.system.pHmax:
+            pH = -np.log10((self.K / self.rQ) ** (1.0 / self.nProtons))
+            if pH < Defaults.minimum_pH_value or pH > Defaults.maximum_pH_value:
                 return None
             return [pH, self.system.Emax, pH, self.system.Emin]
         elif self.echem_reaction:
-            E = self.E0 + (Constants.GAS.value*self.system.temperature/Constants.FARADAY.value/self.nElectrons)*np.log(self.Q)
-            return [self.system.pHmin, E, self.system.pHmax, E]
-            
+            E = self.E0 + (
+                Constants.GAS.value
+                * self.system.temperature
+                / Constants.FARADAY.value
+                / self.nElectrons
+            ) * np.log(self.Q)
+            return [Defaults.minimum_pH_value, E, Defaults.maximum_pH_value, E]
+
     def _sanity_check(self):
         """Perform a sanity check on the total charge and atom balance of all species in the reaction.
 
         :return: A message indicating whether charge and atom balances are correct or if there's a warning.
         :rtype: str
         """
         charge_balance = 0
         for i in self.constituents:
             charge_balance += i.charge * self.constituents[i][0]
-         
+
         balanced_atoms = {}
         for i in self.constituents:
             for j in i.atoms:
                 if j not in balanced_atoms:
-                    balanced_atoms[j] = i.atoms[j]*self.constituents[i][0]
+                    balanced_atoms[j] = i.atoms[j] * self.constituents[i][0]
                 else:
-                    balanced_atoms[j] += i.atoms[j]*self.constituents[i][0]
+                    balanced_atoms[j] += i.atoms[j] * self.constituents[i][0]
         atom_balance = 0
         for h in balanced_atoms:
-            if h != 'e': # !!!! somethings off, should be e|-1|, doesnt work
+            if h != "e":  # !!!! somethings off, should be e|-1|, doesnt work
                 atom_balance += balanced_atoms[h]
         if charge_balance == 0 and atom_balance == 0:
-            return 'Both the charge and the atoms are balanced.'
+            return "Both the charge and the atoms are balanced."
         elif charge_balance == 0:
-            return 'WARNING: The atoms are not balanced.' 
+            return "WARNING: The atoms are not balanced."
         elif atom_balance == 0:
-            return 'WARNING: The charge of the constituents is not balanced.'
+            return "WARNING: The charge of the constituents is not balanced."
         else:
-            return 'WARNING: Neither the charge nor the atoms are balanced.'
-        
-    
+            return "WARNING: Neither the charge nor the atoms are balanced."
+
     def _balanced_charge(self):
         """Check if the reaction is charge-balanced.
 
         :return: True if the reaction's charge is balanced, False otherwise.
         :rtype: bool
         """
         balance = 0
         for i in self.constituents:
             balance += i.charge * self.constituents[i][0]
         return balance == 0
-    
-    
+
     def _balanced_atoms(self):
         """Check if the reaction has balanced numbers of atoms of each chemical element.
 
         :return: True if the reaction's atoms are balanced, False otherwise.
         :rtype: bool
         """
         balanced_atoms = {}
         for i in self.constituents:
             for j in i.atoms:
                 if j not in balanced_atoms:
-                    balanced_atoms[j] = i.atoms[j]*self.constituents[i][0]
+                    balanced_atoms[j] = i.atoms[j] * self.constituents[i][0]
                 else:
-                    balanced_atoms[j] += i.atoms[j]*self.constituents[i][0]
+                    balanced_atoms[j] += i.atoms[j] * self.constituents[i][0]
         balance = 0
         for h in balanced_atoms:
-            if h != 'e|-1|':
+            if h != "e|-1|":
                 balance += balanced_atoms[h]
         return balance == 0
-        
-        
-        
-                
-        
-
```

### Comparing `PourPy-1.0.0/PourPy/system.py` & `pourpy-1.1.0/PourPy/system.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,57 +12,58 @@
 from .reaction import Reaction, Reactant
 from .database import element_list
 from .common import Constants, State, Defaults
 
 from functools import singledispatchmethod
 
 
-
 class System:
-    """System class that contains all required physiochemical parameters, elements and reacion constituents nessecary to create a pourbaix diagram.
-    """
+    """System class that contains all required physiochemical parameters, elements and reacion constituents nessecary to create a pourbaix diagram."""
+
     def __init__(self, filename=None):
         """Constructor method for the System class.
 
         :param filename: Optional filename to read various system parameters from.
         :type filename: str
         """
+
         if filename != None:
             self.read_parameters_from_file(filename)
 
-        self.reactions              = list()
-        self.elements               = dict()
-        self.temperature            = Defaults.temperature
-        self.pressure               = Defaults.pressure
-        self.pHmin                  = Defaults.minimum_pH_value
-        self.pHmax                  = Defaults.maximum_pH_value
-        self.Emin                   = Defaults.minimum_electrode_potenital
-        self.Emax                   = Defaults.maximum_electrode_potential
-        self.reference_electrode    = Defaults.reference_electrode_abbreviation, Defaults.reference_potential_difference
-
+        self.reactions = list()
+        self.elements = dict()
+        self.temperature = Defaults.temperature
+        self.pressure = Defaults.pressure
+        self.pHmin = Defaults.minimum_pH_value
+        self.pHmax = Defaults.maximum_pH_value
+        self.Emin = Defaults.minimum_electrode_potenital
+        self.Emax = Defaults.maximum_electrode_potential
+        self.reference_electrode = (
+            Defaults.reference_electrode_abbreviation,
+            Defaults.reference_potential_difference,
+        )
 
     def set_database(self, database):
         self.db = database
-    
+
     def __str__(self):
         """Generate a string of the System object containing all chemical reactions, its temperature and pressure.
 
         :return: String representation of the System.
         :rtype: str
         """
 
         padding = 8
         print(f"{'System':{'-'}{'^'}{64}}")
-        print(f'Temperature : {self.temperature}, Pressure : {self.pressure}')
-        print(f"{'':{'-'}{'^'}{64}}")      
+        print(f"Temperature : {self.temperature}, Pressure : {self.pressure}")
+        print(f"{'':{'-'}{'^'}{64}}")
 
         for reaction in self.reactions:
             print(f"\t{reaction}")
-        return  f"{'':{'-'}{'^'}{64}}"
-
+        return f"{'':{'-'}{'^'}{64}}"
 
     def initialize(self):
         """Initialize all chemical reactions included in the system using its current physiochemical parameters.
 
         :return: None
         :rtype: None
         """
@@ -93,143 +94,158 @@
         :param pHmin: Minimum pH of the diagram.
         :type pHmin: float
         :param pHmax: Maximum pH of the diagram.
         :type pHmax: float
         :param Emin: Minimum potential of the diagram in volts vs. SHE.
         :type Emin: float
         :param Emax: Maximum potential of the diagram in volts vs. SHE.
-        :type Emax: float 
+        :type Emax: float
         """
         parameter_dictionary = {
-            "constants":[
+            "constants": [
                 {
-                    "R": Constants.GAS.value, 
+                    "R": Constants.GAS.value,
                     "F": Constants.FARADAY.value,
                     "T0": Constants.STANDARD_TEMPERATURE.value,
                     "P0": Constants.STANDARD_PRESSURE.value,
                 }
             ],
-            "reference":[
+            "reference": [
                 {
                     "Reference_abbreviation": self.reference_abbreviation,
-                    "dE": self.deltaE
+                    "dE": self.deltaE,
                 }
             ],
-            "variables":[
+            "variables": [
                 {
                     "T": self.temperature,
                     "P": self.pressure,
                     "pHmin": self.pHmin,
                     "pHmax": self.pHmax,
                     "Emin": self.Emin,
-                    "Emax": self.Emax
+                    "Emax": self.Emax,
                 }
-            ]
+            ],
         }
-        
+
         json_string = json.dumps(parameter_dictionary, indent=2)
-        with open(filename, 'w') as f:
+        with open(filename, "w") as f:
             f.write(json_string)
-    
+
     def read_parameters_from_file(self, filename):
         """Reads system parameters from a JSON file.
 
         :param filename: Name of the JSON file to read parameters from.
         :type filename: str
         :return: None
         :rtype: None
         """
-        with open(filename, 'r') as f:
+        with open(filename, "r") as f:
             json_object = json.loads(f.read())
-        self.temperature  = json_object['variables'][0]['T']
-        self.pressure     = json_object['variables'][0]['P']
-        self.pHs          = (json_object['variables'][0]['pHmin'], 
-                             json_object['variables'][0]['pHmax'])
-        self.electrode_potentials = (json_object['variables'][0]['Emin'], 
-                                     json_object['variables'][0]['Emax'])
-        self.reference_electrode = (json_object['reference'][0]['Reference_abbreviation'],  json_object['reference'][0]['dE'])
+        self.temperature = json_object["variables"][0]["T"]
+        self.pressure = json_object["variables"][0]["P"]
+        self.pHs = (
+            json_object["variables"][0]["pHmin"],
+            json_object["variables"][0]["pHmax"],
+        )
+        self.electrode_potentials = (
+            json_object["variables"][0]["Emin"],
+            json_object["variables"][0]["Emax"],
+        )
+        self.reference_electrode = (
+            json_object["reference"][0]["Reference_abbreviation"],
+            json_object["reference"][0]["dE"],
+        )
 
     @property
     def temperature(self):
         """Get the system temperature.
 
         :return: Temperature in degrees Kelvin.
         :rtype: float
         """
         return self._temperature
 
     @temperature.setter
-    def temperature(self, value : float):
+    def temperature(self, value: float):
         """Validates the user-input temperature. If input is numerical
         and greater than 0, `298.15` otherwise.
-        
+
         :param value: Temperature in degrees Kelvin.
         :type value: float
         :return: None
         :rtype: None
         """
 
-        if not isinstance(value, (int,float)):
-            warnings.warn(f'System temperature provided not a numerical input. It will be reset to {Defaults.temperature} K.')
+        if not isinstance(value, (int, float)):
+            warnings.warn(
+                f"System temperature provided not a numerical input. It will be reset to {Defaults.temperature} K."
+            )
             self._temperature = Defaults.temperature
         elif value < 0:
-            warnings.warn(f'System temperature provided is less than 0 K. It will be reset to {Defaults.temperature} K.')
+            warnings.warn(
+                f"System temperature provided is less than 0 K. It will be reset to {Defaults.temperature} K."
+            )
             self._temperature = Defaults.temperature
         else:
             self._temperature = value
 
     @property
     def pressure(self):
         """Get the system pressure.
 
         :return: Pressure in bar.
         :rtype: float
         """
         return self._pressure
 
     @pressure.setter
-    def pressure(self, value : float):
+    def pressure(self, value: float):
         """Validates the user-input pressure. If input is numerical and
         greater than 0, `1.00` otherwise.
 
         :param value: Pressure in bar.
         :type value: float
         :return: None
         :rtype: None
         """
-        if not isinstance(value, (int,float)):
-            warnings.warn(f'System pressure provided not a numerical input. It will be reset to {Defaults.pressure} bar.')
+        if not isinstance(value, (int, float)):
+            warnings.warn(
+                f"System pressure provided not a numerical input. It will be reset to {Defaults.pressure} bar."
+            )
             self._pressure = Defaults.pressure
         elif value < 0:
-            warnings.warn(f'System temperature provided is less than 0 bar. It will be reset to {Defaults.pressure} bar.')
+            warnings.warn(
+                f"System temperature provided is less than 0 bar. It will be reset to {Defaults.pressure} bar."
+            )
             self._pressure = Defaults.pressure
         else:
             self._pressure = value
 
     @property
     def pHs(self):
         """Get the system pH range.
 
         :return: A tuple containing the minimum and maximum pH values.
         :rtype: tuple
         """
         return (self._pHmin, self._pHmax)
 
     @pHs.setter
-    def pHs(self, value : tuple):
+    def pHs(self, value: tuple):
         """Set the system pH range and automatically check which value is the lower one an which one corresponds to the upper limit.
 
         :param value: A tuple containing the minimum and maximum pH values.
         :type value: tuple
         :return: None
         :rtype: None
         """
         self.pHmin = min(value)
         self.pHmax = max(value)
-        
+
     @property
     def pHmin(self):
         """Get the minimum pH value of the system.
 
         :return: Minimum pH value.
         :rtype: float
         """
@@ -241,56 +257,60 @@
         numerical, `0.00` otherwise
 
         :param value: Minimum pH value.
         :type value: float
         :return: None
         :rtype: None
         """
-        if not isinstance(value, (int,float)):
-            warnings.warn(f'Lower pH limit provided not a numerical input. It will be reset to {Defaults.minimum_pH_value}')
+        if not isinstance(value, (int, float)):
+            warnings.warn(
+                f"Lower pH limit provided not a numerical input. It will be reset to {Defaults.minimum_pH_value}"
+            )
             self._pHmin = Defaults.minimum_pH_value
         else:
             self._pHmin = value
 
     @property
     def pHmax(self):
         """Get the maximum pH value of the system.
 
         :return: Maximum pH value.
         :rtype: float
         """
         return self._pHmax
 
     @pHmax.setter
-    def pHmax(self, value : float):
+    def pHmax(self, value: float):
         """Validates the user-input upper pH limit. If input is
         numerical, `14.00` otherwise.
 
         :param value: Maximum pH value.
         :type value: float
         :return: None
         :rtype: None
         """
-        if not isinstance(value, (int,float)):
-            warnings.warn('Upper pH limit provided not a numerical input. It will be reset to {Defaults.maximum_pH_value}')
+        if not isinstance(value, (int, float)):
+            warnings.warn(
+                "Upper pH limit provided not a numerical input. It will be reset to {Defaults.maximum_pH_value}"
+            )
             self._pHmax = Defaults.maximum_pH_value
         else:
             self._pHmax = value
 
     @property
     def electrode_potentials(self):
         """Get the electrode potential range of the system and automatically check which value is the lower one an which one corresponds to the upper limit.
 
         :return: A tuple containing the minimum and maximum electrode potentials.
         :rtype: tuple
         """
         return (self._Emin, self._Emax)
 
     @electrode_potentials.setter
-    def electrode_potentials(self, value : tuple):
+    def electrode_potentials(self, value: tuple):
         """Set the electrode potential range of the system.
 
         :param value: A tuple containing the minimum and maximum electrode potentials.
         :type value: tuple
         :return: None
         :rtype: None
         """
@@ -303,80 +323,83 @@
 
         :return: Minimum electrode potential value in volts vs. SHE.
         :rtype: float
         """
         return self._Emin
 
     @Emin.setter
-    def Emin(self, value : float):
+    def Emin(self, value: float):
         """Validates the user-input lower potential limit.  If input
         is numerical, `-2.00` otherwise.
 
         :param value: Minimum electrode potential value in volts vs. SHE.
         :type value: float
         :return: None
         :rtype: None
         """
-        if not isinstance(value, (int,float)):
-            warnings.warn(f'Lower potential limit provided not a numerical input. It will be reset to {Defaults.minimum_electrode_potenital}')
+        if not isinstance(value, (int, float)):
+            warnings.warn(
+                f"Lower potential limit provided not a numerical input. It will be reset to {Defaults.minimum_electrode_potenital}"
+            )
             self._Emin = Defaults.minimum_electrode_potenital
         else:
             self._Emin = value
-            
 
     @property
     def Emax(self):
         """Get the maximum electrode potential value of the system.
 
         :return: Maximum electrode potential value in volts vs. SHE.
         :rtype: float
         """
         return self._Emax
 
     @Emax.setter
-    def Emax(self, value : float):
+    def Emax(self, value: float):
         """Validates the user-input upper potential limit. If input is
         numericla, `2.00` otherwise.
 
         :param value: Maximum electrode potential value in volts vs. SHE.
         :type value: float
         :return: None
         :rtype: None
         """
-        if not isinstance(value, (int,float)):
-            warnings.warn(f'Upper potential limit provided not a numerical input. It will be reset to {Defaults.maximum_electrode_potential}')
+        if not isinstance(value, (int, float)):
+            warnings.warn(
+                f"Upper potential limit provided not a numerical input. It will be reset to {Defaults.maximum_electrode_potential}"
+            )
             self._Emax = Defaults.maximum_electrode_potential
         else:
             self._Emax = value
 
     @property
     def reference_electrode(self):
         """Get the reference electrode information.
 
         :return: A tuple containing the reference electrode abbreviation and potential difference.
         :rtype: tuple
         """
         return (self.reference_abbreviation, self.deltaE)
 
     @reference_electrode.setter
-    def reference_electrode(self, value : tuple):
+    def reference_electrode(self, value: tuple):
         """Validates the user-input reference electrode information.
 
         :param value: A tuple containing the reference electrode abbreviation and potential difference.
         :type value: tuple
         :return: None
         :rtype: None
         """
         abbreviation, dE = value
         self._reference_abbreviation = abbreviation
         if abbreviation in Defaults.reference_electrodes.keys():
             self._deltaE = Defaults.reference_electrodes[abbreviation]
         else:
             self._deltaE = dE
-    
+
     @property
     def reference_abbreviation(self):
         """Get the abbreviation of the reference electrode.
 
         :return: Abbreviation of the reference electrode.
         :rtype: str
         """
@@ -386,157 +409,170 @@
     def deltaE(self):
         """Get the potential difference of the reference electrode in volts vs. the standard hydrogen electrode.
 
         :return: Potential difference in volts.
         :rtype: float
         """
         return self._deltaE
-    
-    def add_elements(self, elements : list):
+
+    def add_elements(self, elements: list):
         """Adds elements to the chemical system.
 
         :param elements: List of chemical elements in the system.
         :type elements: list
         """
         self._get_elements(elements)
 
-
     @singledispatchmethod
     def add_reactions(self, reactions):
-        raise NotImplementedError("The reactions type can be either list of dict() or string")
+        raise NotImplementedError(
+            "The reactions type can be either list of dict() or string"
+        )
 
     @add_reactions.register(list)
-    def _(self, reactions : list):
+    def _(self, reactions: list):
         """Adds reactions to the chemical system.
 
         :param reactions: List of chemical reactions in the system.
         :type reactions: list
         """
         self._get_reactions(reactions)
-        
+
     @add_reactions.register(tuple)
-    def _(self, reactions : tuple):
+    def _(self, reactions: tuple):
         reactions = self.db.add_reactions(reactions)
         self._get_reactions(reactions)
 
-    def read_reactions_from_file(self, filename : str):
+    def read_reactions_from_file(self, filename: str):
         """Reads the reactions from a file and adds reactions to the
         chemical system
 
         :param filename: filename with reactions
         :type filename: str
         """
-        with open(filename, 'r', encoding='utf-8') as f:
+        with open(filename, "r", encoding="utf-8") as f:
             lines = f.read().splitlines()
         self.add_reactions(tuple(lines))
 
-    def set_aqueous_activity(self, element : str, activity : float):
-
+    def set_aqueous_activity(self, element: str, activity: float):
         """Modifies the aqueous activity of singular elements previously defined to be included in the chemical system.
 
         :param element: Chemical element in the system.
         :type element: str
         :param activity: Chemical activity of `element`.
         :type activity: float
         """
         self._set_aqueous_activity(element, activity)
-    
+
     def _get_elements(self, elements):
         """Validates the user-input list of chemical elements and updates the dictionary in system_parameters.json to include a dictionary of elements together with their aqueous activities.
 
         :param elements: List of chemical elements in the system.
         :type elements: list
         :raises ValueError: Error raised if the list of elements provided contains entries that are not in `element_list` of know and supported elements.
         :return: Dictionary of validated elements as keys and standard aqueous activities as values.
         :rtype: dict
         """
         for i in elements:
             try:
                 i in element_list
             except ValueError:
-                print(f"Chemical element '{i}' is not in the list of elements added to the reactive system.")
-            
+                print(
+                    f"Chemical element '{i}' is not in the list of elements added to the reactive system."
+                )
+
         # Adding the elements hydrogen (H) and oxygen (O) to element_list since they always have to be present to generate an aqueous Pourbaix diagram.
         elements.append("H")
         elements.append("O")
         for i in set(elements):
             self.elements.update({i: Defaults.activity})
 
-    def construct_reactions_from_reactants(self, reactants : dict):
+    def construct_reactions_from_reactants(self, reactants: dict):
         """Validates the user-input reactants and constructs reactions from reactants from a dictionary containing the reactants and their corresponding activities.
 
         :param reactants: A dictionary of reactants (species) as keys and their corresponding activities as values.
         :type reactants: dict
         :return: A Reaction object created based on the provided reactants and activities.
         :rtype: Reaction
         :raises ValueError: If any reactant contains elements not yet added to the system.
         """
         constituent_dict = {}
         for j in reactants.keys():
             for k in j.atoms.keys():
                 if k != "e" and k not in self.elements:
-                    raise ValueError("Reactions added to the system feature elements that are not yet added to the system yet. Please add them using add_elements().")
+                    raise ValueError(
+                        "Reactions added to the system feature elements that are not yet added to the system yet. Please add them using add_elements()."
+                    )
             if j.state == State.aqueous.value:
-                component_activity = [Defaults.activity]    
+                component_activity = [Defaults.activity]
                 for k in j.atoms.keys():
                     if k != "H" or k != "O" or k != "e":
                         component_activity.append(self.elements[k])
                 activity = min(component_activity)
             else:
                 activity = Defaults.activity
-            constituent_dict.update({j: [reactants[j], activity] })
+            constituent_dict.update({j: [reactants[j], activity]})
 
         return Reaction(constituent_dict, self)
 
     def _get_reactions(self, reactions):
         """Validates the user-input list of chemical reactions to appear on the Pourbaix diagram.
 
         :param reactions: List of chemical reactions in the system.
         :type reactions: list
         :raises ValueError: Error raised if list entries are not in the form of a dictionary. Further error validation upon creating the reaction() object from each entry provided.
         :return: List of chemical reaction objects featuring the systems potential and pH limits as well as the temperature and pressure.
         :rtype: list
         """
         for i in reactions:
             if type(i) != dict:
-                raise ValueError("Reactions added to the system must be a dictionary of the reactants, their stoichiometric coefficients and activities.")
+                raise ValueError(
+                    "Reactions added to the system must be a dictionary of the reactants, their stoichiometric coefficients and activities."
+                )
             constituent_dict = {}
             for j in i.keys():
                 for k in j.atoms.keys():
                     if k != "e" and k not in self.elements:
-                        raise ValueError("Reactions added to the system feature elements that are not yet added to the system yet. Please add them using add_elements().")
+                        raise ValueError(
+                            "Reactions added to the system feature elements that are not yet added to the system yet. Please add them using add_elements()."
+                        )
                 if j.state == State.aqueous.value:
-                    component_activity = [Defaults.activity]    
+                    component_activity = [Defaults.activity]
                     for k in j.atoms.keys():
                         if k != "H" or k != "O" or k != "e":
                             component_activity.append(self.elements[k])
                         activity = min(component_activity)
                 else:
                     activity = Defaults.activity
-                
-                constituent_dict.update({j:[i[j], activity]})
+
+                constituent_dict.update({j: [i[j], activity]})
 
             new_reaction = Reaction(constituent_dict, self)
             self.reactions.append(new_reaction)
 
-
-    def _set_aqueous_activity(self, element : str, activity : float) -> dict:
+    def _set_aqueous_activity(self, element: str, activity: float) -> dict:
         """Validates the user-input element and corresponding chemical activity and updates the dictionary in system_parameters.json.
 
         :param element: Chemical element whose activity is modified.
         :type element: str
         :param activity: Chemical activity of the element.
         :type activity: float
         :raises ValueError: Error raised if element provided is not part of the chemical system.
         :return: Dictionary of elements as keys and updated standard aqueous activities as values.
         :rtype: dict
         """
-        
+
         if element not in self.elements:
-            raise ValueError("Chemical element provided not is the list of chemical elements in the system.")
-        if not isinstance(activity,(int,float)):
-            warnings.warn(f'Chemical activity provided is not numerical. It will be reset to {Defaults.activity}')
+            raise ValueError(
+                "Chemical element provided not is the list of chemical elements in the system."
+            )
+        if not isinstance(activity, (int, float)):
+            warnings.warn(
+                f"Chemical activity provided is not numerical. It will be reset to {Defaults.activity}"
+            )
             activity = Defaults.activity
         if activity < 0:
-            warnings.warn(f'Chemical activity provided is negative. It will be reset to {Defaults.activity}')
+            warnings.warn(
+                f"Chemical activity provided is negative. It will be reset to {Defaults.activity}"
+            )
             activity = Defaults.activity
         self.elements.update({element: activity})
```

### Comparing `PourPy-1.0.0/PourPy.egg-info/PKG-INFO` & `pourpy-1.1.0/PourPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PourPy
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python-based library to generate Pourbaix diagrams (potential/pH diagram)
 Home-page: https://gitlab.com/cmbm-ethz/pourbaix-diagrams
 Author: Fabio Furcas, Anja Korber, Mohit Pundir
 Author-email: Mohit Pundir <mpundir@ethz.ch>, "Fabio E. Furcas" <ffurcas@ethz.ch>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -685,22 +685,23 @@
 Keywords: potential-diagram,pourbaix,chemical
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argparse
-Requires-Dist: pytest
 Requires-Dist: bokeh
 Requires-Dist: matplotlib
 Requires-Dist: shapely
 Requires-Dist: nbsphinx
 Requires-Dist: sphinx-autoapi
 Requires-Dist: sphinx_rtd_theme
 Requires-Dist: tomli; python_version < "3.11"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 PourPy
 =============
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/cmbm-ethz%2Fpourbaix-diagrams/main?labpath=.%2Fexamples%2Fnotebooks%2Firon.ipynb)
 	
 A Python-based library to generate Pourbaix diagrams (potential/pH
 diagram). **PourPy** is an open-source python package,
@@ -729,26 +730,43 @@
 - nbsphinx
 - sphinx-autoapi
 - sphinx_rtd_theme
 
 
 Installation
 ===============
+Install the latest release from the Package repository:
+```
+pip install PourPy
+```
 
 Documentation
 =================
 The latest documentation is available on
 [readthedocs](https://readthedocs.org/). Please refer to the
 documentation on how to use the PourPy package:
 [pourbaix-diagrams.rtfd.io](https://pourbaix-diagrams.readthedocs.io/en/latest/)
 
+Webapp
+======
+PourPy is also available as a webapp with all the functionalities [PourPy Weabpp](https://pourpy-webapp.runmercury.com/app/pourpy-mercury)
+
 
 Examples
 ==========
-
 For live and interacting examples mentioned in the documentation, please check the following link:
 [Interactive examples](https://mybinder.org/v2/gl/cmbm-ethz%2Fpourbaix-diagrams/a20c113396cf23bf1b642c8ccdacc74124a3db5f?urlpath=lab%2Ftree%2Fexamples%2Fnotebooks%2Firon.ipynb)
 
+Contributing
+============
+Contributions to PourPy are welcome! Please follow the guidelines below.
+
+Report an issue
+If you have an account on [gitlab](https://gitlab.com/), you can submit an issue.
+
+Submit a patch / merge-request
+Follow this [guide](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html#new-merge-request-from-a-fork) to create a merge request on GitLab. Please target the repository's `main` branch.
+
 License
 =========
-PyPourbaix is distributed under the terms of [GNU LGPL v3](https://www.gnu.org/licenses/lgpl-3.0.en.html)
+PourPy is distributed under the terms of [GNU LGPL v3](https://www.gnu.org/licenses/lgpl-3.0.en.html)
```

### Comparing `PourPy-1.0.0/README.md` & `pourpy-1.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -29,26 +29,43 @@
 - nbsphinx
 - sphinx-autoapi
 - sphinx_rtd_theme
 
 
 Installation
 ===============
+Install the latest release from the Package repository:
+```
+pip install PourPy
+```
 
 Documentation
 =================
 The latest documentation is available on
 [readthedocs](https://readthedocs.org/). Please refer to the
 documentation on how to use the PourPy package:
 [pourbaix-diagrams.rtfd.io](https://pourbaix-diagrams.readthedocs.io/en/latest/)
 
+Webapp
+======
+PourPy is also available as a webapp with all the functionalities [PourPy Weabpp](https://pourpy-webapp.runmercury.com/app/pourpy-mercury)
+
 
 Examples
 ==========
-
 For live and interacting examples mentioned in the documentation, please check the following link:
 [Interactive examples](https://mybinder.org/v2/gl/cmbm-ethz%2Fpourbaix-diagrams/a20c113396cf23bf1b642c8ccdacc74124a3db5f?urlpath=lab%2Ftree%2Fexamples%2Fnotebooks%2Firon.ipynb)
 
+Contributing
+============
+Contributions to PourPy are welcome! Please follow the guidelines below.
+
+Report an issue
+If you have an account on [gitlab](https://gitlab.com/), you can submit an issue.
+
+Submit a patch / merge-request
+Follow this [guide](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html#new-merge-request-from-a-fork) to create a merge request on GitLab. Please target the repository's `main` branch.
+
 License
 =========
-PyPourbaix is distributed under the terms of [GNU LGPL v3](https://www.gnu.org/licenses/lgpl-3.0.en.html)
+PourPy is distributed under the terms of [GNU LGPL v3](https://www.gnu.org/licenses/lgpl-3.0.en.html)
```

### Comparing `PourPy-1.0.0/pyproject.toml` & `pourpy-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # pyproject.toml
 
 [build-system]
-requires = ["setuptools"]
+requires = ["setuptools", "wheel"]  # PEP 508 specification
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "PourPy"
-version = "1.0.0"
-authors = [
+version = "1.1.0"
+authors = [ 
   { name="Mohit Pundir", email="mpundir@ethz.ch" },
   { name="Fabio E. Furcas", email="ffurcas@ethz.ch"},
 ]
 
 description = "A Python-based library to generate Pourbaix diagrams (potential/pH diagram)"
 
 readme = { file = "README.md", content-type = "text/markdown" }
@@ -22,25 +22,28 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
 ]
 
 keywords = ["potential-diagram", "pourbaix", "chemical"]
 
+
+requires-python = ">=3.8"
+
 dependencies = [
 	  "argparse",
-          "pytest",
           "bokeh",
           "matplotlib",
           "shapely",
           "nbsphinx",
           "sphinx-autoapi",
           "sphinx_rtd_theme",
 	  'tomli; python_version < "3.11"',
 ]
 
-requires-python = ">=3.8"
+[project.optional-dependencies]
+test = ["pytest"]
 
 
 [project.urls]
 Homepage = "https://gitlab.com/cmbm-ethz/pourbaix-diagrams"
 Issues = "https://gitlab.com/cmbm-ethz/pourbaix-diagrams/issues"
```

### Comparing `PourPy-1.0.0/setup.py` & `pourpy-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='PourPy',
-      version='0.1',
+      version='1.1.0',
       description='A Python package for generating potential/pH diagrams',
       url='https://gitlab.com/cmbm-ethz/pourbaix-diagrams',
       author='Fabio Furcas, Anja Korber, Mohit Pundir',
       author_email='mpundir@ethz.ch',
       license='GNU LGPL v3',
       packages=['PourPy'],
       install_requires=[
```

