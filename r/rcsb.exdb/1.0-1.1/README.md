# Comparing `tmp/rcsb.exdb-1.0.tar.gz` & `tmp/rcsb_exdb-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.exdb-1.0.tar", last modified: Tue Jan  9 21:48:56 2024, max compression
+gzip compressed data, was "rcsb_exdb-1.1.tar", last modified: Wed May  8 20:36:31 2024, max compression
```

## Comparing `rcsb.exdb-1.0.tar` & `rcsb_exdb-1.1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-09 21:48:56.981104 rcsb.exdb-1.0/
--rw-r--r--   0 vsts      (1001) docker     (127)     7883 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (127)    11357 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      102 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     6080 2024-01-09 21:48:56.981104 rcsb.exdb-1.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     4716 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-09 21:48:56.969103 rcsb.exdb-1.0/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-09 21:48:56.969103 rcsb.exdb-1.0/rcsb/exdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-09 21:48:56.969103 rcsb.exdb-1.0/rcsb/exdb/branch/
--rw-r--r--   0 vsts      (1001) docker     (127)     2645 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/branch/BranchedEntityExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4000 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/branch/GlycanProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4507 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/branch/GlycanUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/branch/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-09 21:48:56.973104 rcsb.exdb-1.0/rcsb/exdb/chemref/
--rw-r--r--   0 vsts      (1001) docker     (127)     4602 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/chemref/ChemRefEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2538 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/chemref/ChemRefExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5290 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/chemref/ChemRefMappingProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15479 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/chemref/PubChemDataCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11699 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/chemref/PubChemEtlWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29079 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/chemref/PubChemIndexCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/chemref/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-09 21:48:56.973104 rcsb.exdb-1.0/rcsb/exdb/citation/
--rw-r--r--   0 vsts      (1001) docker     (127)     3501 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/citation/CitationAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7574 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/citation/CitationExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1487 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/citation/CitationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/citation/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-09 21:48:56.973104 rcsb.exdb-1.0/rcsb/exdb/cli/
--rw-r--r--   0 vsts      (1001) docker     (127)     9878 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/cli/ExDbExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)      144 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/cli/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-09 21:48:56.973104 rcsb.exdb-1.0/rcsb/exdb/entry/
--rw-r--r--   0 vsts      (1001) docker     (127)     5095 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/entry/EntryInfoProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/entry/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-09 21:48:56.973104 rcsb.exdb-1.0/rcsb/exdb/seq/
--rw-r--r--   0 vsts      (1001) docker     (127)     2741 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/seq/AnnotationExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3423 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/seq/LigandNeighborMappingExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3744 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/seq/LigandNeighborMappingProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14538 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/seq/PolymerEntityExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)    31160 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/seq/ReferenceSequenceAnnotationAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9560 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/seq/ReferenceSequenceAnnotationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25935 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/seq/ReferenceSequenceAssignmentAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18181 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/seq/ReferenceSequenceAssignmentProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19497 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/seq/ReferenceSequenceCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2315 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/seq/TaxonomyExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7477 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/seq/UniProtCoreEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2695 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/seq/UniProtExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/seq/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-09 21:48:56.977104 rcsb.exdb-1.0/rcsb/exdb/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3999 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/fixtureDictMethodResourceProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9679 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/fixturePdbxLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2657 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testAnnotationExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2936 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testBranchedEntityExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3696 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testChemRefLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3353 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testChemRefMappingProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3625 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testCitationAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3141 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testCitationExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3064 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testCitationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2340 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testEntryInfoEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3360 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testEntryInfoProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5294 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testExDbWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2295 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testGlycanEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3201 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testGlycanProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1953 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testGlycanUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3040 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testLigandNeighborMappingProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14144 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testObjectExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2944 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testObjectTransformer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4950 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testObjectUpdater.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3537 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testPolymerEntityExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4679 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testPubChemDataCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5187 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testPubChemEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6511 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testPubChemEtlWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4947 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testPubChemIndexCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4186 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testReferenceSequenceAnnotationAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4897 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5005 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapterValidate.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4631 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testReferenceSequenceAssignmentProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3469 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testReferenceSequenceCacheProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2536 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testTaxonomyExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3654 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testTreeNodeListWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3403 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testUniProtCoreEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2604 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tests/testUniProtExtractor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-09 21:48:56.977104 rcsb.exdb-1.0/rcsb/exdb/tree/
--rw-r--r--   0 vsts      (1001) docker     (127)    12500 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tree/TreeNodeListWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/tree/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-09 21:48:56.981104 rcsb.exdb-1.0/rcsb/exdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)      466 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/utils/ObjectAdapterBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11057 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/utils/ObjectExtractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5210 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/utils/ObjectTransformer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5089 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/utils/ObjectUpdater.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6954 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/utils/ObjectValidator.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-09 21:48:56.981104 rcsb.exdb-1.0/rcsb/exdb/wf/
--rw-r--r--   0 vsts      (1001) docker     (127)     2570 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/wf/EntryInfoEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10838 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/wf/ExDbWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2820 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/wf/GlycanEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10473 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/wf/PubChemEtlWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/rcsb/exdb/wf/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-09 21:48:56.981104 rcsb.exdb-1.0/rcsb.exdb.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     6080 2024-01-09 21:48:56.000000 rcsb.exdb-1.0/rcsb.exdb.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     3525 2024-01-09 21:48:56.000000 rcsb.exdb-1.0/rcsb.exdb.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-01-09 21:48:56.000000 rcsb.exdb-1.0/rcsb.exdb.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       62 2024-01-09 21:48:56.000000 rcsb.exdb-1.0/rcsb.exdb.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-01-09 21:26:37.000000 rcsb.exdb-1.0/rcsb.exdb.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      399 2024-01-09 21:48:56.000000 rcsb.exdb-1.0/rcsb.exdb.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-01-09 21:48:56.000000 rcsb.exdb-1.0/rcsb.exdb.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      443 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-01-09 21:48:56.981104 rcsb.exdb-1.0/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2184 2024-01-09 21:22:10.000000 rcsb.exdb-1.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 20:36:31.250728 rcsb_exdb-1.1/
+-rw-r--r--   0 vsts      (1001) docker     (127)     8046 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)    11357 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      102 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     6115 2024-05-08 20:36:31.250728 rcsb_exdb-1.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     4716 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 20:36:31.234727 rcsb_exdb-1.1/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 20:36:31.234727 rcsb_exdb-1.1/rcsb/exdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 20:36:31.238728 rcsb_exdb-1.1/rcsb/exdb/branch/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2645 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/branch/BranchedEntityExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4000 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/branch/GlycanProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4507 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/branch/GlycanUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/branch/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 20:36:31.238728 rcsb_exdb-1.1/rcsb/exdb/chemref/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4719 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/chemref/ChemRefEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2538 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/chemref/ChemRefExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5290 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/chemref/ChemRefMappingProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15479 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/chemref/PubChemDataCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11699 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/chemref/PubChemEtlWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29394 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/chemref/PubChemIndexCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/chemref/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 20:36:31.238728 rcsb_exdb-1.1/rcsb/exdb/citation/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3501 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/citation/CitationAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7574 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/citation/CitationExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1487 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/citation/CitationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/citation/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 20:36:31.238728 rcsb_exdb-1.1/rcsb/exdb/cli/
+-rw-r--r--   0 vsts      (1001) docker     (127)     9832 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/cli/ExDbExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      143 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/cli/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 20:36:31.238728 rcsb_exdb-1.1/rcsb/exdb/entry/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5095 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/entry/EntryInfoProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/entry/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 20:36:31.242728 rcsb_exdb-1.1/rcsb/exdb/seq/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2741 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/seq/AnnotationExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3423 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/seq/LigandNeighborMappingExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3744 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/seq/LigandNeighborMappingProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14538 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/seq/PolymerEntityExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    31160 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/seq/ReferenceSequenceAnnotationAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9560 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/seq/ReferenceSequenceAnnotationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25935 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/seq/ReferenceSequenceAssignmentAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18181 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/seq/ReferenceSequenceAssignmentProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19497 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/seq/ReferenceSequenceCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2315 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/seq/TaxonomyExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7594 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/seq/UniProtCoreEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2695 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/seq/UniProtExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/seq/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 20:36:31.246728 rcsb_exdb-1.1/rcsb/exdb/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3999 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/fixtureDictMethodResourceProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9761 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/fixturePdbxLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2657 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testAnnotationExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2936 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testBranchedEntityExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3696 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testChemRefLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3353 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testChemRefMappingProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3625 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testCitationAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3141 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testCitationExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3064 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testCitationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2340 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testEntryInfoEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3360 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testEntryInfoProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5353 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testExDbWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2295 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testGlycanEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3201 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testGlycanProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1953 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testGlycanUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3040 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testLigandNeighborMappingProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14144 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testObjectExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2944 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testObjectTransformer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4950 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testObjectUpdater.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3536 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testPolymerEntityExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4679 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testPubChemDataCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5187 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testPubChemEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6511 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testPubChemEtlWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4947 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testPubChemIndexCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4186 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testReferenceSequenceAnnotationAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4897 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5005 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapterValidate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4631 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testReferenceSequenceAssignmentProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3469 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testReferenceSequenceCacheProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2536 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testTaxonomyExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3654 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testTreeNodeListWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3403 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testUniProtCoreEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2604 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tests/testUniProtExtractor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 20:36:31.246728 rcsb_exdb-1.1/rcsb/exdb/tree/
+-rw-r--r--   0 vsts      (1001) docker     (127)    12617 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tree/TreeNodeListWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/tree/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 20:36:31.246728 rcsb_exdb-1.1/rcsb/exdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)      466 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/utils/ObjectAdapterBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11057 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/utils/ObjectExtractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5210 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/utils/ObjectTransformer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5089 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/utils/ObjectUpdater.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6954 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/utils/ObjectValidator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 20:36:31.246728 rcsb_exdb-1.1/rcsb/exdb/wf/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2570 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/wf/EntryInfoEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19806 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/wf/ExDbWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2820 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/wf/GlycanEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11235 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/wf/PubChemEtlWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/rcsb/exdb/wf/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 20:36:31.246728 rcsb_exdb-1.1/rcsb.exdb.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6115 2024-05-08 20:36:31.000000 rcsb_exdb-1.1/rcsb.exdb.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     3525 2024-05-08 20:36:31.000000 rcsb_exdb-1.1/rcsb.exdb.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-08 20:36:31.000000 rcsb_exdb-1.1/rcsb.exdb.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       62 2024-05-08 20:36:31.000000 rcsb_exdb-1.1/rcsb.exdb.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-08 20:14:35.000000 rcsb_exdb-1.1/rcsb.exdb.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      419 2024-05-08 20:36:31.000000 rcsb_exdb-1.1/rcsb.exdb.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-05-08 20:36:31.000000 rcsb_exdb-1.1/rcsb.exdb.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      465 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-05-08 20:36:31.250728 rcsb_exdb-1.1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2184 2024-05-08 20:08:28.000000 rcsb_exdb-1.1/setup.py
```

### Comparing `rcsb.exdb-1.0/HISTORY.txt` & `rcsb_exdb-1.1/HISTORY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -93,7 +93,9 @@
  1-Jun-2023 V0.97 Don't back up resources to GitHub during cache update workflows
  8-Aug-2023 V0.98 Reduce memory and cpu footprint for Azure test cases;
                   Load full (unfiltered) taxonomy tree node list, and stop loading GO tree
 19-Sep-2023 V0.99 Add reload method to ChemRefMappingProvider and LigandNeighborMappingProvider;
                   Add documentation to reference sequence providers
  9-Jan-2024 V1.00 Update PolymerEntityExtractor to turn off usage of uniprot_exdb as source data;
                   This package update also coincides with the turning off of uniprot_exdb data loading during the weekly workflow
