# Comparing `tmp/molsystem-2024.5.6.tar.gz` & `tmp/molsystem-2024.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molsystem-2024.5.6.tar", last modified: Sun May  5 22:14:56 2024, max compression
+gzip compressed data, was "molsystem-2024.5.8.tar", last modified: Wed May  8 16:45:16 2024, max compression
```

## Comparing `molsystem-2024.5.6.tar` & `molsystem-2024.5.8.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:56.811546 molsystem-2024.5.6/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-05 22:14:43.000000 molsystem-2024.5.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-05 22:14:43.000000 molsystem-2024.5.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-05 22:14:43.000000 molsystem-2024.5.6/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-05 22:14:43.000000 molsystem-2024.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-05 22:14:43.000000 molsystem-2024.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-05-05 22:14:56.807546 molsystem-2024.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-05 22:14:43.000000 molsystem-2024.5.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:56.791546 molsystem-2024.5.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-05 22:14:43.000000 molsystem-2024.5.6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:56.795546 molsystem-2024.5.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-05-05 22:14:43.000000 molsystem-2024.5.6/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-05-05 22:14:43.000000 molsystem-2024.5.6/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-05-05 22:14:43.000000 molsystem-2024.5.6/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-05-05 22:14:43.000000 molsystem-2024.5.6/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-05-05 22:14:43.000000 molsystem-2024.5.6/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-05-05 22:14:43.000000 molsystem-2024.5.6/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:56.795546 molsystem-2024.5.6/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-05 22:14:43.000000 molsystem-2024.5.6/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-05 22:14:43.000000 molsystem-2024.5.6/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     9525 2024-05-05 22:14:43.000000 molsystem-2024.5.6/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:56.795546 molsystem-2024.5.6/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-05 22:14:43.000000 molsystem-2024.5.6/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-05 22:14:43.000000 molsystem-2024.5.6/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-05 22:14:43.000000 molsystem-2024.5.6/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-05 22:14:43.000000 molsystem-2024.5.6/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:56.795546 molsystem-2024.5.6/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-05 22:14:43.000000 molsystem-2024.5.6/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-05 22:14:43.000000 molsystem-2024.5.6/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 22:14:43.000000 molsystem-2024.5.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-05 22:14:43.000000 molsystem-2024.5.6/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:56.795546 molsystem-2024.5.6/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-05 22:14:43.000000 molsystem-2024.5.6/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:56.811546 molsystem-2024.5.6/molsystem/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-05 22:14:56.811546 molsystem-2024.5.6/molsystem/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/align.py
--rw-r--r--   0 runner    (1001) docker     (127)    69805 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)    38056 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/bonds.py
--rw-r--r--   0 runner    (1001) docker     (127)    19739 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    38956 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/cif.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/cms_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/column.py
--rw-r--r--   0 runner    (1001) docker     (127)    36450 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/configuration_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:56.803546 molsystem-2024.5.6/molsystem/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/data/standard_properties.csv
--rw-r--r--   0 runner    (1001) docker     (127)    26799 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/frozencolumn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/inchi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/molfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/openbabel.py
--rw-r--r--   0 runner    (1001) docker     (127)    18217 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/pdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    33065 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/pubchem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/qcschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/rdkit_.py
--rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/smiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/subset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/subsets.py
--rw-r--r--   0 runner    (1001) docker     (127)    47649 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    19509 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/system.py
--rw-r--r--   0 runner    (1001) docker     (127)    36917 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/system_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/system_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    26830 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    20863 2024-05-05 22:14:43.000000 molsystem-2024.5.6/molsystem/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:56.807546 molsystem-2024.5.6/molsystem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-05-05 22:14:56.000000 molsystem-2024.5.6/molsystem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-05 22:14:56.000000 molsystem-2024.5.6/molsystem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 22:14:56.000000 molsystem-2024.5.6/molsystem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-05 22:14:56.000000 molsystem-2024.5.6/molsystem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-05 22:14:56.000000 molsystem-2024.5.6/molsystem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-05 22:14:56.811546 molsystem-2024.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-05 22:14:43.000000 molsystem-2024.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:56.807546 molsystem-2024.5.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15839 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 22:14:56.807546 molsystem-2024.5.6/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)   269083 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/data/1n9v.cif
--rw-r--r--   0 runner    (1001) docker     (127)  1055288 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/data/aa-variants-v1.cif
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/data/acy.mmcif
--rw-r--r--   0 runner    (1001) docker     (127)   117392 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/data/aminoacids.mmcif
--rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/data/benzene.cif
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/data/hoh.mmcif
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/data/polyethylene.cif
--rw-r--r--   0 runner    (1001) docker     (127)    71597 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/data/spacegroup_names.json
--rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/data/trigonal.cif
--rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_angiotensin.py
--rw-r--r--   0 runner    (1001) docker     (127)    16521 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_bonds.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    10988 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_cif.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_configuration_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_inchi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_molfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    18800 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_openbabel.py
--rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_pdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_property_timings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_pubchem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_qcschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_rdkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_smiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_subsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_system_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_timings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-05 22:14:43.000000 molsystem-2024.5.6/tests/test_topology.py
--rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-05-05 22:14:43.000000 molsystem-2024.5.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:45:16.731421 molsystem-2024.5.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-08 16:45:00.000000 molsystem-2024.5.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-08 16:45:00.000000 molsystem-2024.5.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-05-08 16:45:00.000000 molsystem-2024.5.8/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-08 16:45:00.000000 molsystem-2024.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-08 16:45:00.000000 molsystem-2024.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-05-08 16:45:16.731421 molsystem-2024.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-08 16:45:00.000000 molsystem-2024.5.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:45:16.711420 molsystem-2024.5.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-08 16:45:00.000000 molsystem-2024.5.8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:45:16.711420 molsystem-2024.5.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-05-08 16:45:00.000000 molsystem-2024.5.8/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-05-08 16:45:00.000000 molsystem-2024.5.8/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-05-08 16:45:00.000000 molsystem-2024.5.8/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-05-08 16:45:00.000000 molsystem-2024.5.8/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-05-08 16:45:00.000000 molsystem-2024.5.8/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-05-08 16:45:00.000000 molsystem-2024.5.8/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:45:16.711420 molsystem-2024.5.8/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-08 16:45:00.000000 molsystem-2024.5.8/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 16:45:00.000000 molsystem-2024.5.8/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9525 2024-05-08 16:45:00.000000 molsystem-2024.5.8/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:45:16.715421 molsystem-2024.5.8/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-08 16:45:00.000000 molsystem-2024.5.8/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-08 16:45:00.000000 molsystem-2024.5.8/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-08 16:45:00.000000 molsystem-2024.5.8/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-08 16:45:00.000000 molsystem-2024.5.8/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:45:16.715421 molsystem-2024.5.8/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-08 16:45:00.000000 molsystem-2024.5.8/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 16:45:00.000000 molsystem-2024.5.8/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-08 16:45:00.000000 molsystem-2024.5.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-08 16:45:00.000000 molsystem-2024.5.8/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:45:16.715421 molsystem-2024.5.8/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-08 16:45:00.000000 molsystem-2024.5.8/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:45:16.731421 molsystem-2024.5.8/molsystem/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-08 16:45:16.731421 molsystem-2024.5.8/molsystem/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/align.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69805 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38056 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/bonds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19739 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38956 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/cif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/cms_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36450 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/configuration_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:45:16.719421 molsystem-2024.5.8/molsystem/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/data/standard_properties.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    26799 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/frozencolumn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/inchi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/molfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/openbabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18217 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/pdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33065 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/pubchem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/qcschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/rdkit_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/smiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/subsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47649 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19509 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36917 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/system_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/system_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26830 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20863 2024-05-08 16:45:00.000000 molsystem-2024.5.8/molsystem/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:45:16.727421 molsystem-2024.5.8/molsystem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-05-08 16:45:16.000000 molsystem-2024.5.8/molsystem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-08 16:45:16.000000 molsystem-2024.5.8/molsystem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:45:16.000000 molsystem-2024.5.8/molsystem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 16:45:16.000000 molsystem-2024.5.8/molsystem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 16:45:16.000000 molsystem-2024.5.8/molsystem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-08 16:45:16.731421 molsystem-2024.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-08 16:45:00.000000 molsystem-2024.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:45:16.727421 molsystem-2024.5.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15839 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:45:16.727421 molsystem-2024.5.8/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   269083 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/data/1n9v.cif
+-rw-r--r--   0 runner    (1001) docker     (127)  1055288 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/data/aa-variants-v1.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/data/acy.mmcif
+-rw-r--r--   0 runner    (1001) docker     (127)   117392 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/data/aminoacids.mmcif
+-rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/data/benzene.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/data/hoh.mmcif
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/data/polyethylene.cif
+-rw-r--r--   0 runner    (1001) docker     (127)    71597 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/data/spacegroup_names.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/data/trigonal.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_angiotensin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16521 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_bonds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10988 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_cif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_configuration_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_inchi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_molfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18800 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_openbabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_property_timings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_pubchem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_qcschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_rdkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_system_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_timings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-08 16:45:00.000000 molsystem-2024.5.8/tests/test_topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-05-08 16:45:00.000000 molsystem-2024.5.8/versioneer.py
```

### Comparing `molsystem-2024.5.6/CONTRIBUTING.rst` & `molsystem-2024.5.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/HISTORY.rst` & `molsystem-2024.5.8/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 =======
 History
 =======
