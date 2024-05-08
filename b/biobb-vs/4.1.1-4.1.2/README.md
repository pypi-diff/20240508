# Comparing `tmp/biobb_vs-4.1.1.tar.gz` & `tmp/biobb_vs-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_vs-4.1.1.tar", last modified: Thu Sep 14 10:14:10 2023, max compression
+gzip compressed data, was "biobb_vs-4.1.2.tar", last modified: Wed May  8 08:10:00 2024, max compression
```

## Comparing `biobb_vs-4.1.1.tar` & `biobb_vs-4.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-14 10:14:10.140351 biobb_vs-4.1.1/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11358 2022-05-26 11:36:06.000000 biobb_vs-4.1.1/LICENSE
--rw-r--r--   0 gbayarri (1147421021) 1791188573     6176 2023-09-14 10:14:10.140187 biobb_vs-4.1.1/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573     5316 2023-09-14 10:11:06.000000 biobb_vs-4.1.1/README.md
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-14 10:14:10.136181 biobb_vs-4.1.1/biobb_vs/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       79 2023-09-14 10:10:54.000000 biobb_vs-4.1.1/biobb_vs/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-14 10:14:10.138026 biobb_vs-4.1.1/biobb_vs/fpocket/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       79 2023-04-13 09:46:16.000000 biobb_vs-4.1.1/biobb_vs/fpocket/__init__.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     6282 2023-04-13 09:41:05.000000 biobb_vs-4.1.1/biobb_vs/fpocket/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10117 2023-04-13 09:43:47.000000 biobb_vs-4.1.1/biobb_vs/fpocket/fpocket_filter.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9781 2023-04-13 09:46:06.000000 biobb_vs-4.1.1/biobb_vs/fpocket/fpocket_run.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7531 2023-04-13 09:48:19.000000 biobb_vs-4.1.1/biobb_vs/fpocket/fpocket_select.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-14 10:14:10.138264 biobb_vs-4.1.1/biobb_vs/test/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-05-26 11:36:06.000000 biobb_vs-4.1.1/biobb_vs/test/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-14 10:14:10.139338 biobb_vs-4.1.1/biobb_vs/utils/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       87 2023-04-13 09:46:25.000000 biobb_vs-4.1.1/biobb_vs/utils/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    18330 2023-09-14 09:20:39.000000 biobb_vs-4.1.1/biobb_vs/utils/bindingsite.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9027 2023-04-13 10:01:05.000000 biobb_vs-4.1.1/biobb_vs/utils/box.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11168 2023-09-14 09:21:33.000000 biobb_vs-4.1.1/biobb_vs/utils/box_residues.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573    42011 2023-09-14 09:21:19.000000 biobb_vs-4.1.1/biobb_vs/utils/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7590 2023-09-14 09:21:44.000000 biobb_vs-4.1.1/biobb_vs/utils/extract_model_pdbqt.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-14 10:14:10.139953 biobb_vs-4.1.1/biobb_vs/vina/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       46 2023-04-13 09:46:34.000000 biobb_vs-4.1.1/biobb_vs/vina/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10744 2023-04-13 10:20:01.000000 biobb_vs-4.1.1/biobb_vs/vina/autodock_vina_run.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     2882 2023-04-13 10:20:42.000000 biobb_vs-4.1.1/biobb_vs/vina/common.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-14 10:14:10.136913 biobb_vs-4.1.1/biobb_vs.egg-info/
--rw-r--r--   0 gbayarri (1147421021) 1791188573     6176 2023-09-14 10:14:10.000000 biobb_vs-4.1.1/biobb_vs.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573      683 2023-09-14 10:14:10.000000 biobb_vs-4.1.1/biobb_vs.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2023-09-14 10:14:10.000000 biobb_vs-4.1.1/biobb_vs.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573      417 2023-09-14 10:14:10.000000 biobb_vs-4.1.1/biobb_vs.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       20 2023-09-14 10:14:10.000000 biobb_vs-4.1.1/biobb_vs.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573        9 2023-09-14 10:14:10.000000 biobb_vs-4.1.1/biobb_vs.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2023-09-14 10:14:10.140398 biobb_vs-4.1.1/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1756 2023-09-14 10:08:37.000000 biobb_vs-4.1.1/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-08 08:10:00.736750 biobb_vs-4.1.2/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11358 2022-05-26 11:36:06.000000 biobb_vs-4.1.2/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6750 2024-05-08 08:10:00.736521 biobb_vs-4.1.2/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5855 2024-05-08 08:01:19.000000 biobb_vs-4.1.2/README.md
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-08 08:10:00.733464 biobb_vs-4.1.2/biobb_vs/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       79 2024-05-08 08:00:58.000000 biobb_vs-4.1.2/biobb_vs/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-08 08:10:00.734900 biobb_vs-4.1.2/biobb_vs/fpocket/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       79 2023-04-13 09:46:16.000000 biobb_vs-4.1.2/biobb_vs/fpocket/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6271 2024-05-08 08:07:28.000000 biobb_vs-4.1.2/biobb_vs/fpocket/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    10117 2023-04-13 09:43:47.000000 biobb_vs-4.1.2/biobb_vs/fpocket/fpocket_filter.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9777 2024-05-07 13:49:44.000000 biobb_vs-4.1.2/biobb_vs/fpocket/fpocket_run.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7531 2023-04-13 09:48:19.000000 biobb_vs-4.1.2/biobb_vs/fpocket/fpocket_select.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-08 08:10:00.735021 biobb_vs-4.1.2/biobb_vs/test/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2022-05-26 11:36:06.000000 biobb_vs-4.1.2/biobb_vs/test/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-08 08:10:00.735884 biobb_vs-4.1.2/biobb_vs/utils/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       87 2023-04-13 09:46:25.000000 biobb_vs-4.1.2/biobb_vs/utils/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    18234 2024-05-08 07:48:18.000000 biobb_vs-4.1.2/biobb_vs/utils/bindingsite.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9027 2023-04-13 10:01:05.000000 biobb_vs-4.1.2/biobb_vs/utils/box.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11168 2023-09-14 09:21:33.000000 biobb_vs-4.1.2/biobb_vs/utils/box_residues.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    42086 2024-05-07 15:02:53.000000 biobb_vs-4.1.2/biobb_vs/utils/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7590 2023-09-14 09:21:44.000000 biobb_vs-4.1.2/biobb_vs/utils/extract_model_pdbqt.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-08 08:10:00.736262 biobb_vs-4.1.2/biobb_vs/vina/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       46 2023-04-13 09:46:34.000000 biobb_vs-4.1.2/biobb_vs/vina/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11684 2024-04-02 08:03:45.000000 biobb_vs-4.1.2/biobb_vs/vina/autodock_vina_run.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2882 2023-04-13 10:20:42.000000 biobb_vs-4.1.2/biobb_vs/vina/common.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-08 08:10:00.734241 biobb_vs-4.1.2/biobb_vs.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6750 2024-05-08 08:10:00.000000 biobb_vs-4.1.2/biobb_vs.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      683 2024-05-08 08:10:00.000000 biobb_vs-4.1.2/biobb_vs.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2024-05-08 08:10:00.000000 biobb_vs-4.1.2/biobb_vs.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      417 2024-05-08 08:10:00.000000 biobb_vs-4.1.2/biobb_vs.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2024-05-08 08:10:00.000000 biobb_vs-4.1.2/biobb_vs.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        9 2024-05-08 08:10:00.000000 biobb_vs-4.1.2/biobb_vs.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2024-05-08 08:10:00.736797 biobb_vs-4.1.2/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1756 2024-05-08 08:00:29.000000 biobb_vs-4.1.2/setup.py
```

### Comparing `biobb_vs-4.1.1/LICENSE` & `biobb_vs-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_vs-4.1.1/PKG-INFO` & `biobb_vs-4.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: biobb_vs
-Version: 4.1.1
+Version: 4.1.2
 Summary: Biobb_vs is the Biobb module collection to perform virtual screening studies.
 Home-page: https://github.com/bioexcel/biobb_vs
 Author: Biobb developers
 Author-email: genis.bayarri@irbbarcelona.org
