# Comparing `tmp/pyCFS-0.0.5.tar.gz` & `tmp/pyCFS-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyCFS-0.0.5.tar", last modified: Mon Apr  8 15:22:17 2024, max compression
+gzip compressed data, was "pyCFS-0.0.6.tar", last modified: Wed May  8 09:52:57 2024, max compression
```

## Comparing `pyCFS-0.0.5.tar` & `pyCFS-0.0.6.tar`

### file list

```diff
@@ -1,144 +1,163 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.521576 pyCFS-0.0.5/
--rw-rw-rw-   0 root         (0) root         (0)     1056 2024-04-08 15:21:18.000000 pyCFS-0.0.5/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.477577 pyCFS-0.0.5/.gitlab/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.483577 pyCFS-0.0.5/.gitlab/issue_templates/
--rw-rw-rw-   0 root         (0) root         (0)      374 2024-04-08 15:21:18.000000 pyCFS-0.0.5/.gitlab/issue_templates/Default.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.484577 pyCFS-0.0.5/.gitlab/merge_request_templates/
--rw-rw-rw-   0 root         (0) root         (0)      657 2024-04-08 15:21:18.000000 pyCFS-0.0.5/.gitlab/merge_request_templates/Default.md
--rw-rw-rw-   0 root         (0) root         (0)     1307 2024-04-08 15:21:18.000000 pyCFS-0.0.5/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     2770 2024-04-08 15:21:18.000000 pyCFS-0.0.5/Changelog.md
--rw-rw-rw-   0 root         (0) root         (0)     1264 2024-04-08 15:21:18.000000 pyCFS-0.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3796 2024-04-08 15:22:17.521576 pyCFS-0.0.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      366 2024-04-08 15:21:18.000000 pyCFS-0.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.484577 pyCFS-0.0.5/docs/
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.486577 pyCFS-0.0.5/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.486577 pyCFS-0.0.5/docs/source/_static/
--rw-rw-rw-   0 root         (0) root         (0)     6346 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/_static/pycfslogo-full-no-text-small.png
--rw-rw-rw-   0 root         (0) root         (0)    65714 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/_static/pycfslogo-full-no-text.png
--rw-rw-rw-   0 root         (0) root         (0)     1929 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/dev_notes.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.487577 pyCFS-0.0.5/docs/source/dev_source/
--rw-rw-rw-   0 root         (0) root         (0)      236 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/dev_source/conventions.md
--rw-rw-rw-   0 root         (0) root         (0)     2194 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/dev_source/data_handling.md
--rw-rw-rw-   0 root         (0) root         (0)     3178 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/dev_source/dev_notes_main.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.478577 pyCFS-0.0.5/docs/source/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.488577 pyCFS-0.0.5/docs/source/examples/basics/
--rw-rw-rw-   0 root         (0) root         (0)     4498 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/examples/basics/a_first_simulation.md
--rw-rw-rw-   0 root         (0) root         (0)     1272 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/examples/basics/cli_tool.md
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/examples/basics/data_processing.md
--rw-rw-rw-   0 root         (0) root         (0)      892 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/examples/basics/introduction.md
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/examples/basics/result_handling.md
--rw-rw-rw-   0 root         (0) root         (0)      576 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/getting_started.md
--rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2599 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/installation.md
--rw-rw-rw-   0 root         (0) root         (0)     2502 2024-04-08 15:21:18.000000 pyCFS-0.0.5/docs/source/pycfs_data.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.489577 pyCFS-0.0.5/pyCFS/
--rw-rw-rw-   0 root         (0) root         (0)      302 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.491577 pyCFS-0.0.5/pyCFS/data/
--rw-rw-rw-   0 root         (0) root         (0)      342 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.493577 pyCFS-0.0.5/pyCFS/data/extras/
--rw-rw-rw-   0 root         (0) root         (0)      525 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/extras/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21452 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/extras/ansys_io.py
--rw-rw-rw-   0 root         (0) root         (0)     1367 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/extras/ansys_to_cfs_element_types.py
--rw-rw-rw-   0 root         (0) root         (0)    10358 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/extras/ensight_io.py
--rw-rw-rw-   0 root         (0) root         (0)     3038 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/extras/nihu_io.py
--rw-rw-rw-   0 root         (0) root         (0)      993 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/extras/nihu_to_cfs_element_types.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/extras/nihu_types.py
--rw-rw-rw-   0 root         (0) root         (0)    20514 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/extras/psv_io.py
--rw-rw-rw-   0 root         (0) root         (0)     5106 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/extras/vtk_to_cfs_element_types.py
--rw-rw-rw-   0 root         (0) root         (0)     2841 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/extras/vtk_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.495577 pyCFS-0.0.5/pyCFS/data/io/
--rw-rw-rw-   0 root         (0) root         (0)     9850 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/io/CFSArray.py
--rw-rw-rw-   0 root         (0) root         (0)    56029 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/io/CFSMeshData.py
--rw-rw-rw-   0 root         (0) root         (0)    32969 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/io/CFSReader.py
--rw-rw-rw-   0 root         (0) root         (0)    21568 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/io/CFSResultData.py
--rw-rw-rw-   0 root         (0) root         (0)    36590 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/io/CFSWriter.py
--rw-rw-rw-   0 root         (0) root         (0)      406 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2394 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/io/cfs_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.496577 pyCFS-0.0.5/pyCFS/data/operators/
--rw-rw-rw-   0 root         (0) root         (0)      212 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/operators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9849 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/operators/fit_geometry.py
--rw-rw-rw-   0 root         (0) root         (0)    11029 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/operators/interpolators.py
--rw-rw-rw-   0 root         (0) root         (0)    13188 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/operators/projection_interpolation.py
--rw-rw-rw-   0 root         (0) root         (0)    18909 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/util.py
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/data/v_def.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    48873 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/pyCFS.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.497577 pyCFS-0.0.5/pyCFS/util/
--rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4213 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/util/hdf5_io.py
--rw-rw-rw-   0 root         (0) root         (0)     1289 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/util/lib_types.py
--rw-rw-rw-   0 root         (0) root         (0)     5658 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/util/setup_generator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.498577 pyCFS-0.0.5/pyCFS/util/templates/
--rw-rw-rw-   0 root         (0) root         (0)      757 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/util/templates/config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      152 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/util/templates/mat.xml
--rw-rw-rw-   0 root         (0) root         (0)      237 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/util/templates/run_sim.py
--rw-rw-rw-   0 root         (0) root         (0)      196 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/util/templates/sim.jou
--rw-rw-rw-   0 root         (0) root         (0)      338 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/util/templates/sim.xml
--rw-rw-rw-   0 root         (0) root         (0)     1408 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/util/templates/sim_setup.py
--rw-rw-rw-   0 root         (0) root         (0)     2280 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyCFS/util/templates/sim_setup_opti.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.490577 pyCFS-0.0.5/pyCFS.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3796 2024-04-08 15:22:17.000000 pyCFS-0.0.5/pyCFS.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3720 2024-04-08 15:22:17.000000 pyCFS-0.0.5/pyCFS.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 15:22:17.000000 pyCFS-0.0.5/pyCFS.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-04-08 15:22:17.000000 pyCFS-0.0.5/pyCFS.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      385 2024-04-08 15:22:17.000000 pyCFS-0.0.5/pyCFS.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-08 15:22:17.000000 pyCFS-0.0.5/pyCFS.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2966 2024-04-08 15:21:18.000000 pyCFS-0.0.5/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.499577 pyCFS-0.0.5/requirements/
--rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-08 15:21:18.000000 pyCFS-0.0.5/requirements/common.txt
--rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-08 15:21:18.000000 pyCFS-0.0.5/requirements/data_extra.txt
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-04-08 15:21:18.000000 pyCFS-0.0.5/requirements/dev.txt
--rw-rw-rw-   0 root         (0) root         (0)      134 2024-04-08 15:22:17.522576 pyCFS-0.0.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       90 2024-04-08 15:21:18.000000 pyCFS-0.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.501577 pyCFS-0.0.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.481577 pyCFS-0.0.5/tests/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.480577 pyCFS-0.0.5/tests/data/extras/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.501577 pyCFS-0.0.5/tests/data/extras/ansys_io/
--rw-rw-rw-   0 root         (0) root         (0)   720896 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/ansys_io/ansys_io.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.507577 pyCFS-0.0.5/tests/data/extras/ensight_io/
--rw-rw-rw-   0 root         (0) root         (0)   970336 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/ensight_io/ensight_io.0000.U
--rw-rw-rw-   0 root         (0) root         (0)  4523376 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/ensight_io/ensight_io.0000.mesh
--rw-rw-rw-   0 root         (0) root         (0)   323936 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/ensight_io/ensight_io.0000.p
--rw-rw-rw-   0 root         (0) root         (0)      422 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/ensight_io/ensight_io.case
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.508576 pyCFS-0.0.5/tests/data/extras/ensight_io/poly/
--rw-rw-rw-   0 root         (0) root         (0)      782 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/ensight_io/poly/data.case
--rw-rw-rw-   0 root         (0) root         (0)    75544 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/ensight_io/poly/data00001.geo
--rw-rw-rw-   0 root         (0) root         (0)     3200 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/ensight_io/poly/data00001.scl1
--rw-rw-rw-   0 root         (0) root         (0)     7152 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/ensight_io/poly/data00001.vel
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.510577 pyCFS-0.0.5/tests/data/extras/nihu_io/
--rw-rw-rw-   0 root         (0) root         (0)  1381491 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/nihu_io/result_field.mat
--rw-rw-rw-   0 root         (0) root         (0)   894200 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/nihu_io/result_surface.mat
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.513576 pyCFS-0.0.5/tests/data/extras/psv_io/
--rw-rw-rw-   0 root         (0) root         (0)      758 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/psv_io/line.npy
--rw-rw-rw-   0 root         (0) root         (0)   356352 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/psv_io/line.svd
--rw-rw-rw-   0 root         (0) root         (0)   158436 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/psv_io/line_h2_accelerance.unv
--rw-rw-rw-   0 root         (0) root         (0)   634880 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/psv_io/surface.svd
--rw-rw-rw-   0 root         (0) root         (0)     1241 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/psv_io/surface_dist.npy
--rw-rw-rw-   0 root         (0) root         (0)   236016 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/psv_io/surface_h1_receptance.npy
--rw-rw-rw-   0 root         (0) root         (0)   394047 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/extras/psv_io/surface_h1_receptance.unv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.481577 pyCFS-0.0.5/tests/data/operators/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.514577 pyCFS-0.0.5/tests/data/operators/fit_geometry/
--rw-rw-rw-   0 root         (0) root         (0)   146369 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/operators/fit_geometry/fit_geometry_src.cfs
--rw-rw-rw-   0 root         (0) root         (0)    86438 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/operators/fit_geometry/fit_geometry_target.cfs
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.517576 pyCFS-0.0.5/tests/data/operators/interpolators/
--rw-rw-rw-   0 root         (0) root         (0)   165563 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/operators/interpolators/interpolators.cfs
--rw-rw-rw-   0 root         (0) root         (0)  2051052 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/operators/interpolators/nn_elem.cfs
--rwxrwxrwx   0 root         (0) root         (0)    73117 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/operators/interpolators/nn_source.cfs
--rwxrwxrwx   0 root         (0) root         (0)    74841 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/operators/interpolators/nn_target.cfs
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.519576 pyCFS-0.0.5/tests/data/operators/projection_interpolation/
--rw-rw-rw-   0 root         (0) root         (0)   981634 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/operators/projection_interpolation/source.cfs
--rw-rw-rw-   0 root         (0) root         (0)    44589 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/operators/projection_interpolation/target.cfs
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:22:17.519576 pyCFS-0.0.5/tests/data/sim_io/
--rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/data/sim_io/elecFieldIntensity-sensor-positions-0.csv-1
--rw-rw-rw-   0 root         (0) root         (0)     3181 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/pycfs_data_fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)     7353 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/pycfs_fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)     8345 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/test_pycfs_core.py
--rw-rw-rw-   0 root         (0) root         (0)     8434 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/test_pycfs_data_extras.py
--rw-rw-rw-   0 root         (0) root         (0)     8105 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/test_pycfs_data_io.py
--rw-rw-rw-   0 root         (0) root         (0)     8526 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/test_pycfs_data_operators.py
--rw-rw-rw-   0 root         (0) root         (0)     2574 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/test_pycfs_data_util.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2024-04-08 15:21:18.000000 pyCFS-0.0.5/tests/test_pycfs_sim_io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.149822 pyCFS-0.0.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-08 09:51:59.000000 pyCFS-0.0.6/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.107823 pyCFS-0.0.6/.gitlab/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.113822 pyCFS-0.0.6/.gitlab/issue_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      374 2024-05-08 09:51:59.000000 pyCFS-0.0.6/.gitlab/issue_templates/Default.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.113822 pyCFS-0.0.6/.gitlab/merge_request_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      657 2024-05-08 09:51:59.000000 pyCFS-0.0.6/.gitlab/merge_request_templates/Default.md
+-rw-rw-rw-   0 root         (0) root         (0)     1452 2024-05-08 09:51:59.000000 pyCFS-0.0.6/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3228 2024-05-08 09:51:59.000000 pyCFS-0.0.6/Changelog.md
+-rw-rw-rw-   0 root         (0) root         (0)     1264 2024-05-08 09:51:59.000000 pyCFS-0.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3796 2024-05-08 09:52:57.149822 pyCFS-0.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      366 2024-05-08 09:51:59.000000 pyCFS-0.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.114822 pyCFS-0.0.6/docs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/.nojekyll
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)      780 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/rst_process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.115822 pyCFS-0.0.6/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.116822 pyCFS-0.0.6/docs/source/_static/
+-rw-rw-rw-   0 root         (0) root         (0)     6346 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/_static/pycfslogo-full-no-text-small.png
+-rw-rw-rw-   0 root         (0) root         (0)    65714 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/_static/pycfslogo-full-no-text.png
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/api.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3088 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/dev_notes.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.116822 pyCFS-0.0.6/docs/source/dev_source/
+-rw-rw-rw-   0 root         (0) root         (0)      236 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/dev_source/conventions.md
+-rw-rw-rw-   0 root         (0) root         (0)     2194 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/dev_source/data_handling.md
+-rw-rw-rw-   0 root         (0) root         (0)     3178 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/dev_source/dev_notes_main.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.108822 pyCFS-0.0.6/docs/source/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.117823 pyCFS-0.0.6/docs/source/examples/basics/
+-rw-rw-rw-   0 root         (0) root         (0)     4498 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/examples/basics/a_first_simulation.md
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/examples/basics/cli_tool.md
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/examples/basics/data_processing.md
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/examples/basics/introduction.md
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/examples/basics/result_handling.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.118822 pyCFS-0.0.6/docs/source/examples/data_tutorial/
+-rw-rw-rw-   0 root         (0) root         (0)     1871 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/examples/data_tutorial/data_tutorial.py
+-rw-rw-rw-   0 root         (0) root         (0)   171649 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/examples/data_tutorial/tutorial_input.cfs
+-rw-rw-rw-   0 root         (0) root         (0)      576 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/getting_started.md
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2793 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/installation.md
+-rw-rw-rw-   0 root         (0) root         (0)     5555 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/pycfs_data.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.120822 pyCFS-0.0.6/docs/source/resources/
+-rw-rw-rw-   0 root         (0) root         (0)    10440 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/resources/cell2node.png
+-rw-rw-rw-   0 root         (0) root         (0)    26803 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/resources/data_structures_CFSMeshData.png
+-rw-rw-rw-   0 root         (0) root         (0)    18718 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/resources/data_structures_CFSRegData.png
+-rw-rw-rw-   0 root         (0) root         (0)    80295 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/resources/data_structures_CFSResultArray.png
+-rw-rw-rw-   0 root         (0) root         (0)    57502 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/resources/data_structures_CFSResultData.png
+-rw-rw-rw-   0 root         (0) root         (0)    68395 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/resources/data_structures_CFSResultInfo.png
+-rw-rw-rw-   0 root         (0) root         (0)    15219 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/resources/data_structures_overview.png
+-rw-rw-rw-   0 root         (0) root         (0)    40408 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/resources/nearest_neighbor.png
+-rw-rw-rw-   0 root         (0) root         (0)    10791 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/resources/node2cell.png
+-rw-rw-rw-   0 root         (0) root         (0)    19990 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/resources/projection_interpolation.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.120822 pyCFS-0.0.6/docs/source/resources/src/
+-rw-rw-rw-   0 root         (0) root         (0)    43112 2024-05-08 09:51:59.000000 pyCFS-0.0.6/docs/source/resources/src/data_structures.drawio
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.121822 pyCFS-0.0.6/pyCFS/
+-rw-rw-rw-   0 root         (0) root         (0)      480 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.123822 pyCFS-0.0.6/pyCFS/data/
+-rw-rw-rw-   0 root         (0) root         (0)     2784 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.124822 pyCFS-0.0.6/pyCFS/data/extras/
+-rw-rw-rw-   0 root         (0) root         (0)      543 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/extras/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21452 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/extras/ansys_io.py
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/extras/ansys_to_cfs_element_types.py
+-rw-rw-rw-   0 root         (0) root         (0)    10570 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/extras/ensight_io.py
+-rw-rw-rw-   0 root         (0) root         (0)     3132 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/extras/nihu_io.py
+-rw-rw-rw-   0 root         (0) root         (0)      993 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/extras/nihu_to_cfs_element_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/extras/nihu_types.py
+-rw-rw-rw-   0 root         (0) root         (0)    20729 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/extras/psv_io.py
+-rw-rw-rw-   0 root         (0) root         (0)     5106 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/extras/vtk_to_cfs_element_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/extras/vtk_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.126822 pyCFS-0.0.6/pyCFS/data/io/
+-rw-rw-rw-   0 root         (0) root         (0)    10017 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/io/CFSArray.py
+-rw-rw-rw-   0 root         (0) root         (0)    61618 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/io/CFSMeshData.py
+-rw-rw-rw-   0 root         (0) root         (0)    35321 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/io/CFSReader.py
+-rw-rw-rw-   0 root         (0) root         (0)    22492 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/io/CFSResultData.py
+-rw-rw-rw-   0 root         (0) root         (0)    36628 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/io/CFSWriter.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2394 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/io/cfs_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.127822 pyCFS-0.0.6/pyCFS/data/operators/
+-rw-rw-rw-   0 root         (0) root         (0)      214 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/operators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14270 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/operators/interpolators.py
+-rw-rw-rw-   0 root         (0) root         (0)    14960 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/operators/projection_interpolation.py
+-rw-rw-rw-   0 root         (0) root         (0)     9933 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/operators/transformation.py
+-rw-rw-rw-   0 root         (0) root         (0)    21020 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/util.py
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/data/v_def.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    49637 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/pyCFS.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.127822 pyCFS-0.0.6/pyCFS/util/
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6720 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/util/hdf5_io.py
+-rw-rw-rw-   0 root         (0) root         (0)     1289 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/util/lib_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     5658 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/util/setup_generator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.129822 pyCFS-0.0.6/pyCFS/util/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      757 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/util/templates/config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      152 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/util/templates/mat.xml
+-rw-rw-rw-   0 root         (0) root         (0)      237 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/util/templates/run_sim.py
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/util/templates/sim.jou
+-rw-rw-rw-   0 root         (0) root         (0)      338 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/util/templates/sim.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1408 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/util/templates/sim_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     2280 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyCFS/util/templates/sim_setup_opti.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.122822 pyCFS-0.0.6/pyCFS.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3796 2024-05-08 09:52:57.000000 pyCFS-0.0.6/pyCFS.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4425 2024-05-08 09:52:57.000000 pyCFS-0.0.6/pyCFS.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 09:52:57.000000 pyCFS-0.0.6/pyCFS.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2024-05-08 09:52:57.000000 pyCFS-0.0.6/pyCFS.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      385 2024-05-08 09:52:57.000000 pyCFS-0.0.6/pyCFS.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-08 09:52:57.000000 pyCFS-0.0.6/pyCFS.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2966 2024-05-08 09:51:59.000000 pyCFS-0.0.6/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.129822 pyCFS-0.0.6/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-05-08 09:51:59.000000 pyCFS-0.0.6/requirements/common.txt
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-05-08 09:51:59.000000 pyCFS-0.0.6/requirements/data_extra.txt
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-08 09:51:59.000000 pyCFS-0.0.6/requirements/dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)      134 2024-05-08 09:52:57.150822 pyCFS-0.0.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       90 2024-05-08 09:51:59.000000 pyCFS-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.131822 pyCFS-0.0.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.111822 pyCFS-0.0.6/tests/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.111822 pyCFS-0.0.6/tests/data/extras/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.131822 pyCFS-0.0.6/tests/data/extras/ansys_io/
+-rw-rw-rw-   0 root         (0) root         (0)   720896 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/extras/ansys_io/ansys_io.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.137822 pyCFS-0.0.6/tests/data/extras/ensight_io/
+-rw-rw-rw-   0 root         (0) root         (0)   970336 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/extras/ensight_io/ensight_io.0000.U
+-rw-rw-rw-   0 root         (0) root         (0)  4523376 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/extras/ensight_io/ensight_io.0000.mesh
+-rw-rw-rw-   0 root         (0) root         (0)   323936 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/extras/ensight_io/ensight_io.0000.p
+-rw-rw-rw-   0 root         (0) root         (0)      422 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/extras/ensight_io/ensight_io.case
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.137822 pyCFS-0.0.6/tests/data/extras/ensight_io/poly/
+-rw-rw-rw-   0 root         (0) root         (0)      782 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/extras/ensight_io/poly/data.case
+-rw-rw-rw-   0 root         (0) root         (0)    75544 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/extras/ensight_io/poly/data00001.geo
+-rw-rw-rw-   0 root         (0) root         (0)     3200 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/extras/ensight_io/poly/data00001.scl1
+-rw-rw-rw-   0 root         (0) root         (0)     7152 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/extras/ensight_io/poly/data00001.vel
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.139822 pyCFS-0.0.6/tests/data/extras/nihu_io/
+-rw-rw-rw-   0 root         (0) root         (0)  1381491 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/extras/nihu_io/result_field.mat
+-rw-rw-rw-   0 root         (0) root         (0)   894200 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/extras/nihu_io/result_surface.mat
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.142822 pyCFS-0.0.6/tests/data/extras/psv_io/
+-rw-rw-rw-   0 root         (0) root         (0)      758 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/extras/psv_io/line.npy
+-rw-rw-rw-   0 root         (0) root         (0)   356352 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/extras/psv_io/line.svd
+-rw-rw-rw-   0 root         (0) root         (0)   158436 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/extras/psv_io/line_h2_accelerance.unv
+-rw-rw-rw-   0 root         (0) root         (0)   634880 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/extras/psv_io/surface.svd
+-rw-rw-rw-   0 root         (0) root         (0)     1241 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/extras/psv_io/surface_dist.npy
+-rw-rw-rw-   0 root         (0) root         (0)   236016 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/extras/psv_io/surface_h1_receptance.npy
+-rw-rw-rw-   0 root         (0) root         (0)   394047 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/extras/psv_io/surface_h1_receptance.unv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.111822 pyCFS-0.0.6/tests/data/operators/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.143822 pyCFS-0.0.6/tests/data/operators/fit_geometry/
+-rw-rw-rw-   0 root         (0) root         (0)   146369 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/operators/fit_geometry/fit_geometry_src.cfs
+-rw-rw-rw-   0 root         (0) root         (0)    86438 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/operators/fit_geometry/fit_geometry_target.cfs
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.146822 pyCFS-0.0.6/tests/data/operators/interpolators/
+-rw-rw-rw-   0 root         (0) root         (0)   165563 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/operators/interpolators/interpolators.cfs
+-rw-rw-rw-   0 root         (0) root         (0)  2051052 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/operators/interpolators/nn_elem.cfs
+-rwxrwxrwx   0 root         (0) root         (0)    73117 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/operators/interpolators/nn_source.cfs
+-rwxrwxrwx   0 root         (0) root         (0)    74841 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/operators/interpolators/nn_target.cfs
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.147822 pyCFS-0.0.6/tests/data/operators/projection_interpolation/
+-rw-rw-rw-   0 root         (0) root         (0)   981634 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/operators/projection_interpolation/source.cfs
+-rw-rw-rw-   0 root         (0) root         (0)    44589 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/operators/projection_interpolation/target.cfs
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 09:52:57.147822 pyCFS-0.0.6/tests/data/sim_io/
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/data/sim_io/elecFieldIntensity-sensor-positions-0.csv-1
+-rw-rw-rw-   0 root         (0) root         (0)     3181 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/pycfs_data_fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)     7353 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/pycfs_fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)     8345 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/test_pycfs_core.py
+-rw-rw-rw-   0 root         (0) root         (0)     8434 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/test_pycfs_data_extras.py
+-rw-rw-rw-   0 root         (0) root         (0)     9540 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/test_pycfs_data_io.py
+-rw-rw-rw-   0 root         (0) root         (0)     8528 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/test_pycfs_data_operators.py
+-rw-rw-rw-   0 root         (0) root         (0)     3397 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/test_pycfs_data_util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2024-05-08 09:51:59.000000 pyCFS-0.0.6/tests/test_pycfs_sim_io.py
```

### Comparing `pyCFS-0.0.5/.gitignore` & `pyCFS-0.0.6/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 coverage.xml
 logs/
 results_hdf5/
 htmlcov/
 coverage/
 .pytest_cache/
 .mypy_cache/