+2024.5.8 -- Added more control over RDKit and OpenBabel creating systems
+    * Added control to from_RDKMol and from_OBMol to allow selectively updating
+      the atoms, coordinates, and bonds
+      
 2024.5.6 -- Rotated molecule from SMILES, InChI, or InChIKey to standard orientation
     * Molecules created from line notation are created in an random orientation. This
       enhancement rotates them to the standard orientation, which will look nice for
       small, symmetric molecules.
       
 2024.5.5 -- Bugfix: bonds in RDKit
     * There was an indexing bug translating bonds back from RDKit to SEAMM. The famous
```

### Comparing `molsystem-2024.5.6/LICENSE` & `molsystem-2024.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/PKG-INFO` & `molsystem-2024.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molsystem
-Version: 2024.5.6
+Version: 2024.5.8
 Summary: molsystem
 Home-page: https://github.com/molssi-seamm/molsystem
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Keywords: molsystem,SEAMM
 Platform: Linux
@@ -113,14 +113,18 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2024.5.8 -- Added more control over RDKit and OpenBabel creating systems
+    * Added control to from_RDKMol and from_OBMol to allow selectively updating
+      the atoms, coordinates, and bonds
+      
 2024.5.6 -- Rotated molecule from SMILES, InChI, or InChIKey to standard orientation
     * Molecules created from line notation are created in an random orientation. This
       enhancement rotates them to the standard orientation, which will look nice for
       small, symmetric molecules.
       
 2024.5.5 -- Bugfix: bonds in RDKit
     * There was an indexing bug translating bonds back from RDKit to SEAMM. The famous