+ 6-May-2024 V1.1  Update ExDbExec CLI and ExDbWorkflow to support CLI usage from weekly-update workflow;
+                  Update unit tests and setuptools config
```

### Comparing `rcsb.exdb-1.0/LICENSE` & `rcsb_exdb-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/PKG-INFO` & `rcsb_exdb-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.exdb
-Version: 1.0
+Version: 1.1
 Summary: RCSB Python ExDB data extraction and loading workflows
 Home-page: https://github.com/rcsb/py-rcsb_exdb
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -26,14 +26,15 @@
 Requires-Dist: rcsb.utils.config>=0.35
 Requires-Dist: rcsb.utils.ec>=0.22
 Requires-Dist: rcsb.utils.go>=0.17
 Requires-Dist: rcsb.utils.seq>=0.63
 Requires-Dist: rcsb.utils.struct>=0.37
 Requires-Dist: rcsb.utils.taxonomy>=0.39
 Requires-Dist: rcsb.utils.dictionary>=0.71
+Requires-Dist: rcsb.workflow>=0.42
 Requires-Dist: statistics; python_version < "3.0"
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 
 # py-rcsb_exdb
```

### Comparing `rcsb.exdb-1.0/README.md` & `rcsb_exdb-1.1/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/branch/BranchedEntityExtractor.py` & `rcsb_exdb-1.1/rcsb/exdb/branch/BranchedEntityExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/branch/GlycanProvider.py` & `rcsb_exdb-1.1/rcsb/exdb/branch/GlycanProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/branch/GlycanUtils.py` & `rcsb_exdb-1.1/rcsb/exdb/branch/GlycanUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/chemref/ChemRefEtlWorker.py` & `rcsb_exdb-1.1/rcsb/exdb/chemref/ChemRefEtlWorker.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,21 +25,22 @@
 
 logger = logging.getLogger(__name__)
 
 
 class ChemRefEtlWorker(object):
     """Prepare and load chemical reference data collections."""
 
-    def __init__(self, cfgOb, cachePath, useCache=True, numProc=2, chunkSize=10, readBackCheck=False, documentLimit=None, verbose=False):
+    def __init__(self, cfgOb, cachePath, useCache=True, numProc=2, chunkSize=10, maxStepLength=2000, readBackCheck=False, documentLimit=None, verbose=False):
         self.__cfgOb = cfgOb
         self.__cachePath = cachePath
         self.__useCache = useCache
         self.__readBackCheck = readBackCheck
         self.__numProc = numProc
         self.__chunkSize = chunkSize
+        self.__maxStepLength = maxStepLength
         self.__documentLimit = documentLimit
         #
         self.__resourceName = "MONGO_DB"
         self.__verbose = verbose
         self.__statusList = []
         self.__schP = SchemaProvider(self.__cfgOb, self.__cachePath, useCache=self.__useCache)
         #