+docs/source/generated
 docs/build/latex/
 docs/build/html/
 docs/build/doctrees/
 
 # temporary : 
 examples/capacitor_3d*/
 examples/clean_capacitor_3d*/
```

### Comparing `pyCFS-0.0.5/.gitlab/merge_request_templates/Default.md` & `pyCFS-0.0.6/.gitlab/merge_request_templates/Default.md`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/.gitlab-ci.yml` & `pyCFS-0.0.6/.gitlab-ci.yml`

 * *Files 7% similar despite different names*

```diff
@@ -12,24 +12,27 @@
   - pip install -r requirements/dev.txt
 
 # build and deploy documentation on gitlab pages : 
 # runs only on 'main' branch if docs were changed
 pages:
   stage: build-docs
   script:
-    - python -m pip install .
+    - python -m pip install .[data]
+    - sphinx-apidoc -f -e -d 2 --separate -l -M -o docs/source/generated pyCFS/
+    - python docs/rst_process.py
     - sphinx-build -M html docs/source/ docs/build/
     - mv docs/build/html public/
   artifacts:
     paths:
       - public
   rules:
     - if: $CI_COMMIT_BRANCH == $CI_DEFAULT_BRANCH
       changes:
-      - docs/source/*
+        - docs/source/**/*
+        - pyCFS/**/*
 
 tests:
   stage: run-tests
   script: 
     - python -m pip install .
     - pytest
   artifacts:
```

### Comparing `pyCFS-0.0.5/Changelog.md` & `pyCFS-0.0.6/Changelog.md`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,28 @@
 
 - ( any bug fixes )
 
 ### Security
 
 - ( in case of vulnerabilities )
 
+## [0.0.6] - 2024-05-08
+
+### Added
+
+- Compute surface normal vectors
+- Option for parallel reading of result data (default now)
+
+### Changed
+
+- Vectorized element centroid computation
+- Renamed "pyCFS.data.operators.fit_geometry" submodule to "pyCFS.data.operators.transformation"
+- Renamed "pyCFS.data.operators.projection_interpolation.interpolation_fe" submodule to
+  "pyCFS.data.operators.projection_interpolation.interpolation_matrix_projection_based"
+
 ## [0.0.5] - 2024-04-08
 
 ### Added
 
 - Support for Reading/Writing MultiStepIDs other than 1.
 - Support for Reading MultiStep with unsorted StepValues (requires sort before writing)
```

### Comparing `pyCFS-0.0.5/LICENSE` & `pyCFS-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/PKG-INFO` & `pyCFS-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCFS
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python library for automating and data handling tasks for openCFS.
 Author-email: IGTE <igte.gitlab@gmail.com>, Eniz Mušeljić <eniz.m@outlook.com>, Andreas Wurzinger <andreas.wurzinger@tugraz.at>
 License: MIT License
         
         Copyright (c) 2024 Verein zur Förderung der Software openCFS
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyCFS-0.0.5/docs/Makefile` & `pyCFS-0.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/docs/make.bat` & `pyCFS-0.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/docs/source/_static/pycfslogo-full-no-text-small.png` & `pyCFS-0.0.6/docs/source/_static/pycfslogo-full-no-text-small.png`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/docs/source/_static/pycfslogo-full-no-text.png` & `pyCFS-0.0.6/docs/source/_static/pycfslogo-full-no-text.png`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/docs/source/conf.py` & `pyCFS-0.0.6/docs/source/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Configuration file for the Sphinx documentation builder.
 #
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
-import pyCFS
+import pyCFS, sys
+
+sys.path.append("../pyCFS")
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = pyCFS.__name__
 copyright = "2024, Verein zur Förderung der Software openCFS"
 author = " and ".join(pyCFS.__author__)
@@ -14,14 +16,19 @@
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.duration",
     "myst_parser",
+    "sphinx.ext.autodoc",  # Parses (sub)modules
+    "sphinx.ext.napoleon",  # Parses Numpy docstrings
+    "sphinx.ext.mathjax",  # Print mathematical expressions
+    "sphinx.ext.autosummary",  # Make module lists in table
+    "sphinx.ext.viewcode",
 ]
 
 templates_path = ["_templates"]
 exclude_patterns = []
 
 myst_enable_extensions = ["colon_fence", "dollarmath", "amsmath"]
 myst_heading_anchors = 3
@@ -57,7 +64,36 @@
             "type": "fontawesome",
         },
     ],
 }
 
 # suppress errors :
 suppress_warnings = ["myst.header"]
+
+# Napoleon settings
+napoleon_google_docstring = True
+napoleon_numpy_docstring = True
+napoleon_include_init_with_doc = True
+napoleon_include_private_with_doc = False
+napoleon_include_special_with_doc = False
+napoleon_use_admonition_for_examples = False
+napoleon_use_admonition_for_notes = False
+napoleon_use_admonition_for_references = False
+napoleon_use_ivar = True
+napoleon_use_param = True
+napoleon_use_rtype = True
+napoleon_preprocess_types = True
+napoleon_type_aliases = {"np": "numpy"}
+napoleon_attr_annotations = True
+
+# Autodoc settings
+autoclass_content = "both"
+autodoc_class_signature = "mixed"
+autodoc_member_order = "groupwise"
+autodoc_default_options = {
+    "member-order": "groupwise",
+    "special-members": "__init__",
+    "undoc-members": True,
+    # "exclude-members": "__weakref__",
+}
+autodoc_typehints = "description"
+autodoc_typehints_format = "short"
```

### Comparing `pyCFS-0.0.5/docs/source/dev_source/data_handling.md` & `pyCFS-0.0.6/docs/source/dev_source/data_handling.md`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/docs/source/dev_source/dev_notes_main.md` & `pyCFS-0.0.6/docs/source/dev_source/dev_notes_main.md`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/docs/source/examples/basics/a_first_simulation.md` & `pyCFS-0.0.6/docs/source/examples/basics/a_first_simulation.md`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/docs/source/examples/basics/cli_tool.md` & `pyCFS-0.0.6/docs/source/examples/basics/cli_tool.md`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/docs/source/examples/basics/introduction.md` & `pyCFS-0.0.6/docs/source/examples/basics/introduction.md`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/docs/source/getting_started.md` & `pyCFS-0.0.6/docs/source/getting_started.md`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/docs/source/installation.md` & `pyCFS-0.0.6/docs/source/installation.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,18 @@
                 ~\.venv\pycfs\Scripts\Activate.ps1
                 ```
 2. Install *pyCFS*
     - Install via pip :
         ```bash
         python -m pip install --upgrade pycfs
         ```
+    - If you want to install a specific branch (e.g. `main`), this can be done with
+        ```bash
+        python -m pip install --upgrade git+https://gitlab.com/opencfs/pycfs@main
+        ```
 3. Install *openCFS* and *coreform cubit* :
     - Follow [this tutorial](https://opencfs.gitlab.io/userdocu/Installation/)
 
 ## Developer install
 
 First you will need to clone the repository and `cd` into the repository root. As a developer you will need to install
 a few dependencies more than what is needed to just use the package.
```