```

### Comparing `molsystem-2024.5.6/README.rst` & `molsystem-2024.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/docs/Makefile` & `molsystem-2024.5.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/docs/_static/SEAMM inverted.png` & `molsystem-2024.5.8/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/docs/_static/SEAMM logo.png` & `molsystem-2024.5.8/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/docs/_static/molssi_main_logo.png` & `molsystem-2024.5.8/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/docs/_static/molssi_main_logo_inverted_white.png` & `molsystem-2024.5.8/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/docs/_static/molssi_square.png` & `molsystem-2024.5.8/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/docs/_static/nsf.png` & `molsystem-2024.5.8/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/docs/conf.py` & `molsystem-2024.5.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/docs/developer_guide/installation.rst` & `molsystem-2024.5.8/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/docs/getting_started/index.rst` & `molsystem-2024.5.8/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/docs/index.rst` & `molsystem-2024.5.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/docs/make.bat` & `molsystem-2024.5.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/docs/user_guide/index.rst` & `molsystem-2024.5.8/docs/user_guide/index.rst`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/__init__.py` & `molsystem-2024.5.8/molsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/align.py` & `molsystem-2024.5.8/molsystem/align.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/atoms.py` & `molsystem-2024.5.8/molsystem/atoms.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/bonds.py` & `molsystem-2024.5.8/molsystem/bonds.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/cell.py` & `molsystem-2024.5.8/molsystem/cell.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/cif.py` & `molsystem-2024.5.8/molsystem/cif.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/cms_schema.py` & `molsystem-2024.5.8/molsystem/cms_schema.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/column.py` & `molsystem-2024.5.8/molsystem/column.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/configuration.py` & `molsystem-2024.5.8/molsystem/configuration.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/configuration_properties.py` & `molsystem-2024.5.8/molsystem/configuration_properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/data/standard_properties.csv` & `molsystem-2024.5.8/molsystem/data/standard_properties.csv`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/elements.py` & `molsystem-2024.5.8/molsystem/elements.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/frozencolumn.py` & `molsystem-2024.5.8/molsystem/frozencolumn.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/inchi.py` & `molsystem-2024.5.8/molsystem/inchi.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/molfile.py` & `molsystem-2024.5.8/molsystem/molfile.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/openbabel.py` & `molsystem-2024.5.8/molsystem/openbabel.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,15 +67,17 @@
             for key, value in data.items():
                 pair.SetAttribute(key)
                 pair.SetValue(str(value))
                 ob_mol.CloneData(pair)
 
         return ob_mol
 