@@ -91,14 +92,15 @@
             #
             dl = DocumentLoader(
                 self.__cfgOb,
                 self.__cachePath,
                 self.__resourceName,
                 numProc=self.__numProc,
                 chunkSize=self.__chunkSize,
+                maxStepLength=self.__maxStepLength,
                 documentLimit=self.__documentLimit,
                 verbose=self.__verbose,
                 readBackCheck=self.__readBackCheck,
             )
             #
             ok = dl.load(databaseName, collectionName, loadType=loadType, documentList=dList, indexAttributeList=indexL, keyNames=None, addValues=addValues)
             self.__updateStatus(updateId, databaseName, collectionName, ok, statusStartTimestamp)
```

### Comparing `rcsb.exdb-1.0/rcsb/exdb/chemref/ChemRefExtractor.py` & `rcsb_exdb-1.1/rcsb/exdb/chemref/ChemRefExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/chemref/ChemRefMappingProvider.py` & `rcsb_exdb-1.1/rcsb/exdb/chemref/ChemRefMappingProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/chemref/PubChemDataCacheProvider.py` & `rcsb_exdb-1.1/rcsb/exdb/chemref/PubChemDataCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/chemref/PubChemEtlWrapper.py` & `rcsb_exdb-1.1/rcsb/exdb/chemref/PubChemEtlWrapper.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/chemref/PubChemIndexCacheProvider.py` & `rcsb_exdb-1.1/rcsb/exdb/chemref/PubChemIndexCacheProvider.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,15 +192,15 @@
     def __createCollections(self, databaseName, collectionName, indexAttributeNames=None):
         obUpd = ObjectUpdater(self.__cfgOb)
         ok = obUpd.createCollection(databaseName, collectionName, indexAttributeNames=indexAttributeNames, checkExists=True, bsonSchema=None)
         return ok
 
     def __chunker(self, iList, chunkSize):
         chunkSize = max(1, chunkSize)
-        return (iList[i : i + chunkSize] for i in range(0, len(iList), chunkSize))
+        return (iList[i: i + chunkSize] for i in range(0, len(iList), chunkSize))
 
 
 class PubChemIndexCacheProvider(StashableBase):
     """Utilities to manage chemical component/BIRD to PubChem compound identifier mapping data."""
 
     def __init__(self, cfgOb, cachePath):
         dirName = "PubChem-index"
@@ -315,14 +315,15 @@
                     "rcsb_id" : "local reference ID (ccid|bird)", << LOCAL ID
                     "rcsb_last_update" : ISODate("2020-04-08T16:26:48.025+0000"),
                 }
         """
         #
         matchD = {}
         matchedIdList = []
+        ok = False
         try:
             # ---
             # Get current the indices of source chemical reference data -
             ok, ccidxP, ccsidxP = self.__rebuildChemCompSourceIndices(numProcChemComp, **kwargs)
             if not ok:
                 return matchD
             #
@@ -342,15 +343,18 @@
             if updateIdList:
                 logger.info("Update reference data cache for %d chemical identifiers", len(updateIdList))
                 ok, failList = self.__updateReferenceData(updateIdList, searchIdxD, numProc, **kwargs)
                 logger.info("Update reference data return status is %r missing count %d", ok, len(failList))
             else:
                 logger.info("No reference data updates required")
             # --
-            return ok
+            if not ok:
+                logger.warning("updateMissing completed with status %r failures %r", ok, len(failList))
+            #
+            return True
         except Exception as e:
             logger.exception("Failing with %s", str(e))
         return ok
 
     def getMatches(self):
         """Get all PubChem correspondences from the current match index..
 
@@ -565,16 +569,18 @@
 
     #                           --- --- ---
     # -- Load or rebuild source chemical reference data indices --
     def __rebuildChemCompSourceIndices(self, numProc, **kwargs):
         """Rebuild source indices of chemical component definitions."""
         logger.info("Rebuilding chemical definition index.")
         ok1, ccidxP = self.__buildChemCompIndex(**kwargs)
+        logger.info("__buildChemCompIndex completed with status %r", ok1)
         logger.info("Rebuilding chemical search indices.")
         ok2, ccsidxP = self.__buildChemCompSearchIndex(numProc, **kwargs)
+        logger.info("__buildChemCompSearchIndex completed with status %r", ok2)
         return ok1 & ok2, ccidxP, ccsidxP
 
     def __buildChemCompIndex(self, **kwargs):
         """Build chemical component cache files from the input component dictionaries"""
         try:
             molLimit = kwargs.get("molLimit", None)
             useCache = not kwargs.get("rebuildChemIndices", False)
```

### Comparing `rcsb.exdb-1.0/rcsb/exdb/citation/CitationAdapter.py` & `rcsb_exdb-1.1/rcsb/exdb/citation/CitationAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/citation/CitationExtractor.py` & `rcsb_exdb-1.1/rcsb/exdb/citation/CitationExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/citation/CitationUtils.py` & `rcsb_exdb-1.1/rcsb/exdb/citation/CitationUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/cli/ExDbExec.py` & `rcsb_exdb-1.1/rcsb/exdb/cli/ExDbExec.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,191 +4,208 @@
 #
 #  Execution wrapper  --  for extract and load operations -
 #
 #  Updates:
 #   4-Sep-2019 jdw add Tree and Drugbank loaders
 #  14-Feb-2020 jdw change over to ReferenceSequenceAnnotationProvider/Adapter
 #   9-Mar-2023 dwp Lower refChunkSize to 10 (UniProt API having trouble streaming XML responses)
-#
+#  25-Apr-2024 dwp Add arguments and logic to support CLI usage from weekly-update workflow;
+#                  Add support for logging output to a specific file
 ##
 __docformat__ = "google en"
 __author__ = "John Westbrook"
 __email__ = "jwest@rcsb.rutgers.edu"
 __license__ = "Apache 2.0"
 
-import argparse
-import logging
 import os
 import sys
+import argparse
+import logging
 
-from rcsb.db.mongo.DocumentLoader import DocumentLoader
-from rcsb.db.utils.TimeUtil import TimeUtil
-from rcsb.exdb.chemref.ChemRefEtlWorker import ChemRefEtlWorker
-from rcsb.exdb.seq.ReferenceSequenceAnnotationAdapter import ReferenceSequenceAnnotationAdapter
-from rcsb.exdb.seq.ReferenceSequenceAnnotationProvider import ReferenceSequenceAnnotationProvider
-from rcsb.exdb.seq.UniProtCoreEtlWorker import UniProtCoreEtlWorker
-from rcsb.exdb.tree.TreeNodeListWorker import TreeNodeListWorker
-from rcsb.exdb.utils.ObjectTransformer import ObjectTransformer
 from rcsb.utils.config.ConfigUtil import ConfigUtil
-from rcsb.utils.dictionary.DictMethodResourceProvider import DictMethodResourceProvider
+from rcsb.exdb.wf.ExDbWorkflow import ExDbWorkflow
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 TOPDIR = os.path.dirname(os.path.dirname(os.path.dirname(HERE)))
 
-logging.basicConfig(level=logging.INFO, format="%(asctime)s [%(levelname)s]-%(module)s.%(funcName)s: %(message)s")
+# logging.basicConfig(level=logging.INFO, format="%(asctime)s [%(levelname)s]-%(module)s.%(funcName)s: %(message)s", stream=sys.stdout)
 logger = logging.getLogger()
 
 