### Comparing `pyCFS-0.0.5/docs/source/pycfs_data.md` & `pyCFS-0.0.6/pyCFS/data/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,105 @@
-# pyCFS-data
+"""
+pyCFS.data
+==========
 
-Data processing framework for openCFS (www.opencfs.org). This project contains Python libraries to easily create and
-manipulate data stored in openCFS type HDF5 file format (`*.cfs`).
+Data processing framework for openCFS (www.opencfs.org). This project
+contains Python libraries to easily create and manipulate data stored in
+openCFS type HDF5 file format (``*.cfs``).
 
-## Installation
+CFS IO
+------------------------------------------
 
-Install via pip
+-  Reader class containing
+   top and low-level methods for reading
+-  Writer class containing
+   top and low-level methods for writing
 
-```sh
-pip install pycfs
-```
+Example
+~~~~~~~
 
-Install with all dependencies for extras functionality.
+.. code:: python
 
-```sh
-pip install pycfs[data]
-```
+   from pyCFS.data.io import CFSReader, CFSWriter
 
-## CFS IO
+   with CFSReader('file.cfs') as f:
+       mesh = f.MeshData
+       results = f.MultiStepData
+   with CFSWriter('file.cfs') as f:
+       f.create_file(mesh_data=mesh, result_data=results)
 
-- Reader class containing top and low-level methods for reading
-- Writer class containing top and low-level methods for writing
+Operators
+----------------------------------------------------
 
-### Example
+Utility functions for performing mesh and/or data manipulation
 
-```python
-from pyCFS.data.io import CFSReader, CFSWriter
+-  Fit geometry based on minimizing the squared source nodal distances
+   to target nearest neighbor nodes.
+-  Interpolators:
+   Node2Cell, Cell2Node, Nearest Neighbor (bidirectional)
+-  Projection based linear Interpolation
 
-with CFSReader('file.cfs') as f:
-    mesh = f.MeshData
-    results = f.MultiStepData
-with CFSWriter('file.cfs') as f:
-    f.create_file(mesh_data=mesh, result_data=results)
-```
+Extra functionality
+-----------------------------------------------------------
 
-## Operators
+*Extras* provides Python libraries to easily manipulate data from
+various formats including
 
-Utility functions for performing mesh and/or data manipulation
+-  EnSight Case Gold (``*.case``).
+-  Ansys result file (``*.rst``). Requires additional dependencies,
+   which can be installed via pip
+
+.. code:: sh
+
+   pip install pycfs[data]
+
+-  PSV measurement data export file (``*.unv``).
+-  MATLAB data files of NiHu structures and simulation results
+   (``*.mat``).
 
-- Fit geometry based on minimizing the squared source nodal distances to target nearest neighbor nodes.
-- Interpolators: Node2Cell, Cell2Node, Nearest Neighbor (bidirectional)
-- Projection based linear Interpolation
+EnSight Case Gold
+~~~~~~~~~~~~~~~~~
 
-## Extra functionality
+-  Utility functions for reading using *vtkEnSightGoldBinaryReader* and
+   writing to *CFS HFD5*
 
-*Extras* provides Python libraries to easily manipulate data from various formats including
+Ansys
+~~~~~
 
-- EnSight Case Gold (`*.case`).
-- Ansys result file (`*.rst`). Requires additional dependencies, which can be installed via pip
+-  Utility functions for reading using *pyAnsys (ansys-dpf-core)* and
+   writing to *CFS HFD5*
+-  Requires a licensed ANSYS DPF server installed on the system!
 
-```sh
-pip install pycfs[data]
-```
+   -  Check if the environment variable ``ANSYSLMD_LICENSE_FILE`` is set
+      to the license server)!
+   -  Check if the environment variable ``AWP_ROOTXXX`` is set to the
+      ANSYS installation root folder of the version you want to use
+      (``vXXX`` folder).
 
-- PSV measurement data export file (`*.unv`).
-- MATLAB data files of NiHu structures and simulation results (`*.mat`).
+.. code:: sh
 
-### EnSight Case Gold
+   export ANSYSLMD_LICENSE_FILE=1055@my_license_server.ansys.com
+   export AWP_ROOTXXX=/usr/ansys_inc/vXXX
 
-- Utility functions for reading using *vtkEnSightGoldBinaryReader* and writing to *CFS HFD5*
+PSV - Measurement data
+~~~~~~~~~~~~~~~~~~~~~~
 
-### Ansys
+-  Utility functions for reading ``*.unv`` export files using *pyUFF*
+   and writing to *CFS HFD5*
+-  Utility functions for manipulating data dictionary:
 
-- Utility functions for reading using *pyAnsys (ansys-dpf-core)* and writing to *CFS HFD5*
-- Requires a licensed ANSYS DPF server installed on the system!
-    - Check if the environment variable `ANSYSLMD_LICENSE_FILE` is set to the license server)!
-    - Check if the environment variable `AWP_ROOTXXX` is set to the ANSYS installation root folder of the version you
-      want to use (`vXXX` folder).
+   -  Interpolate data points from neighboring data points
+   -  Combine 3 measurements to 3D measurement
 
-```sh
-export ANSYSLMD_LICENSE_FILE=1055@my_license_server.ansys.com
-export AWP_ROOTXXX=/usr/ansys_inc/vXXX
-```
+NiHu
+~~~~
 
-### PSV - Measurement data
+-  Utility functions for reading ``*.mat`` MATLAB data files of NiHu
+   structures and simulation results and writing to *CFS HFD5*
 
-- Utility functions for reading `*.unv` export files using *pyUFF* and writing to *CFS HFD5*
-- Utility functions for manipulating data dictionary:
-    - Interpolate data points from neighboring data points
-    - Combine 3 measurements to 3D measurement
 
-### NiHu
+"""
 
-- Utility functions for reading `*.mat` MATLAB data files of NiHu structures and simulation results and writing to *CFS
-  HFD5*
+from . import io  # noqa
+from . import util  # noqa
+from . import extras  # noqa
+from . import operators  # noqa
```

### Comparing `pyCFS-0.0.5/pyCFS/data/extras/__init__.py` & `pyCFS-0.0.6/pyCFS/data/extras/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 pyCFS.data.extras
 
-Libraries to read and write data in from various formats
+Library of modules to read from, convert to, and write in various formats.
 """
 
 import importlib.util
 
 if importlib.util.find_spec("ansys") is not None:
     from . import ansys_io  # noqa
     from . import ansys_to_cfs_element_types  # noqa
```

### Comparing `pyCFS-0.0.5/pyCFS/data/extras/ansys_io.py` & `pyCFS-0.0.6/pyCFS/data/extras/ansys_io.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/pyCFS/data/extras/ansys_to_cfs_element_types.py` & `pyCFS-0.0.6/pyCFS/data/extras/ansys_to_cfs_element_types.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/pyCFS/data/extras/ensight_io.py` & `pyCFS-0.0.6/pyCFS/data/extras/ensight_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Module containing data processing utilities for reading EnSight Case Gold files
+"""
+
 from __future__ import annotations
 
 import os
 import vtk
 from typing import List, Dict, Tuple
 
 # noinspection PyUnresolvedReferences
@@ -17,19 +21,23 @@
 def ensightInitReader(file: str) -> vtk.vtkEnSightGoldBinaryReader:
     """
     Initializes an EnSight reader object with the specified filename and filepath.
 
     This function creates an instance of the class vtkEnSightGoldBinaryReader and sets the
     case file name and path for reading EnSight files. The reader object is then updated.
 
-    Args:
-        file (str): Path to the EnSight case file.
-
-    Returns:
-        vtk.vtkEnSightGoldBinaryReader: The initialized EnSight reader object.
+    Parameters
+    ----------
+    file : str
+        Path to the EnSight case file.
+
+    Returns
+    -------
+    vtk.vtkEnSightGoldBinaryReader
+        The initialized EnSight reader object.
 
     """
 
     filepath, filename = os.path.split(file)
     if filepath == "":
         filepath = "../ensight/"
     reader = vtk.vtkEnSightGoldBinaryReader()
@@ -44,27 +52,29 @@
     """
     Retrieves information about the EnSight file using the provided reader object.
 
     This function extracts the names and data types of cell and point arrays in the EnSight file.
     It also retrieves the number of time steps, the time range and generates an array with the time
     steps. Every time a Cell/Point Array is found, its name is printed. Finally, the function returns
     a dictionary with the following keys:
-     - 'fieldNames' (list): List of field names (meaning cell and point arrays).
-     - 'fieldDataTypes' (list): List of field data types (types: 'Cell' or 'Point').
-     - 'numSteps' (int): Number of time steps.
-     - 'timeRange' (tuple): start and end point of the time values.
-     - 'timeSteps' (numpy array) : one-dimensional array of time steps.
-
-    Args:
-    -----
-        reader (vtk.vtkEnSightGoldBinaryReader): The EnSight reader object.
+    - 'fieldNames' (list): List of field names (meaning cell and point arrays).
+    - 'fieldDataTypes' (list): List of field data types (types: 'Cell' or 'Point').
+    - 'numSteps' (int): Number of time steps.
+    - 'timeRange' (tuple): start and end point of the time values.
+    - 'timeSteps' (numpy array) : one-dimensional array of time steps.
+
+    Parameters
+    ----------
+    reader : vtk.vtkEnSightGoldBinaryReader
+        The EnSight reader object.
 
-    Returns:
+    Returns
     --------
-        dict: A dictionary containing the retrieved information.
+    dict
+        A dictionary containing the retrieved information.
 
     """
 
     field_name_list = []
     field_data_type_list = []
 
     # append names and types of all Cell/Point Arrays to field_name_list and field_data_type_list
@@ -109,22 +119,29 @@
      - 'Coordinates' (numpy array): An array with the node Coordinates.
      - 'Connectivity' (numpy array): A 2D array containing the Connectivity information, where
         each row corresponds to a cell and the columns represent the nodes connected to that cell.
      - 'types' (numpy array): A 1D array containing the element types of the field.
      - 'num_grid' (dict): A dictionary containing information about the number of certain element
         types and the number of nodes.
 
-    Args:
-        reader (vtk.vtkEnSightGoldBinaryReader): The EnSight reader object.
-        block (int): The index of the block to read from the EnSight file. Defaults to 0.
-        processes (int): Number of parallel processes for Connectivity build up.
-        verbosity (int): Verbosity level
-
-    Returns:
-        dict: A dictionary containing the retrieved information.
+    Parameters
+    ----------
+    reader : vtk.vtkEnSightGoldBinaryReader
+        The EnSight reader object.
+    block : int, optional
+        The index of the block to read from the EnSight file. Defaults to 0.
+    processes : int, optional
+        Number of parallel processes for Connectivity build up.
+    verbosity : int, optional
+        Verbosity level
+
+    Returns
+    -------
+    dict
+        A dictionary containing the retrieved information.
 
     """
 
     data = reader.GetOutput()
 
     bdata = data.GetBlock(block)
```

### Comparing `pyCFS-0.0.5/pyCFS/data/extras/nihu_io.py` & `pyCFS-0.0.6/pyCFS/data/extras/nihu_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-# Imports
+"""
+Module containing data processing utilities for reading NiHu structures as Matlab export files
+"""
+
 from __future__ import annotations
 
 import scipy
 import numpy as np
 from typing import List, Dict
 
 from pyCFS.data.io import cfs_types
```

### Comparing `pyCFS-0.0.5/pyCFS/data/extras/nihu_to_cfs_element_types.py` & `pyCFS-0.0.6/pyCFS/data/extras/nihu_to_cfs_element_types.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/pyCFS/data/extras/psv_io.py` & `pyCFS-0.0.6/pyCFS/data/extras/psv_io.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,28 +23,49 @@
     ref_channel=1,
     read_coordinates=False,
     read_elements=False,
     dist_file: str | None = None,
 ) -> dict:
     """
     Reads data_frf from unv file, returns data_frf['frequency'] and data_frf['data'] in format usable in sdypy-EMA
-    :param file_path: path to unv file, incl. file name
-    :param frf_form: form of frf:
-        'receptance' = displacement/force,
-        'mobility' = velocity/force,
-        'accelerance' = acceleration/force,
-        'raw' = all datasets,
-        _custom_string_ = data_frf labeled with _custom_string_
-    :param frf_type: type of frf calculation: H1, H2
-    :param ref_channel: channel number for reference signal
-    :param read_coordinates: read Coordinates of nodes
-    :param read_elements: read element Connectivity and elem_types (Triangle = 3, Quad = 4) (requires read_coordinates)
-    :param dist_file: path to csv file containing the distance from the scanning head to each measurement point
-    :return data_frf: dict with keys: 'Coordinates', 'Connectivity', 'elem_types', 'frequency',
-                                  'frf_form', 'frf_type', 'data_frf', 'ref_channel'
+
+    Parameters
+    ----------
+    file_path : str
+        path to unv file, incl. file name
+    frf_form : str, optional
+        form of frf:
+         'receptance' = displacement/force,
+         'mobility' = velocity/force,
+         'accelerance' = acceleration/force,
+         'raw' = all datasets,
+         _custom_string_ = data_frf labeled with _custom_string_
+    frf_type : str, optional
+        type of frf calculation: H1, H2
+    ref_channel : int, optional
+        channel number for reference signal
+    read_coordinates : bool, optional
+        read Coordinates of nodes
+    read_elements : bool, optional
+        read element Connectivity and elem_types (Triangle = 3, Quad = 4) (requires read_coordinates)
+    dist_file : str, optional
+        path to csv file containing the distance from the scanning head to each measurement point
+
+    Returns
+    -------
+    data_frf : dict
+        Dictionary with keys:
+         'Coordinates',
+         'Connectivity',
+         'elem_types',
+         'frequency',
+         'frf_form',
+         'frf_type',
+         'data_frf',
+         'ref_channel'
     """
 
     uff_file = pyuff.UFF(file_path)
 
     if frf_form == "raw":
         print("Reading data_frf")
         raw_meas_data = uff_file.read_sets()
```

### Comparing `pyCFS-0.0.5/pyCFS/data/extras/vtk_to_cfs_element_types.py` & `pyCFS-0.0.6/pyCFS/data/extras/vtk_to_cfs_element_types.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/pyCFS/data/extras/vtk_types.py` & `pyCFS-0.0.6/pyCFS/data/extras/vtk_types.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/pyCFS/data/io/CFSArray.py` & `pyCFS-0.0.6/pyCFS/data/io/CFSArray.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 class CFSResultArray(np.ndarray):
     # TODO: fix getitem to hint correct type
     # noinspection PyUnresolvedReferences
     """
     Overload/Subclass of numpy.ndarray <https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html>`_
     adding attributes according to CFS HDF5 result data structure.
 
+    .. figure:: ../../../docs/source/resources/data_structures_CFSResultArray.png
+
     Parameters
     ----------
     input_array : array_like
         Input data, in any form that can be converted to an array.  This
         includes lists, lists of tuples, tuples, tuples of tuples, tuples
         of lists and ndarrays.
     quantity : str, optional
@@ -196,15 +198,18 @@
             self.MultiStepID = multi_step_id
         if analysis_type is not None:
             self.AnalysisType = analysis_type
 
 
 class CFSResultInfo:
     """
-    Data structure containing result information for one result
+    Data structure containing result information for one result.
+
+    .. figure:: ../../../docs/source/resources/data_structures_CFSResultInfo.png
+
     """
 
     def __init__(
         self,
         quantity: str | None = None,
         region: str | None = None,
         res_type=cfs_result_type.UNDEFINED,
```

