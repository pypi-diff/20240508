# Comparing `tmp/ft2bt-0.1.3.tar.gz` & `tmp/ft2bt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ft2bt-0.1.3.tar", last modified: Tue Apr  2 10:28:10 2024, max compression
+gzip compressed data, was "ft2bt-0.2.0.tar", last modified: Wed May  8 15:58:25 2024, max compression
```

## Comparing `ft2bt-0.1.3.tar` & `ft2bt-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-02 10:28:10.112641 ft2bt-0.1.3/
--rw-rw-r--   0 tda       (1000) tda       (1000)    35148 2024-04-02 10:18:35.000000 ft2bt-0.1.3/LICENSE
--rw-r--r--   0 tda       (1000) tda       (1000)     4640 2024-04-02 10:28:10.112641 ft2bt-0.1.3/PKG-INFO
--rw-rw-r--   0 tda       (1000) tda       (1000)     4034 2024-04-02 10:20:23.000000 ft2bt-0.1.3/README.md
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-02 10:28:10.108641 ft2bt-0.1.3/ft2bt/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-02 10:18:35.000000 ft2bt-0.1.3/ft2bt/__init__.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-02 10:28:10.108641 ft2bt-0.1.3/ft2bt/scripts/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-02 10:18:35.000000 ft2bt-0.1.3/ft2bt/scripts/__init__.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-02 10:28:10.112641 ft2bt-0.1.3/ft2bt/scripts/behavior_trees/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-02 10:18:35.000000 ft2bt-0.1.3/ft2bt/scripts/behavior_trees/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)    11665 2024-04-02 10:18:35.000000 ft2bt-0.1.3/ft2bt/scripts/behavior_trees/behavior_tree.py
--rw-rw-r--   0 tda       (1000) tda       (1000)      313 2024-04-02 10:18:35.000000 ft2bt-0.1.3/ft2bt/scripts/behavior_trees/behavior_tree_node.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-02 10:28:10.112641 ft2bt-0.1.3/ft2bt/scripts/code_generator/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-02 10:18:35.000000 ft2bt-0.1.3/ft2bt/scripts/code_generator/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     9283 2024-04-02 10:18:35.000000 ft2bt-0.1.3/ft2bt/scripts/code_generator/code_generator.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     2316 2024-04-02 10:18:35.000000 ft2bt-0.1.3/ft2bt/scripts/code_generator/header_file.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     2891 2024-04-02 10:18:35.000000 ft2bt-0.1.3/ft2bt/scripts/code_generator/main_file.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     3417 2024-04-02 10:18:35.000000 ft2bt-0.1.3/ft2bt/scripts/code_generator/source_file.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-02 10:28:10.112641 ft2bt-0.1.3/ft2bt/scripts/fault_trees/
--rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-02 10:18:35.000000 ft2bt-0.1.3/ft2bt/scripts/fault_trees/__init__.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     7623 2024-04-02 10:18:35.000000 ft2bt-0.1.3/ft2bt/scripts/fault_trees/xml_fta_parser.py
--rw-rw-r--   0 tda       (1000) tda       (1000)     2553 2024-04-02 10:18:35.000000 ft2bt-0.1.3/ft2bt/scripts/ft2bt.py
-drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-04-02 10:28:10.112641 ft2bt-0.1.3/ft2bt.egg-info/
--rw-r--r--   0 tda       (1000) tda       (1000)     4640 2024-04-02 10:28:10.000000 ft2bt-0.1.3/ft2bt.egg-info/PKG-INFO
--rw-rw-r--   0 tda       (1000) tda       (1000)      707 2024-04-02 10:28:10.000000 ft2bt-0.1.3/ft2bt.egg-info/SOURCES.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)        1 2024-04-02 10:28:10.000000 ft2bt-0.1.3/ft2bt.egg-info/dependency_links.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)       51 2024-04-02 10:28:10.000000 ft2bt-0.1.3/ft2bt.egg-info/entry_points.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)       51 2024-04-02 10:28:10.000000 ft2bt-0.1.3/ft2bt.egg-info/requires.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)        6 2024-04-02 10:28:10.000000 ft2bt-0.1.3/ft2bt.egg-info/top_level.txt
--rw-rw-r--   0 tda       (1000) tda       (1000)       38 2024-04-02 10:28:10.112641 ft2bt-0.1.3/setup.cfg
--rw-rw-r--   0 tda       (1000) tda       (1000)      980 2024-04-02 10:25:50.000000 ft2bt-0.1.3/setup.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-08 15:58:25.428395 ft2bt-0.2.0/
+-rw-rw-r--   0 tda       (1000) tda       (1000)    35148 2024-04-06 09:05:53.000000 ft2bt-0.2.0/LICENSE
+-rw-rw-r--   0 tda       (1000) tda       (1000)       24 2024-05-08 15:55:27.000000 ft2bt-0.2.0/MANIFEST.in
+-rw-r--r--   0 tda       (1000) tda       (1000)     5282 2024-05-08 15:58:25.428395 ft2bt-0.2.0/PKG-INFO
+-rw-rw-r--   0 tda       (1000) tda       (1000)     4676 2024-05-08 12:26:20.000000 ft2bt-0.2.0/README.md
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-08 15:58:25.428395 ft2bt-0.2.0/ft2bt/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.0/ft2bt/__init__.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-08 15:58:25.428395 ft2bt-0.2.0/ft2bt/scripts/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.0/ft2bt/scripts/__init__.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-08 15:58:25.428395 ft2bt-0.2.0/ft2bt/scripts/behavior_trees/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.0/ft2bt/scripts/behavior_trees/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)    21197 2024-04-25 13:52:26.000000 ft2bt-0.2.0/ft2bt/scripts/behavior_trees/behavior_tree.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)      418 2024-04-11 05:51:28.000000 ft2bt-0.2.0/ft2bt/scripts/behavior_trees/behavior_tree_node.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-08 15:58:25.428395 ft2bt-0.2.0/ft2bt/scripts/code_generator/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.0/ft2bt/scripts/code_generator/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     9283 2024-04-06 09:05:53.000000 ft2bt-0.2.0/ft2bt/scripts/code_generator/code_generator.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     2316 2024-04-06 09:05:53.000000 ft2bt-0.2.0/ft2bt/scripts/code_generator/header_file.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     2891 2024-04-06 09:05:53.000000 ft2bt-0.2.0/ft2bt/scripts/code_generator/main_file.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     3417 2024-04-06 09:05:53.000000 ft2bt-0.2.0/ft2bt/scripts/code_generator/source_file.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-08 15:58:25.428395 ft2bt-0.2.0/ft2bt/scripts/fault_trees/
+-rw-rw-r--   0 tda       (1000) tda       (1000)        0 2024-04-06 09:05:53.000000 ft2bt-0.2.0/ft2bt/scripts/fault_trees/__init__.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)    10354 2024-04-09 06:16:12.000000 ft2bt-0.2.0/ft2bt/scripts/fault_trees/xml_fta_parser.py
+-rw-rw-r--   0 tda       (1000) tda       (1000)     3962 2024-04-25 13:51:47.000000 ft2bt-0.2.0/ft2bt/scripts/ft2bt.py
+drwxrwxr-x   0 tda       (1000) tda       (1000)        0 2024-05-08 15:58:25.428395 ft2bt-0.2.0/ft2bt.egg-info/
+-rw-r--r--   0 tda       (1000) tda       (1000)     5282 2024-05-08 15:58:25.000000 ft2bt-0.2.0/ft2bt.egg-info/PKG-INFO
+-rw-rw-r--   0 tda       (1000) tda       (1000)      736 2024-05-08 15:58:25.000000 ft2bt-0.2.0/ft2bt.egg-info/SOURCES.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)        1 2024-05-08 15:58:25.000000 ft2bt-0.2.0/ft2bt.egg-info/dependency_links.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)       51 2024-05-08 15:58:25.000000 ft2bt-0.2.0/ft2bt.egg-info/entry_points.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)       51 2024-05-08 15:58:25.000000 ft2bt-0.2.0/ft2bt.egg-info/requires.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)        6 2024-05-08 15:58:25.000000 ft2bt-0.2.0/ft2bt.egg-info/top_level.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)       51 2024-05-08 15:42:53.000000 ft2bt-0.2.0/requirements.txt
+-rw-rw-r--   0 tda       (1000) tda       (1000)       38 2024-05-08 15:58:25.428395 ft2bt-0.2.0/setup.cfg
+-rw-rw-r--   0 tda       (1000) tda       (1000)      980 2024-05-08 15:56:14.000000 ft2bt-0.2.0/setup.py
```

### Comparing `ft2bt-0.1.3/LICENSE` & `ft2bt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ft2bt-0.1.3/PKG-INFO` & `ft2bt-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft2bt
-Version: 0.1.3
+Version: 0.2.0
 Summary: Automatic conversion from fault trees into behavior trees
 Home-page: https://github.com/cconejob/ft2bt_converter.git
 Author: Carlos Conejo
 Author-email: carlos.conejo@upc.edu
 License: GNU GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -37,46 +37,56 @@
 ### Preparing Your Fault Tree Diagram
 
 1. **Create or Open Your Fault Tree Diagram in Draw.io**:
     * First, visit [draw.io](https://draw.io/) to create or edit your fault tree diagram. You may refer to their [documentation](https://www.drawio.com/doc/) for guidance on using the tool.
 2. **Diagram Structure & Symbols**:
     * **Hazards**: Represent hazards using rectangles. This is a required element in your diagram.
     * **Events**: Depict events using circles. These are also required elements.
-    * **Actions**: Actions can be represented by processes. Including actions is optional but helpful to clarify how the hazard should be handled.
     * **AND/OR Gates**: Use the respective symbols for AND/OR gates in your diagram. These are required for depicting logical relationships in the fault tree.
+    * **Probabilities**: Use text below the events to indicate the correspondent probability. Example: `p = 0.1`. These elements are not required.
 3. **Exporting the Diagram as XML**:
     * Once your fault tree diagram is ready, you need to export it in XML format. In draw.io, go to `File` > `Export as` > `XML` to save your diagram as an XML file.
-4. **Save the XML File in the `/fault_trees` Folder**:
-    * After exporting your diagram as an XML file, save it in the `/fault_trees` folder within the project directory.
 
-**Warning!**: All the fault tree elements need to be connected by directional arrows. Ensure that all of them are physically attached to their related elements.
+<p align="center">
+  <img src="ft2bt/test/fault_trees/fta_example.png" alt="Fault Tree Example">
+</p>
 
-### Input Example: Fault Tree Diagram
+**Warning!**: All fault tree elements, with the exception of text probabilities, should be connected by directional arrows. Ensure that each arrow is physically attached to its corresponding elements to maintain clarity and accuracy in the diagram.
 
-Below is an example of a fault tree diagram generated in a Draw.io file:
+### Preparing Your Hazard Analysis and Risk Assessment (Opitonal)
+
+Create a *.csv file with some required column names:
+
+1. **Item_ID**: Identificator of the Item analyzed.
+2. **Hazard_ID**:  Identificator of the possible Hazard. The ID must match with the name of the correspondent Hazard in the Fault Tree.
+3. **Operating_Scenario_ID**: Identificator of the Operating Scenario.
+4. **ASIL**: Automotive Safety Integrity Level. Options: A, B, C, D
+5. **Safety_State_ID**: Identificator of the Safety State action.
 
 <p align="center">
-  <img src="ft2bt/test/fault_trees/fta_example.png" alt="Fault Tree Example">
+  <img src="ft2bt/test/hara/hara_example.png" alt="Fault Tree Example">
 </p>
 
 ### Running the Conversion Tool
 
 Run the conversion command:
 
 ```bash
-ft2bt [-h] -f FTA_FILENAME [-v] [-c] [-r] [-o]
+ft2bt [-h] -f FTA_FILEPATH [-v] [-c] [-r] [-o OUTPUT_FOLDER] [-p] [-H HARA_FILEPATH]
 ```
 
 Where:
 
 * **-f**: (Required) Specifies the XML global filepath name of the draw.io diagram.
 * **-v**: (Optional) Automatically shows and saves the renders. Defaults to false.
 * **-c**: (Optional) Generate a cpp ROS node template for the behavior tree. Defaults to false.
 * **-r**: (Optional) Replaces current code if previously generated and -c is set to True.
 * **-o**: (Optional) Specifies the global folder path, where the behavior tree XML diagram is saved.
+* **-p**: (Optional) Probabilities are considered to sort the behavior tree nodes.
+* **-H**: (Optional) Specifies the CSV global file name of the Hazard Analysis and Risk Assessment (HARA).
 
 ### Output Example: Behavior Tree Diagram
 
 Below is an example of the behavior tree diagrams generated from the fault tree. The XML file is loaded using [Groot](https://github.com/BehaviorTree/Groot):
 
 The order of the events is randomly selected in this version of the software. Future versions will sort the events by probability of occurrence.
```

### Comparing `ft2bt-0.1.3/README.md` & `ft2bt-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -19,46 +19,56 @@
 ### Preparing Your Fault Tree Diagram
 
 1. **Create or Open Your Fault Tree Diagram in Draw.io**:
     * First, visit [draw.io](https://draw.io/) to create or edit your fault tree diagram. You may refer to their [documentation](https://www.drawio.com/doc/) for guidance on using the tool.
 2. **Diagram Structure & Symbols**:
     * **Hazards**: Represent hazards using rectangles. This is a required element in your diagram.
     * **Events**: Depict events using circles. These are also required elements.
-    * **Actions**: Actions can be represented by processes. Including actions is optional but helpful to clarify how the hazard should be handled.
     * **AND/OR Gates**: Use the respective symbols for AND/OR gates in your diagram. These are required for depicting logical relationships in the fault tree.
+    * **Probabilities**: Use text below the events to indicate the correspondent probability. Example: `p = 0.1`. These elements are not required.
 3. **Exporting the Diagram as XML**:
     * Once your fault tree diagram is ready, you need to export it in XML format. In draw.io, go to `File` > `Export as` > `XML` to save your diagram as an XML file.
-4. **Save the XML File in the `/fault_trees` Folder**:
-    * After exporting your diagram as an XML file, save it in the `/fault_trees` folder within the project directory.
 
-**Warning!**: All the fault tree elements need to be connected by directional arrows. Ensure that all of them are physically attached to their related elements.
+<p align="center">
+  <img src="ft2bt/test/fault_trees/fta_example.png" alt="Fault Tree Example">
+</p>
 
-### Input Example: Fault Tree Diagram
+**Warning!**: All fault tree elements, with the exception of text probabilities, should be connected by directional arrows. Ensure that each arrow is physically attached to its corresponding elements to maintain clarity and accuracy in the diagram.
 
-Below is an example of a fault tree diagram generated in a Draw.io file:
+### Preparing Your Hazard Analysis and Risk Assessment (Opitonal)
+
+Create a *.csv file with some required column names:
+
+1. **Item_ID**: Identificator of the Item analyzed.
+2. **Hazard_ID**:  Identificator of the possible Hazard. The ID must match with the name of the correspondent Hazard in the Fault Tree.
+3. **Operating_Scenario_ID**: Identificator of the Operating Scenario.
+4. **ASIL**: Automotive Safety Integrity Level. Options: A, B, C, D
+5. **Safety_State_ID**: Identificator of the Safety State action.
 
 <p align="center">
-  <img src="ft2bt/test/fault_trees/fta_example.png" alt="Fault Tree Example">
+  <img src="ft2bt/test/hara/hara_example.png" alt="Fault Tree Example">
 </p>
 
 ### Running the Conversion Tool
 
 Run the conversion command:
 
 ```bash
-ft2bt [-h] -f FTA_FILENAME [-v] [-c] [-r] [-o]
+ft2bt [-h] -f FTA_FILEPATH [-v] [-c] [-r] [-o OUTPUT_FOLDER] [-p] [-H HARA_FILEPATH]
 ```
 
 Where:
 
 * **-f**: (Required) Specifies the XML global filepath name of the draw.io diagram.
 * **-v**: (Optional) Automatically shows and saves the renders. Defaults to false.
 * **-c**: (Optional) Generate a cpp ROS node template for the behavior tree. Defaults to false.
 * **-r**: (Optional) Replaces current code if previously generated and -c is set to True.
 * **-o**: (Optional) Specifies the global folder path, where the behavior tree XML diagram is saved.
+* **-p**: (Optional) Probabilities are considered to sort the behavior tree nodes.
+* **-H**: (Optional) Specifies the CSV global file name of the Hazard Analysis and Risk Assessment (HARA).
 
 ### Output Example: Behavior Tree Diagram
 
 Below is an example of the behavior tree diagrams generated from the fault tree. The XML file is loaded using [Groot](https://github.com/BehaviorTree/Groot):
 
 The order of the events is randomly selected in this version of the software. Future versions will sort the events by probability of occurrence.
```

### Comparing `ft2bt-0.1.3/ft2bt/scripts/code_generator/code_generator.py` & `ft2bt-0.2.0/ft2bt/scripts/code_generator/code_generator.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.1.3/ft2bt/scripts/code_generator/header_file.py` & `ft2bt-0.2.0/ft2bt/scripts/code_generator/header_file.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.1.3/ft2bt/scripts/code_generator/main_file.py` & `ft2bt-0.2.0/ft2bt/scripts/code_generator/main_file.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.1.3/ft2bt/scripts/code_generator/source_file.py` & `ft2bt-0.2.0/ft2bt/scripts/code_generator/source_file.py`

 * *Files identical despite different names*

### Comparing `ft2bt-0.1.3/ft2bt/scripts/ft2bt.py` & `ft2bt-0.2.0/ft2bt/scripts/ft2bt.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,59 +1,84 @@
 import argparse
 from pathlib import Path
 
 from ft2bt.scripts.fault_trees.xml_fta_parser import XMLFTAParser
 from ft2bt.scripts.behavior_trees.behavior_tree import BehaviorTree
 from ft2bt.scripts.code_generator.code_generator import CodeGenerator
+from ft2bt.scripts.hara.hara_parser import HARAParser
 
 
 def main():  
     parser = argparse.ArgumentParser(description='Convert xml file from drawio to behavior tree xml file for Groot.')
     
     # Limit coordinates
     parser.add_argument('-f', '--fta_filepath', type=str, help="*.xml fault tree global path", required=True)
     parser.add_argument('-v', '--view', action='store_true', help="View the behavior tree renders?")
     parser.add_argument('-c', '--generate_cpp', action='store_true', help="Generate C++ code template?")
     parser.add_argument('-r', '--replace', action='store_true', help="Replace existing files?")
     parser.add_argument('-o', '--output_folder', type=str, help="Output folder for the behavior trees.")
+    parser.add_argument('-p', '--probabilistic', action='store_true', help="Generate probabilistic behavior trees.")
+    parser.add_argument('-H', '--HARA_filepath', type=str, help="*.csv HARA file global path.", default=None, required=False)
     args = parser.parse_args()
     
     # Get the path to the package
     module_path = Path(__file__).resolve()
     package_path = module_path.parent.parent.parent
+    hara_available = args.HARA_filepath is not None
     
     # Add the .xml extension if it is not present
     if not args.fta_filepath.endswith('.xml'):
         args.fta_filepath += '.xml'
         print('.xml extension not found in the file path.')
         print(f'Added .xml extension to the file path: {args.fta_filepath}')
     
     # Generate the fault tree diagram from the XML file
     fta_filename = Path(args.fta_filepath).stem
-    fta_parser = XMLFTAParser(xml_file=args.fta_filepath)
+    fta_parser = XMLFTAParser(xml_file=args.fta_filepath, probabilistic=args.probabilistic)
     fta_list = fta_parser.generate_fault_trees(plot=args.view)
 
     # Initialize the behavior tree and code generator objects
-    prev_bt = BehaviorTree(name='prev')
+    prev_bt = None
     code_generator = CodeGenerator(replace=args.replace, filename=fta_filename.lower())
     
     # Create the folder for the behavior trees
     if args.output_folder:
         behavior_tree_folder = args.output_folder
     else:
         behavior_tree_folder = package_path / 'behavior_trees'
+        
+    # Read the HARA CSV file if it is provided
+    if hara_available:
+        hara_generator = HARAParser(hara_file=args.HARA_filepath)
+        for item_id, hazard_dict in hara_generator.hara_dict.items():
+            bt_hara = BehaviorTree(name=item_id, probabilistic=args.probabilistic)
+            bt_hara.generate_from_hara(hazard_dict)
     
-    # Generate the behavior tree diagram from every fault tree diagram
     for fta in fta_list:
-        bt = BehaviorTree(name=fta.name)
+        # Generate the behavior tree diagram from every fault tree diagram
+        bt = BehaviorTree(name=fta.name, probabilistic=args.probabilistic)
+        if prev_bt is None:
+            prev_bt = bt
         bt.event_number = prev_bt.event_number
-        bt.action_number = prev_bt.action_number
+        if args.probabilistic:
+            bt.node_probabilities = fta_parser.node_probabilities
         bt.generate_from_fault_tree(fta)
         bt.generate_xml_file(folder_name=behavior_tree_folder, view=args.view)
         
-        if args.generate_cpp:
+        # Attach the singular hazard detection nodes to the HARA behavior tree
+        if hara_available:
+            bt_hara.attach_hazard_detection(bt, hara_generator.hara_dict)
+
+        # Generate the C++ code template for the behavior tree if the flag is set
+        if args.generate_cpp and not hara_available:
             code_generator.generate_main_cpp_file(xml_file_path=bt.xml_file_path, bt_name=bt.name)
+            
         prev_bt = bt
-    
+        
+    if hara_available:
+        bt_hara.generate_xml_file(folder_name=behavior_tree_folder, view=args.view)
+        if args.generate_cpp:
+            code_generator.generate_main_cpp_file(xml_file_path=bt_hara.xml_file_path, bt_name=bt_hara.name)
+        
 
 if __name__ == "__main__":    
     main()
```

### Comparing `ft2bt-0.1.3/ft2bt.egg-info/PKG-INFO` & `ft2bt-0.2.0/ft2bt.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft2bt
-Version: 0.1.3
+Version: 0.2.0
 Summary: Automatic conversion from fault trees into behavior trees
 Home-page: https://github.com/cconejob/ft2bt_converter.git
 Author: Carlos Conejo
 Author-email: carlos.conejo@upc.edu
 License: GNU GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -37,46 +37,56 @@
 ### Preparing Your Fault Tree Diagram
 
 1. **Create or Open Your Fault Tree Diagram in Draw.io**:
     * First, visit [draw.io](https://draw.io/) to create or edit your fault tree diagram. You may refer to their [documentation](https://www.drawio.com/doc/) for guidance on using the tool.
 2. **Diagram Structure & Symbols**:
     * **Hazards**: Represent hazards using rectangles. This is a required element in your diagram.
     * **Events**: Depict events using circles. These are also required elements.
-    * **Actions**: Actions can be represented by processes. Including actions is optional but helpful to clarify how the hazard should be handled.
     * **AND/OR Gates**: Use the respective symbols for AND/OR gates in your diagram. These are required for depicting logical relationships in the fault tree.
+    * **Probabilities**: Use text below the events to indicate the correspondent probability. Example: `p = 0.1`. These elements are not required.
 3. **Exporting the Diagram as XML**:
     * Once your fault tree diagram is ready, you need to export it in XML format. In draw.io, go to `File` > `Export as` > `XML` to save your diagram as an XML file.
-4. **Save the XML File in the `/fault_trees` Folder**:
-    * After exporting your diagram as an XML file, save it in the `/fault_trees` folder within the project directory.
 
-**Warning!**: All the fault tree elements need to be connected by directional arrows. Ensure that all of them are physically attached to their related elements.
+<p align="center">
+  <img src="ft2bt/test/fault_trees/fta_example.png" alt="Fault Tree Example">
+</p>
 
-### Input Example: Fault Tree Diagram
+**Warning!**: All fault tree elements, with the exception of text probabilities, should be connected by directional arrows. Ensure that each arrow is physically attached to its corresponding elements to maintain clarity and accuracy in the diagram.
 
-Below is an example of a fault tree diagram generated in a Draw.io file:
+### Preparing Your Hazard Analysis and Risk Assessment (Opitonal)
+
+Create a *.csv file with some required column names:
+
+1. **Item_ID**: Identificator of the Item analyzed.
+2. **Hazard_ID**:  Identificator of the possible Hazard. The ID must match with the name of the correspondent Hazard in the Fault Tree.
+3. **Operating_Scenario_ID**: Identificator of the Operating Scenario.
+4. **ASIL**: Automotive Safety Integrity Level. Options: A, B, C, D
+5. **Safety_State_ID**: Identificator of the Safety State action.
 
 <p align="center">
-  <img src="ft2bt/test/fault_trees/fta_example.png" alt="Fault Tree Example">
+  <img src="ft2bt/test/hara/hara_example.png" alt="Fault Tree Example">
 </p>
 
 ### Running the Conversion Tool
 
 Run the conversion command:
 
 ```bash
-ft2bt [-h] -f FTA_FILENAME [-v] [-c] [-r] [-o]
+ft2bt [-h] -f FTA_FILEPATH [-v] [-c] [-r] [-o OUTPUT_FOLDER] [-p] [-H HARA_FILEPATH]
 ```
 
 Where:
 
 * **-f**: (Required) Specifies the XML global filepath name of the draw.io diagram.
 * **-v**: (Optional) Automatically shows and saves the renders. Defaults to false.
 * **-c**: (Optional) Generate a cpp ROS node template for the behavior tree. Defaults to false.
 * **-r**: (Optional) Replaces current code if previously generated and -c is set to True.
 * **-o**: (Optional) Specifies the global folder path, where the behavior tree XML diagram is saved.
+* **-p**: (Optional) Probabilities are considered to sort the behavior tree nodes.
+* **-H**: (Optional) Specifies the CSV global file name of the Hazard Analysis and Risk Assessment (HARA).
 
 ### Output Example: Behavior Tree Diagram
 
 Below is an example of the behavior tree diagrams generated from the fault tree. The XML file is loaded using [Groot](https://github.com/BehaviorTree/Groot):
 
 The order of the events is randomly selected in this version of the software. Future versions will sort the events by probability of occurrence.
```

### Comparing `ft2bt-0.1.3/ft2bt.egg-info/SOURCES.txt` & `ft2bt-0.2.0/ft2bt.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 LICENSE
+MANIFEST.in
 README.md
+requirements.txt
 setup.py
 ft2bt/__init__.py
 ft2bt.egg-info/PKG-INFO
 ft2bt.egg-info/SOURCES.txt
 ft2bt.egg-info/dependency_links.txt
 ft2bt.egg-info/entry_points.txt
 ft2bt.egg-info/requires.txt
```

### Comparing `ft2bt-0.1.3/setup.py` & `ft2bt-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your requirements.txt file
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='ft2bt',
-    version='0.1.3',
+    version='0.2.0',
     packages=find_packages(),
     install_requires=required,  # Use the list from requirements.txt
     entry_points={
         'console_scripts': [
             'ft2bt=ft2bt.scripts.ft2bt:main',
         ],
     },
```