-def loadStatus(statusList, cfgOb, cachePath, readBackCheck=True):
-    sectionName = "data_exchange_configuration"
-    dl = DocumentLoader(cfgOb, cachePath, "MONGO_DB", numProc=2, chunkSize=2, documentLimit=None, verbose=False, readBackCheck=readBackCheck)
-    #
-    databaseName = cfgOb.get("DATABASE_NAME", sectionName=sectionName)
-    collectionName = cfgOb.get("COLLECTION_UPDATE_STATUS", sectionName=sectionName)
-    ok = dl.load(databaseName, collectionName, loadType="append", documentList=statusList, indexAttributeList=["update_id", "database_name", "object_name"], keyNames=None)
-    return ok
-
-
-def buildResourceCache(cfgOb, configName, cachePath, rebuildCache=False):
-    """Generate and cache resource dependencies."""
-    ret = False
-    try:
-        rp = DictMethodResourceProvider(cfgOb, configName=configName, cachePath=cachePath)
-        ret = rp.cacheResources(useCache=not rebuildCache)
-    except Exception as e:
-        logger.exception("Failing with %s", str(e))
-    return ret
-
-
-def doReferenceSequenceUpdate(cfgOb, databaseName, collectionName, polymerType, cachePath, useCache, fetchLimit=None, refChunkSize=10):
-    try:
-        #  -- create cache ---
-        rsaP = ReferenceSequenceAnnotationProvider(
-            cfgOb, databaseName, collectionName, polymerType, maxChunkSize=refChunkSize, useCache=useCache, cachePath=cachePath, fetchLimit=fetchLimit, siftsAbbreviated="TEST"
-        )
-        ok = rsaP.testCache()
-        if not ok:
-            logger.error("Cache construction fails %s", ok)
-            return False
-        logger.info("Cached reference data count is %d", rsaP.getRefDataCount())
-        rsa = ReferenceSequenceAnnotationAdapter(rsaP)
-        obTr = ObjectTransformer(cfgOb, objectAdapter=rsa)
-        ok = obTr.doTransform(databaseName=databaseName, collectionName=collectionName, fetchLimit=fetchLimit, selectionQuery={"entity_poly.rcsb_entity_polymer_type": polymerType})
-        return ok
-    except Exception as e:
-        logger.exception("Failing with %s", str(e))
-
-
 def main():
     parser = argparse.ArgumentParser()
     #
-    defaultConfigName = "site_info_configuration"
-    parser.add_argument("--data_set_id", default=None, help="Data set identifier (default= 2019_14 for current week)")
-    parser.add_argument("--full", default=True, action="store_true", help="Fresh full load in a new tables/collections (Default)")
-    parser.add_argument("--etl_chemref", default=False, action="store_true", help="ETL integrated chemical reference data")
-    parser.add_argument("--etl_uniprot_core", default=False, action="store_true", help="ETL UniProt core reference data")
-    parser.add_argument("--etl_tree_node_lists", default=False, action="store_true", help="ETL tree node lists")
-    parser.add_argument("--upd_ref_seq", default=False, action="store_true", help="Update reference sequence assignments")
+    parser.add_argument(
+        "--op",
+        default=None,
+        required=True,
+        help="Loading operation to perform",
+        choices=[
+            "etl_chemref",  # ETL integrated chemical reference data
+            "etl_uniprot_core",  # ETL UniProt core reference data
+            "etl_tree_node_lists",  # ETL tree node lists
+            "upd_ref_seq",  # Update reference sequence assignments
+            "upd_neighbor_interactions",
+            "upd_uniprot_taxonomy",
+            "upd_targets_cofactors",
+            "upd_pubchem",
+            "upd_entry_info",
+            "upd_glycan_idx",
+            "upd_resource_stash",
+        ]
+    )
+    parser.add_argument(
+        "--load_type",
+        default="full",
+        help="Type of load ('full' for complete and fresh single-worker load, 'replace' for incremental and multi-worker load)",
+        choices=["full", "replace"],
+    )
     #
     parser.add_argument("--config_path", default=None, help="Path to configuration options file")
-    parser.add_argument("--config_name", default=defaultConfigName, help="Configuration section name")
-    parser.add_argument("--db_type", default="mongo", help="Database server type (default=mongo)")
-    parser.add_argument("--read_back_check", default=False, action="store_true", help="Perform read back check on all documents")
+    parser.add_argument("--config_name", default="site_info_remote_configuration", help="Configuration section name")
+    parser.add_argument("--cache_path", default=None, help="Cache path for resource files")
     parser.add_argument("--num_proc", default=2, help="Number of processes to execute (default=2)")
     parser.add_argument("--chunk_size", default=10, help="Number of files loaded per process")
+    parser.add_argument("--max_step_length", default=500, help="Maximum subList size (default=500)")
+    parser.add_argument("--db_type", default="mongo", help="Database server type (default=mongo)")
     parser.add_argument("--document_limit", default=None, help="Load document limit for testing")
+    #
+    parser.add_argument("--rebuild_cache", default=False, action="store_true", help="Rebuild cached resource files")
+    parser.add_argument("--rebuild_sequence_cache", default=False, action="store_true", help="Rebuild cached resource files for reference sequence updates")
+    parser.add_argument("--provider_type_exclude", default=None, help="Resource provider types to exclude")
+    parser.add_argument("--use_filtered_tax_list", default=False, action="store_true", help="Use filtered list for taxonomy tree loading")
+    parser.add_argument("--disable_read_back_check", default=False, action="store_true", help="Disable read back check on all documents")
     parser.add_argument("--debug", default=False, action="store_true", help="Turn on verbose logging")
     parser.add_argument("--mock", default=False, action="store_true", help="Use MOCK repository configuration for testing")
-    parser.add_argument("--cache_path", default=None, help="Top cache path for external and local resource files")
-    parser.add_argument("--rebuild_cache", default=False, action="store_true", help="Rebuild cached files from remote resources")
-    # parser.add_argument("--test_req_seq_cache", default=False, action="store_true", help="Test reference sequence cached files")
+    parser.add_argument("--log_file_path", default=None, help="Path to runtime log file output.")
     #
+    # Arguments specific for op == 'upd_ref_seq'
+    parser.add_argument("--ref_chunk_size", default=10, help="Max chunk size for reference sequence updates (for op 'upd_ref_seq')")
+    parser.add_argument("--min_missing", default=0, help="Minimum number of allowed missing reference sequences (for op 'upd_ref_seq')")
+    parser.add_argument("--min_match_primary_percent", default=None, help="Minimum reference sequence match percentage (for op 'upd_ref_seq')")
+    parser.add_argument("--test_mode", default=False, action="store_true", help="Test mode for reference sequence updates (for op 'upd_ref_seq')")
+    #
+    # Arguments buildExdbResources
+    parser.add_argument("--rebuild_all_neighbor_interactions", default=False, action="store_true", help="Rebuild all neighbor interactions from scratch (default is incrementally)")
+    parser.add_argument("--cc_file_prefix", default="cc-full", help="File name discriminator for index sets")
+    parser.add_argument("--cc_url_target", default=None, help="target url for chemical component dictionary resource file (default: None=all public)")
+    parser.add_argument("--bird_url_target", default=None, help="target url for bird dictionary resource file (cc format) (default: None=all public)")
     #
     args = parser.parse_args()
     #