### Comparing `pyCFS-0.0.5/pyCFS/data/io/CFSMeshData.py` & `pyCFS-0.0.6/pyCFS/data/io/CFSMeshData.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 """
-Module containing data processing utilities for writing HDF5 files in openCFS format
+Module defining data structures describing the computational grid.
+
+.. figure:: ../../../docs/source/resources/data_structures_overview.png
+
 """
 
 from __future__ import annotations
 
 import textwrap
 import datetime
 import time
 from functools import partial
 from multiprocessing import Pool
 
 import numpy as np
 from scipy.spatial import Delaunay, KDTree
-from typing import Iterable, Any, List, Dict, Tuple
+from typing import Iterable, Any, List, Dict, Tuple, Optional
 
 from pyCFS.data.io import CFSResultArray
 from pyCFS.data.io.CFSResultData import CFSResultData
 from pyCFS.data.io.cfs_types import cfs_element_type, cfs_result_type
 from pyCFS.data.util import (
     vprint,
     progressbar,
     element_quality,
     list_search,
     element_centroid,
+    element_normal_2d,
+    node_normal_2d,
 )
 from pyCFS.data import v_def
 
 
 class CFSMeshInfo:
     """
     Data structure containing mesh information
 
-    Methods
-    -------
-    * `update_by_coord_types` `(coordinates: np.ndarray, types: np.ndarray)`
+    Notes
+    -----
+    -  ``update_by_coord_types`` ``(coordinates: np.ndarray, types: np.ndarray)``
         Update structure based on coordinate and element types as defined in CFSMeshData
 
     Examples
     --------
     >>> from pyCFS.data.io import CFSReader, CFSMeshInfo
     >>> with CFSReader('file.cfs') as f:
     >>>     coordinates = f.Coordinates
@@ -212,14 +217,16 @@
             self.Dimension = -1
 
 
 class CFSMeshData:
     """
     Data structure containing mesh definition
 
+    .. figure:: ../../../docs/source/resources/data_structures_CFSMeshData.png
+
     Parameters
     ----------
     coordinates : numpy.ndarray, optional
         Coordinate array (Nx3) of the whole mesh (N number of nodes)
     connectivity : numpy.ndarray, optional
         Connectivity array (NxM) of the whole mesh (N number of elements, M maximum number of nodes per element).
         Includes zero entries in case of different element types.
@@ -231,63 +238,82 @@
     verbosity : int, optional
         Verbosity level <=1000 ; see v_def.py for predefined levels. Default is v_def.release.
 
     Attributes
     ----------
     Coordinates : np.ndarray
         Coordinate array (Nx3) of the whole mesh (N number of nodes)
-    Connectivity
+    Connectivity : np.ndarray
+        Connectivity array (NxM) of the whole mesh (N number of elements, M maximum number of nodes per element).
+        Includes zero entries in case of different element types.
     Types : np.ndarray
         Element type array (Nx1) of the whole mesh (N number of elements).
         Element definitions based on pyCFS.data.io.cfs_types.cfs_element_type
     MeshInfo : CFSMeshInfo
         Data structure containing mesh information
     Regions : list[CFSRegData]
         List of data structures containing mesh region definition
-    ElementCentroids
-    Quality
+    ElementCentroids : np.ndarray
+        Centroids of mesh elements
+    Quality : np.ndarray
+        Quality metric of mesh elements
+
+    Notes
+    -----
+    -  ``update_mesh_centroids`` ``(processes: int = None)`` Compute element centroids.
 
-    Methods
-    -------
-    * `update_mesh_centroids` `(processes: int = None)`
-        Compute element centroids.
-    * `get_mesh_centroids` `(el_idx: np.ndarray = None, processes: int = None) -> np.ndarray`
+    -  ``get_mesh_centroids`` ``(el_idx: np.ndarray = None, processes: int = None) -> np.ndarray``
         Compute geometric centers of mesh elements.
-    * `update_mesh_quality` `(metric='quality', processes: int = None)`
-        Compute mesh metric based on 'metric'.
-    * `merge` `(other: CFSMeshData) -> CFSMeshData`
+
+    -  ``get_mesh_surface_normals`` ``(restype: restype=cfs_result_type.ELEMENT, node_idx_include: np.ndarray = None, el_idx_include: np.ndarray = None, rocesses: int = None) -> np.ndarray``
+        Compute surface normal vectors of surface mesh.
+
+    -  ``update_mesh_quality`` ``(metric='quality', processes: int = None)``
+        Compute mesh metric based on ‘metric’.
+
+    -  ``merge`` ``(other: CFSMeshData) -> CFSMeshData``
         Merges mesh with other mesh removing duplicate coordinates and elements
-    * `update_info()`
-        Update structure based on coordinate and element types
-    * `drop_unused_nodes_elements` `(reg_data_list: list[CFSRegData])`
+
+    -  ``update_info()`` Update structure based on coordinate and element types
+
+    -  ``drop_unused_nodes_elements`` ``(reg_data_list: list[CFSRegData])``
         Drop nodes and elements that are not used in the given list of groups/regions.
-    * `convert_to_simplex` `(idx_convert: np.ndarray = None, result_data=None)`
+
+    -  ``convert_to_simplex`` ``(idx_convert: np.ndarray = None, result_data=None)``
         Convert arbitrary 3D elements into simplexes (tetrahedra), by applying Delaunay triangulation.
-    * `convert_quad2tria` `(idx_convert: np.ndarray = None, result_data=None)`
-        Convert QUAD4 elements into TRIA3 elements. If 'idx_convert' is unspecified all QUAD4 in the mesh are converted.
-    * `get_region_nodes` `(region: str) -> np.ndarray`
-    * `get_region_elements` `(region: str) -> np.ndarray`
-    * `get_region_coordinates` `(region: str) -> np.ndarray`
-    * `get_region_connectivity` `(region: str) -> np.ndarray`
-    * `get_region_centroids` `(region: str, processes: int = None) -> np.ndarray`
-    * `reorient_region` `(region_name: str) -> None`
-    * `reorient_elements` `(idx_reorient: list) -> None`
+
+    -  ``convert_quad2tria`` ``(idx_convert: np.ndarray = None, result_data=None)``
+        Convert QUAD4 elements into TRIA3 elements. If ‘idx_convert’ is unspecified all QUAD4 in the mesh are converted.
+
+    -  ``get_region_nodes`` ``(region: str) -> np.ndarray``
+
+    -  ``get_region_elements`` ``(region: str) -> np.ndarray``
+
+    -  ``get_region_coordinates`` ``(region: str) -> np.ndarray``
+
+    -  ``get_region_connectivity`` ``(region: str) -> np.ndarray``
+
+    -  ``get_region_centroids`` ``(region: str, processes: int = None) -> np.ndarray``
+
+    -  ``reorient_region`` ``(region_name: str) -> None``
+
+    -  ``reorient_elements`` ``(idx_reorient: list) -> None``
 
     Examples
     --------
     >>> from pyCFS.data.io import CFSReader, CFSMeshInfo
     >>> with CFSReader('file.cfs') as f:
     >>>     coordinates = f.Coordinates
     >>>     connectivity = f.Connectivity
     >>>     ElementTypes = f.ElementTypes
     >>>     region_data = f.MeshGroupsRegions
     >>> mesh = CFSMeshData(coordinates=coordinates, connectivity=connectivity, ElementTypes=ElementTypes,
     >>>                    regions=region_data)
 
-    """
+    """  # noqa : E501
 
     def __init__(
         self,
         coordinates=np.empty((0, 3)),
         connectivity=np.empty((0, 1)),
         types=np.empty(0),
         regions: List[CFSRegData] | None = None,
@@ -413,36 +439,123 @@
         if el_idx is None:
             el_idx_it: Iterable[Any] = range(self.Connectivity.shape[0])
         elif isinstance(el_idx, np.ndarray):
             el_idx_it = el_idx
         else:
             raise TypeError("el_idx must be of type numpy.ndarray, or None")
 
-        mesh_centroids = np.zeros((self.Connectivity.shape[0], 3), dtype=float)
-        vprint("Computing mesh centroids", end="", verbose=self._Verbosity >= v_def.debug)
+        mesh_centroids = np.zeros((self.Connectivity[el_idx_it].shape[0], 3), dtype=float)
 
-        with Pool(processes=processes) as pool:
-            t_start = time.time()
-            for i, res in enumerate(
-                pool.map(
-                    partial(
-                        _compute_mesh_centroids,
-                        connectivity=self.Connectivity,
-                        coordinates=self.Coordinates,
-                    ),
-                    el_idx_it,
-                )
-            ):
-                mesh_centroids[i] = res
-        vprint(
-            f" | Elapsed time: {datetime.timedelta(seconds=round(time.time() - t_start))}",
+        t_start = time.time()
+        el_idx_it_done: List = []
+        for cidx in progressbar(
+            range(self.Connectivity.shape[1]),
+            prefix="Computing mesh centroids: ",
             verbose=self._Verbosity >= v_def.debug,
-        )
+        ):
+            if cidx == 0:
+                conn = self.Connectivity[el_idx_it, :]
+            else:
+                conn = self.Connectivity[el_idx_it, 0:-cidx]
+
+            el_idx_it_cur = np.intersect1d(el_idx_it, np.argwhere(np.all(conn, axis=1)))  # type: ignore[call-overload]
+            el_idx_it_cur = el_idx_it_cur[~np.in1d(el_idx_it_cur, el_idx_it_done)]
+            element_connectivity = conn[el_idx_it_cur, :]
+            element_coordinates = self.Coordinates[element_connectivity - 1, :]
+            mesh_centroids[el_idx_it_cur] = element_centroid(element_coordinates)
+
+            el_idx_it_done += list(el_idx_it_cur)
+            if el_idx_it_cur.size > 0 and np.all(conn):
+                vprint(
+                    f"Computing mesh centroids | Elapsed time: {datetime.timedelta(seconds=int(time.time() - t_start))}",
+                    verbose=self._Verbosity >= v_def.debug,
+                )
+                break
+
         return mesh_centroids
 
+    def get_mesh_surface_normals(
+        self,
+        restype=cfs_result_type.ELEMENT,
+        node_idx_include: Optional[np.ndarray] = None,
+        el_idx_include: Optional[np.ndarray] = None,
+        processes: Optional[int] = None,
+    ) -> np.ndarray:
+        """
+        Compute surface normal vectors of surface mesh.
+
+        Parameters
+        ----------
+        restype: cfs_result_type, optional
+        node_idx_include: numpy.ndarray, optional
+        el_idx_include: numpy.ndarray, optional
+        processes: int, optional
+
+        Returns
+        -------
+        numpy.ndarray
+
+        Examples
+        --------
+        >>> from pyCFS.data.io import CFSReader
+        >>> with CFSReader('file.cfs') as f:
+        >>>     mesh = f.MeshData
+        >>> mesh_normal_vectors = mesh.get_mesh_surface_normals()
+        """
+        _supported_types = [cfs_element_type.TRIA3, cfs_element_type.QUAD4, cfs_element_type.POLYGON]
+
+        if node_idx_include is None:
+            node_idx_include = np.arange(self.Coordinates.shape[0])
+        if el_idx_include is None:
+            el_idx_include = np.arange(self.Connectivity.shape[0])
+
+        # Get supported elements
+        el_idx_supported = np.argwhere(np.in1d(self.Types[el_idx_include], _supported_types)).flatten()
+
+        if restype == cfs_result_type.ELEMENT:
+            surface_normals = np.zeros((self.Connectivity[el_idx_include, :].shape[0], 3))
+            surface_normals.fill(np.nan)
+            # Extract element coordinates for supported elements
+            el_coord = self.Coordinates[self.Connectivity[el_idx_supported, 0:3] - 1]
+            # Compute element surface normal vecotors
+            surface_normals[el_idx_supported, :] = element_normal_2d(element_coordinates=el_coord)
+
+        elif restype == cfs_result_type.NODE:
+            # raise NotImplementedError("Evaluating surface normal on nodes currently not implemented.")
+            coord = self.Coordinates[node_idx_include, :]
+            conn = self.Connectivity[el_idx_include, :][el_idx_supported, :]
+
+            surface_normals = np.zeros((coord.shape[0], 3))
+            surface_normals.fill(np.nan)
+
+            vprint("Computing node normals ", end="", verbose=self._Verbosity >= v_def.debug)
+            with Pool(processes=processes) as pool:
+                t_start = time.time()
+                for idx, res in enumerate(
+                    pool.map(
+                        partial(
+                            _compute_mesh_node_normal,
+                            connectivity=conn,
+                            coordinates=coord,
+                        ),
+                        node_idx_include,
+                    )
+                ):
+                    surface_normals[node_idx_include[idx], :] = res
+            vprint(
+                f" | Elapsed time: {datetime.timedelta(seconds=int(time.time() - t_start))}",
+                verbose=self._Verbosity >= v_def.debug,
+            )
+        else:
+            raise NotImplementedError(
+                f"Evaluating surface normal on {restype} not implemented. Supported on NODE and ELEMENT, only!"
+            )
+
+        return surface_normals
+
     @property
     def Quality(self) -> np.ndarray | None:
         """
         Compute mesh metric with standard parameters. Doesn't update automatically for large meshes.
 
         Returns
         -------
@@ -662,34 +775,36 @@
                 # Add elements to connectivity and types
                 conn_add = np.zeros((reg.Nodes.size, self.Connectivity.shape[1]))
                 conn_add[:, 0] = reg.Nodes
                 el_types_add = np.array([cfs_element_type.POINT for _ in range(reg.Nodes.size)], dtype=np.int32)
                 self.Connectivity = np.vstack((self.Connectivity, conn_add))
                 self.Types = np.hstack((self.Types, el_types_add))
 
-    def drop_unused_nodes_elements(self, reg_data_list: List[CFSRegData]):
+    def drop_unused_nodes_elements(self, reg_data_list: Optional[List[CFSRegData]] = None):
         """
         Drop nodes and elements that are not used in the given list of groups/regions.
 
         Parameters
         ----------
-        reg_data_list : list[CFSRegData]
+        reg_data_list : list[CFSRegData], optional
             List of groups/regions
 
         Examples
         --------
         >>> from pyCFS.data.io import CFSReader
         >>> from pyCFS.data.util import list_search
         >>> with CFSReader('file1.cfs') as f:
         >>>     mesh = f.MeshData
         >>>     regions_data = f.MeshGroupsRegions
         >>> regions_data_keep = [list_search(regions_data, 'region_name')]
         >>> mesh.drop_unused_nodes_elements(reg_data_list=regions_data_keep)
 
         """
+        if reg_data_list is None:
+            reg_data_list = self.Regions
         self._drop_unused_elements(reg_data_list)
         self._drop_unused_nodes(reg_data_list)
         self.Regions = reg_data_list
 
     # noinspection PyTypeChecker,LongLine
     def _drop_unused_elements(self, reg_data_list: List[CFSRegData]) -> bool:
         """
@@ -1138,14 +1253,16 @@
                 raise NotImplementedError(f"Reorienting of element type {self.Types[el_idx]} not implemented!")
 
 
 class CFSRegData:
     """
     Data structure containing mesh region definition
 
+    .. figure:: ../../../docs/source/resources/data_structures_CFSRegData.png
+
     Parameters
     ----------
     name : str, optional
         Group/Region name
     elements : numpy.ndarray, optional
         array of element ids (Nx1) of the group/region (N number of elements in the group/region).
     nodes : numpy.ndarray, optional