-    def from_OBMol(self, ob_mol, properties="all"):
+    def from_OBMol(
+        self, ob_mol, properties="all", atoms=True, coordinates=True, bonds=True
+    ):
         """Transform an Open Babel molecule into the current object."""
         atnos = []
         Xs = []
         Ys = []
         Zs = []
         qs = []
         for ob_atom in ob.OBMolAtomIter(ob_mol):
@@ -97,29 +99,39 @@
             j = ob_j.GetIdx()
             bondorder = ob_bond.GetBondOrder()
             Is.append(i)
             Js.append(j)
             BondOrders.append(bondorder)
             logger.debug(f"bond {i} - {j} {bondorder}")
 
-        self.clear()
+        if atoms:
+            self.clear()
 
         if self.__class__.__name__ == "_Configuration":
             self.charge = ob_mol.GetTotalCharge()
             self.spin_multiplicity = ob_mol.GetTotalSpinMultiplicity()
 
-        if any([i != 0.0 for i in qs]):
-            if "formal_charge" not in self.atoms:
-                self.atoms.add_attribute("formal_charge", coltype="int", default=0)
-            ids = self.atoms.append(x=Xs, y=Ys, z=Zs, atno=atnos, formal_charge=qs)
+        if atoms:
+            if any([i != 0.0 for i in qs]):
+                if "formal_charge" not in self.atoms:
+                    self.atoms.add_attribute("formal_charge", coltype="int", default=0)
+                ids = self.atoms.append(x=Xs, y=Ys, z=Zs, atno=atnos, formal_charge=qs)
+            else:
+                ids = self.atoms.append(x=Xs, y=Ys, z=Zs, atno=atnos)
         else:
-            ids = self.atoms.append(x=Xs, y=Ys, z=Zs, atno=atnos)
-        i = [ids[x - 1] for x in Is]
-        j = [ids[x - 1] for x in Js]
-        self.bonds.append(i=i, j=j, bondorder=BondOrders)
+            ids = self.atoms.ids
+
+            if coordinates:
+                xyz = [[x, y, z] for x, y, z in zip(Xs, Ys, Zs)]
+                self.atoms.coordinates = xyz
+
+        if atoms or bonds:
+            i = [ids[x - 1] for x in Is]
+            j = [ids[x - 1] for x in Js]
+            self.bonds.append(i=i, j=j, bondorder=BondOrders)
 
         # Record any properties in the database if desired
         if properties == "all":
             data = ob_mol.GetData()
             for item in data:
                 attribute = item.GetAttribute()
                 value = item.GetValue()