+    try:
+        op, commonD, loadD = processArguments(args)
+    except Exception as err:
+        logger.exception("Argument processing problem %s", str(err))
+        raise ValueError("Argument processing problem") from err
+    #
+    #
+    # Log input arguments
+    loadLogD = {k: v for d in [commonD, loadD] for k, v in d.items() if k != "inputIdCodeList"}
+    logger.info("running load op %r on loadLogD %r:", op, loadLogD)
+    #
+    # Run the operation
+    okR = False
+    exWf = ExDbWorkflow(**commonD)
+    if op in ["etl_chemref", "etl_uniprot_core", "etl_tree_node_lists", "upd_ref_seq"]:
+        okR = exWf.load(op, **loadD)
+    elif op in ["upd_neighbor_interactions", "upd_uniprot_taxonomy", "upd_targets_cofactors", "upd_pubchem", "upd_entry_info", "upd_glycan_idx", "upd_resource_stash"]:
+        okR = exWf.buildExdbResource(op, **loadD)
+    else:
+        logger.error("Unsupported op %r", op)
+    #
+    logger.info("Operation %r completed with status %r", op, okR)
+    #
+    if not okR:
+        logger.error("Operation %r failed with status %r", op, okR)
+        raise ValueError("Operation %r failed" % op)
+
+
+def processArguments(args):
+    # Logging details
+    logFilePath = args.log_file_path
     debugFlag = args.debug
     if debugFlag:
         logger.setLevel(logging.DEBUG)
-    # ----------------------- - ----------------------- - ----------------------- - ----------------------- - ----------------------- -
-    #                                       Configuration Details
-    configPath = args.config_path
-    configName = args.config_name
-    rebuildCache = args.rebuild_cache
-    useCache = not args.rebuild_cache
-
-    if not configPath:
-        configPath = os.getenv("DBLOAD_CONFIG_PATH", None)
-    try:
-        if os.access(configPath, os.R_OK):
-            os.environ["DBLOAD_CONFIG_PATH"] = configPath
-            logger.info("Using configuation path %s (%s)", configPath, configName)
+    else:
+        logger.setLevel(logging.INFO)
+    if logFilePath:
+        logDir = os.path.dirname(logFilePath)
+        if not os.path.isdir(logDir):
+            os.makedirs(logDir)
+        handler = logging.FileHandler(logFilePath, mode="a")
+        if debugFlag:
+            handler.setLevel(logging.DEBUG)
         else:
-            logger.error("Missing or access issue with config file %r", configPath)
-            exit(1)
-        mockTopPath = os.path.join(TOPDIR, "rcsb", "mock-data") if args.mock else None
-        cfgOb = ConfigUtil(configPath=configPath, defaultSectionName=configName, mockTopPath=mockTopPath)
-    except Exception as e:
-        logger.error("Missing or access issue with config file %r with %s", configPath, str(e))
-        exit(1)
-
+            handler.setLevel(logging.INFO)
+        formatter = logging.Formatter("%(asctime)s [%(levelname)s]-%(module)s.%(funcName)s: %(message)s")
+        handler.setFormatter(formatter)
+        logger.addHandler(handler)
     #
-    try:
-        readBackCheck = args.read_back_check
-        tU = TimeUtil()
-        dataSetId = args.data_set_id if args.data_set_id else tU.getCurrentWeekSignature()
-        numProc = int(args.num_proc)
-        chunkSize = int(args.chunk_size)
-        documentLimit = int(args.document_limit) if args.document_limit else None
-        loadType = "full" if args.full else "replace"
-        cachePath = args.cache_path if args.cache_path else "."
+    # Configuration details
+    configPath = args.config_path
+    configName = args.config_name
+    if not (configPath and configName):
+        logger.error("Config path and/or name not provided: %r, %r", configPath, configName)
+        raise ValueError("Config path and/or name not provided: %r, %r" % (configPath, configName))
+    mockTopPath = os.path.join(TOPDIR, "rcsb", "mock-data") if args.mock else None
+    logger.info("Using configuration file %r (section %r)", configPath, configName)
+    cfgOb = ConfigUtil(configPath=configPath, defaultSectionName=configName, mockTopPath=mockTopPath)
+    cfgObTmp = cfgOb.exportConfig()
+    logger.info("Length of config object (%r)", len(cfgObTmp))
+    if len(cfgObTmp) == 0:
+        logger.error("Missing or access issue for config file %r", configPath)
+        raise ValueError("Missing or access issue for config file %r" % configPath)
+    else:
+        del cfgObTmp
+    #
+    # Do any additional argument checking
+    op = args.op
+    if not op:
+        raise ValueError("Must supply a value to '--op' argument")
+    #
+    cachePath = args.cache_path if args.cache_path else "."
+    cachePath = os.path.abspath(cachePath)
+
+    if args.db_type != "mongo":
+        logger.error("Unsupported database type %r (must be 'mongo')", args.db_type)
+        raise ValueError("Unsupported database type %r (must be 'mongo')" % args.db_type)
+
+    # Now collect arguments into dictionaries
+    commonD = {
+        "configPath": configPath,
+        "configName": configName,
+        "cachePath": cachePath,
+        "mockTopPath": mockTopPath,
+        "debugFlag": debugFlag,
+        "rebuildCache": args.rebuild_cache,
+        "providerTypeExclude": args.provider_type_exclude,
+    }
+    loadD = {
+        "loadType": args.load_type,
+        "numProc": int(args.num_proc),
+        "chunkSize": int(args.chunk_size),
+        "maxStepLength": int(args.max_step_length),
+        "dbType": args.db_type,
+        "documentLimit": int(args.document_limit) if args.document_limit else None,
+        "readBackCheck": not args.disable_read_back_check,
+        "rebuildSequenceCache": args.rebuild_sequence_cache,
+        "useFilteredLists": args.use_filtered_tax_list,
+        "refChunkSize": int(args.ref_chunk_size),
+        "minMissing": int(args.min_missing),
+        "minMatchPrimaryPercent": float(args.min_match_primary_percent) if args.min_match_primary_percent else None,
+        "testMode": args.test_mode,
+        "rebuildAllNeighborInteractions": args.rebuild_all_neighbor_interactions,
+        "ccFileNamePrefix": args.cc_file_prefix,
+        "ccUrlTarget": args.cc_url_target,
+        "birdUrlTarget": args.bird_url_target,
+    }
 
-        if args.db_type != "mongo":
-            logger.error("Unsupported database server type %s", args.db_type)
-    except Exception as e:
-        logger.exception("Argument processing problem %s", str(e))
-        parser.print_help(sys.stderr)
-        exit(1)
-    # ----------------------- - ----------------------- - ----------------------- - ----------------------- - ----------------------- -
-    ##
-    #  Rebuild or check resource cache
-    okS = True
-    ok = buildResourceCache(cfgOb, configName, cachePath, rebuildCache=rebuildCache)
-    if not ok:
-        logger.error("Cache rebuild or check failure (rebuild %r) %r", rebuildCache, cachePath)
-        exit(1)
-    # if not useCache:
-    #    buildResourceCache(cfgOb, configName, cachePath, rebuildCache=True)
-    #
-    if args.db_type == "mongo":
-        if args.etl_tree_node_lists:
-            rhw = TreeNodeListWorker(
-                cfgOb, cachePath, numProc=numProc, chunkSize=chunkSize, documentLimit=documentLimit, verbose=debugFlag, readBackCheck=readBackCheck, useCache=useCache
-            )
-            ok = rhw.load(dataSetId, loadType=loadType)
-            okS = loadStatus(rhw.getLoadStatus(), cfgOb, cachePath, readBackCheck=readBackCheck)
-
-        if args.etl_chemref:
-            crw = ChemRefEtlWorker(
-                cfgOb, cachePath, numProc=numProc, chunkSize=chunkSize, documentLimit=documentLimit, verbose=debugFlag, readBackCheck=readBackCheck, useCache=useCache
-            )
-            ok = crw.load(dataSetId, extResource="DrugBank", loadType=loadType)
-            okS = loadStatus(crw.getLoadStatus(), cfgOb, cachePath, readBackCheck=readBackCheck)
-
-        if args.etl_uniprot_core:
-            crw = UniProtCoreEtlWorker(
-                cfgOb, cachePath, numProc=numProc, chunkSize=chunkSize, documentLimit=documentLimit, verbose=debugFlag, readBackCheck=readBackCheck, useCache=useCache
-            )
-            ok = crw.load(dataSetId, extResource="UniProt", loadType=loadType)
-            okS = loadStatus(crw.getLoadStatus(), cfgOb, cachePath, readBackCheck=readBackCheck)
-
-        if args.upd_ref_seq:
-            databaseName = "pdbx_core"
-            collectionName = "pdbx_core_polymer_entity"
-            polymerType = "Protein"
-            ok = doReferenceSequenceUpdate(cfgOb, databaseName, collectionName, polymerType, cachePath, useCache, fetchLimit=documentLimit, refChunkSize=10)
-            okS = ok
-        #
-        logger.info("Operation completed with status %r " % ok and okS)
+    return op, commonD, loadD
 
 
 if __name__ == "__main__":