@@ -1157,26 +1274,28 @@
     verbosity : int, optional
         Verbosity level <=1000 ; see v_def.py for predefined levels. Default is v_def.release.
 
     Attributes
     ----------
     Name : str
         Group/Region name
-    Elements
-    Nodes
+    Elements : numpy.ndarray
+        array of element ids, starting from 1, (Nx1) of the group/region (N number of elements in the group/region).
+    Nodes : numpy.ndarray
+        array of node ids, starting from 1, (Nx1) of the group/region (N number of nodes in the group/region).
     Dimension : int
         Group/Region dimension
     IsGroup : bool
         flag indicating if the entity is a group.
 
-    Methods
-    -------
-    * `merge` `(other: CFSRegData)`
-        Merges region with other region removing duplicate node/element indices
-    * `update_nodes_from_elements` `(elems: np.ndarray, connectivity: np.ndarray) -> (np.ndarray, np.ndarray)`
+    Notes
+    -----
+    -  ``merge`` ``(other: CFSRegData)`` Merges region with other region removing duplicate node/element indices
+
+    -  ``update_nodes_from_elements`` ``(elems: np.ndarray, connectivity: np.ndarray) -> (np.ndarray, np.ndarray)``
         Update region nodes based on element ids.
 
     Examples
     --------
     >>> from pyCFS.data.io import CFSReader, CFSMeshInfo
     >>> with CFSReader('file.cfs') as f:
     >>>     coordinates = f.Coordinates
@@ -1326,22 +1445,42 @@
         self.Nodes = nodes
         self.Elements = elems
 
         return node_idx, elem_idx
 
 
 # Usability functions
-def _compute_mesh_centroids(idx: int, connectivity: np.ndarray, coordinates: np.ndarray):
-    """Helper function for CFSMeshData._get_mesh_centroids. Computes element centroid for single element in mesh"""
-    element_connectivity = connectivity[idx, :]
-    # Remove 0 entries
-    idx_zeros = np.argwhere(element_connectivity == 0)
-    element_connectivity = np.delete(element_connectivity, idx_zeros)
-    element_coordinates = coordinates[element_connectivity - 1, :]
-    return element_centroid(element_coordinates)
+def _compute_mesh_node_normal(node_idx: int, connectivity: np.ndarray, coordinates: np.ndarray) -> np.ndarray:
+    """
+    Helper function for CFSMeshData.get_surface_normals. Computes node surface normal for single node in mesh.
+
+    Parameters
+    ----------
+    node_idx : int
+    connectivity : np.ndarray
+    coordinates : np.ndarray
+
+    Returns
+    -------
+    np.ndarray
+
+    """
+    el_idx = np.argwhere(np.any(connectivity == node_idx + 1, axis=1)).flatten()
+    node_close_ids = connectivity[el_idx, :]
+    # Put center node id in 1st position
+    node_neighbor_ids = np.empty_like(node_close_ids, dtype=int)
+    for row in range(node_neighbor_ids.shape[0]):
+        neighbor_n_idx = np.argwhere(node_close_ids[row, :] != node_idx + 1).flatten()
+        # Ensure consistent node sequence (23,13->31,12), when common node is 2nd node in connectivity
+        if (node_close_ids[row, :] == node_idx + 1)[1]:
+            neighbor_n_idx[:2] = np.array([2, 0])
+        node_neighbor_ids[row, 1:] = node_close_ids[row, neighbor_n_idx]
+        node_neighbor_ids[row, 0] = node_idx + 1
+    neighbor_coord = coordinates[node_neighbor_ids - 1, 0:3]
+    return node_normal_2d(neighbor_coord)
 
 
 def _compute_mesh_quality(
     idx: int, connectivity: np.ndarray, coordinates: np.ndarray, el_types: np.ndarray, metric: str
 ):
     """Helper function for CFSMeshData._get_mesh_quality. Computes element quality for single element in mesh"""
     element_connectivity = connectivity[idx, :]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyCFS-0.0.5/pyCFS/data/io/CFSReader.py` & `pyCFS-0.0.6/pyCFS/data/io/CFSReader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """
 Module containing data processing utilities for writing HDF5 files in openCFS format
 """
 
 from __future__ import annotations
 
+import datetime
 import functools
+import time
+from multiprocessing import Pool
 
 import h5py
 import numpy as np
 from scipy.spatial import KDTree
-from typing import List, Tuple
+from typing import List, Tuple, Optional
 
 from pyCFS.data.io.CFSMeshData import CFSMeshData, CFSMeshInfo, CFSRegData
 from pyCFS.data.io.CFSResultData import CFSResultData, CFSResultInfo
 from pyCFS.data.io.cfs_types import cfs_result_type, cfs_analysis_type
 
 from pyCFS.data.util import vprint, progressbar
 
@@ -43,14 +46,19 @@
     """
     Base class for all reading operations
 
     Parameters
     ----------
     filename : str
         Path to the hdf5 file.
+    multistep_id : int, optional
+        MultiStepID to read result data from. The default is ``1``
+    processes : int, optional
+        Number of processes to use for parallelized operations. The default is ``None``, in which case all available
+        cores are used.
     h5driver : str, optional
         Driver used to read the hdf5 file (see h5py documentation). The default is ``None``, in which case the standard
         driver is used
     verbosity : int, optional
         Verbosity level <=1000 ; see v_def.py for predefined levels. Default is v_def.release.
 
     Attributes
@@ -65,60 +73,86 @@
     MeshRegions
     ResultInfo
     MultiStepIDs
     MultiStepData
     AnalysisType
     ResultQuantities
 
-    Methods
-    -------
-    * `set_multi_step` `(multi_step_id: int)`
-        Sets the multiStepID
-    * `check_group_region` `(region: str) -> bool`
-        Checks whether a mesh entity is a group or a region instead.
-    * `get_mesh_region` `(region: str, is_group: bool = None) -> CFSRegData`
-        Reads mesh region or group.
-    * `get_mesh_region_dimension` `(region: str, is_group: bool = None)`
-    * `get_mesh_region_nodes` `(region: str, is_group: bool = None)`
-    * `get_mesh_region_elements` `(region: str, is_group: bool = None)`
-    * `get_mesh_region_coordinates` `(region: str, is_group: bool = None) -> np.ndarray`
+    Notes
+    -----
+    -  ``set_multi_step`` ``(multi_step_id: int)`` Sets the multiStepID
+
+    -  ``check_group_region`` ``(region: str) -> bool`` Checks whether a mesh entity is a group or a region instead.
+
+    -  ``get_mesh_region`` ``(region: str, is_group: bool = None) -> CFSRegData`` Reads mesh region or group.
+
+    -  ``get_mesh_region_dimension`` ``(region: str, is_group: bool = None)``
+
+    -  ``get_mesh_region_nodes`` ``(region: str, is_group: bool = None)``
+
+    -  ``get_mesh_region_elements`` ``(region: str, is_group: bool = None)``
+
+    -  ``get_mesh_region_coordinates`` ``(region: str, is_group: bool = None) -> np.ndarray``
         Reads node Coordinates of a region or group.
-    * `get_mesh_region_connectivity` `(region: str, is_group: bool = None) -> np.ndarray`
+
+    -  ``get_mesh_region_connectivity`` ``(region: str, is_group: bool = None) -> np.ndarray``
         Reads element Connectivity of a region or group.
-    * `get_mesh_region_types` `(region: str, is_group: bool = None) -> np.ndarray`
+
+    -  ``get_mesh_region_types`` ``(region: str, is_group: bool = None) -> np.ndarray``
         Reads element types of a region or group.
-    * `get_closest_node` `(coordinate: np.ndarray, region: str = None, eps: float = 1e-3) -> np.ndarray`
+
+    -  ``get_closest_node`` ``(coordinate: np.ndarray, region: str = None, eps: float = 1e-3) -> np.ndarray``
         Return node ids of closest nodes to coordinate array.
-    * `get_closest_element` `(coordinate: np.ndarray, region: str = None, eps=1e-3)`
+
+    -  ``get_closest_element`` ``(coordinate: np.ndarray, region: str = None, eps=1e-3)``
         Return element ids of closest element centroids to coordinate array.
-    * `get_result_info_quantity` `(quantity: str) -> CFSResultInfo`
-    * `get_result_regions` `(quantity) -> list[str]`
-    * `get_dim_names` `(quantity) -> list[str]`
-    * `get_restype` `(quantity) -> cfs_result_type`
-    * `get_step_numbers` `(quantity) -> np.ndarray`
-    * `get_step_values` `(quantity) -> np.ndarray`
-    * `get_data_step` `(step_num: int, quantity: str, region: str, restype: cfs_result_type, ds_idx: tuple[int, :] = ()) -> (np.ndarray, bool)`
-    * `get_data_steps` `(quantity, region, ds_idx: tuple[int, :] = ()) -> (list[np.ndarray], bool)`
-    * `check_data_complex` `(quantity: str, region: str, restype: cfs_result_type) -> bool`
+
+    -  ``get_result_info_quantity`` ``(quantity: str) -> CFSResultInfo``
+
+    -  ``get_result_regions`` ``(quantity) -> list[str]``
+
+    -  ``get_dim_names`` ``(quantity) -> list[str]``
+
+    -  ``get_restype`` ``(quantity) -> cfs_result_type``
+
+    -  ``get_step_numbers`` ``(quantity) -> np.ndarray``
+
+    -  ``get_step_values`` ``(quantity) -> np.ndarray``
+
+    -  ``get_data_step`` ``(step_num: int, quantity: str, region: str, restype: cfs_result_type, ds_idx: tuple[int, :] = ()) -> (np.ndarray, bool)``
+
+    -  ``get_data_steps`` ``(quantity, region, ds_idx: tuple[int, :] = ()) -> (list[np.ndarray], bool)``
+
+    -  ``check_data_complex`` ``(quantity: str, region: str, restype: cfs_result_type) -> bool``
         Checks if result contains real or complex data
-    * `get_single_data_steps` `(quantity: str, region: str, entity_id: int) -> np.ndarray`
+
+    -  ``get_single_data_steps`` ``(quantity: str, region: str, entity_id: int) -> np.ndarray``
         Get data over all steps of given element/node id (id starting from 0).
 
+
     Examples
     --------
     >>> from pyCFS.data.io import CFSReader
     >>> with CFSReader('file.cfs') as f:
     >>>     mesh = f.MeshData
     >>>     results = f.MultiStepData
 
     """
 
-    def __init__(self, filename: str, multistep_id=1, h5driver: str | None = None, verbosity=v_def.release) -> None:
+    def __init__(
+        self,
+        filename: str,
+        multistep_id=1,
+        processes: Optional[int] = None,
+        h5driver: Optional[str] = None,
+        verbosity=v_def.release,
+    ) -> None:
         """Initialize the reader"""
         self._filename = filename
+        self.Processes = processes
         self._h5driver = h5driver
         self._multiStepID = multistep_id
         self._Verbosity = verbosity
 
     def __enter__(self):
         return self
 
@@ -803,62 +837,89 @@
         self,
         step_num: int,
         quantity: str,
         region: str,
         restype: cfs_result_type,
         ds_idx: tuple = (),
     ) -> Tuple[np.ndarray, bool]:
-        with h5py.File(self._filename, driver=self._h5driver) as f:
-            h5_data_path = f"Results/Mesh/MultiStep_{self._multiStepID}/Step_{step_num}/{quantity}/{region}/{restype}"
-            data_names = list(f[h5_data_path].keys())
-            if "Imag" in data_names:
-                data_step = f[f"{h5_data_path}/Real"][ds_idx] + f[f"{h5_data_path}/Imag"][ds_idx] * 1j
-                is_complex = True
-            else:
-                data_step = f[f"{h5_data_path}/Real"][ds_idx]
-                is_complex = False
-
-        if data_step.ndim == 1:
-            data_step = data_step.reshape((data_step.shape[0], 1))
 
-        return data_step, is_complex
+        return _get_data_step(
+            step_num=step_num,
+            filename=self._filename,
+            h5driver=self._h5driver,
+            multiStepID=self._multiStepID,
+            quantity=quantity,
+            region=region,
+            restype=restype,
+            ds_idx=ds_idx,
+        )
 
     def get_data_steps(self, quantity, region, ds_idx: tuple = ()) -> Tuple[np.ndarray, bool]:
         step_numbers = self.get_step_numbers(quantity)
         # Initialize with 1st step
         is_complex = False
+        res_type = self.get_restype(quantity)
         data_step, flag_complex = self.get_data_step(
             int(step_numbers[0]),
             quantity,
             region,
-            self.get_restype(quantity),
+            res_type,
             ds_idx=ds_idx,
         )
         is_complex = is_complex or flag_complex
         data_dtype: type[float] | type[complex]
         if is_complex:
             data_dtype = complex
         else:
             data_dtype = float
 
         data = np.zeros([step_numbers.size] + list(data_step.shape), dtype=data_dtype)
         data[0, :, :] = data_step
 