```

### Comparing `molsystem-2024.5.6/molsystem/pdb.py` & `molsystem-2024.5.8/molsystem/pdb.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/properties.py` & `molsystem-2024.5.8/molsystem/properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/pubchem.py` & `molsystem-2024.5.8/molsystem/pubchem.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/qcschema.py` & `molsystem-2024.5.8/molsystem/qcschema.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/rdkit_.py` & `molsystem-2024.5.8/molsystem/rdkit_.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Interface to RDKit."""
 
 import logging
+import pprint
+
 
 try:
     from rdkit import Chem
 except ModuleNotFoundError:
     print(
         "Please install rdkit using conda:\n" "     conda install -c conda-forge rdkit"
     )
@@ -78,16 +80,34 @@
             conf.SetAtomPosition(idx, xyz)
 
         rdk_mol.AddConformer(conf)
         Chem.rdmolops.SanitizeMol(rdk_mol)
 
         return rdk_mol
 
-    def from_RDKMol(self, rdk_mol):
-        """Transform an RDKit molecule into the current object."""
+    def from_RDKMol(self, rdk_mol, atoms=True, coordinates=True, bonds=True):
+        """Transform an RDKit molecule into the current object.
+
+        Parameters
+        ----------
+        rdk_mol : rdkit.chem.molecule
+            The RDKit molecule object
+
+        atoms : bool = True
+            Recreate the atoms
+
+        coordinates : bool = True
+            Update the coordinates
+
+        bonds : bool = True
+            Recreate the bonds from the RDKit molecule
+        """
+
+        # print("from_RDKMol before")
+        # self.debug_print()
 
         atnos = []
         for rdk_atom in rdk_mol.GetAtoms():
             atnos.append(rdk_atom.GetAtomicNum())
             logger.debug(f"atom {atnos}")
 
         # TODO: Generalize to handling multiple conformers
@@ -116,14 +136,31 @@
             j = rdk_bond.GetEndAtom().GetIdx()
             bondorder = bond_types[rdk_bond.GetBondType()]
             Is.append(i)
             Js.append(j)
             BondOrders.append(bondorder)
             logger.debug(f"bond {i} - {j} {bondorder}")
 
-        self.clear()
-        ids = self.atoms.append(x=Xs, y=Ys, z=Zs, atno=atnos)
-        i = [ids[x] for x in Is]
-        j = [ids[x] for x in Js]
-        self.bonds.append(i=i, j=j, bondorder=BondOrders)
+        if atoms:
+            self.clear()
+            ids = self.atoms.append(x=Xs, y=Ys, z=Zs, atno=atnos)
+        else:
+            ids = self.atoms.ids
+
+            if coordinates:
+                xyz = [[x, y, z] for x, y, z in zip(Xs, Ys, Zs)]
+                self.atoms.coordinates = xyz
+
+        if atoms or bonds:
+            i = [ids[x] for x in Is]
+            j = [ids[x] for x in Js]
+            self.bonds.append(i=i, j=j, bondorder=BondOrders)
+
+        # print("from_RDKMol after")
+        # self.debug_print()
 
         return self
+
+    def debug_print(self):
+        pprint.pprint(str(self.atoms._atom_table))
+        pprint.pprint(str(self.atoms._coordinates_table))
+        pprint.pprint(str(self.bonds))
```

### Comparing `molsystem-2024.5.6/molsystem/smiles.py` & `molsystem-2024.5.8/molsystem/smiles.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/subset.py` & `molsystem-2024.5.8/molsystem/subset.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/subsets.py` & `molsystem-2024.5.8/molsystem/subsets.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/symmetry.py` & `molsystem-2024.5.8/molsystem/symmetry.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/system.py` & `molsystem-2024.5.8/molsystem/system.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/system_db.py` & `molsystem-2024.5.8/molsystem/system_db.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/system_properties.py` & `molsystem-2024.5.8/molsystem/system_properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/table.py` & `molsystem-2024.5.8/molsystem/table.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/template.py` & `molsystem-2024.5.8/molsystem/template.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/templates.py` & `molsystem-2024.5.8/molsystem/templates.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem/topology.py` & `molsystem-2024.5.8/molsystem/topology.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/molsystem.egg-info/PKG-INFO` & `molsystem-2024.5.8/molsystem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molsystem
-Version: 2024.5.6
+Version: 2024.5.8
 Summary: molsystem
 Home-page: https://github.com/molssi-seamm/molsystem
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Keywords: molsystem,SEAMM
 Platform: Linux
@@ -113,14 +113,18 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2024.5.8 -- Added more control over RDKit and OpenBabel creating systems
+    * Added control to from_RDKMol and from_OBMol to allow selectively updating
+      the atoms, coordinates, and bonds
+      
 2024.5.6 -- Rotated molecule from SMILES, InChI, or InChIKey to standard orientation
     * Molecules created from line notation are created in an random orientation. This
       enhancement rotates them to the standard orientation, which will look nice for
       small, symmetric molecules.
       
 2024.5.5 -- Bugfix: bonds in RDKit
     * There was an indexing bug translating bonds back from RDKit to SEAMM. The famous
```

### Comparing `molsystem-2024.5.6/molsystem.egg-info/SOURCES.txt` & `molsystem-2024.5.8/molsystem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/setup.py` & `molsystem-2024.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/conftest.py` & `molsystem-2024.5.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/data/1n9v.cif` & `molsystem-2024.5.8/tests/data/1n9v.cif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/data/aa-variants-v1.cif` & `molsystem-2024.5.8/tests/data/aa-variants-v1.cif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/data/acy.mmcif` & `molsystem-2024.5.8/tests/data/acy.mmcif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/data/aminoacids.mmcif` & `molsystem-2024.5.8/tests/data/aminoacids.mmcif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/data/benzene.cif` & `molsystem-2024.5.8/tests/data/benzene.cif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/data/hoh.mmcif` & `molsystem-2024.5.8/tests/data/hoh.mmcif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/data/polyethylene.cif` & `molsystem-2024.5.8/tests/data/polyethylene.cif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/data/spacegroup_names.json` & `molsystem-2024.5.8/tests/data/spacegroup_names.json`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/data/trigonal.cif` & `molsystem-2024.5.8/tests/data/trigonal.cif`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_angiotensin.py` & `molsystem-2024.5.8/tests/test_angiotensin.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_atoms.py` & `molsystem-2024.5.8/tests/test_atoms.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_bonds.py` & `molsystem-2024.5.8/tests/test_bonds.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_cell.py` & `molsystem-2024.5.8/tests/test_cell.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_cif.py` & `molsystem-2024.5.8/tests/test_cif.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_configuration_properties.py` & `molsystem-2024.5.8/tests/test_configuration_properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_configurations.py` & `molsystem-2024.5.8/tests/test_configurations.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_inchi.py` & `molsystem-2024.5.8/tests/test_inchi.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_molfile.py` & `molsystem-2024.5.8/tests/test_molfile.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_openbabel.py` & `molsystem-2024.5.8/tests/test_openbabel.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_pdb.py` & `molsystem-2024.5.8/tests/test_pdb.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_properties.py` & `molsystem-2024.5.8/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_property_timings.py` & `molsystem-2024.5.8/tests/test_property_timings.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_pubchem.py` & `molsystem-2024.5.8/tests/test_pubchem.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_qcschema.py` & `molsystem-2024.5.8/tests/test_qcschema.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_rdkit.py` & `molsystem-2024.5.8/tests/test_rdkit.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_smiles.py` & `molsystem-2024.5.8/tests/test_smiles.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_subsets.py` & `molsystem-2024.5.8/tests/test_subsets.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_symmetry.py` & `molsystem-2024.5.8/tests/test_symmetry.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_system.py` & `molsystem-2024.5.8/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_system_db.py` & `molsystem-2024.5.8/tests/test_system_db.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_table.py` & `molsystem-2024.5.8/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_templates.py` & `molsystem-2024.5.8/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_timings.py` & `molsystem-2024.5.8/tests/test_timings.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/tests/test_topology.py` & `molsystem-2024.5.8/tests/test_topology.py`

 * *Files identical despite different names*

### Comparing `molsystem-2024.5.6/versioneer.py` & `molsystem-2024.5.8/versioneer.py`

 * *Files identical despite different names*