-    main()
+    try:
+        main()
+    except Exception as e:
+        logger.exception("Run failed %s", str(e))
+        sys.exit(1)
```

### Comparing `rcsb.exdb-1.0/rcsb/exdb/entry/EntryInfoProvider.py` & `rcsb_exdb-1.1/rcsb/exdb/entry/EntryInfoProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/seq/AnnotationExtractor.py` & `rcsb_exdb-1.1/rcsb/exdb/seq/AnnotationExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/seq/LigandNeighborMappingExtractor.py` & `rcsb_exdb-1.1/rcsb/exdb/seq/LigandNeighborMappingExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/seq/LigandNeighborMappingProvider.py` & `rcsb_exdb-1.1/rcsb/exdb/seq/LigandNeighborMappingProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/seq/PolymerEntityExtractor.py` & `rcsb_exdb-1.1/rcsb/exdb/seq/PolymerEntityExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/seq/ReferenceSequenceAnnotationAdapter.py` & `rcsb_exdb-1.1/rcsb/exdb/seq/ReferenceSequenceAnnotationAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/seq/ReferenceSequenceAnnotationProvider.py` & `rcsb_exdb-1.1/rcsb/exdb/seq/ReferenceSequenceAnnotationProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/seq/ReferenceSequenceAssignmentAdapter.py` & `rcsb_exdb-1.1/rcsb/exdb/seq/ReferenceSequenceAssignmentAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/seq/ReferenceSequenceAssignmentProvider.py` & `rcsb_exdb-1.1/rcsb/exdb/seq/ReferenceSequenceAssignmentProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/seq/ReferenceSequenceCacheProvider.py` & `rcsb_exdb-1.1/rcsb/exdb/seq/ReferenceSequenceCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/seq/TaxonomyExtractor.py` & `rcsb_exdb-1.1/rcsb/exdb/seq/TaxonomyExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/seq/UniProtCoreEtlWorker.py` & `rcsb_exdb-1.1/rcsb/exdb/seq/UniProtCoreEtlWorker.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,21 +28,22 @@
 
 logger = logging.getLogger(__name__)
 
 
 class UniProtCoreEtlWorker(object):
     """Prepare and load UniProt 'core' sequence reference data collections."""
 
-    def __init__(self, cfgOb, cachePath, useCache=True, numProc=2, chunkSize=10, readBackCheck=False, documentLimit=None, doValidate=False, verbose=False):
+    def __init__(self, cfgOb, cachePath, useCache=True, numProc=2, chunkSize=10, maxStepLength=2000, readBackCheck=False, documentLimit=None, doValidate=False, verbose=False):
         self.__cfgOb = cfgOb
         self.__cachePath = cachePath
         self.__useCache = useCache
         self.__readBackCheck = readBackCheck
         self.__numProc = numProc
         self.__chunkSize = chunkSize
+        self.__maxStepLength = maxStepLength
         self.__documentLimit = documentLimit
         #
         self.__resourceName = "MONGO_DB"
         self.__verbose = verbose
         self.__statusList = []
         self.__schP = SchemaProvider(self.__cfgOb, self.__cachePath, useCache=self.__useCache)
         self.__docHelper = DocumentDefinitionHelper(cfgOb=self.__cfgOb)
@@ -124,14 +125,15 @@
             #
             dl = DocumentLoader(
                 self.__cfgOb,
                 self.__cachePath,
                 self.__resourceName,
                 numProc=self.__numProc,
                 chunkSize=self.__chunkSize,
+                maxStepLength=self.__maxStepLength,
                 documentLimit=self.__documentLimit,
                 verbose=self.__verbose,
                 readBackCheck=self.__readBackCheck,
             )
             #
             ok = dl.load(databaseName, collectionName, loadType=loadType, documentList=dList, indexAttributeList=indexL, keyNames=None, addValues=addValues)
             okS = self.__updateStatus(updateId, databaseName, collectionName, ok, statusStartTimestamp)
```

### Comparing `rcsb.exdb-1.0/rcsb/exdb/seq/UniProtExtractor.py` & `rcsb_exdb-1.1/rcsb/exdb/seq/UniProtExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/fixtureDictMethodResourceProvider.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/fixtureDictMethodResourceProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/fixturePdbxLoader.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/fixturePdbxLoader.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         self.__cfgOb = ConfigUtil(configPath=configPath, defaultSectionName=configName, mockTopPath=self.__mockTopPath)
         #
         self.__resourceName = "MONGO_DB"
         self.__failedFilePath = os.path.join(HERE, "test-output", "failed-list.txt")
         self.__cachePath = os.path.join(TOPDIR, "CACHE")
         self.__readBackCheck = True
         self.__numProc = 1