-        for step_idx, step_num in enumerate(
-            progressbar(
-                step_numbers[1:],
-                prefix=f"Reading {quantity} on {region}: ",
+        if self.Processes == 1:
+            # Implement without map for improved performance
+            for step_idx, step_num in enumerate(
+                progressbar(
+                    step_numbers[1:],
+                    prefix=f"Reading {quantity} on {region}: ",
+                    verbose=self._Verbosity >= v_def.more,
+                )
+            ):
+                data_step, flag_complex = self.get_data_step(step_num, quantity, region, res_type, ds_idx=ds_idx)
+                is_complex = is_complex or flag_complex
+                data[step_idx + 1, :, :] = data_step
+        else:
+            # Execute on multiprocessing pool
+            vprint(f"Reading {quantity} on {region}", end="", verbose=self._Verbosity >= v_def.more)
+            with Pool(processes=self.Processes) as pool:
+                t_start = time.time()
+                for step_idx, res in enumerate(
+                    pool.map(
+                        functools.partial(
+                            _get_data_step,
+                            filename=self._filename,
+                            h5driver=self._h5driver,
+                            multiStepID=self._multiStepID,
+                            quantity=quantity,
+                            region=region,
+                            restype=res_type,
+                            ds_idx=ds_idx,
+                        ),
+                        step_numbers[1:],
+                    )
+                ):
+                    data_step, flag_complex = res
+                    is_complex = is_complex or flag_complex
+                    data[step_idx + 1, :, :] = data_step
+
+            vprint(
+                f" | Elapsed time: {datetime.timedelta(seconds=round(time.time() - t_start))}",
                 verbose=self._Verbosity >= v_def.more,
             )
-        ):
-            data_step, flag_complex = self.get_data_step(
-                step_num, quantity, region, self.get_restype(quantity), ds_idx=ds_idx
-            )
-            is_complex = is_complex or flag_complex
-            data[step_idx + 1, :, :] = data_step
+
         return data, is_complex
 
     @_catch_key_error
     def check_data_complex(self, quantity: str, region: str, restype: cfs_result_type) -> bool:
         """Checks if result contains real or complex data"""
         step_num = self.get_step_numbers(quantity)[0]
         with h5py.File(self._filename, driver=self._h5driver) as f:
@@ -874,7 +935,33 @@
         """Get data over all steps of given element/node id (id starting from 0)."""
 
         dim = len(self.get_dim_names(quantity=quantity))
         ds_idx = (entity_id, range(dim))
         data, _ = self.get_data_steps(quantity, region, ds_idx)
 
         return np.array(data)
+
+
+def _get_data_step(
+    step_num: int,
+    filename,
+    h5driver,
+    multiStepID,
+    quantity: str,
+    region: str,
+    restype: cfs_result_type,
+    ds_idx: tuple = (),
+) -> Tuple[np.ndarray, bool]:
+    with h5py.File(filename, driver=h5driver) as f:
+        h5_data_path = f"Results/Mesh/MultiStep_{multiStepID}/Step_{step_num}/{quantity}/{region}/{restype}"
+        data_names = list(f[h5_data_path].keys())
+        if "Imag" in data_names:
+            data_step = f[f"{h5_data_path}/Real"][ds_idx] + f[f"{h5_data_path}/Imag"][ds_idx] * 1j
+            is_complex = True
+        else:
+            data_step = f[f"{h5_data_path}/Real"][ds_idx]
+            is_complex = False
+
+    if data_step.ndim == 1:
+        data_step = data_step.reshape((data_step.shape[0], 1))
+
+    return data_step, is_complex
```

### Comparing `pyCFS-0.0.5/pyCFS/data/io/CFSResultData.py` & `pyCFS-0.0.6/pyCFS/data/io/CFSResultData.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """
-Module containing data processing utilities for writing HDF5 files in openCFS format
+Module defining data structures describing the result data.
+
+.. figure:: ../../../docs/source/resources/data_structures_overview.png
+
 """
 
 from __future__ import annotations
 
 import textwrap
 
 import numpy as np
@@ -17,25 +20,40 @@
 
 
 # noinspection PyAttributeOutsideInit
 class CFSResultData:
     """
     Data structure containing result data (one object supports currently a single MultiStep only!)
 
+    .. figure:: ../../../docs/source/resources/data_structures_CFSResultData.png
+
     Parameters
     ----------
     analysis_type : pyCFS.data.io.cfs_types.cfs_analysis_type, optional
         Analysis type. Definitions based on pyCFS.data.io.cfs_types.cfs_analysis_type. The default is ``NO_ANALYSIS``.
     multi_step_id : int, optional
         MultiStep (also known as SequenceStep) ID. The default value is ``1``.
     data : list[pyCFS.data.io.CFSResultArray], optional
         List of result arrays. The default is ``None`` in which case the result data object will be initialized empty.
     verbosity : int, optional
         Verbosity level <=1000 ; see v_def.py for predefined levels. Default is v_def.release.
 
+    Attributes
+    ----------
+    AnalysisType : pyCFS.data.io.cfs_types.cfs_analysis_type
+        Analysis type. Definitions based on pyCFS.data.io.cfs_types.cfs_analysis_type.
+    MultiStepID : int
+        MultiStep (also known as SequenceStep) ID.
+    Data : List[pyCFS.data.io.CFSResultArray]
+        List of data arrays containing result data (with metadata).
+    ResultInfo : List[pyCFS.data.io.CFSResultInfo]
+        List of structures containing information about the corresponding CFSResultArray object in self.Data.
+    StepValues : numpy.ndarray
+        Step Values of MultiStep property. All data sets of one MultiStep must have the same step values currently!
+
     Examples
     --------
     >>> import numpy
     >>> from pyCFS.data.io import CFSResultArray, CFSResultData
     >>> from pyCFS.data.io.cfs_types import cfs_result_type
     >>> data = numpy.array([0,1,2,3])
     >>> result_array = CFSResultArray(data,quantity='quantity_name', region='region_name', step_value=0,
@@ -297,16 +315,24 @@
                 if restype is None or restype == item.ResType:
                     return item
         raise LookupError(f"Could not find result data array for ({quantity}, {region})")
 
     def combine_with(self, other: CFSResultData, resolve_match="exception") -> CFSResultData:
         """
         Merges result data structures
-        param: resolve_match= 'exception' raises exception on matching datasets
-                              'add'       adds datasets on matching datasets
+
+        Parameters
+        ----------
+        other : CFSResultData
+        resolve_match : str, optional
+            'exception' (Default) raises exception on matching datasets, 'add' adds datasets on matching datasets
+
+        Returns
+        -------
+        CFSResultData
         """
         for array_idx, r_data in enumerate(other.Data):
             if r_data.Quantity is None or r_data.Region is None:
                 raise ValueError(f"MetaData {r_data.MetaData} of result not properly defined!")
             # Check if dataset alread exists
             try:
                 r_data_match = self.get_data_array(
```

### Comparing `pyCFS-0.0.5/pyCFS/data/io/CFSWriter.py` & `pyCFS-0.0.6/pyCFS/data/io/CFSWriter.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,32 +38,39 @@
         Verbosity level <=1000 ; see v_def.py for predefined levels. Default is v_def.release.
 
     Attributes
     ----------
     CompressionLvl : int
         GZIP compression level used for writing all large datasets in the hdf5 file.
 
-    Methods
-    -------
-    * `create_file` `(mesh_data: CFSMeshData = None, result_data: CFSResultData = None)`
+    Notes
+    -----
+    -  ``create_file`` ``(mesh_data: CFSMeshData = None, result_data: CFSResultData = None)``
         Perform all steps to create an empty HDF5 file and write Mesh and (optionally) Results to it.
-    * `create_mesh` `(MeshInfo: CFSMeshInfo, regions_data: list[CFSRegData])`
+
+    -  ``create_mesh`` ``(MeshInfo: CFSMeshInfo, regions_data: list[CFSRegData])``
         Create Mesh structure and write mesh information to the active hdf5 file.
-    * `write_mesh` `(mesh_data: CFSMeshData)`
+
+    -  ``write_mesh`` ``(mesh_data: CFSMeshData)``
         Write Mesh data to the active hdf5 file.
-    * `prepare_write_multistep` `(res_info: list[CFSResultInfo], res_shape_dict: dict, multiStep=1, AnalysisType='transient')`
+
+    -  ``prepare_write_multistep`` ``(res_info: list[CFSResultInfo], res_shape_dict: dict, multiStep=1, AnalysisType='transient')``
         Write ResultDescription and create datasets (needs to be done a priori in case of parallel write)
-    * `perform_write_multistep` `(result_data: CFSResultData)`
+
+    -  ``perform_write_multistep`` ``(result_data: CFSResultData)``
         Write data to MultiStep
-    * `finalize_write_multistep` `(res_info: list[CFSResultInfo], multiStep=1)`
+
+    -  ``finalize_write_multistep`` ``(res_info: list[CFSResultInfo], multiStep=1)``
         Write datasets to ResultsDescription that need to be written after the data (in case of parallel write)
-    * `write_multistep` `(result_data: CFSResultData)`
+
+    -  ``write_multistep`` ``(result_data: CFSResultData)``
         Write ResultDescription and create datasets, write data to multistep and write datasets to ResultsDescription
         that need to be written after the data (in case of parallel write)
 
+
     Examples
     --------
     >>> from pyCFS.data.io import CFSReader, CFSWriter
     >>> with CFSReader('file.cfs') as f:
     >>>     mesh = f.MeshData
     >>>     results = f.MultiStepData
     >>> with CFSWriter('file.cfs') as f:
```

### Comparing `pyCFS-0.0.5/pyCFS/data/io/cfs_types.py` & `pyCFS-0.0.6/pyCFS/data/io/cfs_types.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/pyCFS/data/operators/fit_geometry.py` & `pyCFS-0.0.6/pyCFS/data/operators/transformation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+"""
+Module containing methods for mesh/data transformation operations.
+"""
+
 #    Fit Geometry
 #
 #      Processing Tool for CFS HDF5 files
 #
 #      This script fits a region to a target region by means of rotation and translation transformations based on
 #      minimizing the squared distance of all source nodes to the respective nearest neighbor on the target mesh.
 #
 # Usage
-#   python fit_geometry.py --file-target filename_target.cfs --file-src filename_src.cfs --file-out filename_out.cfs
+#   python transformation.py --file-target filename_target.cfs --file-src filename_src.cfs --file-out filename_out.cfs
 #   # Fits all regions in "filename_src.cfs" to all regions in "filename_target.cfs" with initially no transformation
-#   python fit_geometry.py ... --regions-target region1,region2
+#   python transformation.py ... --regions-target region1,region2
 #   # Fits all regions in "filename_src.cfs" to "region1" and "region2" in "filename_target.cfs"
-#   python fit_geometry.py ... --regions-src region1,region2
+#   python transformation.py ... --regions-src region1,region2
 #   # Fits regions "region1" and "region2" in "filename_src.cfs" to all regions in "filename_target.cfs"
-#   python fit_geometry.py ... --init-param 0,1,0,0,3.14,0
+#   python transformation.py ... --init-param 0,1,0,0,3.14,0
 #   # Fits all regions in "filename_src.cfs" to all regions in "filename_target.cfs" with initial transformation
 #     parameters [x,y,z,rx,ry,rz] with Euler parameters in 'XYZ' sequence (for more than 1 source region add
 #     additional initial transformation parameters)
 #
 # Input Parameters
 #   * filename_src - filename of HDF5 file source
 #   * filename_out - filename of HDF5 file output
```

### Comparing `pyCFS-0.0.5/pyCFS/data/operators/interpolators.py` & `pyCFS-0.0.6/pyCFS/data/operators/interpolators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,33 @@
+"""
+Module containing methods for interpolation operations.
+"""
+
 from __future__ import annotations
 
-from typing import Optional
+from typing import Optional, List
 
 import numpy as np
 import scipy
 from scipy.spatial import KDTree
 
 from pyCFS.data.io import cfs_types
 from pyCFS.data import io
+from pyCFS.data.operators import projection_interpolation
 from pyCFS.data.util import progressbar
 
 
 def interpolation_matrix_cell_to_node(coordinates, connectivity) -> scipy.sparse.csc_array:
     """
-    Computes interpolation matrix such that e = sum_{i=1}^n  v_i. Thereby, e is the data_N2C assigned to the cell,
-    n the number of nodes of one element, and v_i the nodal data_N2C
-    """
+    Computes interpolation matrix such that :math:`e = \\sum_{i=1}^n  v_i`. Thereby, e is the data_N2C assigned to
+    the cell, n the number of nodes of one element, and v_i the nodal data_N2C
+
+    .. figure:: ../../../docs/source/resources/cell2node.png
+
+    """  # noqa : W605
     # TODO Investigate why csc array does produce crashes (double corrupted,m_alloc,...)
     matrix_shape = (coordinates.shape[0], connectivity.shape[0])
 
     val_lst = []
     row_ind_lst = []
     col_ptr_lst = []
     counter = 0
@@ -40,16 +48,19 @@
         (val.flatten(), row_ind.flatten(), col_ptr), matrix_shape, dtype=float
     )
     return interpolation_matrix
 
 
 def interpolation_matrix_node_to_cell(coordinates, connectivity) -> scipy.sparse.csr_array:
     """
-    Computes interpolation matrix such that v = 1/n  e_i. Thereby, v is the data_N2C located to the node,
+    Computes interpolation matrix such that :math:`v = (1/n)  e_i`. Thereby, v is the data_N2C located to the node,
     n the number of nodes of the element, and e_i the data_N2C of cell i.
+
+    .. figure:: ../../../docs/source/resources/node2cell.png
+
     """
     matrix_shape = (connectivity.shape[0], coordinates.shape[0])
 
     val_lst = []
     col_ind_lst = []
     row_ptr_lst = []
     counter = 0
@@ -77,16 +88,17 @@
     interpolation_exp=2.0,
     max_distance: float | None = None,
     formulation: Optional[str] = None,
 ) -> scipy.sparse.csr_array | scipy.sparse.csc_array:
     """
     Computes interpolation matrix based on nearest neighbor search with inverse distance weighting (Shepard's method)
     (see https://opencfs.gitlab.io/userdocu/DataExplanations/NN/). Nearest neighbors are searched for each point on the
-    source (forward) or target (backward) grid.
+    source (forward) or target (backward) grid. Forward search is depicted in the following:
 
+    .. figure:: ../../../docs/source/resources/nearest_neighbor.png
 
     Parameters
     ----------
     source_coord: np.ndarray
         Coordinate array of m source points. Expected shape (m, 3)
     target_coord: np.ndarray
         Coordinates of n target points. Expected shape (n, 3)
@@ -97,15 +109,15 @@
     max_distance: str, optional
         Set interpolation weights to zero if max_distance is exceeded.
     formulation: str, optional
         Search direction for nearest neighbor search. By default, direction is chosen automatically based on number of
         source and target points.
         'forward': Nearest neighbors are searched for each point on the (coarser) target grid. Leads to checkerboard
         if the target grid is finer than the source grid.
-        'bakcward': Nearest neighbors are searched for each point on the (coarser) source grid. Leads to overprediction
+        'backward': Nearest neighbors are searched for each point on the (coarser) source grid. Leads to overprediction
         if the source grid is finer than the target grid.
 
     Returns
     -------
     scipy.sparse.csr_array or scipy.sparse.csc_array
         Sparse operator matrix. Type depends on formulation. 'forward' returns csc_array, 'backward' returns csr_array.
     """
@@ -119,15 +131,15 @@
             )
             formulation = "forward"
         else:
             print(
                 "Detected coarse target grid (based on number of points). "
                 "Automatically selected 'backward' nearest neighbor search. This can lead to overprediction. "
                 "Please check the result, "
-                " 'forward' formulation yields better results for coarse target grids."
+                " 'forward' formulation yields better results for fine target grids."
             )
             formulation = "backward"
     if formulation == "forward":
         return _interpolation_matrix_nearest_neighbor_forward(
             source_coord, target_coord, num_neighbors, interpolation_exp, max_distance
         )
     elif formulation == "backward":
@@ -244,14 +256,90 @@
     interpolation_matrix = scipy.sparse.csc_array(
         (val, np.array(row_ind).flatten(), np.array(col_ptr)), matrix_shape, dtype=float
     )
 
     return interpolation_matrix
 
 
+def interpolation_matrix_projection_based(
+    src_coord: np.ndarray,
+    src_conn: np.ndarray,
+    src_reg_node: np.ndarray,
+    src_reg_elem: np.ndarray,
+    trgt_coord: np.ndarray,
+    trgt_conn: np.ndarray,
+    trgt_reg_node: np.ndarray,
+    trgt_reg_elem: np.ndarray,
+    proj_direction: np.ndarray | List[np.ndarray] | None = None,
+    max_distance=0.03,
+    search_radius: float | None = None,
+    workers: Optional[int] = None,
+):
+    """
+    Interpolation matrix for projection-based interpolation. Points of the target mesh are projected onto the
+    source mesh and evaluated based on linear FE basis functions.
+
+    .. figure:: ../../../docs/source/resources/projection_interpolation.png
+
+    Parameters
+    ----------
+    src_coord : np.ndarray
+        Source mesh coordinate array
+    src_conn : np.ndarray
+        Source mesh connectivity array
+    src_reg_node : np.ndarray
+        Source mesh region node ids
+    src_reg_elem : np.ndarray
+        Source mesh region element ids
+    trgt_coord : np.ndarray
+        Target mesh coordinate array
+    trgt_conn : np.ndarray
+        Target mesh connectivity array
+    trgt_reg_node : np.ndarray
+        Target mesh region node ids
+    trgt_reg_elem : np.ndarray
+        Target mesh region element ids
+    proj_direction : np.ndarray, List[np.ndarray], optional
+        Direction vector used for projection. Can be specified constant, or indivitually for each node.
+        By default, the node normal vector (based on averaded neighboring element normal vectors) is used.
+    max_distance : float, optional
+        Lower values speed up interpolation matrix build and prevent projecting onto far surfaces.
+    search_radius : float, optional
+        Should be chosed at least to the maximum element size of the target grid.
+    workers : int, optional
+        Number of processes to use in parallel. The default is ``None``, in which case all cores are used.
+
+    Returns
+    -------
+    scipy.sparse.csr_array
+        Sparse operator matrix.
+
+    References
+    ----------
+    Wurzinger A, Kraxberger F, Maurerlehner P, Mayr-Mittermüller B, Rucz P, Sima H, Kaltenbacher M, Schoder S.
+    Experimental Prediction Method of Free-Field Sound Emissions Using the Boundary Element Method and
+    Laser Scanning Vibrometry. Acoustics. 2024; 6(1):65-82. https://doi.org/10.3390/acoustics6010004
+
+    """
+    return projection_interpolation.interpolation_matrix_projection_based(
+        src_coord=src_coord,
+        src_conn=src_conn,
+        src_reg_node=src_reg_node,
+        src_reg_elem=src_reg_elem,
+        trgt_coord=trgt_coord,
+        trgt_conn=trgt_conn,
+        trgt_reg_node=trgt_reg_node,
+        trgt_reg_elem=trgt_reg_elem,
+        proj_direction=proj_direction,
+        max_distance=max_distance,
+        search_radius=search_radius,
+        workers=workers,
+    )
+
+
 def apply_interpolation(
     result_array: io.CFSResultArray,
     interpolation_matrix: scipy.sparse.csr_array | scipy.sparse.csc_array,
     restype_out: Optional[cfs_types.cfs_result_type] = None,
     quantity_out: Optional[str] = None,
     region_out: Optional[str] = None,
 ) -> io.CFSResultArray:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyCFS-0.0.5/pyCFS/data/operators/projection_interpolation.py` & `pyCFS-0.0.6/pyCFS/data/operators/projection_interpolation.py`

 * *Files 10% similar despite different names*

```diff
@@ -199,15 +199,15 @@
         col_idx = np.array([triangle.id_a, triangle.id_b, triangle.id_c])
 
         return col_idx, phi
 
     return None
 
 