-Project-URL: Documentation, http://biobb_vs.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-vs.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: biobb_common==4.1.0
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_vs?label=Version)](https://GitHub.com/bioexcel/biobb_vs/tags/)
 [![](https://img.shields.io/pypi/v/biobb-vs.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-vs/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_vs?label=Conda)](https://anaconda.org/bioconda/biobb_vs)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_vs?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_vs)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_vs?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_vs:4.1.1--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_vs:4.1.2--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_vs)
 [![](https://img.shields.io/pypi/pyversions/biobb-vs.svg?label=Python%20Versions)](https://pypi.org/project/biobb-vs/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_vs)
 
 [![](https://readthedocs.org/projects/biobb-vs/badge/?version=latest&label=Docs)](https://biobb-vs.readthedocs.io/en/latest/?badge=latest)
@@ -39,85 +40,92 @@
 
 [![](https://docs.bioexcel.eu/biobb_vs/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_vs/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_vs/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_vs/coverage/)
 [![](https://docs.bioexcel.eu/biobb_vs/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_vs/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_vs?label=Last%20Commit)](https://github.com/bioexcel/biobb_vs/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_vs.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_vs/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_vs
 
 ### Introduction
 Biobb_vs is the Biobb module collection to perform virtual screening studies.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_vs.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-vs.readthedocs.io/en/latest/).
 
 > At the time of publishing the current version, **autodock_vina has not been compiled for the new ARM mac M1/M2 chips**. So the vina.autodock_vina_run only work in these computers through docker containers.
 
 ### Version
-v4.1.1 2023.3
+v4.1.2 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
 
-        pip install "biobb_vs>=4.1.1"
+        pip install "biobb_vs>=4.1.2"
 
 
 * Usage: [Python API documentation](https://biobb-vs.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_vs>=4.1.1"
+        conda install -c bioconda "biobb_vs>=4.1.2"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-vs.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-vs.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_vs:4.1.1--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_vs:4.1.2--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_vs:4.1.1--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_vs:4.1.2--pyhdfd78af_0 <command>
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_vs.sif https://depot.galaxyproject.org/singularity/biobb_vs:4.1.1--pyhdfd78af_0
+        singularity pull --name biobb_vs.sif https://depot.galaxyproject.org/singularity/biobb_vs:4.1.2--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_vs.sif <command>
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-vs.readthedocs.io/en/latest/command_line.html).
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_vs-4.1.1/README.md` & `biobb_vs-4.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_vs?label=Version)](https://GitHub.com/bioexcel/biobb_vs/tags/)
 [![](https://img.shields.io/pypi/v/biobb-vs.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-vs/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_vs?label=Conda)](https://anaconda.org/bioconda/biobb_vs)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_vs?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_vs)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_vs?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_vs:4.1.1--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_vs:4.1.2--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_vs)
 [![](https://img.shields.io/pypi/pyversions/biobb-vs.svg?label=Python%20Versions)](https://pypi.org/project/biobb-vs/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_vs)
 
 [![](https://readthedocs.org/projects/biobb-vs/badge/?version=latest&label=Docs)](https://biobb-vs.readthedocs.io/en/latest/?badge=latest)
@@ -18,85 +18,92 @@
 
 [![](https://docs.bioexcel.eu/biobb_vs/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_vs/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_vs/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_vs/coverage/)
 [![](https://docs.bioexcel.eu/biobb_vs/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_vs/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_vs?label=Last%20Commit)](https://github.com/bioexcel/biobb_vs/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_vs.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_vs/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_vs
 
 ### Introduction
 Biobb_vs is the Biobb module collection to perform virtual screening studies.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_vs.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-vs.readthedocs.io/en/latest/).
 
 > At the time of publishing the current version, **autodock_vina has not been compiled for the new ARM mac M1/M2 chips**. So the vina.autodock_vina_run only work in these computers through docker containers.
 
 ### Version
-v4.1.1 2023.3
+v4.1.2 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
 
-        pip install "biobb_vs>=4.1.1"
+        pip install "biobb_vs>=4.1.2"
 
 
 * Usage: [Python API documentation](https://biobb-vs.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_vs>=4.1.1"
+        conda install -c bioconda "biobb_vs>=4.1.2"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-vs.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-vs.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_vs:4.1.1--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_vs:4.1.2--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_vs:4.1.1--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_vs:4.1.2--pyhdfd78af_0 <command>
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_vs.sif https://depot.galaxyproject.org/singularity/biobb_vs:4.1.1--pyhdfd78af_0
+        singularity pull --name biobb_vs.sif https://depot.galaxyproject.org/singularity/biobb_vs:4.1.2--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_vs.sif <command>
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-vs.readthedocs.io/en/latest/command_line.html).
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_vs-4.1.1/biobb_vs/fpocket/common.py` & `biobb_vs-4.1.2/biobb_vs/fpocket/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 # CHECK PROPERTIES
 
 def check_range(name, property, values, out_log, classname):
     """ Checks the format of a range for fpocket_filter """
 
-    if not type(property) == list or len(property) != 2 or not all(isinstance(n, int) or isinstance(n, float) for n in property):
+    if not isinstance(property, list) or len(property) != 2 or not all(isinstance(n, (int, float)) for n in property):
         fu.log(classname + ': Incorrect format for %s property, exiting' % name, out_log)
         raise SystemExit(classname + ': Incorrect format for %s property, exiting' % name)
 
     if property[0] < values[0] or property[1] > values[1]:
         fu.log(classname + ': %s is out of [%s] range, exiting' % (name, ', '.join(str(v) for v in values)), out_log)
         raise SystemExit(classname + ': %s is out of [%s] range, exiting' % (name, ', '.join(str(v) for v in values)))
```

### Comparing `biobb_vs-4.1.1/biobb_vs/fpocket/fpocket_filter.py` & `biobb_vs-4.1.2/biobb_vs/fpocket/fpocket_filter.py`

 * *Files identical despite different names*

### Comparing `biobb_vs-4.1.1/biobb_vs/fpocket/fpocket_run.py` & `biobb_vs-4.1.2/biobb_vs/fpocket/fpocket_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                     output_pockets_zip='/path/to/newPockets.zip',
                     output_summary='/path/to/newSummary.json',
                     properties=prop)
 
     Info:
         * wrapped_software:
             * name: fpocket
-            * version: >=3.1.4.2
+            * version: ==4.1
             * license: MIT
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
```

### Comparing `biobb_vs-4.1.1/biobb_vs/fpocket/fpocket_select.py` & `biobb_vs-4.1.2/biobb_vs/fpocket/fpocket_select.py`

 * *Files identical despite different names*

### Comparing `biobb_vs-4.1.1/biobb_vs/utils/bindingsite.py` & `biobb_vs-4.1.2/biobb_vs/utils/bindingsite.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,27 +33,27 @@
         input_pdb_path (str): Path to the PDB structure where the binding site is to be found. File type: input. `Sample file <https://github.com/bioexcel/biobb_vs/raw/master/biobb_vs/test/data/utils/bindingsite.pdb>`_. Accepted formats: pdb (edam:format_1476).
         input_clusters_zip (str): Path to the ZIP file with all the PDB members of the identity cluster. File type: input. `Sample file <https://github.com/bioexcel/biobb_vs/raw/master/biobb_vs/test/data/utils/bindingsite.zip>`_. Accepted formats: zip (edam:format_3987).
         output_pdb_path (str): Path to the PDB containig the residues belonging to the binding site. File type: output. `Sample file <https://github.com/bioexcel/biobb_vs/raw/master/biobb_vs/test/reference/utils/ref_output_bindingsite.pdb>`_. Accepted formats: pdb (edam:format_1476).
         properties (dic - Python dictionary object containing the tool parameters, not input/output files):
             * **ligand** (*str*) - (None) Ligand to be found in the protein structure. If no ligand provided, the largest one will be selected, if more than one.
             * **radius** (*float*) - (5.0) [0.1~1000|0.1] Cut-off distance (Ångstroms) around ligand atoms to consider a protein atom as a binding site atom.
             * **max_num_ligands** (*int*) - (15) [0~1000|1] Total number of superimposed ligands to be extracted from the identity cluster. For populated clusters, the restriction avoids to superimpose redundant structures. If 0, all ligands extracted will be considered.
-            * **matrix_name** (*str*) - ("blosum62") Substitution matrices for use in alignments. Values: benner6, benner22, benner74, blosum100, blosum30, blosum35, blosum40, blosum45, blosum50, blosum55, blosum60, blosum62, blosum65, blosum70, blosum75, blosum80, blosum85, blosum90, blosum95, feng, fitch, genetic, gonnet, grant, ident, johnson, levin, mclach, miyata, nwsgappep, pam120, pam180, pam250, pam30, pam300, pam60, pam90, rao, risler, structure.
+            * **matrix_name** (*str*) - ("BLOSUM62") Substitution matrices for use in alignments. Values: BENNER22, BENNER6, BENNER74, BLASTN, BLASTP, BLOSUM45, BLOSUM50, BLOSUM62, BLOSUM80, BLOSUM90, DAYHOFF, FENG, GENETIC, GONNET1992, HOXD70, JOHNSON, JONES, LEVIN, MCLACHLAN, MDM78, MEGABLAST, NUC.4.4, PAM250, PAM30, PAM70, RAO, RISLER, SCHNEIDER, STR, TRANS.
             * **gap_open** (*float*) - (-10.0) [-1000~1000|0.1] Gap open penalty.
             * **gap_extend** (*float*) - (-0.5) [-1000~1000|0.1] Gap extend penalty.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
             from biobb_vs.utils.bindingsite import bindingsite
             prop = {
                 'ligand': 'PGA',
-                'matrix_name': 'blosum62',
+                'matrix_name': 'BLOSUM62',
                 'gap_open': -10.0,
                 'gap_extend': -0.5,
                 'max_num_ligands': 15,
                 'radius': 5
             }
             bindingsite(input_pdb_path='/path/to/myStructure.pdb',
                         input_clusters_zip='/path/to/myCluster.zip',
@@ -85,15 +85,15 @@
             "out": {"output_pdb_path": output_pdb_path}
         }
 
         # Properties specific for BB
         self.ligand = properties.get('ligand', None)
         self.radius = float(properties.get('radius', 5.0))
         self.max_num_ligands = properties.get('max_num_ligands', 15)
-        self.matrix_name = properties.get('matrix_name', 'blosum62')
+        self.matrix_name = properties.get('matrix_name', 'BLOSUM62')
         self.gap_open = properties.get('gap_open', -10.0)
         self.gap_extend = properties.get('gap_extend', -0.5)
         self.properties = properties
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
```

### Comparing `biobb_vs-4.1.1/biobb_vs/utils/box.py` & `biobb_vs-4.1.2/biobb_vs/utils/box.py`

 * *Files identical despite different names*

### Comparing `biobb_vs-4.1.1/biobb_vs/utils/box_residues.py` & `biobb_vs-4.1.2/biobb_vs/utils/box_residues.py`

 * *Files identical despite different names*

### Comparing `biobb_vs-4.1.1/biobb_vs/utils/common.py` & `biobb_vs-4.1.2/biobb_vs/utils/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,16 @@
     warnings.simplefilter("ignore", BiopythonDeprecationWarning)
     import Bio.PDB
     import Bio.pairwise2
     try:
         import Bio.SubsMat.MatrixInfo
     except ImportError:
         import Bio.Align.substitution_matrices
-    from Bio.Data.SCOPData import protein_letters_3to1 as prot_one_letter
+    # from Bio.Data.SCOPData import protein_letters_3to1 as prot_one_letter
+    from Bio.Data.PDBData import protein_letters_3to1 as prot_one_letter
 
 
 # CHECK PARAMETERS
 
 def check_input_path(path, argument, out_log, classname):
     """ Checks input file """
     if not Path(path).exists():
@@ -86,15 +87,15 @@
 
     seq = []
     for nuc in structure:
         seq.append(nuc)
     return seq
 
 
-def align_sequences(seqA, seqB, matrix_name='blosum62', gap_open=-10.0, gap_extend=-0.5):
+def align_sequences(seqA, seqB, matrix_name='BLOSUM62', gap_open=-10.0, gap_extend=-0.5):
     """
     Performs a global pairwise alignment between two sequences using the Needleman-Wunsch algorithm as implemented in Biopython.
     Returns the alignment and the residue mapping between both original sequences.
     """
 
     # seq list to seq string
     sequence_A = ''.join([i[1] for i in seqA])
```

### Comparing `biobb_vs-4.1.1/biobb_vs/utils/extract_model_pdbqt.py` & `biobb_vs-4.1.2/biobb_vs/utils/extract_model_pdbqt.py`

 * *Files identical despite different names*

### Comparing `biobb_vs-4.1.1/biobb_vs/vina/autodock_vina_run.py` & `biobb_vs-4.1.2/biobb_vs/vina/autodock_vina_run.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,18 @@
         input_ligand_pdbqt_path (str): Path to the input PDBQT ligand. File type: input. `Sample file <https://github.com/bioexcel/biobb_vs/raw/master/biobb_vs/test/data/vina/vina_ligand.pdbqt>`_. Accepted formats: pdbqt (edam:format_1476).
         input_receptor_pdbqt_path (str): Path to the input PDBQT receptor. File type: input. `Sample file <https://github.com/bioexcel/biobb_vs/raw/master/biobb_vs/test/data/vina/vina_receptor.pdbqt>`_. Accepted formats: pdbqt (edam:format_1476).
         input_box_path (str): Path to the PDB containig the residues belonging to the binding site. File type: input. `Sample file <https://github.com/bioexcel/biobb_vs/raw/master/biobb_vs/test/data/vina/vina_box.pdb>`_. Accepted formats: pdb (edam:format_1476).
         output_pdbqt_path (str): Path to the output PDBQT file. File type: output. `Sample file <https://github.com/bioexcel/biobb_vs/raw/master/biobb_vs/test/reference/vina/ref_output_vina.pdbqt>`_. Accepted formats: pdbqt (edam:format_1476).
         output_log_path (str) (Optional): Path to the log file. File type: output. `Sample file <https://github.com/bioexcel/biobb_vs/raw/master/biobb_vs/test/reference/vina/ref_output_vina.log>`_. Accepted formats: log (edam:format_2330).
         properties (dic - Python dictionary object containing the tool parameters, not input/output files):
             * **cpu** (*int*) - (1) [1~1000|1] the number of CPUs to use.
+            * **exhaustiveness** (*int*) - (8) [1~10000|1] exhaustiveness of the global search (roughly proportional to time).
+            * **num_modes** (*int*) - (9) [1~1000|1] maximum number of binding modes to generate.
+            * **min_rmsd** (*int*) - (1) [1~1000|1] minimum RMSD between output poses.
+            * **energy_range** (*int*) - (3) [1~1000|1] maximum energy difference between the best binding mode and the worst one displayed (kcal/mol).
             * **binary_path** (*string*) - ('vina') path to vina in your local computer.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
             * **container_path** (*str*) - (None) Container path definition.
             * **container_image** (*str*) - ('biocontainers/autodock-vina:v1.1.2-5b1-deb_cv1') Container image definition.
             * **container_volume_path** (*str*) - ('/tmp') Container volume path definition.
             * **container_working_dir** (*str*) - (None) Container working directory definition.
@@ -70,14 +74,18 @@
         self.io_dict = {
             "in": {"input_ligand_pdbqt_path": input_ligand_pdbqt_path, "input_receptor_pdbqt_path": input_receptor_pdbqt_path, "input_box_path": input_box_path},
             "out": {"output_pdbqt_path": output_pdbqt_path, "output_log_path": output_log_path}
         }
 
         # Properties specific for BB
         self.cpu = properties.get('cpu', 1)
+        self.exhaustiveness = properties.get('exhaustiveness', 8)
+        self.num_modes = properties.get('num_modes', 9)
+        self.min_rmsd = properties.get('min_rmsd', 1)
+        self.energy_range = properties.get('energy_range', 3)
         self.binary_path = properties.get('binary_path', 'vina')
         self.properties = properties
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
@@ -122,14 +130,18 @@
         # create cmd
         self.cmd = [self.binary_path,
                     '--ligand', self.stage_io_dict["in"]["input_ligand_pdbqt_path"],
                     '--receptor', self.stage_io_dict["in"]["input_receptor_pdbqt_path"],
                     '--center_x=' + x0, '--center_y=' + y0, '--center_z=' + z0,
                     '--size_x=' + sidex, '--size_y=' + sidey, '--size_z=' + sidez,
                     '--cpu', str(self.cpu),
+                    '--exhaustiveness', str(self.exhaustiveness),
+                    '--num_modes', str(self.num_modes),
+                    '--min_rmsd', str(self.min_rmsd),
+                    '--energy_range', str(self.energy_range),
                     '--out', self.stage_io_dict["out"]["output_pdbqt_path"],
                     '--verbosity', '1',
                     '>', self.stage_io_dict["out"]["output_log_path"]]
 
         # Run Biobb block
         self.run_biobb()
```

### Comparing `biobb_vs-4.1.1/biobb_vs/vina/common.py` & `biobb_vs-4.1.2/biobb_vs/vina/common.py`

 * *Files identical despite different names*

### Comparing `biobb_vs-4.1.1/biobb_vs.egg-info/PKG-INFO` & `biobb_vs-4.1.2/biobb_vs.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: biobb-vs
-Version: 4.1.1
+Version: 4.1.2
 Summary: Biobb_vs is the Biobb module collection to perform virtual screening studies.
 Home-page: https://github.com/bioexcel/biobb_vs
 Author: Biobb developers
 Author-email: genis.bayarri@irbbarcelona.org
-Project-URL: Documentation, http://biobb_vs.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-vs.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: biobb_common==4.1.0
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_vs?label=Version)](https://GitHub.com/bioexcel/biobb_vs/tags/)
 [![](https://img.shields.io/pypi/v/biobb-vs.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-vs/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_vs?label=Conda)](https://anaconda.org/bioconda/biobb_vs)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_vs?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_vs)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_vs?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_vs:4.1.1--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_vs:4.1.2--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_vs)
 [![](https://img.shields.io/pypi/pyversions/biobb-vs.svg?label=Python%20Versions)](https://pypi.org/project/biobb-vs/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_vs)
 
 [![](https://readthedocs.org/projects/biobb-vs/badge/?version=latest&label=Docs)](https://biobb-vs.readthedocs.io/en/latest/?badge=latest)
@@ -39,85 +40,92 @@
 
 [![](https://docs.bioexcel.eu/biobb_vs/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_vs/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_vs/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_vs/coverage/)
 [![](https://docs.bioexcel.eu/biobb_vs/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_vs/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_vs?label=Last%20Commit)](https://github.com/bioexcel/biobb_vs/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_vs.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_vs/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_vs
 
 ### Introduction
 Biobb_vs is the Biobb module collection to perform virtual screening studies.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_vs.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-vs.readthedocs.io/en/latest/).
 
 > At the time of publishing the current version, **autodock_vina has not been compiled for the new ARM mac M1/M2 chips**. So the vina.autodock_vina_run only work in these computers through docker containers.
 
 ### Version
-v4.1.1 2023.3
+v4.1.2 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
 
-        pip install "biobb_vs>=4.1.1"
+        pip install "biobb_vs>=4.1.2"
 
 
 * Usage: [Python API documentation](https://biobb-vs.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_vs>=4.1.1"
+        conda install -c bioconda "biobb_vs>=4.1.2"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-vs.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-vs.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_vs:4.1.1--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_vs:4.1.2--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_vs:4.1.1--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_vs:4.1.2--pyhdfd78af_0 <command>
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_vs.sif https://depot.galaxyproject.org/singularity/biobb_vs:4.1.1--pyhdfd78af_0
+        singularity pull --name biobb_vs.sif https://depot.galaxyproject.org/singularity/biobb_vs:4.1.2--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_vs.sif <command>
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-vs.readthedocs.io/en/latest/command_line.html).
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_vs-4.1.1/biobb_vs.egg-info/SOURCES.txt` & `biobb_vs-4.1.2/biobb_vs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_vs-4.1.1/setup.py` & `biobb_vs-4.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_vs",
-    version="4.1.1",
+    version="4.1.2",
     author="Biobb developers",
     author_email="genis.bayarri@irbbarcelona.org",
     description="Biobb_vs is the Biobb module collection to perform virtual screening studies.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_vs",
     project_urls={
-        "Documentation": "http://biobb_vs.readthedocs.io/en/latest/",
+        "Documentation": "http://biobb-vs.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
     install_requires=['biobb_common==4.1.0'],
     python_requires='>=3.8',
     entry_points={
         "console_scripts": [
```