-        self.__chunkSize = 5
+        self.__chunkSize = 2
         self.__fileLimit = 38
         self.__documentStyle = "rowwise_by_name_with_cardinality"
         #
         self.__birdChemCompCoreIdList = [
             "PRD_000010",
             "PRD_000060",
             "PRD_000220",
@@ -117,52 +117,52 @@
             "STL",
             "UNK",
             "UNX",
             "UVL",
         ]
         #
         self.__pdbIdList = [
-            "1ah1",
-            "1b5f",
-            "1bmv",
-            "1c58",
-            "1dsr",
-            "1dul",
-            "1kqe",
-            "1o3q",
-            "1sfo",
-            "2hw3",
-            "2hyv",
-            "2osl",
-            "2voo",
-            "2wmg",
-            "3ad7",
-            "3hya",
-            "3iyd",
-            "3mbg",
-            "3rer",
-            "3vd8",
-            "3vfj",
-            "3x11",
-            "3ztj",
-            "4e2o",
-            "4en8",
-            "4mey",
-            "5eu8",
-            "5kds",
-            "5tm0",
-            "5vh4",
-            "5vp2",
-            "6fsz",
-            "6lu7",
-            "6nn7",
-            "6q20",
-            "6rfk",
-            "6rku",
-            "6yrq",
+            "1AH1",
+            "1B5F",
+            "1BMV",
+            "1C58",
+            "1DSR",
+            "1DUL",
+            "1KQE",
+            "1O3Q",
+            "1SFO",
+            "2HW3",
+            "2HYV",
+            "2OSL",
+            "2VOO",
+            "2WMG",
+            "3AD7",
+            "3HYA",
+            "3IYD",
+            "3MBG",
+            "3RER",
+            "3VD8",
+            "3VFJ",
+            "3X11",
+            "3ZTJ",
+            "4E2O",
+            "4EN8",
+            "4MEY",
+            "5EU8",
+            "5KDS",
+            # "5TM0",
+            "5VH4",
+            # "5VP2",
+            # "6FSZ",
+            "6LU7",
+            "6NN7",
+            # "6Q20",
+            "6RFK",
+            "6RKU",
+            "6YRQ",
         ]
         self.__ldList = [
             {
                 "databaseName": "bird_chem_comp_core",
                 "collectionNameList": None,
                 "loadType": "full",
                 "mergeContentTypes": None,
@@ -209,18 +209,20 @@
     #         h1 = uId[-6:-4]
     #         oPath = os.path.join(self.__cachePath, "computed-models", h1, h2, h3, fn)
     #         fU.put(iPath, oPath)
 
     def testPdbxLoader(self):
         #
         for ld in self.__ldList:
-            self.__pdbxLoaderWrapper(**ld)
+            ok = self.__pdbxLoaderWrapper(**ld)
+            self.assertTrue(ok)
 
     def __pdbxLoaderWrapper(self, **kwargs):
         """Wrapper for the PDBx loader module"""
+        ok = False
         try:
             logger.info("Loading %s", kwargs["databaseName"])
             mw = PdbxLoader(
                 self.__cfgOb,
                 cachePath=self.__cachePath,
                 resourceName=self.__resourceName,
                 numProc=self.__numProc,
@@ -253,14 +255,15 @@
             )
             self.assertTrue(ok)
             ok = self.__loadStatus(mw.getLoadStatus())
             self.assertTrue(ok)
         except Exception as e:
             logger.exception("Failing with %s", str(e))
             self.fail()
+        return ok
 
     def __loadStatus(self, statusList):
         sectionName = "data_exchange_configuration"
         dl = DocumentLoader(
             self.__cfgOb,
             self.__cachePath,
             resourceName=self.__resourceName,
```

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testAnnotationExtractor.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testAnnotationExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testBranchedEntityExtractor.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testBranchedEntityExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testChemRefLoader.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testChemRefLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testChemRefMappingProvider.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testChemRefMappingProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testCitationAdapter.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testCitationAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testCitationExtractor.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testCitationExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testCitationUtils.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testCitationUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testEntryInfoEtlWorkflow.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testEntryInfoEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testEntryInfoProvider.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testEntryInfoProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testExDbWorkflow.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testExDbWorkflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,16 @@
         logger.info("Maximum resident memory size %.4f %s", rusageMax / 10 ** 6, unitS)
         endTime = time.time()
         logger.info("Completed %s at %s (%.4f seconds)", self.id(), time.strftime("%Y %m %d %H:%M:%S", time.localtime()), endTime - self.__startTime)
 
     def testExDbLoaderWorkflows(self):
         """Test run workflow steps ..."""
         try:
-            opL = ["etl_chemref", "upd_ref_seq", "etl_tree_node_lists"]
+            # opL = ["etl_chemref", "upd_ref_seq", "etl_tree_node_lists"]
+            opL = ["etl_chemref", "etl_tree_node_lists"]
             rlWf = ExDbWorkflow(**self.__commonD)
             for op in opL:
                 ok = rlWf.load(op, **self.__loadCommonD)
                 self.assertTrue(ok)
         except Exception as e:
             logger.exception("Failing with %s", str(e))
             self.fail()
```

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testGlycanEtlWorkflow.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testGlycanEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testGlycanProvider.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testGlycanProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testGlycanUtils.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testGlycanUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testLigandNeighborMappingProvider.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testLigandNeighborMappingProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testObjectExtractor.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testObjectExtractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
                 selectionQuery={"rcsb_accession_info.initial_release_date": {"$gt": tD}},
                 selectionList=["rcsb_id", "rcsb_accession_info"],
             )
             eD = obEx.getObjects()
             eCount = obEx.getCount()
             logger.info("Entry count is %d", eCount)
             logger.info("Entries are %r", list(eD.keys()))
-            self.assertGreaterEqual(eCount, 6)
+            self.assertGreaterEqual(eCount, 5)
         except Exception as e:
             logger.exception("Failing with %s", str(e))
             self.fail()
 
     def testExtractEntries(self):
         """Test case - extract entries"""
         try:
```

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testObjectTransformer.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testObjectTransformer.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testObjectUpdater.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testObjectUpdater.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testPolymerEntityExtractor.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testPolymerEntityExtractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     def testGetProteinEntityDetails(self):
         """Test case - get protein entity sequences and essential details"""
         try:
             pEx = PolymerEntityExtractor(self.__cfgOb)
             pD, _ = pEx.getProteinSequenceDetails()
             #
-            self.assertGreaterEqual(len(pD), 100)
+            self.assertGreaterEqual(len(pD), 70)
             logger.info("Polymer entity count %d", len(pD))
         except Exception as e:
             logger.exception("Failing with %s", str(e))
             self.fail()
 
     def testExportProteinEntityFasta(self):
         """Test case - export protein entity sequence Fasta"""
```

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testPubChemDataCacheProvider.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testPubChemDataCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testPubChemEtlWorkflow.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testPubChemEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testPubChemEtlWrapper.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testPubChemEtlWrapper.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testPubChemIndexCacheProvider.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testPubChemIndexCacheProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testReferenceSequenceAnnotationAdapter.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testReferenceSequenceAnnotationAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapter.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapterValidate.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testReferenceSequenceAssignmentAdapterValidate.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testReferenceSequenceAssignmentProvider.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testReferenceSequenceAssignmentProvider.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,24 +87,24 @@
                 cacheKwargs=self.__testEntityCacheKwargs,
                 fetchLimit=self.__fetchLimitTest,
                 siftsAbbreviated="TEST",
             )
             ok = rsaP.testCache()
             self.assertTrue(ok)
             numRef = rsaP.getRefDataCount()
-            self.assertGreaterEqual(numRef, 90)
+            self.assertGreaterEqual(numRef, 49)
             #
             # ---  Reload from cache ---
             rsaP = ReferenceSequenceAssignmentProvider(
                 self.__cfgOb, referenceDatabaseName="UniProt", useCache=True, cachePath=self.__cachePath, cacheKwargs=self.__testEntityCacheKwargs
             )
             ok = rsaP.testCache()
             self.assertTrue(ok)
             numRef = rsaP.getRefDataCount()
-            self.assertGreaterEqual(numRef, 90)
+            self.assertGreaterEqual(numRef, 49)
         except Exception as e:
             logger.exception("Failing with %s", str(e))
             self.fail()
 
 
 def referenceSequenceAssignmentProviderSuite():
     suiteSelect = unittest.TestSuite()
```

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testReferenceSequenceCacheProvider.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testReferenceSequenceCacheProvider.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,22 +66,22 @@
             collectionName = "pdbx_core_polymer_entity"
             polymerType = "Protein"
             #
             rsaP = ReferenceSequenceCacheProvider(self.__cfgOb, databaseName, collectionName, polymerType, maxChunkSize=50, numProc=2, expireDays=0)
             ok = rsaP.testCache()
             self.assertTrue(ok)
             numRef = rsaP.getRefDataCount()
-            self.assertGreaterEqual(numRef, 90)
+            self.assertGreaterEqual(numRef, 49)
             #
             # ---  Reload from cache ---
             rsaP = ReferenceSequenceCacheProvider(self.__cfgOb, databaseName, collectionName, polymerType, maxChunkSize=50, numProc=2, expireDays=14)
             ok = rsaP.testCache()
             self.assertTrue(ok)
             numRef = rsaP.getRefDataCount()
-            self.assertGreaterEqual(numRef, 90)
+            self.assertGreaterEqual(numRef, 49)
         except Exception as e:
             logger.exception("Failing with %s", str(e))
             self.fail()
 
 
 def referenceSequenceCacheProviderSuite():
     suiteSelect = unittest.TestSuite()
```

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testTaxonomyExtractor.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testTaxonomyExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testTreeNodeListWorker.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testTreeNodeListWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testUniProtCoreEtlWorker.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testUniProtCoreEtlWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tests/testUniProtExtractor.py` & `rcsb_exdb-1.1/rcsb/exdb/tests/testUniProtExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/tree/TreeNodeListWorker.py` & `rcsb_exdb-1.1/rcsb/exdb/tree/TreeNodeListWorker.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,20 +35,21 @@
 
 logger = logging.getLogger(__name__)
 
 
 class TreeNodeListWorker(object):
     """Prepare and load repository holdings and repository update data."""
 
-    def __init__(self, cfgOb, cachePath, numProc=1, chunkSize=10, readBackCheck=False, documentLimit=None, verbose=False, useCache=False, useFilteredLists=False):
+    def __init__(self, cfgOb, cachePath, numProc=1, chunkSize=10, maxStepLength=4000, readBackCheck=False, documentLimit=None, verbose=False, useCache=False, useFilteredLists=False):
         self.__cfgOb = cfgOb
         self.__cachePath = os.path.abspath(cachePath)
         self.__readBackCheck = readBackCheck
         self.__numProc = numProc
         self.__chunkSize = chunkSize
+        self.__maxStepLength = maxStepLength
         self.__documentLimit = documentLimit
         self.__resourceName = "MONGO_DB"
         self.__filterType = "assign-dates"
         self.__verbose = verbose
         self.__statusList = []
         self.__useCache = useCache
         self.__useFilteredLists = useFilteredLists
@@ -111,14 +112,15 @@
             statusStartTimestamp = desp.setStartTime()
             dl = DocumentLoader(
                 self.__cfgOb,
                 self.__cachePath,
                 self.__resourceName,
                 numProc=self.__numProc,
                 chunkSize=self.__chunkSize,
+                maxStepLength=self.__maxStepLength,
                 documentLimit=self.__documentLimit,
                 verbose=self.__verbose,
                 readBackCheck=self.__readBackCheck,
             )
             #
             databaseName = "tree_node_lists"
             # collectionVersion = self.__cfgOb.get("COLLECTION_VERSION_STRING", sectionName=sectionName)
```

### Comparing `rcsb.exdb-1.0/rcsb/exdb/utils/ObjectExtractor.py` & `rcsb_exdb-1.1/rcsb/exdb/utils/ObjectExtractor.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/utils/ObjectTransformer.py` & `rcsb_exdb-1.1/rcsb/exdb/utils/ObjectTransformer.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/utils/ObjectUpdater.py` & `rcsb_exdb-1.1/rcsb/exdb/utils/ObjectUpdater.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/utils/ObjectValidator.py` & `rcsb_exdb-1.1/rcsb/exdb/utils/ObjectValidator.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/wf/EntryInfoEtlWorkflow.py` & `rcsb_exdb-1.1/rcsb/exdb/wf/EntryInfoEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/wf/GlycanEtlWorkflow.py` & `rcsb_exdb-1.1/rcsb/exdb/wf/GlycanEtlWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/rcsb/exdb/wf/PubChemEtlWorkflow.py` & `rcsb_exdb-1.1/rcsb/exdb/wf/PubChemEtlWorkflow.py`

 * *Files 16% similar despite different names*

```diff
@@ -177,17 +177,20 @@
                 birdUrlTarget=birdUrlTarget,
                 ccFileNamePrefix=ccFileNamePrefix,
                 exportPath=exportPath,
                 rebuildChemIndices=rebuildChemIndices,
                 numProcChemComp=numProcChemComp,
                 numProc=numProc,
             )