-def interpolation_fe(
+def interpolation_matrix_projection_based(
     src_coord: np.ndarray,
     src_conn: np.ndarray,
     src_reg_node: np.ndarray,
     src_reg_elem: np.ndarray,
     trgt_coord: np.ndarray,
     trgt_conn: np.ndarray,
     trgt_reg_node: np.ndarray,
@@ -216,14 +216,56 @@
     max_distance=0.03,
     search_radius: float | None = None,
     workers: Optional[int] = None,
 ):
     """
     Interpolation matrix for projection-based interpolation. Points of the target mesh are projected onto the
     source mesh and evaluated based on linear FE basis functions.
+
+    .. figure:: ../../../docs/source/resources/projection_interpolation.png
+
+    Parameters
+    ----------
+    src_coord : np.ndarray
+        Source mesh coordinate array
+    src_conn : np.ndarray
+        Source mesh connectivity array
+    src_reg_node : np.ndarray
+        Source mesh region node ids
+    src_reg_elem : np.ndarray
+        Source mesh region element ids
+    trgt_coord : np.ndarray
+        Target mesh coordinate array
+    trgt_conn : np.ndarray
+        Target mesh connectivity array
+    trgt_reg_node : np.ndarray
+        Target mesh region node ids
+    trgt_reg_elem : np.ndarray
+        Target mesh region element ids
+    proj_direction : np.ndarray, List[np.ndarray], optional
+        Direction vector used for projection. Can be specified constant, or indivitually for each node.
+        By default, the node normal vector (based on averaded neighboring element normal vectors) is used.
+    max_distance : float, optional
+        Lower values speed up interpolation matrix build and prevent projecting onto far surfaces.
+    search_radius : float, optional
+        Should be chosed at least to the maximum element size of the target grid.
+    workers : int, optional
+        Number of processes to use in parallel. The default is ``None``, in which case all cores are used.
+
+    Returns
+    -------
+    scipy.sparse.csr_array
+        Sparse operator matrix.
+
+    References
+    ----------
+    Wurzinger A, Kraxberger F, Maurerlehner P, Mayr-Mittermüller B, Rucz P, Sima H, Kaltenbacher M, Schoder S.
+    Experimental Prediction Method of Free-Field Sound Emissions Using the Boundary Element Method and
+    Laser Scanning Vibrometry. Acoustics. 2024; 6(1):65-82. https://doi.org/10.3390/acoustics6010004
+
     """
     src_coord_reg = src_coord[src_reg_node - 1]
     src_conn_reg = src_conn[src_reg_elem - 1, :]
     trgt_coord_reg = trgt_coord[trgt_reg_node - 1]
     trgt_conn_reg = trgt_conn[trgt_reg_elem - 1, :]
 
     connectivity_map_src = {v: k + 1 for k, v in dict(enumerate(src_reg_node.flatten())).items()}
@@ -303,15 +345,15 @@
             target_coord = target_mesh.Coordinates
             target_connectivity = target_mesh.Connectivity
             target_reg_nodes = target_region.Nodes
             target_reg_elems = target_region.Elements
 
             # Get interpolation matrix
             print(f'Computing interpolation matrix: "{src_region.Name}"-> "{target_region.Name}"')
-            interpolation_matrix = interpolation_fe(
+            interpolation_matrix = interpolation_matrix_projection_based(
                 src_coord,
                 src_connectivity,
                 src_reg_nodes,
                 src_reg_elems,
                 target_coord,
                 target_connectivity,
                 target_reg_nodes,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyCFS-0.0.5/pyCFS/data/util.py` & `pyCFS-0.0.6/pyCFS/data/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -111,14 +111,70 @@
         Angle between vectors v1 and v2 in radians.
 
     """
     cosine_angle = np.dot(v1, v2) / (np.linalg.norm(v1) * np.linalg.norm(v2))
     return np.arccos(cosine_angle)
 
 
+def element_normal_2d(element_coordinates: np.ndarray) -> np.ndarray:
+    """
+    Compute normal vector of flat 2d elements.
+
+    Parameters
+    ----------
+    element_coordinates : numpy.ndarray
+        Coordinate array of N point flat element. shape = (N,3) or (M,N,3) for M elements
+
+    Returns
+    -------
+    np.ndarray
+
+    Examples
+    --------
+    >>> element_normal_vec = element_normal_2d(element_coordinates)
+
+    """
+
+    # get edge vectors
+    if element_coordinates.ndim == 2:
+        edge_vec = element_coordinates[[1, 2], :] - element_coordinates[[0], :]
+        return vecnorm(np.cross(edge_vec[0, :], edge_vec[1, :]))
+    elif element_coordinates.ndim == 3:
+        edge_vec = element_coordinates[:, [1, 2], :] - element_coordinates[:, [0], :]
+        return vecnorm(np.cross(edge_vec[:, 0, :], edge_vec[:, 1, :]), axis=1)
+    else:
+        raise ValueError("element_coordinates must be of shape (N,3) or (M,N,3).")
+
+
+def node_normal_2d(element_coordinates: np.ndarray) -> np.ndarray:
+    """
+    Computes surface normal vector by averaging the element normal vectors of neighboring elements.
+
+    Parameters
+    ----------
+    element_coordinates : numpy.ndarray
+        Coordinate array of M neighboring N-point flat elements. shape = (M,N,3)
+        The common node must be at the first index [:,0,:]
+
+    Returns
+    -------
+    np.ndarray
+        Normalized normal vector. shape=(3,)
+
+    Examples
+    --------
+    >>> node_normal_vec = node_normal_2d(element_coordinates)
+
+    """
+
+    element_normal_vec = element_normal_2d(element_coordinates)
+
+    return vecnorm(np.mean(element_normal_vec, axis=0))
+
+
 def element_angle_2d(element_coordinates: np.ndarray) -> List[float]:
     """
     Compute corner angles of 2D element
 
     Parameters
     ----------
     element_coordinates : numpy.ndarray
@@ -202,14 +258,18 @@
     Notes
     -----
     This metric is based on the ratio of the volume to the sum of the square of the edge lengths for 2D
     quad/tri elements, or the square root of the cube of the sum of the square of the edge lengths for
     3D elements. A value of 1 indicates a perfect cube or square while a value of 0 indicates that the
     element has a zero or negative volume. (extracted from "Ansys Meshing User's Guide 2021R2" p.130)
 
+    References
+    ----------
+    "Ansys Meshing User's Guide 2021R2" p.130
+
     """
     # Factor extracted from "Ansys Meshing User's Guide 2021R2" p.130
     factor = {
         cfs_element_type.TRIA3: 6.92820323,
         cfs_element_type.QUAD4: 4.0,
         cfs_element_type.TET4: 124.70765802,
         cfs_element_type.HEXA8: 41.56921938,
@@ -331,23 +391,32 @@
 def element_centroid(element_coordinates: np.ndarray) -> np.ndarray:
     """
     Compute geometric center of element
 
     Parameters
     ----------
     element_coordinates : numpy.ndarray
-        Array of element Coordinates (Nx3), where N is the number of nodes.
+        Array of node Coordinates (Nx3) or Array of elements (MxNx3), where M is the number of elements and N is the
+        number of nodes.
 
     Returns
     -------
     numpy.ndarray
         Geometric center of element
 
     """
-    return np.mean(element_coordinates, axis=0)
+    if element_coordinates.ndim == 2:
+        return np.mean(element_coordinates, axis=0)
+    elif element_coordinates.ndim == 3:
+        return np.mean(element_coordinates, axis=1)
+    else:
+        raise ValueError(
+            "Expect element coordinates to be of shape (MxNx3) or (Nx3), "
+            "where M is the number of elements and N is the number of nodes."
+        )
 
 
 def vecnorm(v: np.ndarray, order: int | None = None, axis: int | None = None) -> np.ndarray:
     """
     Normalize vector
 
     Parameters
@@ -409,15 +478,15 @@
     Returns
     -------
     p1 : numpy.ndarray
         Coordinates of intersection point 1
     p2 : numpy.ndarray
         Coordinates of intersection point 2
 
-    Notes
+    References
     -----
     Implementaton based on Wikipedia Trilateration article:
     https://en.wikipedia.org/wiki/True-range_multilateration#Three_Cartesian_dimensions,_three_measured_slant_ranges
 
     """
 
     # Define coordinate system with origin in C1, C2 on x-axis, and C3 in xy-plane
```

### Comparing `pyCFS-0.0.5/pyCFS/pyCFS.py` & `pyCFS-0.0.6/pyCFS/pyCFS.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,24 @@
+"""
+pyCFS.pyCFS
+==========
+pyCFS is an automation and data processing library for the `openCFS <https://opencfs.org/>`_ software. It enables the user to build an abstraction
+layer around the openCFS simulation which means that the user can execute simulations directly from a python script or notebook without worrying
+about the individual simulation files.
+"""
+
 import os
 import re
 import time
 from glob import glob
 from tqdm.auto import tqdm
 from multiprocessing import Pool
 import numpy as np
 import numpy.typing as npt
-from typing import List, Callable, Optional, TypeAlias, Dict
+from typing import List, Callable, Optional, Tuple, TypeAlias, Dict
 
 from .util import hdf5_io as h5io
 from .util.lib_types import (
     pyCFSparamVec,
     pyCFSparam,
     nestedResultDict,
     resultVec,
@@ -62,15 +70,15 @@
         clean_finish: bool = False,
         save_hdf_results: bool = False,
         array_fill_value: pyCFSparam = np.nan,
         parallelize: bool = False,
         remeshing_on: bool = False,
         n_jobs_max: int = 1000,
         testing: bool = False,
-        track_results: Optional[List[str]] = None,
+        track_results: Optional[str | List[str]] = None,
         dump_results: bool = False,
     ):
         """
 
         OpenCFS and Trelis/CoreformCubit python interfacing package. The main
         goal of this module is to make an easy to use interface which provides
         a class that handles the automatic simulation setup from given CFS and
@@ -125,16 +133,18 @@
             clean_finish (bool): Delete all generated simulation files. Does not touch
                                 result files. Defaults to False.
 
             testing (bool): If true will indicate to not create any directories or leave
                             footprints. Used for clean automated testing.
 
             track_results (List[str], optional): List of results which are to be tracked from
-                                                 the main hdf file. If `None` then all results
-                                                 are tracked. (default = None).
+                                                 the main hdf file. If `None` then no results
+                                                 are tracked. If 'all' then all results are tracked.
+                                                 Else one can select individual results by name.
+                                                 (default = None).
 
             dump_results (bool, optional): If True then after each run the tracked results are
                                            saved to disk. (default = False).
         """
 
         self.pyCFSobj: TypeAlias = pyCFS
 
@@ -377,14 +387,15 @@
     def _init_results(self) -> None:
         """
 
         Initializes an empty list for storing the hdf file results into.
 
         """
         self.results: List[nestedResultDict] = []
+        self.hist_results: List[nestedResultDict] = []
         self.sa_results: List[sensorArrayResultPacket] = []
 
     def _init_sensor_array_patterns(self) -> None:
 
         self.sensor_array_pattern = r'<sensorArray *fileName="" *type=".*" *csv="yes" *delimiter=",">\n*\
  *<coordinateFile *fileName=".*" *delimiter="," *commentCharacter="#"/>\n* *</sensorArray>'
         self.result_name_pattern = r'<sensorArray fileName="" type="([^"]*)" csv="yes" delimiter=",">'
@@ -633,15 +644,15 @@
         return (self.params_changed[2] and (ind is None) and not self.mesh_present) or (
             self.remeshing_on and self.parallelize and not self.mesh_present
         )
 
     # * ------------------ Result handler methods ------------------
     def _generate_data_dump_path(self) -> str:
         t = time.ctime(time.time())
-        t = t.replace(" ", "_").replace(":", "-")
+        t = t.replace("  ", " ").replace(" ", "_").replace(":", "-")
         return f"{self.data_dump_path}data_dump_run_{t}.npy"
 
     def _contruct_run_metadata(self, X: pyCFSparamVec) -> None:
         file_paths = glob(f"{self.cfs_proj_path}/**/*.csv", recursive=True) + glob(
             f"{self.cfs_proj_path}/**/*.py", recursive=True
         )
         other_files = {k: pyCFS.read_file_contents(k) for k in file_paths}
@@ -655,14 +666,15 @@
             "run_finish": self.time[LAST_EXEC_STOP],
             "note": "",
         }
 
     def _dump_results(self) -> None:
         result_packet = {
             "results_hdf": self.results,
+            "results_history_hdf": self.hist_results,
             "results_sensor_array": self.sa_results,
             "meta_data": self.run_metadata,
         }
 
         self.result_dump_path = self._generate_data_dump_path()
         np.save(self.result_dump_path, result_packet, allow_pickle=True)  # type: ignore[arg-type]
 
@@ -696,15 +708,15 @@
         return {"data": data, "columns": col_names}
 
     @staticmethod
     def _split_sa_result_name(res_name: str, storage_path: str) -> List[str]:
         res_name = res_name.removeprefix(storage_path)
         return res_name.split(SA_NAME_SEPARATOR)
 
-    def _get_hdf_curr_package(self, ind: Optional[int] = None) -> nestedResultDict:
+    def _get_hdf_curr_package(self, ind: Optional[int] = None) -> Tuple[nestedResultDict, nestedResultDict]:
         """
 
         Gets the hdf package for the current simulation run by extracting all
         results from the hdf file for the result regions defined in the inital
         run.
 
         Returns:
@@ -742,16 +754,17 @@
         Reads the hdf results from the current file and appends the generated packet
         to the list of hdf results.
 
         Args:
             ind (int): Job index to get correct parameters for simulation
                        and to read correct results from the result dir.
         """
-        hdf_package: nestedResultDict = self._get_hdf_curr_package(ind)
+        hdf_package, hdf_hist_package = self._get_hdf_curr_package(ind)
         self.results.append(hdf_package)
+        self.hist_results.append(hdf_hist_package)
 
     @staticmethod
     def _is_coord_col(col_name: str) -> bool:
         return True in [key in col_name for key in SA_COORD_KEYS]
 
     @staticmethod
     def _remove_coord_cols(sa_res: sensorArrayResult) -> sensorArrayResult:
```

### Comparing `pyCFS-0.0.5/pyCFS/util/lib_types.py` & `pyCFS-0.0.6/pyCFS/util/lib_types.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/pyCFS/util/setup_generator.py` & `pyCFS-0.0.6/pyCFS/util/setup_generator.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/pyCFS/util/templates/config.yaml` & `pyCFS-0.0.6/pyCFS/util/templates/config.yaml`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/pyCFS/util/templates/sim_setup.py` & `pyCFS-0.0.6/pyCFS/util/templates/sim_setup.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/pyCFS/util/templates/sim_setup_opti.py` & `pyCFS-0.0.6/pyCFS/util/templates/sim_setup_opti.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/pyCFS.egg-info/PKG-INFO` & `pyCFS-0.0.6/pyCFS.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCFS
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python library for automating and data handling tasks for openCFS.
 Author-email: IGTE <igte.gitlab@gmail.com>, Eniz Mušeljić <eniz.m@outlook.com>, Andreas Wurzinger <andreas.wurzinger@tugraz.at>
 License: MIT License
         
         Copyright (c) 2024 Verein zur Förderung der Software openCFS
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyCFS-0.0.5/pyCFS.egg-info/SOURCES.txt` & `pyCFS-0.0.6/pyCFS.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 .gitlab/issue_templates/Default.md
 .gitlab/merge_request_templates/Default.md
+docs/.nojekyll
 docs/Makefile
 docs/make.bat
+docs/rst_process.py
+docs/source/api.rst
 docs/source/conf.py
 docs/source/dev_notes.md
 docs/source/getting_started.md
 docs/source/index.rst
 docs/source/installation.md
 docs/source/pycfs_data.md
 docs/source/_static/pycfslogo-full-no-text-small.png
@@ -22,14 +25,27 @@
 docs/source/dev_source/data_handling.md
 docs/source/dev_source/dev_notes_main.md
 docs/source/examples/basics/a_first_simulation.md
 docs/source/examples/basics/cli_tool.md
 docs/source/examples/basics/data_processing.md
 docs/source/examples/basics/introduction.md
 docs/source/examples/basics/result_handling.md
+docs/source/examples/data_tutorial/data_tutorial.py
+docs/source/examples/data_tutorial/tutorial_input.cfs
+docs/source/resources/cell2node.png
+docs/source/resources/data_structures_CFSMeshData.png
+docs/source/resources/data_structures_CFSRegData.png
+docs/source/resources/data_structures_CFSResultArray.png
+docs/source/resources/data_structures_CFSResultData.png
+docs/source/resources/data_structures_CFSResultInfo.png
+docs/source/resources/data_structures_overview.png
+docs/source/resources/nearest_neighbor.png
+docs/source/resources/node2cell.png
+docs/source/resources/projection_interpolation.png
+docs/source/resources/src/data_structures.drawio
 pyCFS/__init__.py
 pyCFS/py.typed
 pyCFS/pyCFS.py
 pyCFS.egg-info/PKG-INFO
 pyCFS.egg-info/SOURCES.txt
 pyCFS.egg-info/dependency_links.txt
 pyCFS.egg-info/entry_points.txt
@@ -52,17 +68,17 @@
 pyCFS/data/io/CFSMeshData.py
 pyCFS/data/io/CFSReader.py
 pyCFS/data/io/CFSResultData.py
 pyCFS/data/io/CFSWriter.py
 pyCFS/data/io/__init__.py
 pyCFS/data/io/cfs_types.py
 pyCFS/data/operators/__init__.py
-pyCFS/data/operators/fit_geometry.py
 pyCFS/data/operators/interpolators.py
 pyCFS/data/operators/projection_interpolation.py
+pyCFS/data/operators/transformation.py
 pyCFS/util/__init__.py
 pyCFS/util/hdf5_io.py
 pyCFS/util/lib_types.py
 pyCFS/util/setup_generator.py
 pyCFS/util/templates/config.yaml
 pyCFS/util/templates/mat.xml
 pyCFS/util/templates/run_sim.py
```

### Comparing `pyCFS-0.0.5/pyproject.toml` & `pyCFS-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/extras/ansys_io/ansys_io.rst` & `pyCFS-0.0.6/tests/data/extras/ansys_io/ansys_io.rst`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/extras/ensight_io/ensight_io.0000.U` & `pyCFS-0.0.6/tests/data/extras/ensight_io/ensight_io.0000.U`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/extras/ensight_io/ensight_io.0000.mesh` & `pyCFS-0.0.6/tests/data/extras/ensight_io/ensight_io.0000.mesh`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/extras/ensight_io/ensight_io.0000.p` & `pyCFS-0.0.6/tests/data/extras/ensight_io/ensight_io.0000.p`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/extras/ensight_io/poly/data.case` & `pyCFS-0.0.6/tests/data/extras/ensight_io/poly/data.case`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/extras/ensight_io/poly/data00001.geo` & `pyCFS-0.0.6/tests/data/extras/ensight_io/poly/data00001.geo`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/extras/ensight_io/poly/data00001.scl1` & `pyCFS-0.0.6/tests/data/extras/ensight_io/poly/data00001.scl1`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/extras/ensight_io/poly/data00001.vel` & `pyCFS-0.0.6/tests/data/extras/ensight_io/poly/data00001.vel`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/extras/nihu_io/result_field.mat` & `pyCFS-0.0.6/tests/data/extras/nihu_io/result_field.mat`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/extras/nihu_io/result_surface.mat` & `pyCFS-0.0.6/tests/data/extras/nihu_io/result_surface.mat`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/extras/psv_io/line.npy` & `pyCFS-0.0.6/tests/data/extras/psv_io/line.npy`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/extras/psv_io/line.svd` & `pyCFS-0.0.6/tests/data/extras/psv_io/line.svd`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/extras/psv_io/line_h2_accelerance.unv` & `pyCFS-0.0.6/tests/data/extras/psv_io/line_h2_accelerance.unv`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/extras/psv_io/surface.svd` & `pyCFS-0.0.6/tests/data/extras/psv_io/surface.svd`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/extras/psv_io/surface_dist.npy` & `pyCFS-0.0.6/tests/data/extras/psv_io/surface_dist.npy`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/extras/psv_io/surface_h1_receptance.npy` & `pyCFS-0.0.6/tests/data/extras/psv_io/surface_h1_receptance.npy`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/extras/psv_io/surface_h1_receptance.unv` & `pyCFS-0.0.6/tests/data/extras/psv_io/surface_h1_receptance.unv`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/operators/fit_geometry/fit_geometry_src.cfs` & `pyCFS-0.0.6/tests/data/operators/fit_geometry/fit_geometry_src.cfs`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/operators/fit_geometry/fit_geometry_target.cfs` & `pyCFS-0.0.6/tests/data/operators/fit_geometry/fit_geometry_target.cfs`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/operators/interpolators/interpolators.cfs` & `pyCFS-0.0.6/tests/data/operators/interpolators/interpolators.cfs`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/operators/interpolators/nn_elem.cfs` & `pyCFS-0.0.6/tests/data/operators/interpolators/nn_elem.cfs`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/operators/interpolators/nn_source.cfs` & `pyCFS-0.0.6/tests/data/operators/interpolators/nn_source.cfs`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/operators/interpolators/nn_target.cfs` & `pyCFS-0.0.6/tests/data/operators/interpolators/nn_target.cfs`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/operators/projection_interpolation/source.cfs` & `pyCFS-0.0.6/tests/data/operators/projection_interpolation/source.cfs`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/operators/projection_interpolation/target.cfs` & `pyCFS-0.0.6/tests/data/operators/projection_interpolation/target.cfs`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/data/sim_io/elecFieldIntensity-sensor-positions-0.csv-1` & `pyCFS-0.0.6/tests/data/sim_io/elecFieldIntensity-sensor-positions-0.csv-1`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/pycfs_data_fixtures.py` & `pyCFS-0.0.6/tests/pycfs_data_fixtures.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         ]
     )
     mesh_data.MeshInfo.NumNodes = 8
     mesh_data.Connectivity = np.array(
         [
             [1, 2, 4, 3, 5, 6, 8, 7],
             [1, 2, 3, 0, 0, 0, 0, 0],
-            [2, 3, 4, 0, 0, 0, 0, 0],
+            [2, 4, 3, 0, 0, 0, 0, 0],
             [5, 6, 8, 7, 0, 0, 0, 0],
         ]
     )
     mesh_data.Types = np.array(
         [
             cfs_element_type.HEXA8,
             cfs_element_type.TRIA3,
```

### Comparing `pyCFS-0.0.5/tests/pycfs_fixtures.py` & `pyCFS-0.0.6/tests/pycfs_fixtures.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/test_pycfs_core.py` & `pyCFS-0.0.6/tests/test_pycfs_core.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/test_pycfs_data_extras.py` & `pyCFS-0.0.6/tests/test_pycfs_data_extras.py`

 * *Files identical despite different names*

### Comparing `pyCFS-0.0.5/tests/test_pycfs_data_io.py` & `pyCFS-0.0.6/tests/test_pycfs_data_io.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import copy
 from copy import deepcopy
 
 import h5py
 import numpy as np
 from pyCFS.data import io, v_def
-from pyCFS.data.io.cfs_types import cfs_analysis_type
+from pyCFS.data.io.cfs_types import cfs_analysis_type, cfs_result_type
 from .pycfs_data_fixtures import dummy_CFSMeshData_obj, dummy_CFSResultData_obj
 
 
 def test_CFSMeshData(dummy_CFSMeshData_obj):
 
     print(dummy_CFSMeshData_obj.Quality)
 
@@ -20,14 +20,32 @@
     coord = dummy_CFSMeshData_obj.Coordinates
     conn = dummy_CFSMeshData_obj.Connectivity[1:, :]
     mesh_coord = io.mesh_from_coordinates_connectivity(coordinates=coord, connectivity=conn, element_dimension=2)
     print(mesh_coord)
     print(mesh_coord.Regions[0])
 
 
+def test_CFSMeshData_element_centroids(dummy_CFSMeshData_obj):
+    ref_sol = np.array([[0.5, 0.5, 0.5], [0.0, 1 / 3.0, 1 / 3.0], [0.0, 2 / 3.0, 2 / 3.0], [1.0, 0.5, 0.5]])
+    np.testing.assert_array_equal(dummy_CFSMeshData_obj.ElementCentroids, ref_sol)
+
+    ref_sol_reg = np.array([[0.5, 0.5, 0.5]])
+    np.testing.assert_array_equal(dummy_CFSMeshData_obj.get_region_centroids(region="Vol"), ref_sol_reg)
+
+
+def test_CFSMeshData_surface_normal(dummy_CFSMeshData_obj):
+    ref_sol_el = np.array([[np.nan, np.nan, np.nan], [-1.0, 0, 0], [-1.0, 0, 0], [-1.0, 0, 0]])
+    np.testing.assert_array_equal(dummy_CFSMeshData_obj.get_mesh_surface_normals(), ref_sol_el)
+
+    ref_sol_node = np.tile(np.array([-1.0, 0, 0]), (8, 1))
+    np.testing.assert_array_equal(
+        dummy_CFSMeshData_obj.get_mesh_surface_normals(restype=cfs_result_type.NODE), ref_sol_node
+    )
+
+
 def test_write(dummy_CFSMeshData_obj, dummy_CFSResultData_obj, working_directory="."):
     file = f"{working_directory}/tests/data_tmp/pycfs_data_io.cfs"
 
     print("Write demo file")
     with io.CFSWriter(file, verbosity=v_def.all) as h5writer:
         h5writer.create_file(mesh_data=dummy_CFSMeshData_obj, result_data=dummy_CFSResultData_obj)
 
@@ -97,14 +115,29 @@
             mesh_data_read.get_closest_element(coordinate=np.array([[1, 1, 1], [0, 0, 0]]), region="Surf1"), el_id
         )
         result_data_1_3 = [
             h5reader.get_single_data_steps(quantity="quantity3", region="Surf1", entity_id=el_id[i]) for i in el_id
         ]
 
 
+def test_read_data_sequential(dummy_CFSMeshData_obj, dummy_CFSResultData_obj, working_directory="."):
+    file = f"{working_directory}/tests/data_tmp/pycfs_data_io.cfs"
+
+    test_write(dummy_CFSMeshData_obj, dummy_CFSResultData_obj, working_directory)
+
+    print("Read demo file")
+    with io.CFSReader(file, processes=1, verbosity=v_def.all) as h5reader:
+        # Read Mesh
+        print("Read Demo Mesh")
+        mesh_data_read = h5reader.MeshData
+
+        # Read Data
+        np.testing.assert_equal(h5reader.MultiStepData, dummy_CFSResultData_obj)
+
+
 def test_read_group_wo_elements(dummy_CFSMeshData_obj, dummy_CFSResultData_obj, working_directory="."):
     """Read group/region without elements (nodes only)."""
 
     file = f"{working_directory}/tests/data_tmp/pycfs_data_io.cfs"
 
     test_write(dummy_CFSMeshData_obj, dummy_CFSResultData_obj, working_directory)
```

### Comparing `pyCFS-0.0.5/tests/test_pycfs_data_operators.py` & `pyCFS-0.0.6/tests/test_pycfs_data_operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pyCFS.data.io import CFSReader, cfs_types, CFSWriter, CFSResultData
 from pyCFS.data.operators import interpolators
 
 
 def test_fit_coordinates(working_directory="."):
-    from pyCFS.data.operators.fit_geometry import fit_coordinates
+    from pyCFS.data.operators.transformation import fit_coordinates
 
     filename_src = f"{working_directory}/tests/data/operators/fit_geometry/fit_geometry_src.cfs"
     filename_target = f"{working_directory}/tests/data/operators/fit_geometry/fit_geometry_target.cfs"
     filename_out = f"{working_directory}/tests/data_tmp/operators/fit_geometry/fit_geometry_out.cfs"
 
     regions_target = ["HULL_TARGET"]
     regions_fit = ["surface"]
```

### Comparing `pyCFS-0.0.5/tests/test_pycfs_data_util.py` & `pyCFS-0.0.6/tests/test_pycfs_data_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 import random
 import time
 
 import numpy as np
 import pytest
 
 from pyCFS.data.io.cfs_types import cfs_element_type
-from pyCFS.data.util import trilateration, element_quality, progressbar, connectivity_list_to_matrix
+from pyCFS.data.util import (
+    trilateration,
+    element_quality,
+    progressbar,
+    connectivity_list_to_matrix,
+    element_normal_2d,
+    node_normal_2d,
+)
 
 
 def test_trilateration():
     A = np.array([1, 1, 2])
     B = np.array([4, 7, 2])
     C = np.array([0, -2, 4])
     P = np.array([1, 2, 3])
@@ -17,14 +24,43 @@
     R1 = np.linalg.norm(P - A)
     R2 = np.linalg.norm(P - B)
     R3 = np.linalg.norm(P - C)
 
     print(trilateration(A, B, C, R1, R2, R3))
 
 
+def test_element_normal():
+    coord = np.array([[1, 1, 1], [2, 3, 1], [1, 4, 1], [-1, 2, 1]], dtype=float)
+    normal_vec = element_normal_2d(coord)
+    np.testing.assert_array_equal(normal_vec, np.array([0, 0, 1.0]))
+
+    coord = np.tile(coord, (3, 1, 1))
+    normal_vec = element_normal_2d(coord)
+    np.testing.assert_array_equal(normal_vec, np.tile(np.array([0, 0, 1.0]), (3, 1)))
+
+
+def test_node_normal():
+    coord = np.array(
+        [
+            [0, 0, 0],
+            [0, 0, 1],
+            [0, 1, 0],
+            [0, 1, 1],
+        ]
+    )
+    conn = np.array(
+        [
+            [2, 3, 1],
+            [2, 4, 3],
+        ]
+    )
+
+    np.testing.assert_array_equal(node_normal_2d(element_coordinates=coord[conn - 1]), np.array([-1.0, 0, 0]))
+
+
 def test_element_quality():
     A = np.array([1, 1, 2])
     B = np.array([4, 7, 2])
     C = np.array([0, -2, 4])
     P = np.array([1, 2, 3])
 
     coordinates = np.array([A, B, C])
```

### Comparing `pyCFS-0.0.5/tests/test_pycfs_sim_io.py` & `pyCFS-0.0.6/tests/test_pycfs_sim_io.py`

 * *Files identical despite different names*