+            logger.info("updateIndex completed with status %r", ok1)
             ok2 = pcewP.dump(contentType="index")
+            logger.info("dump completed with status %r", ok2)
             if useGit or useStash:
                 ok3 = pcewP.toStash(contentType="index", useStash=useStash, useGit=useGit)
+                logger.info("toStash completed with status %r", ok3)
             else:
                 ok3 = True
         except Exception as e:
             logger.exception("Failing with %s", str(e))
         #
         return ok1 and ok2 and ok3
 
@@ -208,24 +211,30 @@
             #  --
             numProc = kwargs.get("numProc", 2)
             useStash = kwargs.get("useStash", True)
             useGit = kwargs.get("useGit", False)
             #
             pcewP = PubChemEtlWrapper(self.__cfgOb, self.__cachePath, stashRemotePrefix=self.__stashRemotePrefix)
             ok1 = pcewP.updateMatchedData(numProc=numProc)
+            logger.info("PubChemEtlWrapper.updateMatchedData completed with status %r", ok1)
             ok2 = pcewP.dump(contentType="data")
+            logger.info("PubChemEtlWrapper.dump 'data' completed with status %r", ok2)
             if useGit or useStash:
                 ok3 = pcewP.toStash(contentType="data", useStash=useStash, useGit=useGit)
+                logger.info("PubChemEtlWrapper.toStash 'data' completed with status %r", ok3)
             else:
                 ok3 = True
             #
             ok4 = pcewP.updateIdentifiers()
+            logger.info("PubChemEtlWrapper.updateIdentifiers completed with status %r", ok4)
             ok5 = pcewP.dump(contentType="identifiers")
+            logger.info("PubChemEtlWrapper.dump 'identifiers' completed with status %r", ok5)
             if useGit or useStash:
                 ok6 = pcewP.toStash(contentType="identifiers", useStash=useStash, useGit=useGit)
+                logger.info("PubChemEtlWrapper.toStash 'identifiers' completed with status %r", ok6)
             else:
                 ok6 = True
             #
         except Exception as e:
             logger.exception("Failing with %s", str(e))
         #
         return ok1 and ok2 and ok3 and ok4 and ok5 and ok6
```

### Comparing `rcsb.exdb-1.0/rcsb.exdb.egg-info/PKG-INFO` & `rcsb_exdb-1.1/rcsb.exdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.exdb
-Version: 1.0
+Version: 1.1
 Summary: RCSB Python ExDB data extraction and loading workflows
 Home-page: https://github.com/rcsb/py-rcsb_exdb
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -26,14 +26,15 @@
 Requires-Dist: rcsb.utils.config>=0.35
 Requires-Dist: rcsb.utils.ec>=0.22
 Requires-Dist: rcsb.utils.go>=0.17
 Requires-Dist: rcsb.utils.seq>=0.63
 Requires-Dist: rcsb.utils.struct>=0.37
 Requires-Dist: rcsb.utils.taxonomy>=0.39
 Requires-Dist: rcsb.utils.dictionary>=0.71
+Requires-Dist: rcsb.workflow>=0.42
 Requires-Dist: statistics; python_version < "3.0"
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 
 # py-rcsb_exdb
```

### Comparing `rcsb.exdb-1.0/rcsb.exdb.egg-info/SOURCES.txt` & `rcsb_exdb-1.1/rcsb.exdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.exdb-1.0/setup.py` & `rcsb_exdb-1.1/setup.py`

 * *Files identical despite different names*

