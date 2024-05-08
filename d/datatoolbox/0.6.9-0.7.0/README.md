# Comparing `tmp/datatoolbox-0.6.9.tar.gz` & `tmp/datatoolbox-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatoolbox-0.6.9.tar", last modified: Tue Apr 30 07:55:20 2024, max compression
+gzip compressed data, was "datatoolbox-0.7.0.tar", last modified: Wed May  8 14:07:30 2024, max compression
```

## Comparing `datatoolbox-0.6.9.tar` & `datatoolbox-0.7.0.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.321687 datatoolbox-0.6.9/
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      159 2022-05-25 07:15:53.000000 datatoolbox-0.6.9/.gitignore
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      950 2022-10-19 13:17:33.000000 datatoolbox-0.6.9/.gitlab-ci.yml
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      703 2020-10-14 14:04:18.000000 datatoolbox-0.6.9/.travis.yml
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1073 2020-10-14 14:04:18.000000 datatoolbox-0.6.9/LICENSE
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1564 2024-04-30 07:55:20.321408 datatoolbox-0.6.9/PKG-INFO
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1298 2023-09-22 10:59:58.000000 datatoolbox-0.6.9/README.md
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1225 2020-10-14 14:04:18.000000 datatoolbox-0.6.9/appveyor.yml
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.273494 datatoolbox-0.6.9/ci/
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.280489 datatoolbox-0.6.9/ci/appveyor/
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     3111 2020-10-14 14:04:18.000000 datatoolbox-0.6.9/ci/appveyor/install.ps1
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1842 2020-10-14 14:04:18.000000 datatoolbox-0.6.9/ci/appveyor/run_with_env.cmd
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.290595 datatoolbox-0.6.9/datatoolbox/
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     5681 2023-08-18 10:53:24.000000 datatoolbox-0.6.9/datatoolbox/__init__.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)    15513 2023-06-08 08:12:18.000000 datatoolbox-0.6.9/datatoolbox/admin.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     3753 2024-04-17 07:49:21.000000 datatoolbox-0.6.9/datatoolbox/aggregator.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     6846 2024-04-29 10:25:24.000000 datatoolbox-0.6.9/datatoolbox/config.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)    18681 2023-08-29 12:09:48.000000 datatoolbox-0.6.9/datatoolbox/converters.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    17879 2024-04-30 07:21:37.000000 datatoolbox-0.6.9/datatoolbox/core.py
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.295201 datatoolbox-0.6.9/datatoolbox/data/
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    15781 2020-10-14 14:04:18.000000 datatoolbox-0.6.9/datatoolbox/data/GHG_alternative_naming.pkl
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    13482 2023-05-23 13:04:06.000000 datatoolbox-0.6.9/datatoolbox/data/GHG_properties_2019_CA.csv
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.295890 datatoolbox-0.6.9/datatoolbox/data/SANDBOX_datashelf/
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      286 2024-04-30 07:49:57.000000 datatoolbox-0.6.9/datatoolbox/data/SANDBOX_datashelf/inventory.csv
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.296794 datatoolbox-0.6.9/datatoolbox/data/SANDBOX_datashelf/mappings/
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    10757 2024-04-30 07:49:53.000000 datatoolbox-0.6.9/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     8466 2024-04-30 07:49:53.000000 datatoolbox-0.6.9/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      999 2024-04-30 07:49:53.000000 datatoolbox-0.6.9/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      161 2024-04-30 07:49:57.000000 datatoolbox-0.6.9/datatoolbox/data/SANDBOX_datashelf/sources.csv
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    22865 2020-10-14 14:04:18.000000 datatoolbox-0.6.9/datatoolbox/data/all.csv
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    14615 2020-10-14 14:04:18.000000 datatoolbox-0.6.9/datatoolbox/data/compatible1_5_unfiltered.xlsx
--rwxrwx---   0 andreasgeiges   (501) staff       (20)    10757 2020-04-20 12:32:09.000000 datatoolbox-0.6.9/datatoolbox/data/continent.csv
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     8466 2021-09-15 15:48:16.000000 datatoolbox-0.6.9/datatoolbox/data/country_codes.csv
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1711 2022-05-25 07:15:53.000000 datatoolbox-0.6.9/datatoolbox/data/datashelf_contents.csv
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     2923 2021-12-16 12:32:58.000000 datatoolbox-0.6.9/datatoolbox/data/external_mappings.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      178 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/data/personal_template.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)      999 2019-08-14 10:00:22.000000 datatoolbox-0.6.9/datatoolbox/data/regions.csv
--rw-r--r--   0 andreasgeiges   (501) staff       (20)   237445 2024-04-03 07:39:56.000000 datatoolbox-0.6.9/datatoolbox/data_readers.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    70580 2024-04-15 09:57:54.000000 datatoolbox-0.6.9/datatoolbox/data_structures.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    65668 2024-03-20 09:16:19.000000 datatoolbox-0.6.9/datatoolbox/database.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     6730 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/greenhouse_gas_database.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     3542 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/init_tools.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    21653 2023-08-18 10:29:12.000000 datatoolbox-0.6.9/datatoolbox/interfaces.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)    11022 2024-04-04 14:18:18.000000 datatoolbox-0.6.9/datatoolbox/io_tools.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    41818 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/mapping.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     2854 2022-12-01 09:27:15.000000 datatoolbox-0.6.9/datatoolbox/naming_convention.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     3305 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/patches.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     2189 2023-08-17 09:12:01.000000 datatoolbox-0.6.9/datatoolbox/pint_definitions.txt
--rw-r--r--   0 andreasgeiges   (501) staff       (20)        0 2020-06-08 07:09:19.000000 datatoolbox-0.6.9/datatoolbox/relations.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)    26449 2023-07-17 09:50:44.000000 datatoolbox-0.6.9/datatoolbox/sets.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)        0 2020-06-08 07:09:19.000000 datatoolbox-0.6.9/datatoolbox/storage.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1632 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/templates.py
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.306907 datatoolbox-0.6.9/datatoolbox/tools/
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    16351 2021-04-19 11:31:45.000000 datatoolbox-0.6.9/datatoolbox/tools/CRF_extract_CA_2021.xlsx
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    28022 2021-02-02 15:17:26.000000 datatoolbox-0.6.9/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    17445 2021-02-02 12:48:44.000000 datatoolbox-0.6.9/datatoolbox/tools/IEA_B2DS_4.SCEN
--rwxrwx---   0 andreasgeiges   (501) staff       (20)    17375 2019-12-20 11:46:57.000000 datatoolbox-0.6.9/datatoolbox/tools/WEO_2019_test.SCEN
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      587 2023-08-29 11:46:45.000000 datatoolbox-0.6.9/datatoolbox/tools/__init__.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     4320 2022-11-17 09:58:39.000000 datatoolbox-0.6.9/datatoolbox/tools/conversion_to_v0.3.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    45928 2024-04-30 07:25:50.000000 datatoolbox-0.6.9/datatoolbox/tools/excel.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      370 2022-11-17 09:58:39.000000 datatoolbox-0.6.9/datatoolbox/tools/export_all.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     4441 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/tools/for_datatables.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     8132 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/tools/html.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      182 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/tools/install_support.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     7188 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/tools/kaya_idendentiy_decomposition.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     4283 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/tools/magicc6.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     5931 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/tools/matplotlib.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      892 2023-08-04 09:51:33.000000 datatoolbox-0.6.9/datatoolbox/tools/new_SR15_pathway_matching.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     3797 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/tools/pandas.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     5533 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/tools/py_magicc_tools.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     7948 2023-08-18 10:42:50.000000 datatoolbox-0.6.9/datatoolbox/tools/pyam.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      965 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/tools/renaming_DB.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)    84992 2019-08-14 10:26:08.000000 datatoolbox-0.6.9/datatoolbox/tools/run_MAGICC_startup_simple.xlsx
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1830 2021-02-02 14:03:36.000000 datatoolbox-0.6.9/datatoolbox/tools/run_magicc6.m
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     1044 2022-11-17 09:58:40.000000 datatoolbox-0.6.9/datatoolbox/tools/statistics.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    61174 2021-06-03 14:06:07.000000 datatoolbox-0.6.9/datatoolbox/tools/test.docx
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     8625 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/tools/word.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     9597 2023-08-18 10:43:36.000000 datatoolbox-0.6.9/datatoolbox/tools/xarray.py
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.310830 datatoolbox-0.6.9/datatoolbox/tutorials/
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     2996 2022-05-25 07:15:53.000000 datatoolbox-0.6.9/datatoolbox/tutorials/00_search_find_and_access_data.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1019 2020-10-14 14:04:18.000000 datatoolbox-0.6.9/datatoolbox/tutorials/01_emission_comparison.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     2096 2022-05-25 07:15:53.000000 datatoolbox-0.6.9/datatoolbox/tutorials/02_unit_conversion.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     5685 2020-10-14 14:04:18.000000 datatoolbox-0.6.9/datatoolbox/tutorials/03_intermediate_example.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1416 2020-10-14 14:04:19.000000 datatoolbox-0.6.9/datatoolbox/tutorials/04_sources.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      382 2020-10-14 14:04:19.000000 datatoolbox-0.6.9/datatoolbox/tutorials/05_plot_source_content.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      734 2020-12-22 15:09:15.000000 datatoolbox-0.6.9/datatoolbox/tutorials/06_xarray_examples.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     1142 2021-05-11 13:19:29.000000 datatoolbox-0.6.9/datatoolbox/tutorials/07_renewable_share_compuation.py
--rw-rw-r--   0 andreasgeiges   (501) staff       (20)      793 2021-05-11 12:59:38.000000 datatoolbox-0.6.9/datatoolbox/tutorials/08_low_carbon_fuel_computation.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)   137631 2020-10-14 14:04:19.000000 datatoolbox-0.6.9/datatoolbox/tutorials/introduction_v1.ipynb
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     4631 2022-03-22 14:54:50.000000 datatoolbox-0.6.9/datatoolbox/tutorials/jump_start.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)      417 2023-05-12 14:15:39.000000 datatoolbox-0.6.9/datatoolbox/units.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)    43885 2023-08-18 10:28:42.000000 datatoolbox-0.6.9/datatoolbox/util.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      160 2024-04-30 07:55:19.000000 datatoolbox-0.6.9/datatoolbox/version.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      746 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/datatoolbox/workflows.py
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.292296 datatoolbox-0.6.9/datatoolbox.egg-info/
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1564 2024-04-30 07:55:20.000000 datatoolbox-0.6.9/datatoolbox.egg-info/PKG-INFO
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     3787 2024-04-30 07:55:20.000000 datatoolbox-0.6.9/datatoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 andreasgeiges   (501) staff       (20)        1 2024-04-30 07:55:20.000000 datatoolbox-0.6.9/datatoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      157 2024-04-30 07:55:20.000000 datatoolbox-0.6.9/datatoolbox.egg-info/requires.txt
--rw-r--r--   0 andreasgeiges   (501) staff       (20)       12 2024-04-30 07:55:20.000000 datatoolbox-0.6.9/datatoolbox.egg-info/top_level.txt
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.316137 datatoolbox-0.6.9/doc/
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     7755 2024-04-02 13:29:36.000000 datatoolbox-0.6.9/doc/Makefile
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     9684 2024-04-02 12:29:22.000000 datatoolbox-0.6.9/doc/conf.py
--rwxr-x---   0 andreasgeiges   (501) staff       (20)      101 2024-04-02 13:46:58.000000 datatoolbox-0.6.9/doc/core.rst
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      236 2024-04-02 14:07:33.000000 datatoolbox-0.6.9/doc/data_structures.rst
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      122 2021-01-11 16:19:59.000000 datatoolbox-0.6.9/doc/database.rst
--rw-r--r--   0 andreasgeiges   (501) staff       (20)       91 2021-01-11 16:18:53.000000 datatoolbox-0.6.9/doc/database_database.rst
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      130 2021-01-11 16:21:50.000000 datatoolbox-0.6.9/doc/database_gitrepomanager.rst
--rwxr-x---   0 andreasgeiges   (501) staff       (20)       93 2021-01-11 16:03:03.000000 datatoolbox-0.6.9/doc/excel.rst
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.316704 datatoolbox-0.6.9/doc/figures/
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    21579 2020-11-09 13:08:35.000000 datatoolbox-0.6.9/doc/figures/ID_meta_data.svg
--rw-r--r--   0 andreasgeiges   (501) staff       (20)    67463 2021-05-17 15:08:58.000000 datatoolbox-0.6.9/doc/figures/config_input.png
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     7008 2023-06-08 10:16:48.000000 datatoolbox-0.6.9/doc/first_steps.md
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      100 2020-12-22 15:09:15.000000 datatoolbox-0.6.9/doc/foo.rst_template
--rw-r--r--   0 andreasgeiges   (501) staff       (20)       77 2020-12-22 15:09:15.000000 datatoolbox-0.6.9/doc/help.rst
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      463 2024-04-02 11:53:11.000000 datatoolbox-0.6.9/doc/index.rst
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     1655 2023-06-08 08:19:25.000000 datatoolbox-0.6.9/doc/installation.md
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1080 2020-12-22 15:09:15.000000 datatoolbox-0.6.9/doc/license.rst
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     7353 2020-10-14 14:04:19.000000 datatoolbox-0.6.9/doc/make.bat
--rwxr-x---   0 andreasgeiges   (501) staff       (20)      103 2021-01-11 16:09:22.000000 datatoolbox-0.6.9/doc/matplotlib.rst
--rwxr-x---   0 andreasgeiges   (501) staff       (20)       95 2021-01-11 16:10:43.000000 datatoolbox-0.6.9/doc/pandas.rst
--rwxr-x---   0 andreasgeiges   (501) staff       (20)      243 2024-04-02 12:12:03.000000 datatoolbox-0.6.9/doc/tools.rst
--rwxr-x---   0 andreasgeiges   (501) staff       (20)       95 2021-01-11 16:09:13.000000 datatoolbox-0.6.9/doc/xarray.rst
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.317139 datatoolbox-0.6.9/documentation/
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     7761 2020-12-22 15:09:15.000000 datatoolbox-0.6.9/documentation/Datatoolbox - First steps.md
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      396 2023-10-10 10:32:47.000000 datatoolbox-0.6.9/environment.yml
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      418 2020-10-14 14:04:19.000000 datatoolbox-0.6.9/make_proj.sh
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      598 2024-04-02 14:16:29.000000 datatoolbox-0.6.9/readthedocs.yml
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      233 2024-04-29 10:26:45.000000 datatoolbox-0.6.9/requirements.txt
--rw-r--r--   0 andreasgeiges   (501) staff       (20)       38 2024-04-30 07:55:20.321779 datatoolbox-0.6.9/setup.cfg
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     1862 2023-09-22 10:49:18.000000 datatoolbox-0.6.9/setup.py
-drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-04-30 07:55:20.321038 datatoolbox-0.6.9/tests/
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     7292 2022-12-19 11:29:58.000000 datatoolbox-0.6.9/tests/test_calculations.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      696 2022-11-18 16:16:07.000000 datatoolbox-0.6.9/tests/test_converters.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     3941 2024-04-22 08:16:23.000000 datatoolbox-0.6.9/tests/test_database.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     1640 2023-03-30 13:32:13.000000 datatoolbox-0.6.9/tests/test_dataset.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     7741 2022-05-25 07:15:53.000000 datatoolbox-0.6.9/tests/test_datatable.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     1063 2022-11-16 11:59:46.000000 datatoolbox-0.6.9/tests/test_io.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      390 2022-11-22 09:54:34.000000 datatoolbox-0.6.9/tests/test_linked_functions.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     1563 2023-05-04 07:49:24.000000 datatoolbox-0.6.9/tests/test_pyam.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     3570 2022-05-25 07:15:53.000000 datatoolbox-0.6.9/tests/test_tableset.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     2610 2022-05-25 07:15:53.000000 datatoolbox-0.6.9/tests/test_tools.py
--rwxrwx---   0 andreasgeiges   (501) staff       (20)     1768 2023-10-11 06:54:12.000000 datatoolbox-0.6.9/tests/test_units.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)      870 2020-10-14 14:04:19.000000 datatoolbox-0.6.9/tests/test_utilities.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     2437 2022-10-19 13:17:33.000000 datatoolbox-0.6.9/tests/test_xarray.py
--rw-r--r--   0 andreasgeiges   (501) staff       (20)     2959 2022-05-25 07:15:53.000000 datatoolbox-0.6.9/tests/util_for_testing.py
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-05-08 14:07:30.850394 datatoolbox-0.7.0/
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      159 2022-05-25 07:15:53.000000 datatoolbox-0.7.0/.gitignore
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      950 2022-10-19 13:17:33.000000 datatoolbox-0.7.0/.gitlab-ci.yml
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      703 2020-10-14 14:04:18.000000 datatoolbox-0.7.0/.travis.yml
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1073 2020-10-14 14:04:18.000000 datatoolbox-0.7.0/LICENSE
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1976 2024-05-08 14:07:30.849512 datatoolbox-0.7.0/PKG-INFO
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1298 2023-09-22 10:59:58.000000 datatoolbox-0.7.0/README.md
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1225 2020-10-14 14:04:18.000000 datatoolbox-0.7.0/appveyor.yml
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-05-08 14:07:30.712402 datatoolbox-0.7.0/ci/
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-05-08 14:07:30.721922 datatoolbox-0.7.0/ci/appveyor/
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     3111 2020-10-14 14:04:18.000000 datatoolbox-0.7.0/ci/appveyor/install.ps1
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1842 2020-10-14 14:04:18.000000 datatoolbox-0.7.0/ci/appveyor/run_with_env.cmd
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-05-08 14:07:30.738034 datatoolbox-0.7.0/datatoolbox/
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     5681 2023-08-18 10:53:24.000000 datatoolbox-0.7.0/datatoolbox/__init__.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)    15513 2023-06-08 08:12:18.000000 datatoolbox-0.7.0/datatoolbox/admin.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     3753 2024-04-17 07:49:21.000000 datatoolbox-0.7.0/datatoolbox/aggregator.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     6846 2024-04-29 10:25:24.000000 datatoolbox-0.7.0/datatoolbox/config.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)    18681 2023-08-29 12:09:48.000000 datatoolbox-0.7.0/datatoolbox/converters.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    17489 2024-05-08 09:37:09.000000 datatoolbox-0.7.0/datatoolbox/core.py
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-05-08 14:07:30.746194 datatoolbox-0.7.0/datatoolbox/data/
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    15781 2020-10-14 14:04:18.000000 datatoolbox-0.7.0/datatoolbox/data/GHG_alternative_naming.pkl
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    13482 2023-05-23 13:04:06.000000 datatoolbox-0.7.0/datatoolbox/data/GHG_properties_2019_CA.csv
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-05-08 14:07:30.747642 datatoolbox-0.7.0/datatoolbox/data/SANDBOX_datashelf/
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      286 2024-05-08 13:53:23.000000 datatoolbox-0.7.0/datatoolbox/data/SANDBOX_datashelf/inventory.csv
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-05-08 14:07:30.750999 datatoolbox-0.7.0/datatoolbox/data/SANDBOX_datashelf/mappings/
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    10757 2024-05-08 13:53:23.000000 datatoolbox-0.7.0/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     8466 2024-05-08 13:53:23.000000 datatoolbox-0.7.0/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      999 2024-05-08 13:53:23.000000 datatoolbox-0.7.0/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      161 2024-05-08 13:53:23.000000 datatoolbox-0.7.0/datatoolbox/data/SANDBOX_datashelf/sources.csv
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    22865 2020-10-14 14:04:18.000000 datatoolbox-0.7.0/datatoolbox/data/all.csv
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    14615 2020-10-14 14:04:18.000000 datatoolbox-0.7.0/datatoolbox/data/compatible1_5_unfiltered.xlsx
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)    10757 2020-04-20 12:32:09.000000 datatoolbox-0.7.0/datatoolbox/data/continent.csv
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     8466 2021-09-15 15:48:16.000000 datatoolbox-0.7.0/datatoolbox/data/country_codes.csv
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1711 2022-05-25 07:15:53.000000 datatoolbox-0.7.0/datatoolbox/data/datashelf_contents.csv
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     2923 2021-12-16 12:32:58.000000 datatoolbox-0.7.0/datatoolbox/data/external_mappings.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      178 2022-11-18 16:16:07.000000 datatoolbox-0.7.0/datatoolbox/data/personal_template.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)      999 2019-08-14 10:00:22.000000 datatoolbox-0.7.0/datatoolbox/data/regions.csv
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)   237445 2024-04-03 07:39:56.000000 datatoolbox-0.7.0/datatoolbox/data_readers.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    83428 2024-05-08 07:50:13.000000 datatoolbox-0.7.0/datatoolbox/data_structures.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    65668 2024-03-20 09:16:19.000000 datatoolbox-0.7.0/datatoolbox/database.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     6730 2022-11-18 16:16:07.000000 datatoolbox-0.7.0/datatoolbox/greenhouse_gas_database.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     3542 2022-11-18 16:16:07.000000 datatoolbox-0.7.0/datatoolbox/init_tools.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    21661 2024-05-08 07:43:31.000000 datatoolbox-0.7.0/datatoolbox/interfaces.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     8561 2024-05-08 07:35:14.000000 datatoolbox-0.7.0/datatoolbox/io_tools.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    41818 2022-11-18 16:16:07.000000 datatoolbox-0.7.0/datatoolbox/mapping.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     2854 2022-12-01 09:27:15.000000 datatoolbox-0.7.0/datatoolbox/naming_convention.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     3305 2022-11-18 16:16:07.000000 datatoolbox-0.7.0/datatoolbox/patches.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     2189 2023-08-17 09:12:01.000000 datatoolbox-0.7.0/datatoolbox/pint_definitions.txt
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)        0 2020-06-08 07:09:19.000000 datatoolbox-0.7.0/datatoolbox/relations.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)    26449 2023-07-17 09:50:44.000000 datatoolbox-0.7.0/datatoolbox/sets.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)        0 2020-06-08 07:09:19.000000 datatoolbox-0.7.0/datatoolbox/storage.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1632 2022-11-18 16:16:07.000000 datatoolbox-0.7.0/datatoolbox/templates.py
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-05-08 14:07:30.772183 datatoolbox-0.7.0/datatoolbox/tools/
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    16351 2021-04-19 11:31:45.000000 datatoolbox-0.7.0/datatoolbox/tools/CRF_extract_CA_2021.xlsx
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    28022 2021-02-02 15:17:26.000000 datatoolbox-0.7.0/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    17445 2021-02-02 12:48:44.000000 datatoolbox-0.7.0/datatoolbox/tools/IEA_B2DS_4.SCEN
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)    17375 2019-12-20 11:46:57.000000 datatoolbox-0.7.0/datatoolbox/tools/WEO_2019_test.SCEN
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      559 2024-05-08 07:53:49.000000 datatoolbox-0.7.0/datatoolbox/tools/__init__.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     4320 2022-11-17 09:58:39.000000 datatoolbox-0.7.0/datatoolbox/tools/conversion_to_v0.3.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    31376 2024-05-08 08:05:41.000000 datatoolbox-0.7.0/datatoolbox/tools/excel.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      370 2022-11-17 09:58:39.000000 datatoolbox-0.7.0/datatoolbox/tools/export_all.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      251 2024-05-08 07:14:12.000000 datatoolbox-0.7.0/datatoolbox/tools/for_datatables.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     8286 2024-05-08 07:01:38.000000 datatoolbox-0.7.0/datatoolbox/tools/html.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      182 2022-11-18 16:16:07.000000 datatoolbox-0.7.0/datatoolbox/tools/install_support.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     7188 2022-11-18 16:16:07.000000 datatoolbox-0.7.0/datatoolbox/tools/kaya_idendentiy_decomposition.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     4283 2022-11-18 16:16:07.000000 datatoolbox-0.7.0/datatoolbox/tools/magicc6.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     5931 2022-11-18 16:16:07.000000 datatoolbox-0.7.0/datatoolbox/tools/matplotlib.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      892 2023-08-04 09:51:33.000000 datatoolbox-0.7.0/datatoolbox/tools/new_SR15_pathway_matching.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     3795 2024-05-08 07:55:12.000000 datatoolbox-0.7.0/datatoolbox/tools/pandas.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     5533 2022-11-18 16:16:07.000000 datatoolbox-0.7.0/datatoolbox/tools/py_magicc_tools.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     7948 2023-08-18 10:42:50.000000 datatoolbox-0.7.0/datatoolbox/tools/pyam.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      965 2022-11-18 16:16:07.000000 datatoolbox-0.7.0/datatoolbox/tools/renaming_DB.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)    84992 2019-08-14 10:26:08.000000 datatoolbox-0.7.0/datatoolbox/tools/run_MAGICC_startup_simple.xlsx
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1830 2021-02-02 14:03:36.000000 datatoolbox-0.7.0/datatoolbox/tools/run_magicc6.m
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     1044 2022-11-17 09:58:40.000000 datatoolbox-0.7.0/datatoolbox/tools/statistics.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    61174 2021-06-03 14:06:07.000000 datatoolbox-0.7.0/datatoolbox/tools/test.docx
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     8625 2022-11-18 16:16:07.000000 datatoolbox-0.7.0/datatoolbox/tools/word.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     1066 2024-05-08 07:48:19.000000 datatoolbox-0.7.0/datatoolbox/tools/xarray.py
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-05-08 14:07:30.785360 datatoolbox-0.7.0/datatoolbox/tutorials/
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     2996 2022-05-25 07:15:53.000000 datatoolbox-0.7.0/datatoolbox/tutorials/00_search_find_and_access_data.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1019 2020-10-14 14:04:18.000000 datatoolbox-0.7.0/datatoolbox/tutorials/01_emission_comparison.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     2096 2022-05-25 07:15:53.000000 datatoolbox-0.7.0/datatoolbox/tutorials/02_unit_conversion.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     5685 2020-10-14 14:04:18.000000 datatoolbox-0.7.0/datatoolbox/tutorials/03_intermediate_example.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1416 2020-10-14 14:04:19.000000 datatoolbox-0.7.0/datatoolbox/tutorials/04_sources.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      382 2020-10-14 14:04:19.000000 datatoolbox-0.7.0/datatoolbox/tutorials/05_plot_source_content.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      734 2020-12-22 15:09:15.000000 datatoolbox-0.7.0/datatoolbox/tutorials/06_xarray_examples.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     1142 2021-05-11 13:19:29.000000 datatoolbox-0.7.0/datatoolbox/tutorials/07_renewable_share_compuation.py
+-rw-rw-r--   0 andreasgeiges   (501) staff       (20)      793 2021-05-11 12:59:38.000000 datatoolbox-0.7.0/datatoolbox/tutorials/08_low_carbon_fuel_computation.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)   137631 2020-10-14 14:04:19.000000 datatoolbox-0.7.0/datatoolbox/tutorials/introduction_v1.ipynb
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     4631 2022-03-22 14:54:50.000000 datatoolbox-0.7.0/datatoolbox/tutorials/jump_start.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)      417 2023-05-12 14:15:39.000000 datatoolbox-0.7.0/datatoolbox/units.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)    43708 2024-05-08 06:59:17.000000 datatoolbox-0.7.0/datatoolbox/util.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      160 2024-05-08 14:07:30.000000 datatoolbox-0.7.0/datatoolbox/version.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      746 2022-11-18 16:16:07.000000 datatoolbox-0.7.0/datatoolbox/workflows.py
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-05-08 14:07:30.845914 datatoolbox-0.7.0/datatoolbox.egg-info/
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1976 2024-05-08 14:07:30.000000 datatoolbox-0.7.0/datatoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     3787 2024-05-08 14:07:30.000000 datatoolbox-0.7.0/datatoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)        1 2024-05-08 14:07:30.000000 datatoolbox-0.7.0/datatoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      157 2024-05-08 14:07:30.000000 datatoolbox-0.7.0/datatoolbox.egg-info/requires.txt
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)       12 2024-05-08 14:07:30.000000 datatoolbox-0.7.0/datatoolbox.egg-info/top_level.txt
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-05-08 14:07:30.807209 datatoolbox-0.7.0/doc/
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     7755 2024-04-02 13:29:36.000000 datatoolbox-0.7.0/doc/Makefile
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     9684 2024-04-02 12:29:22.000000 datatoolbox-0.7.0/doc/conf.py
+-rwxr-x---   0 andreasgeiges   (501) staff       (20)      101 2024-04-02 13:46:58.000000 datatoolbox-0.7.0/doc/core.rst
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      236 2024-04-02 14:07:33.000000 datatoolbox-0.7.0/doc/data_structures.rst
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      122 2021-01-11 16:19:59.000000 datatoolbox-0.7.0/doc/database.rst
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)       91 2021-01-11 16:18:53.000000 datatoolbox-0.7.0/doc/database_database.rst
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      130 2021-01-11 16:21:50.000000 datatoolbox-0.7.0/doc/database_gitrepomanager.rst
+-rwxr-x---   0 andreasgeiges   (501) staff       (20)       93 2021-01-11 16:03:03.000000 datatoolbox-0.7.0/doc/excel.rst
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-05-08 14:07:30.808867 datatoolbox-0.7.0/doc/figures/
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    21579 2020-11-09 13:08:35.000000 datatoolbox-0.7.0/doc/figures/ID_meta_data.svg
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)    67463 2021-05-17 15:08:58.000000 datatoolbox-0.7.0/doc/figures/config_input.png
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     7008 2023-06-08 10:16:48.000000 datatoolbox-0.7.0/doc/first_steps.md
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      100 2020-12-22 15:09:15.000000 datatoolbox-0.7.0/doc/foo.rst_template
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)       77 2020-12-22 15:09:15.000000 datatoolbox-0.7.0/doc/help.rst
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      463 2024-04-02 11:53:11.000000 datatoolbox-0.7.0/doc/index.rst
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     1655 2023-06-08 08:19:25.000000 datatoolbox-0.7.0/doc/installation.md
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     1080 2020-12-22 15:09:15.000000 datatoolbox-0.7.0/doc/license.rst
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     7353 2020-10-14 14:04:19.000000 datatoolbox-0.7.0/doc/make.bat
+-rwxr-x---   0 andreasgeiges   (501) staff       (20)      103 2021-01-11 16:09:22.000000 datatoolbox-0.7.0/doc/matplotlib.rst
+-rwxr-x---   0 andreasgeiges   (501) staff       (20)       95 2021-01-11 16:10:43.000000 datatoolbox-0.7.0/doc/pandas.rst
+-rwxr-x---   0 andreasgeiges   (501) staff       (20)      243 2024-04-02 12:12:03.000000 datatoolbox-0.7.0/doc/tools.rst
+-rwxr-x---   0 andreasgeiges   (501) staff       (20)       95 2021-01-11 16:09:13.000000 datatoolbox-0.7.0/doc/xarray.rst
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-05-08 14:07:30.810224 datatoolbox-0.7.0/documentation/
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     7761 2020-12-22 15:09:15.000000 datatoolbox-0.7.0/documentation/Datatoolbox - First steps.md
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      402 2024-05-08 08:08:15.000000 datatoolbox-0.7.0/environment.yml
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      418 2020-10-14 14:04:19.000000 datatoolbox-0.7.0/make_proj.sh
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      598 2024-04-02 14:16:29.000000 datatoolbox-0.7.0/readthedocs.yml
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      280 2024-05-08 09:29:46.000000 datatoolbox-0.7.0/requirements.txt
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)       38 2024-05-08 14:07:30.850915 datatoolbox-0.7.0/setup.cfg
+-rwxr-xr-x   0 andreasgeiges   (501) staff       (20)     1862 2023-09-22 10:49:18.000000 datatoolbox-0.7.0/setup.py
+drwxr-xr-x   0 andreasgeiges   (501) staff       (20)        0 2024-05-08 14:07:30.838089 datatoolbox-0.7.0/tests/
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     7292 2022-12-19 11:29:58.000000 datatoolbox-0.7.0/tests/test_calculations.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      696 2022-11-18 16:16:07.000000 datatoolbox-0.7.0/tests/test_converters.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     3941 2024-04-22 08:16:23.000000 datatoolbox-0.7.0/tests/test_database.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     1640 2023-03-30 13:32:13.000000 datatoolbox-0.7.0/tests/test_dataset.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     7741 2022-05-25 07:15:53.000000 datatoolbox-0.7.0/tests/test_datatable.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     1063 2022-11-16 11:59:46.000000 datatoolbox-0.7.0/tests/test_io.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      390 2022-11-22 09:54:34.000000 datatoolbox-0.7.0/tests/test_linked_functions.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     1563 2023-05-04 07:49:24.000000 datatoolbox-0.7.0/tests/test_pyam.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     3570 2022-05-25 07:15:53.000000 datatoolbox-0.7.0/tests/test_tableset.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     2595 2024-05-08 07:49:03.000000 datatoolbox-0.7.0/tests/test_tools.py
+-rwxrwx---   0 andreasgeiges   (501) staff       (20)     1768 2023-10-11 06:54:12.000000 datatoolbox-0.7.0/tests/test_units.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)      870 2020-10-14 14:04:19.000000 datatoolbox-0.7.0/tests/test_utilities.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     2437 2022-10-19 13:17:33.000000 datatoolbox-0.7.0/tests/test_xarray.py
+-rw-r--r--   0 andreasgeiges   (501) staff       (20)     2954 2024-05-08 07:45:25.000000 datatoolbox-0.7.0/tests/util_for_testing.py
```

### Comparing `datatoolbox-0.6.9/.gitlab-ci.yml` & `datatoolbox-0.7.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/.travis.yml` & `datatoolbox-0.7.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/LICENSE` & `datatoolbox-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/PKG-INFO` & `datatoolbox-0.7.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: datatoolbox
-Version: 0.6.9
-Summary: The Python Data Toolbox
-Home-page: https://gitlab.com/climateanalytics/datatoolbox
-Author: Andreas Geiges
-Author-email: a.geiges@gmail.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 DATATOOLBOX
 =====================
 
 This is a python package for handling global datasets. It contains the following features:
 
 1. Augumented pandas DataFrames adding meta data
 2. Automatic unit conversion and dataframe based computations
```

### Comparing `datatoolbox-0.6.9/appveyor.yml` & `datatoolbox-0.7.0/appveyor.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/ci/appveyor/install.ps1` & `datatoolbox-0.7.0/ci/appveyor/install.ps1`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/ci/appveyor/run_with_env.cmd` & `datatoolbox-0.7.0/ci/appveyor/run_with_env.cmd`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/__init__.py` & `datatoolbox-0.7.0/datatoolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/admin.py` & `datatoolbox-0.7.0/datatoolbox/admin.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/aggregator.py` & `datatoolbox-0.7.0/datatoolbox/aggregator.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/config.py` & `datatoolbox-0.7.0/datatoolbox/config.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/converters.py` & `datatoolbox-0.7.0/datatoolbox/converters.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/core.py` & `datatoolbox-0.7.0/datatoolbox/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,228 +4,222 @@
 Core contains some very basic functions that are used within the package
 in various locations and tools.
 
 @author: Andreas Geiges
 """
 
 import time
-tt = time.time()
+
 
 import re
 
 import numpy as np
 import pandas as pd
 from datatoolbox import config
 from datatoolbox import naming_convention
 import pandas_indexing as pix
+import pint
 
-if config.DEBUG:
-    print('Core import in {:2.4f} seconds'.format(time.time() - tt))
+from copy import copy
+from treelib import Tree
+from openscm_units import unit_registry as ur
 
 
+tt = time.time()
+if config.DEBUG:
+    print("Core import in {:2.4f} seconds".format(time.time() - tt))
 
-import pint
 
-from copy import copy
-from treelib import Node, Tree
+# %% Aggregator class
+class Aggregator:
+    """
+    This class is used to support aggregation of data according a constructed
+    hierachical tree.
+    The tree is constructe by added multiple mapping dictionaries with overlapping
+    leaves.
+    """
 
-from colorama import init as colorama_init
-from colorama import Fore
-from colorama import Style
-
-colorama_init()
-
-def colored_string(string,color):
-    
-    color_mapping = {
-        'r' : Fore.RED,
-        'y' : Fore.LIGHTYELLOW_EX,
-        'g' : Fore.GREEN
-        }
-    return f"{color_mapping[color]}{string}{Style.RESET_ALL}"
-    
-#%% Aggregator class
-class Aggregator():
-    
     def __init__(self):
-        
         self.tree = None
-        
+
         class bc:
-            HEADER = '\033[95m'
-            OKBLUE = '\033[94m'
-            OKCYAN = '\033[96m'
-            OKGREEN = '\033[92m'
-            WARNING = '\033[93m'
-            FAIL = '\033[91m'
-            ENDC = '\033[0m'
-            BOLD = '\033[1m'
-            UNDERLINE = '\033[4m'
+            HEADER = "\033[95m"
+            OKBLUE = "\033[94m"
+            OKCYAN = "\033[96m"
+            OKGREEN = "\033[92m"
+            WARNING = "\033[93m"
+            FAIL = "\033[91m"
+            ENDC = "\033[0m"
+            BOLD = "\033[1m"
+            UNDERLINE = "\033[4m"
 
-        
     def __str__(self):
         return self.tree.__str__()
-     
-    def _dict2tree(self, relation:dict):
-        
+
+    def _dict2tree(self, relation: dict):
         trees = list()
         for source, target in relation.items():
-            
             tree = Tree()
             root = tree.create_node(source, source)
-            
+
             if isinstance(target, list):
-                
                 for target_node in target:
-                    tree.create_node(target_node, target_node, parent = root)
-            
+                    tree.create_node(target_node, target_node, parent=root)
+
             else:
-                tree.create_node(target, target, parent = root)
-                
+                tree.create_node(target, target, parent=root)
+
             trees.append(tree)
-            
+
         return trees
-            
+
     def _add2tree(self, tree2add):
-        
-       
-            
-       if self.tree is None:
-           
-           self.tree = tree2add
-           
-       else:
-           
-           # check if root in existing tree
-           
-           if tree2add.root in self.tree:
-               
-               # new tree is child of existing tree
-               
-               
-               for node in tree2add.children(tree2add.root):
-                   
-                   sub_tree = tree2add.subtree(node.tag)
-                   self.tree.paste(tree2add.root, sub_tree)
-                   
-               
-           elif self.tree.root in tree2add:
-                   
-               # new tree is parent of existing tree
-               
-               old_tree = copy(self.tree)
-               
-               self.tree = tree2add
-               
-               for node in old_tree.children(old_tree.root):
-                   sub_tree = old_tree.subtree(node.tag)
-                   self.tree.paste(old_tree.root, sub_tree)
-                   
-           else:
-               raise(Exception('No connecting node found'))
-        
-    def add_relations(self, relations : dict):
-        
+        if self.tree is None:
+            self.tree = tree2add
+
+        else:
+            # check if root in existing tree
+
+            if tree2add.root in self.tree:
+                # new tree is child of existing tree
+
+                for node in tree2add.children(tree2add.root):
+                    sub_tree = tree2add.subtree(node.tag)
+                    self.tree.paste(tree2add.root, sub_tree)
+
+            elif self.tree.root in tree2add:
+                # new tree is parent of existing tree
+
+                old_tree = copy(self.tree)
+
+                self.tree = tree2add
+
+                for node in old_tree.children(old_tree.root):
+                    sub_tree = old_tree.subtree(node.tag)
+                    self.tree.paste(old_tree.root, sub_tree)
+
+            else:
+                raise (Exception("No connecting node found"))
+
+    def add_relations(self, relations: dict):
+        """
+        Add mappings to existing tree
+
+
+        Parameters
+        ----------
+        relations : dict
+            mapping.
+
+        Returns
+        -------
+        None.
+
+        """
         trees = self._dict2tree(relations)
-        
+
         for tree in trees:
             self._add2tree(tree)
-    
-    
+
     def _leave_to_dict(self, nid, mappings):
-        
         self.tree.subtree(nid).to_dict()
-        
+
         subtree = self.tree.children(nid)
-        if len(subtree)>0:
-            
+        if len(subtree) > 0:
             mapping = {nid: []}
             for node in self.tree.children(nid):
-                
                 self._leave_to_dict(node.identifier, mappings)
                 mapping[nid].append(node.identifier)
-                
+
             mappings.append(mapping)
             return mappings
-            
-            
+
         else:
             return mappings
-        
-        
-            
-        
+
     def bottom_up_aggregations(self):
-        
+        """
+        Generation of sequential mapping dictionaries for bottom up aggregation
+        according to tree
+
+        Returns
+        -------
+        mappings : TYPE
+            DESCRIPTION.
+
+        """
+
         root = self.tree.root
-        
+
         mappings = list()
-        
+
         self._leave_to_dict(root, mappings)
-        	
+
         return mappings
-    
+
     # def show_availability_data(self, wdf, index_name):
     #     #%%
     #     wdf = all_data.copy().loc[pix.isin(entity='Emissions|CO2', region='POL')]
-        
+
     #     string_lines = self.__str__()
     #     new_string_lines = list()
     #     for line in string_lines.split('\n'):
     #         sel_str = line.split('──')[-1].strip()
     #         data = wdf.loc[pix.isin(**{index_name: sel_str})]
-            
+
     #         if len(data) == 0 or (data.isnull().all(axis=1).all()):
     #             new_string_lines.append(colored_string(line, color='r'))
     #         elif data.isnull().any(axis=1).any():
     #             new_string_lines.append(colored_string(line, color='y'))
-                
+
     #         else:
     #             new_string_lines.append(colored_string(line, color='g'))
-                
+
     #     new_string_lines = '\n'.join(new_string_lines)
     #     print(new_string_lines)
-                
-#%% Pint unit handling
+
+
+# %% Pint unit handling
 gases = {
     "CO2eq": "carbon_dioxide_equivalent",
     # "CO2e": "CO2eq",
     "NO2": "NO2",
-    'PM25': 'PM25',
+    "PM25": "PM25",
 }
 
 tt_pint = time.time()
-from openscm_units import unit_registry as ur
 
 # self.ur = self_ur
 
 try:
-    
-   ur._add_gases(gases)
-    
-   ur.define('fraction = [] = frac')
-   ur.define('percent = 1e-2 frac = pct')
-   ur.define('sqkm = km * km')
-   ur.define('none = dimensionless')
+    ur._add_gases(gases)
+
+    ur.define("fraction = [] = frac")
+    ur.define("percent = 1e-2 frac = pct")
+    ur.define("sqkm = km * km")
+    ur.define("none = dimensionless")
 
-   ur.load_definitions(config.PATH_PINT_DEFINITIONS)
-   ur.define('CO2eq = CO2')
+    ur.load_definitions(config.PATH_PINT_DEFINITIONS)
+    ur.define("CO2eq = CO2")
 except pint.errors.DefinitionSyntaxError:
     # avoid double import of units defintions
     pass
-   
-import pint
 
-if config.DEBUG:
-    print('pint unit handling initialised in core in {:2.4f} seconds'.format(time.time() - tt_pint))
 
+if config.DEBUG:
+    print(
+        "pint unit handling initialised in core in {:2.4f} seconds".format(
+            time.time() - tt_pint
+        )
+    )
 
 
 LOG = dict()
-LOG['tableIDs'] = list()
+LOG["tableIDs"] = list()
+
 
 def slim_index(df):
     """
     Function to move all unique index levels to the meta of the dataframe
 
     Parameters
     ----------
@@ -234,55 +228,60 @@
 
     Returns
     -------
     df : pd.Dataframe
         resulting dataframe with squeezed index and filled meta.
 
     """
-    
-    levels_to_squeeze  = [l.name  for l in df.index.levels if len(pix.projectlevel(df.index, l.name).unique()) == 1]
-    level_values = [l[0] for l in df.index.levels if l.name in levels_to_squeeze]
-    
+
+    levels_to_squeeze = [
+        x.name
+        for x in df.index.levels
+        if len(pix.projectlevel(df.index, x.name).unique()) == 1
+    ]
+    level_values = [x[0] for x in df.index.levels if x.name in levels_to_squeeze]
+
     for level, value in zip(levels_to_squeeze, level_values):
         df.meta[level] = value
-        
+
     df = df.droplevel(levels_to_squeeze)
-    
+
     return df
 
-def blow_index(df, levels_to_add = None):
+
+def blow_index(df, levels_to_add=None):
     """
-    Unsqueeze levels from meta into the (multi-index) of the dataframe. 
+    Unsqueeze levels from meta into the (multi-index) of the dataframe.
 
     Parameters
     ----------
     df : pd.Dataframe
         Dataframe with levels squeezed to meta.
     levels_to_add : list, optional
         Optional parameter to restrict the unsqueezed levels to the given list. The default is None.
- 
+
     Returns
     -------
     df : pd.Dataframe
         resulting dataframe with unsqueezed meta.
 
 
     """
-   
-    #check that values are str
-    idx_meta = {x : y for x,y in df.meta.items() if isinstance(y, (int, float, str))}
-    
+
+    # check that values are str
+    idx_meta = {x: y for x, y in df.meta.items() if isinstance(y, (int, float, str))}
+
     if levels_to_add is not None:
-        idx_meta = {x : y for x,y in idx_meta.items() if x in levels_to_add}    
+        idx_meta = {x: y for x, y in idx_meta.items() if x in levels_to_add}
     df = pix.assignlevel(df, **idx_meta)
-    
+
     return df
 
+
 def is_known_entity(variable):
-    entity_matches = list()
     for entity in naming_convention.entities:
         if variable.startswith(entity):
             return True
 
     return False
 
 
@@ -301,39 +300,39 @@
     None.
 
     """
 
     # Find entity
     entity_matches = list()
     for entity in naming_convention.entities:
-        if metaDict['variable'].startswith(entity):
+        if metaDict["variable"].startswith(entity):
             entity_matches.append(entity)
 
     if len(entity_matches) > 0:
         longest_matchg = max(entity_matches, key=len)
-        metaDict['entity'] = longest_matchg
+        metaDict["entity"] = longest_matchg
 
     else:
         if config.DEBUG:
             print(f'Warning: Entity could not be derived from {metaDict["variable"]}')
 
         # exit here
         return metaDict
 
     # derive or check category
-    if 'category' not in metaDict.keys():
-        metaDict['category'] = (
-            metaDict['variable'].replace(longest_matchg, '').strip('|')
+    if "category" not in metaDict.keys():
+        metaDict["category"] = (
+            metaDict["variable"].replace(longest_matchg, "").strip("|")
         )
     else:
-        if metaDict['category'] != metaDict['variable'].replace(
-            longest_matchg, ''
-        ).strip('|'):
+        if metaDict["category"] != metaDict["variable"].replace(
+            longest_matchg, ""
+        ).strip("|"):
             print(
-                'Warming current category not fitting derived category, please review'
+                "Warming current category not fitting derived category, please review"
             )
     return metaDict
 
 
 def _update_meta(metaDict):
     """
     Private funcion to update the meta data of a datatable
@@ -345,40 +344,39 @@
         new data to overwrite.
 
     Returns
     -------
     metaDict : dict
 
     """
-    if 'entity' not in metaDict.keys():
-
+    if "entity" not in metaDict.keys():
         metaDict = _split_variable(metaDict)
 
     for key in list(metaDict.keys()):
-        if (metaDict[key] is np.nan) or metaDict[key] == '':
-            if key != 'unit':
+        if (metaDict[key] is np.nan) or metaDict[key] == "":
+            if key != "unit":
                 del metaDict[key]
 
     for id_field in config.ID_FIELDS:
         fieldList = [
             metaDict[key]
             for key in config.SUB_FIELDS[id_field]
             if key in metaDict.keys()
         ]
         if len(fieldList) > 0:
             new_value = (
-                config.SUB_SEP[id_field].join([str(x) for x in fieldList]).strip('|')
+                config.SUB_SEP[id_field].join([str(x) for x in fieldList]).strip("|")
             )
             if (
                 config.DEBUG
                 and id_field in metaDict.keys()
                 and metaDict[id_field] != new_value
             ):
                 print(
-                    f'Warning: {id_field} will be overritten {metaDict[id_field]} -> {new_value}'
+                    f"Warning: {id_field} will be overritten {metaDict[id_field]} -> {new_value}"
                 )
             metaDict[id_field] = new_value
 
     return metaDict
 
 
 def _fix_filename(name, max_length=255):
@@ -417,18 +415,18 @@
     Returns
     -------
     bool
         is valid.
 
     """
     try:
-        getUnit(table.meta['unit'])
+        getUnit(table.meta["unit"])
 
         return True
-    except:
+    except Exception:
         return False
 
 
 def generate_table_file_name(ID):
     """
     Generate table ID using the meta data and separators given in the config
 
@@ -440,16 +438,16 @@
     Returns
     -------
     str
         ID
 
     """
     ID_for_filename = _fix_filename(ID)
-    ID_for_filename = ID.replace('|', '-').replace('/', '-')
-    return ID_for_filename + '.csv'
+    ID_for_filename = ID.replace("|", "-").replace("/", "-")
+    return ID_for_filename + ".csv"
 
 
 def _createDatabaseID(metaDict):
     ID = config.ID_SEPARATOR.join([metaDict[key] for key in config.ID_FIELDS])
     # ID = _fix_filename(ID)
     return ID
 
@@ -470,47 +468,46 @@
         DESCRIPTION. The default is 0.
 
     Returns
     -------
     None.
 
     """
-    fid = open(filename, 'w', encoding='utf-8')
+    fid = open(filename, "w", encoding="utf-8")
     fid.write(config.META_DECLARATION)
 
     for key, value in sorted(meta.items()):
         #            if key == 'unit':
         #                value = str(value.u)
-        fid.write(key + ',' + str(value) + '\n')
+        fid.write(key + "," + str(value) + "\n")
 
     fid.write(config.DATA_DECLARATION)
     if index == 0:
-        dataframe.to_csv(fid, sep=',')
+        dataframe.to_csv(fid, sep=",")
     elif index is None:
-        dataframe.to_csv(fid, index=None, sep=';')
+        dataframe.to_csv(fid, index=None, sep=";")
     fid.close()
 
 
 def excel_writer(
-    
     writer, dataframe, meta, sheet_name="Sheet1", index=False, engine=None
 ):
     """
     Excel writer to include head of meta data before the csv like data block.
-    
+
     """
     if isinstance(writer, pd.ExcelWriter):
         need_save = False
     else:
         writer = pd.ExcelWriter(pd.io.common.stringify_path(writer), engine=engine)
         need_save = True
 
     metaSeries = pd.Series(
-        data=[''] + list(meta.values()) + [''],
-        index=['###META###'] + list(meta.keys()) + ['###DATA###'],
+        data=[""] + list(meta.values()) + [""],
+        index=["###META###"] + list(meta.keys()) + ["###DATA###"],
     )
 
     metaSeries.to_excel(writer, sheet_name=sheet_name, header=None, columns=None)
     pd.DataFrame(dataframe).to_excel(
         writer, sheet_name=sheet_name, index=index, startrow=len(metaSeries)
     )
 
@@ -524,15 +521,15 @@
 
 
     Returns
     -------
     bool
 
     """
-    if (config.OS == 'win32') | (config.OS == "Windows"):
+    if (config.OS == "win32") | (config.OS == "Windows"):
         return True
     else:
         return False
 
 
 def getUnit(string, ur=ur):
     """
@@ -546,23 +543,24 @@
         unit string (e.g. "km / s" or "€  / capita")
 
     Returns
     -------
     unit : pint unit
     """
     import pint
+
     # if not isinstance(string, str):
     #     string = str(string)
     # capture if already is pint unit
     if isinstance(string, pint.Unit):
         string = str(string)
     if string is None:
-        string = ''
+        string = ""
     else:
-        string = string.replace('$', 'USD').replace('€', 'EUR').replace('%', 'percent')
+        string = string.replace("$", "USD").replace("€", "EUR").replace("%", "percent")
     return ur(string)
 
 
 def getUnitWindows(string):
     """
     Equivalent version of getUnit  but adapted for windows system.
 
@@ -573,28 +571,25 @@
 
     Returns
     -------
     unit : pint unit
 
     """
     if string is None:
-        string = ''
+        string = ""
     else:
         string = (
-            string.replace('$', 'USD')
-            .replace('€', 'EUR')
-            .replace('%', 'percent')
-            .replace('Â', '')
+            string.replace("$", "USD")
+            .replace("€", "EUR")
+            .replace("%", "percent")
+            .replace("Â", "")
         )
     return ur(string)
 
 
-
-
-
 def get_time_string():
     """
     Return formated time string.
 
     Returns
     -------
     time string : str
@@ -631,68 +626,69 @@
 
     Returns
     -------
     TYPE
         DESCRIPTION.
 
     """
-    
-    if context == 'GWPAR4':
+
+    if context == "GWPAR4":
         import warnings
-        warnings.warn('The context "AR4GWP" is depricated. Pleases use "AR4GWP100" instead')
+
+        warnings.warn(
+            'The context "AR4GWP" is depricated. Pleases use "AR4GWP100" instead'
+        )
         context = "AR4GWP100"
     if context is None:
         return getUnit(unitFrom).to(getUnit(unitTo)).m
 
-    else:   
+    else:
         with ur.context(context) as urc:
-            factor =getUnit(unitFrom, ur=urc).to(getUnit(unitTo, ur=urc))
-            
+            factor = getUnit(unitFrom, ur=urc).to(getUnit(unitTo, ur=urc))
+
         return factor.m
 
+
 def _findGases(string, candidateList):
     hits = list()
     for key in candidateList:
         if key in string:
             hits.append(key)
-            string = string.replace(key, '')
+            string = string.replace(key, "")
     return hits
 
 
-
 def get_dimension_extend(table_iterable, dimensions):
     """
     This functions assesses the the unique extend for various dimensions
     given a set of datatables
     """
     fullIdx = dict()
     # for dim in dimensions:
     #     fullIdx[dim] = set()
 
     for table in table_iterable:
-
         #        for metaKey, metaValue in table.meta.items():
         #            if metaKey not in metaDict.keys():
         #                metaDict[metaKey] = set([metaValue])
         #            else:
         #                metaDict[metaKey].add(metaValue)
 
         for dim in dimensions:
-
             if dim not in fullIdx.keys():
                 fullIdx[dim] = set()
 
-            if dim == 'region':
+            if dim == "region":
                 fullIdx[dim] = fullIdx[dim].union(table.index)
-            elif dim == 'time':
+            elif dim == "time":
                 fullIdx[dim] = fullIdx[dim].union(table.columns)
             elif dim in table.meta.keys():
                 fullIdx[dim].add(table.meta[dim])
             else:
-                raise (BaseException('Dimension not available'))
+                raise (BaseException("Dimension not available"))
 
     dimSize = [len(fullIdx[x]) for x in dimensions]
     dimList = [sorted(list(fullIdx[x])) for x in dimensions]
 
     return dimSize, dimList
 
 
@@ -711,24 +707,24 @@
     metaCollection : TYPE
         DESCRIPTION.
 
     """
 
     metaCollection = dict()
     for table in table_iterable:
-
         for key in table.meta.keys():
-            if key in dimensions or key == 'ID':
+            if key in dimensions or key == "ID":
                 continue
             if key not in metaCollection.keys():
                 metaCollection[key] = set()
 
             metaCollection[key].add(table.meta[key])
 
     return metaCollection
 
+
 # re-defintion of getUnit function for windows users
 if osIsWindows():
     getUnit = getUnitWindows
-    
+
 if config.DEBUG:
-    print('core loaded in {:2.4f} seconds'.format(time.time() - tt))
+    print("core loaded in {:2.4f} seconds".format(time.time() - tt))
```

### Comparing `datatoolbox-0.6.9/datatoolbox/data/GHG_alternative_naming.pkl` & `datatoolbox-0.7.0/datatoolbox/data/GHG_alternative_naming.pkl`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/data/GHG_properties_2019_CA.csv` & `datatoolbox-0.7.0/datatoolbox/data/GHG_properties_2019_CA.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv` & `datatoolbox-0.7.0/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv` & `datatoolbox-0.7.0/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv` & `datatoolbox-0.7.0/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/data/all.csv` & `datatoolbox-0.7.0/datatoolbox/data/all.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/data/compatible1_5_unfiltered.xlsx` & `datatoolbox-0.7.0/datatoolbox/data/compatible1_5_unfiltered.xlsx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/data/continent.csv` & `datatoolbox-0.7.0/datatoolbox/data/continent.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/data/country_codes.csv` & `datatoolbox-0.7.0/datatoolbox/data/country_codes.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/data/datashelf_contents.csv` & `datatoolbox-0.7.0/datatoolbox/data/datashelf_contents.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/data/external_mappings.py` & `datatoolbox-0.7.0/datatoolbox/data/external_mappings.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/data/regions.csv` & `datatoolbox-0.7.0/datatoolbox/data/regions.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/data_readers.py` & `datatoolbox-0.7.0/datatoolbox/data_readers.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/data_structures.py` & `datatoolbox-0.7.0/datatoolbox/data_structures.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,17 +17,435 @@
 from copy import copy, deepcopy
 import ast
 from . import core
 from . import config
 import traceback
 from . import util
 import os
-from . import tools
+#from . import tools
 from . import converters
+from time import time
 
+#%% Functions
+
+def interpolate(datatable, method="linear"):
+
+    datatable = copy(datatable)
+
+    if method == 'linear':
+        from scipy import interpolate
+        import numpy as np
+
+        if pd.api.types.is_datetime64_any_dtype(datatable.columns.dtype):
+            xData = (
+                datatable.columns.values.astype(int) // 10**9
+            )  # timestamp in seconds
+        elif pd.api.types.is_integer_dtype(
+            datatable.columns.dtype
+        ):  # assuming year as int
+            xData = datatable.columns.values.astype(float)
+        else:
+            raise (
+                BaseException(
+                    'Expecting column dtype to be integer for years or datetime'
+                )
+            )
+
+        yData = datatable.values
+        for row in yData:
+            idxNan = np.isnan(row)
+            if sum(~idxNan) < 2:
+                continue
+            interpolator = interpolate.interp1d(
+                xData[~idxNan], row[~idxNan], kind='linear'
+            )
+            col_idx = xData[idxNan].astype(int)
+            col_idx = col_idx[col_idx > xData[~idxNan].min()]
+            col_idx = col_idx[col_idx < xData[~idxNan].max()]
+            new_idx = (
+                idxNan & (xData > xData[~idxNan].min()) & (xData < xData[~idxNan].max())
+            )
+            row[new_idx] = interpolator(col_idx)
+        return datatable
+    else:
+        raise (NotImplementedError())
+
+
+def aggregate_region(table, mapping, skipna=False):
+
+    table = copy(table)
+    missingCountryDict = dict()
+
+    for region in mapping.keys():
+
+        missingCountries = set(mapping[region]) - set(table.index)
+        #                print('missing countries: {}'.format(missingCountries))
+        missingCountryDict[region] = list(missingCountries)
+        availableCountries = set(mapping[region]).intersection(table.index)
+        if len(availableCountries) > 0:
+            table.loc[region, :] = table.loc[list(availableCountries), :].sum(
+                axis=0, skipna=skipna
+            )
+
+    return table, missingCountryDict
+
+
+def growth_rate(datatable):
+    """
+    Computes the growth rates for the given datatable
+    """
+    #    tempTable = copy(datatable)
+    #    years = tempTable.columns
+    #    completeYears = list(range(years.min() - periods, years.max()))
+    #    for year in set(completeYears).difference(tempTable.columns):
+    #        tempTable.loc[:,year] = np.nan
+    #    tempTable =tempTable.loc[:,completeYears]
+    #    growth_rates = tempTable.diff(axis=1,periods=periods).iloc[:,periods+1:] / tempTable.iloc[:,periods:-1].values
+    #    growth_rates = growth_rates.loc[~growth_rates.isnull().all(axis=1),:]
+    #    growth_rates = growth_rates.loc[:,~growth_rates.isnull().all(axis=0)]
+    #
+    #    return growth_rates
+
+    # t0 = tempTable.loc[:,years[1:]]
+    # t1 = tempTable.loc[:,[x-period for x in years if x-period in tempTable.columns]]
+    tempTable = copy(datatable)
+    growth_rates = tempTable.loc[:, tempTable.columns] * np.nan
+    for i_year in range(1, len(tempTable.columns)):
+        t0 = tempTable.columns[i_year - 1]
+        t1 = tempTable.columns[i_year]
+
+        diff = tempTable.loc[:, t1].values - tempTable.loc[:, t0].values
+        growth_rate = diff / tempTable.loc[:, t0]
+        growth_rates.loc[:, t1] = growth_rate
+    return growth_rates
+
+
+def composite_dataframe(tablePrioryList):
+
+    newColumns = set()
+    newIndex = set()
+    for table in tablePrioryList:
+        newColumns = newColumns.union(table.columns)
+        newIndex = newIndex.union(table.index)
+
+    newTable = Datatable(data=None, columns=newColumns, index=newIndex)
+
+    metaCollection = dict()
+    for table in tablePrioryList:
+        newTable = newTable.combine_first(table)
+
+        for key in table.meta.keys():
+            if key not in metaCollection.keys():
+                metaCollection[key] = set()
+
+            metaCollection[key] = metaCollection[key].union([table.meta[key]])
+
+    for key in metaCollection.keys():
+        if len(metaCollection[key]) == 1:
+            newTable.meta[key] = list(metaCollection[key])[0]
+        else:
+            newTable.meta[key] = 'merged - meta quantity'
+    return newTable
+
+
+def to_XDataArray(tableSet, dimensions=['region', 'time', 'pathway']):
+
+    #    dimensions = ['region', 'time', 'scenario', 'model']
+
+    #    metaDict = dict()
+
+    dimSize, dimList = core.get_dimension_extend(tableSet, dimensions)
+    metaCollection = core.get_meta_collection(tableSet, dimensions)
+
+    xData = xr.DataArray(np.zeros(dimSize) * np.nan, coords=dimList, dims=dimensions)
+
+    for table in tableSet:
+
+        indexTuple = list()
+        for dim in dimensions:
+            if dim == 'region':
+                indexTuple.append(list(table.index))
+            elif dim == 'time':
+                indexTuple.append(list(table.columns))
+            else:
+                indexTuple.append(table.meta[dim])
+
+        #        xx = (table.index,table.columns,table.meta['pathway'])
+        xData.loc[tuple(indexTuple)] = table.values
+
+    # only implemented for homgeneous physical units
+    assert len(metaCollection['unit']) == 1
+    xData.attrs['unit'] = list(metaCollection['unit'])[0]
+
+    for metaKey, metaValue in metaCollection.items():
+        if len(metaValue) == 1:
+            xData.attrs[metaKey] = metaValue.pop()
+        else:
+            print('Warning, dropping meta data: ' + metaKey + ' ' + str(metaValue))
+
+    return xData
+
+
+def to_XDataSet(tableSet, dimensions=['region', 'time']):
+    """
+    Convert datatoolbox tableSet to a xarray data set
+
+    Parameters
+    ----------
+    tableSet : datatoolbox.Tableset
+        DESCRIPTION.
+    dimensions : list of str
+        Full dimensions of the xarray array. Other remaining dimensions will be
+        added as dict like elements.
+
+    Returns
+    -------
+    dSet : xarray.Dataset
+        DESCRIPTION.
+
+    """
+    dimSize, dimList = core.get_dimension_extend(tableSet, dimensions=dimensions)
+
+    # dimensions= ['region', 'time']
+
+    dSet = xr.Dataset(coords={key: val for (key, val) in zip(dimensions, dimList)})
+
+    for key, table in tableSet.items():
+        dSet[key] = table
+        dSet[key].attrs = table.meta
+
+    return dSet
+
+
+def _get_unique_labels(table, dim):
+
+    if isinstance(dim, tuple):
+        unique_lables = [
+            tuple(_get_unique_labels(table, sub_dim)[0] for sub_dim in dim)
+        ]
+        # unique_lables = [tuple(d for sub_dim in dim for d in _get_unique_labels(table, sub_dim))] # todo find better way
+    elif dim == table.index.name:
+        unique_lables = table.index
+    elif dim == table.columns.name:
+        unique_lables = table.columns
+    elif dim in table.meta.keys():
+        unique_lables = [table.meta[dim]]
+    else:
+        # raise(Exception(f'Dimension {dim} not available'))
+        unique_lables = [np.nan]
+
+    return unique_lables
+
+def get_dimension_indices(table, dimensions):
+
+    ind = list()
+    for dim in dimensions:
+        if isinstance(dim, tuple):
+
+            index = [
+                tuple(_get_unique_labels(table, sub_dim)[0] for sub_dim in dim)
+            ]  # todo find better way
+        elif dim == table.index.name:
+            index = list(table.index)
+        elif dim == table.columns.name:
+            index = list(table.columns)
+        elif dim in table.attrs.keys():
+            index = [table.attrs[dim]]
+        ind.append(index)
+
+    return ind
+
+
+
+
+
+
+
+
+
+
+
+
+def key_set_to_xdataset(
+    dict_of_data,
+    dimensions=['model', 'scenario', 'region', 'time'],
+    stacked_dims={'pathway': ('model', 'scenario')},
+):
+    """
+    Returns xarry dataset converted from a dict of pandas dataframes  or dt.TableSet. Differenty variables
+    are stored as key variables. The xarray dimensions (coordiantes) are defined
+    by the provided dimensions. A multi-index for a coordinate can be created
+    by using stacked_dims.
+
+    Usage:
+    -------
+    dimensions :  Iterable[str]]
+        Dimensions of the shared yarray dimensions / coordinates
+    stacked_dims : Dict[str]]
+        Dictionary of all mutli-index coordinates and their sub-dimensions
+
+    Returns
+    -------
+    matches : xarray.Dataset + pint quantification
+    """
+
+    dim_to_sort = 'variable'
+    sort_dict = dict()
+    for key, table in dict_of_data.items():
+
+        var = table.meta['variable']
+
+        if var in sort_dict.keys():
+            sort_dict[var].append(table)
+        else:
+            sort_dict[var] = [table]
+
+    variables = sort_dict.keys()
+
+    data = list()
+    for variable in variables:
+        tables = sort_dict[variable]
+
+        xarray = _to_xarray(tables, dimensions, stacked_dims)
+        data.append(xr.Dataset({variable: xarray}))
+
+    ds = xr.merge(data)
+
+    return ds
+
+def get_dimensions(table_iterable, dimensions):
+
+    dims = dict()
+
+    for table in table_iterable:
+
+        for dim in dimensions:
+
+            dims[dim] = dims.get(dim, set()).union(_get_unique_labels(table, dim))
+    return dims
+
+def _to_xarray(tables, dimensions, stacked_dims):
+    """
+    Return a database query result as an xarray . This constuctor allows only for
+    one unit, since the full array is quantified using pint-xarray.
+    The xarray dimensions (coordiantes) are defined
+    by the provided dimensions. A multi-index for a coordinate can be created
+    by using stacked_dims.
+
+    Usage:
+    -------
+    tables : Iterable[[dt.Datatable]]
+    dimensions :  Iterable[str]]
+        Dimensions of the shared yarray dimensions / coordinates
+    stacked_dims : Dict[str]]
+        Dictionary of all mutli-index coordinates and their sub-dimensions
+
+    Returns
+    -------
+    matches : xarray.Dataset + pint quantification
+    """
+    tt = time()
+    metaCollection = core.get_meta_collection(tables, dimensions)
+    if config.DEBUG:
+        print(f'ime required for meta collection: {time()-tt:2.2f}s')
+
+    tt = time()
+    final_dims = dimensions.copy()
+    xdims = dimensions.copy()
+    for st_dim, sub_dims in stacked_dims.items():
+        [xdims.remove(dim) for dim in sub_dims]
+        xdims.append(sub_dims)
+
+        [final_dims.remove(dim) for dim in sub_dims]
+        final_dims.append(st_dim)
+
+    dims = get_dimensions(tables, xdims)
+    if config.DEBUG:
+        print(dims)
+    coords = {x: sorted(list(dims[x])) for x in dims.keys()}
+    labels = dict()
+    for st_dim, sub_dims in stacked_dims.items():
+        coords[st_dim] = range(len(coords[sub_dims]))
+        sub_labels = list()
+        for i_dim, sub_dim in enumerate(sub_dims):
+
+            sub_labels.append(
+                pd.Index([x[i_dim] for x in coords[sub_dims]], name=sub_dim)
+            )
+        labels[st_dim] = pd.MultiIndex.from_arrays(sub_labels, names=sub_dims)
+        del coords[sub_dims]
+
+    dimSize = [len(labels) for dim, labels in dims.items()]
+
+    if config.DEBUG:
+        print(f'Get timension: {time()-tt:2.2f}s')
+
+    tt = time()
+    xData = xr.DataArray(
+        np.zeros(dimSize) * np.nan, coords=coords, dims=final_dims
+    ).assign_coords(labels)
+
+    tt = time()
+    for table in tables:
+        ind = get_dimension_indices(table, xdims)
+        # xData.loc[tuple(ind)] = table.values.reshape(len(table.index),len(table.columns),1)
+
+        xData.loc[tuple(ind)] = table.values.reshape(*[len(x) for x in ind])
+    if config.DEBUG:
+        print(f'Time required for xr data filling: {time()-tt:2.2f}s')
+    tt = time()
+    metaCollection['unit'] = list(metaCollection['unit'])[0]
+    xData = xData.pint.quantify(metaCollection['unit']).assign_coords(labels)
+    xData.attrs = metaCollection
+
+    return xData
+
+def load_as_xdataset(
+    query_results,
+    dimensions=['model', 'scenario', 'region', 'time', 'source'],
+    stacked_dims={'pathway': ('model', 'scenario')},
+    native_regions=False,
+):
+    """
+    Returns xarry dataset pruduced from a database result. Differenty variables
+    are stored as key variables. The xarray dimensions (coordiantes) are defined
+    by the provided dimensions. A multi-index for a coordinate can be created
+    by using stacked_dims.
+
+    Usage:
+    -------
+    dimensions :  Iterable[str]]
+        Dimensions of the shared yarray dimensions / coordinates
+    stacked_dims : Dict[str]]
+        Dictionary of all mutli-index coordinates and their sub-dimensions
+    native_regions : bool, optional
+        Load native region defintions if available. The default is False.
+
+    Returns
+    -------
+    matches : xarray.Dataset + pint quantification
+    """
+
+    variables = query_results.variable.unique()
+
+    data = list()
+    for variable in variables:
+        tables = [
+            core.DB.getTable(x, native_regions)
+            for x in query_results.filterp(variable=variable).index
+        ]
+
+        xarray = _to_xarray(tables, dimensions, stacked_dims)
+        data.append(xr.Dataset({variable: xarray}))
+
+    ds = xr.merge(data)
+
+    return ds
+
+#%% 
 class Datatable(pd.DataFrame):
     """
     Datatable
     
 
     Datatable is derrived from pandas dataframe.  Datatables contain the 
     addition meta attribute and have autotmated unit conversions
@@ -323,15 +741,15 @@
     def aggregate_region(self, mapping, skipna=False):
         """
         This functions added the aggregates to the table according to the provided
         mapping.( See datatools.mapp.regions)
 
         Returns the result, but does not inplace add it.
         """
-        from datatoolbox.tools.for_datatables import aggregate_region
+        #from datatoolbox.tools.for_datatables import aggregate_region
 
         return aggregate_region(self, mapping, skipna)
     
     def append(self, other, **kwargs):
         """
         Append data to the datatable
 
@@ -807,15 +1225,15 @@
 
         Returns
         -------
         datatable
             Interpolated dataframe.
 
         """
-        from datatoolbox.tools.for_datatables import interpolate
+        #from datatoolbox.tools.for_datatables import interpolate
 
         if add_missing_years:
             for col in list(range(self.columns.min(), self.columns.max() + 1)):
                 if col not in self.columns:
                     self.loc[:, col] = np.nan
             self = self.loc[:, list(range(self.columns.min(), self.columns.max() + 1))]
 
@@ -1481,15 +1899,15 @@
                 BaseException(
                     'Different units in dataset can not be merged in one xarray'
                 )
             )
 
         if not config.AVAILABLE_XARRAY:
             raise (BaseException('module xarray not available'))
-        return tools.xarray.to_XDataArray(self, dimensions)
+        return to_XDataArray(self, dimensions)
 
     def to_xset(self, dimensions=['region', 'time']):
         """
         Convert table set to an xarray data set.
 
         Parameters
         ----------
@@ -1501,15 +1919,15 @@
         xr.Dataset
             DESCRIPTION.
 
         """
         dimensions = ['region', 'time']
         if not config.AVAILABLE_XARRAY:
             raise (BaseException('module xarray not available'))
-        return tools.xarray.to_XDataSet(self, dimensions)
+        return to_XDataSet(self, dimensions)
 
     def to_list(self):
         """
         Convert to list of tables
 
         Returns
         -------
@@ -1686,15 +2104,15 @@
 
         return cls.from_wide_dataframe(data, meta, stacked_dims)
 
     @classmethod
     def from_query(cls, query, stacked_dims={'pathway': ("model", "scenario")}):
         #dimensions = ['model', 'scenario', 'region', 'variable', 'source', 'unit']
         # data = query.as_wide_dataframe(meta_list=dimensions)
-        return tools.xarray.load_as_xdataset(query, stacked_dims=stacked_dims)
+        return load_as_xdataset(query, stacked_dims=stacked_dims)
         #return cls.from_wide_dataframe(data, meta=None, stacked_dims=stacked_dims)
 
 
 class Visualization:
     """
     This class addes handy built-in visualizations to datatables
     """
```

### Comparing `datatoolbox-0.6.9/datatoolbox/database.py` & `datatoolbox-0.7.0/datatoolbox/database.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/greenhouse_gas_database.py` & `datatoolbox-0.7.0/datatoolbox/greenhouse_gas_database.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/init_tools.py` & `datatoolbox-0.7.0/datatoolbox/init_tools.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/interfaces.py` & `datatoolbox-0.7.0/datatoolbox/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,20 +386,20 @@
         if config.OS == 'Linux':
             os.system('libreoffice ' + filePath)
         elif config.OS == 'Darwin':
             os.system('open -a "Microsoft Excel" ' + filePath)
 
 
 # if config.AVAILABLE_XARRAY:
-from datatoolbox.tools import xarray as _xr
+from datatoolbox import data_structures
 
 
 class _Xarray:
 
-    to_Xarray = _xr.to_XDataArray
+    to_Xarray = data_structures.to_XDataArray
 
 
 #%%
 
 
 class IAMC_PYAM:
     def __init__(self):
```

### Comparing `datatoolbox-0.6.9/datatoolbox/mapping.py` & `datatoolbox-0.7.0/datatoolbox/mapping.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/naming_convention.py` & `datatoolbox-0.7.0/datatoolbox/naming_convention.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/patches.py` & `datatoolbox-0.7.0/datatoolbox/patches.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/pint_definitions.txt` & `datatoolbox-0.7.0/datatoolbox/pint_definitions.txt`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/sets.py` & `datatoolbox-0.7.0/datatoolbox/sets.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/templates.py` & `datatoolbox-0.7.0/datatoolbox/templates.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tools/CRF_extract_CA_2021.xlsx` & `datatoolbox-0.7.0/datatoolbox/tools/CRF_extract_CA_2021.xlsx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN` & `datatoolbox-0.7.0/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tools/IEA_B2DS_4.SCEN` & `datatoolbox-0.7.0/datatoolbox/tools/IEA_B2DS_4.SCEN`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tools/WEO_2019_test.SCEN` & `datatoolbox-0.7.0/datatoolbox/tools/WEO_2019_test.SCEN`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tools/__init__.py` & `datatoolbox-0.7.0/datatoolbox/tools/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 # -*- coding: utf-8 -*-
 """
 Created on Tue Oct 27 11:05:30 2020
 
 @author: ageiges
 """
 from .. import config
-from . import for_datatables
 
 from . import pandas
 from . import excel
 
 from . import matplotlib
 
 #%% optional
 if config.AVAILABLE_XARRAY:
-    from . import xarray
+    #from . import xarray
     import pint_xarray
     from datatoolbox.core import ur
     
     
     pint_xarray.accessors.setup_registry(ur)
     pint_xarray.unit_registry = ur
     pint_xarray.accessors.default_registry = ur
```

### Comparing `datatoolbox-0.6.9/datatoolbox/tools/conversion_to_v0.3.py` & `datatoolbox-0.7.0/datatoolbox/tools/conversion_to_v0.3.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tools/excel.py` & `datatoolbox-0.7.0/datatoolbox/tools/excel.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 import re
 import string
 import pandas as pd
 import tqdm
 import platform
 from pandas_indexing import accessors
 from openpyxl import load_workbook
-
-
+import numpy as np
+from datatoolbox import config, mapp, core, io_tools, util
+from shutil import copyfile
+from copy import copy
 #%% Defintions
 OS = platform.system()  #'win32' , linux, #Darwin
 
 
 REQUIRED_SETUP_FIELDS = [
     'filePath',
     'fileName',
@@ -288,15 +290,15 @@
             return np.nan
         #        try:
         print(x)
         return float(x)
 
 
 #%% Functions
-
+getAllSheetNames = io_tools.getAllSheetNames
 
 def alphaCol2Num(col):
     num = 0
     for c in col:
         if c in string.ascii_letters:
             num = num * 26 + (ord(c.upper()) - ord('A')) + 1
     return num - 1
@@ -467,15 +469,15 @@
     except:
         return False
     
 class Excel_Reader():
     
     def __init__(self, filename):
         self.filename = filename
-        self.xls = pd.ExcelFile(self.filename)
+        self.xls = pd.ExcelFile(self.filename, engine='calamine')
 
     
     def extract_data(self, 
                      xlsx_layout :dict,
                      data_layout: dict,
                      column_mapping: dict = None,
                      index_mapping: dict = None,
@@ -489,15 +491,15 @@
         # column_mapping = test_config['column_mapping']
         # index_mapping = test_config['index_mapping']
         
         df = pd.read_excel(self.xls, **xlsx_layout)
         df.columns.names = data_layout['column_names']
         df.index.names = data_layout['index_names']
         
-        df = df[df.applymap(isnumber)]
+        df = df[df.map(isnumber)]
         
         missing_in_col =[x for x in column_mapping.keys() if not x in df.columns]
         if len(missing_in_col)>0:
             raise(Exception(
                 f'{df.columns} does not contain: {missing_in_col}')
                 )
         #apply mapping
@@ -530,385 +532,16 @@
         return ldf
     
     def openSourceFile(self):
         if OS == 'Linux':
             os.system('libreoffice ' + self.filename)
         elif OS == 'Darwin':
             os.system('open -a "Microsoft Excel" ' + self.filename)
-#%%
-
-
-#%%
 
-# class Excel_Reader:
-#     """
-#     Reader clase that uses an setup information provided in the excel file
-#     to extract data
-#     """
-
-#     def __init__(self, setup=None, fileName=None, overwrite=False, setupSheet='OUTPUT'):
-
-#         self.overwrite = overwrite
-#         self.setupSheet = setupSheet
-#         if setup:
-#             self.setup = setup
-#             fileSetup = True
-#         else:
-#             self.setup = dict()
-#             self.setup['fileName'] = fileName
-#             fileSetup = False
-
-#     def close(self):
-#         self.wb.close()
-
-#     def openSourceFile(self):
-#         if OS == 'Linux':
-#             os.system('libreoffice ' + self.setup['fileName'])
-#         elif OS == 'Darwin':
-#             os.system('open -a "Microsoft Excel" ' + self.setup['fileName'])
-
-#     def getSetups(self):
-#         self.wb_read = load_workbook(self.setup['fileName'], data_only=True)
-#         self.wb = load_workbook(self.setup['fileName'], data_only=True)
-#         setup = dict()
-#         setup['fileName'] = self.setup['fileName']
-
-#         mapping = pd.read_excel(self.setup['fileName'], sheet_name=self.setupSheet)
-
-#         setupDict = {
-#             'sheetName': 'sheetName',
-#             'timeIdxList': 'timeCells',
-#             'spaceIdxList': 'spaceCells',
-#             'dataID': 'dataCells',
-#             'unit': 'unit',
-#             'unitTo': 'unitTo',
-#         }
-
-#         setupDict = {
-#             'sheetName': 'Sheetname',
-#             'timeIdxList': 'Time',
-#             'spaceIdxList': 'Region',
-#             'dataID': 'Variable',
-#             'unit': 'Unit',
-#             'unitTo': 'UnitTo',
-#             'scenario': 'Scenario',
-#             'source': 'Source',
-#         }
-
-#         for i, setupMapp in mapping.iterrows():
-#             for key in setupDict.keys():
-#                 setup[key] = str(setupMapp[setupDict[key]])
-#                 if setup[key] == 'nan':
-#                     setup[key] = None
-
-#             yield (dict(setup))
-
-#     #        setupSheet = self.wb[self.setupSheet]
-#     #        for row in setupSheet.rows:
-#     #            if row[0].value == 'sheet':
-#     #                continue
-#     #
-#     #            setup['sheetName']   = row[0].value
-#     #            setup['timeIdxList']  = row[1].value
-#     #            setup['spaceIdxList'] = row[2].value
-#     #            setup['dataID']      = row[3].value
-#     #            setup['unit']        = row[4].value
-#     #
-#     #            for key in setup.keys():
-#     #                if isinstance(setup[key],str):
-#     #                    setup[key] = setup[key].replace('\ufeff','')
-#     #            yield(setup)
-
-#     def read_data(self):
-#         replaceDict = {'EU': 'EU28'}
-#         from shutil import copyfile
-#         from copy import copy
-#         import mapping as mapp
-#         import datatoolbox as dt
-
-#         wb = load_workbook(self.setup['fileName'], data_only=True)
-
-#         validSpatialIDs = mapp.getValidSpatialIDs()
-#         self.setupList = list()
-
-#         tablesToReturn = dt.TableSet()
-
-#         for setup in self.getSetups():
-#             if isinstance(setup['timeIdxList'], int):
-#                 setup['timeIdxList'] = str(setup['timeIdxList'])
-#             if isinstance(setup['spaceIdxList'], int):
-#                 setup['spaceIdxList'] = str(setup['spaceIdxList'])
-#             print(setup)
-#             self.setupList.append(copy(setup))
-#             args = None, None, None, None, None
-#             wksSheet = wb[setup['sheetName']]
-
-#             args = [None, None, None, None, None]
-#             for argsTime in _iterTime(setup['timeIdxList'], wksSheet, *args):
-
-#                 if argsTime[TI_ARG] is None:
-#                     print('No time defintion found')
-#                     print(setup['timeIdxList'])
-
-#                     continue
-#                 print(argsTime[TI_ARG])
-#                 print(setup['spaceIdxList'])
-#                 for argsSpace in _iterSpace(setup['spaceIdxList'], wksSheet, *argsTime):
-#                     if argsSpace[SP_ARG] is None:
-#                         print('Not space defintion found')
-#                         continue
-
-#                     if argsSpace[SP_ARG] not in validSpatialIDs:
-#                         print('No valid ISO code...')
-
-#                         if argsSpace[SP_ARG] in replaceDict.keys():
-#                             newID = replaceDict[argsSpace[SP_ARG]]
-#                         else:
-#                             newID = util.getCountryISO(argsSpace[SP_ARG])
-
-#                         if newID in validSpatialIDs:
-#                             argsSpace[SP_ARG] = newID
-#                             print('Set iso code to: ' + argsSpace[SP_ARG])
-#                         else:
-#                             print('No ISO code found')
-#                             print(argsSpace[SP_ARG] + ' not found')
-#                             continue
-
-#                     print(argsSpace)
-#                     for argData in _iterData(setup['dataID'], wksSheet, *argsSpace):
-#                         if argData[DT_ARG] is None:
-#                             print('No fitting dataID code found')
-#                             continue
-
-#                         meta = {
-#                             'entity': argData[DT_ARG],
-#                             'unit': setup['unit'],
-#                             'category': '',
-#                             'scenario': setup['scenario'],
-#                             'source': setup['source'],
-#                         }
-#                         #                        print(meta)
-#                         ID = core._createDatabaseID(meta)
-
-#                         if ID not in tablesToReturn.keys():
-#                             table = Datatable()
-#                             table.meta = {
-#                                 'entity': argData[DT_ARG],
-#                                 'unit': setup['unit'],
-#                                 'category': '',
-#                                 'scenario': setup['scenario'],
-#                                 'source': setup['source'],
-#                             }
-
-#                             tablesToReturn.add(table)
-#                         #                        print(argData)
-#                         value = self._readValue(
-#                             wksSheet, xlsRow=argData[0], xlsCol=argData[1]
-#                         )
-
-#                         if isinstance(value, pd.DataFrame):
-#                             value = pandasStr2floatPercent(value)
-#                         else:
-#                             if value != '#VALUE!':
-#                                 value = _str2float(value)
-#                         #                        print(value)
-
-#                         #                        if  setup['unit'] == '%':
-#                         #                            value = value*100
-#                         #                        sdf
-#                         tablesToReturn[ID].loc[argData[SP_ARG], argData[TI_ARG]] = value
-#         #                            print('success')
-#         #                        iCount +=1
-
-#         #                        except Exception as e:
-#         ##                            print(e)
-#         #                            pass
-#         #                    self.wb.save(self.setup['fileName'])
-#         #                            import pdb
-#         #                            pdb.set_trace()
-
-#         for table in tablesToReturn:
-#             table.columns = table.columns.astype(int)
-#             if '%' in table.meta['unit']:
-#                 table.loc[:, :] = table.loc[:, :] * 100
-#                 tablesToReturn[table.ID] = table
-
-#         return tablesToReturn
-
-#     #            wb.save(self.setup['fileName'])
-#     #            print('{} items inserted'.format(iCount))
-#     #
-#     #            wb.close()
-
-#     def _readValue(self, wrkSheet, xlsRow, xlsCol):
-#         #        if self.overwrite or pd.isna():
-#         #            wrkSheet.cell(row=xlsRow, column=xlsCol, value = value)
-#         return wrkSheet.cell(row=xlsRow, column=xlsCol).value
-
-
-# #    def _writeMultipleIndicators(self, setup):
-# #        ws_readValues = load_workbook(self.setup['fileName'], data_only=True)[setup['sheetName']]
-# #        try:
-# #            tableIDs = [cell.value for cell in ws_readValues[setup['dataID']]]
-# #        except:
-# #            tableIDs = [cell[0].value for cell in ws_readValues[setup['dataID']]]
-# #
-# #            tables = dt.getTables(tableIDs)
-# #
-# #            REG_FIND_ROWS.search(setup['timeIdxList'])
-
-
-# class ExcelReader:
-#     def __init__(self, setupDict, xlsFile=None):
-#         """
-#         Required setup parameters:
-#             filePath    = './data/'
-#             fileName    = "test.xls"
-#             sheetName   = "Sheet0"
-#             timeIdxList  = ("B1", "C1")
-#             spaceIdxList = ('A2', 'A10')
-
-#         """
-#         self.setup(**setupDict)
-#         if xlsFile is not None:
-#             self.xlsFile = xlsFile
-
-#     #    def setSetup(self, **kwargs):
-#     #        for key in kwargs.keys():
-#     #            self.setup[key] = kwargs[key]
-
-#     def setup(self, **kwargs):
-#         for key in kwargs.keys():
-
-#             if 'Idx' in key:
-#                 # conversion of index
-#                 setattr(self, key, [excel_to_pandas_idx(x) for x in kwargs[key]])
-#             else:
-#                 setattr(self, key, kwargs[key])
-#         if hasattr(self, 'df'):
-#             del self.df
-
-#     #
-#     #        self.validate()
-
-#     def getAllSheetNames(self):
-#         xlFile = pd.ExcelFile(os.path.join(self.filePath, self.fileName))
-#         sheetNameList = xlFile.sheet_names
-#         xlFile.close()
-#         return sheetNameList
-
-#     def validate(
-#         self,
-#     ):
-#         for attr in REQUIRED_SETUP_FIELDS:
-#             if not hasattr(self, attr):
-#                 print(attr + " is missing")
-
-#     def gatherValue(self, excelIdx):
-#         if not hasattr(self, 'df'):
-#             if hasattr(self, 'xlsFile'):
-#                 self.df = pd.read_excel(
-#                     self.xlsFile, sheet_name=self.sheetName, header=None
-#                 )
-#             else:
-#                 self.df = pd.read_excel(
-#                     os.path.join(self.filePath, self.fileName),
-#                     sheet_name=self.sheetName,
-#                     header=None,
-#                 )
-#         # elif core.config.DEBUG:
-#         # print('use loaded df')
-#         return self.df.iloc[excel_to_pandas_idx(excelIdx)]
-
-#     def getAllData(self):
-#         return self.df
-
-#     def openFile(self):
-#         import os
-
-#         os.system('libreoffice ' + os.path.join(self.filePath, self.fileName))
-
-#     def gatherData(self, load=True):
-
-#         if load:
-#             self.df = pd.read_excel(
-#                 os.path.join(self.filePath, self.fileName),
-#                 sheet_name=self.sheetName,
-#                 header=None,
-#             )
-#         #            print('df loaded')
-#         elif core.config.DEBUG:
-#             print('use loaded df')
-
-#         #        print(self.spaceIdxList)
-#         #        print(self.timeIdxList)
-
-#         if len(self.timeIdxList) > 1:
-#             timeIdx = self.df.iloc[
-#                 self.timeIdxList[0][0],
-#                 self.timeIdxList[0][1] : self.timeIdxList[1][1] + 1,
-#             ]
-#             columns = self.df.columns[
-#                 self.timeIdxList[0][1] : self.timeIdxList[1][1] + 1
-#             ]
-#         #            print(timeIdx)
-#         else:
-#             timeIdx = self.df.iloc[self.timeIdxList[0][0], [self.timeIdxList[0][1]]]
-#             columns = self.df.columns[[self.timeIdxList[0][1]]]
-
-#         if len(self.spaceIdxList) > 1:
-#             regions = self.df.iloc[
-#                 self.spaceIdxList[0][0] : self.spaceIdxList[1][0] + 1,
-#                 self.spaceIdxList[0][1],
-#             ]
-#             index = self.df.index[self.spaceIdxList[0][0] : self.spaceIdxList[1][0] + 1]
-#         else:
-#             regions = self.df.iloc[[self.spaceIdxList[0][0]], self.spaceIdxList[0][1]]
-#             index = self.df.index[[self.spaceIdxList[0][0]]]
-
-#         if len(index) == 1:
-#             #            print(index)
-#             #            print(columns)
-#             #            print(regions)
-#             #            print(timeIdx)
-
-#             if len(columns) == 1:
-#                 # extraction of a single value
-#                 data = self.df.loc[index, columns]
-#                 return pd.DataFrame(data.values, columns=regions, index=timeIdx).T
-
-#             else:
-#                 # extraction of time serie
-#                 data = self.df.iloc[
-#                     self.spaceIdxList[0][0],
-#                     self.timeIdxList[0][1] : self.timeIdxList[1][1] + 1,
-#                 ]
-#                 # print(type(data))
-#                 # print(data.index)
-#                 return pd.DataFrame(data.values, columns=regions, index=timeIdx).T
-#         #                return pd.Series(data.values, index=columns)
-
-#         else:
-
-#             if len(columns) == 1:
-#                 # extraction of spatial series
-#                 data = self.df.loc[index, columns]
-
-#                 return pd.DataFrame(data.values, columns=regions, index=timeIdx).T
-#             #                return pd.Series(data.values, index=index)
-#             else:
-#                 # extraction of both spatial and time data
-#                 #                print(self.df)
-#                 #                print(index)
-#                 #                print(timeIdx)
-#                 #                print(columns)
-#                 data = self.df.loc[index, columns]
-#                 #                print(data)
 
-#                 return pd.DataFrame(data.values, columns=timeIdx, index=regions)
 
 
 class ExcelWriter:
     """
     More complex excel interface
     Author: Andreas Geiges
     """
@@ -958,36 +591,19 @@
         for i, setupMapp in mapping.iterrows():
             print(setupMapp)
             for key in setupDict.keys():
                 setup[key] = str(setupMapp[setupDict[key]])
                 if setup[key] == 'nan':
                     setup[key] = None
             yield (dict(setup))
-        # old
-
-    #        setupSheet = self.wb[self.setupSheet]
-    #        for row in setupSheet.rows:
-    #            if row[0].value == 'sheet':
-    #                continue
-    #
-    #            setup['sheetName']   = row[0].value
-    #            setup['timeIdxList']  = row[1].value
-    #            setup['spaceIdxList'] = row[2].value
-    #            setup['dataID']      = row[3].value
-    #            setup['unit']        = row[4].value
-    #
-    #            for key in setup.keys():
-    #                if isinstance(setup[key],str):
-    #                    setup[key] = setup[key].replace('\ufeff','')
-    #            yield(setup)
+    
 
     def insert_data(self):
         replaceDict = {'EU': 'EU28'}
-        from shutil import copyfile
-        from copy import copy
+
 
         # Copy old file with "_filled" extension and load it
         if '.xlsx' in self.setup['fileName']:
             saveFileName = self.setup['fileName'].replace('.xlsx', '_filled.xlsx')
         elif '.xls' in self.setup['fileName']:
             saveFileName = self.setup['fileName'].replace('.xls', '_filled.xlsx')
         else:
@@ -1247,15 +863,15 @@
         row += 1
         #        dsf
         _create_source_inventory(sourceID)
 
     sht.autofit()
 
 
-#%%
+
 def _create_source_inventory(sourceID):
     #%
     import os
     import datatoolbox as dt
     import xlwings as xl
     import pandas as pd
     import time
```

### Comparing `datatoolbox-0.6.9/datatoolbox/tools/html.py` & `datatoolbox-0.7.0/datatoolbox/tools/html.py`

 * *Files 5% similar despite different names*

```diff
@@ -296,7 +296,17 @@
 
     def appendText(self, htmlText):
         self.buffer += htmlText
 
     def close(self):
         self._appendFooder()
         self._writeFile()
+        
+
+
+def export_to_pdf(dataframe, fileName):
+    html = _html.export_to_html(dataframe)
+    import pdfkit
+
+    pdfkit.from_string(html, fileName)
+
+
```

### Comparing `datatoolbox-0.6.9/datatoolbox/tools/kaya_idendentiy_decomposition.py` & `datatoolbox-0.7.0/datatoolbox/tools/kaya_idendentiy_decomposition.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tools/magicc6.py` & `datatoolbox-0.7.0/datatoolbox/tools/magicc6.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tools/matplotlib.py` & `datatoolbox-0.7.0/datatoolbox/tools/matplotlib.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tools/new_SR15_pathway_matching.py` & `datatoolbox-0.7.0/datatoolbox/tools/new_SR15_pathway_matching.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tools/pandas.py` & `datatoolbox-0.7.0/datatoolbox/tools/pandas.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 Created on Tue Dec 22 09:34:50 2020
 
 @author: ageiges
 """
 import numpy as np
 
-# from ..util import identifyCountry
+from ..util import identifyCountry
 from .. import mapping as mapp
 
 
 def addCountryNames(table, as_index=False):
     names = list()
     for idx in table.index:
         if idx in mapp.countries.codes.index:
```

### Comparing `datatoolbox-0.6.9/datatoolbox/tools/py_magicc_tools.py` & `datatoolbox-0.7.0/datatoolbox/tools/py_magicc_tools.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tools/pyam.py` & `datatoolbox-0.7.0/datatoolbox/tools/pyam.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tools/renaming_DB.py` & `datatoolbox-0.7.0/datatoolbox/tools/renaming_DB.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tools/run_MAGICC_startup_simple.xlsx` & `datatoolbox-0.7.0/datatoolbox/tools/run_MAGICC_startup_simple.xlsx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tools/run_magicc6.m` & `datatoolbox-0.7.0/datatoolbox/tools/run_magicc6.m`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tools/statistics.py` & `datatoolbox-0.7.0/datatoolbox/tools/statistics.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tools/test.docx` & `datatoolbox-0.7.0/datatoolbox/tools/test.docx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tools/word.py` & `datatoolbox-0.7.0/datatoolbox/tools/word.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tutorials/00_search_find_and_access_data.py` & `datatoolbox-0.7.0/datatoolbox/tutorials/00_search_find_and_access_data.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tutorials/01_emission_comparison.py` & `datatoolbox-0.7.0/datatoolbox/tutorials/01_emission_comparison.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tutorials/02_unit_conversion.py` & `datatoolbox-0.7.0/datatoolbox/tutorials/02_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tutorials/03_intermediate_example.py` & `datatoolbox-0.7.0/datatoolbox/tutorials/03_intermediate_example.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tutorials/04_sources.py` & `datatoolbox-0.7.0/datatoolbox/tutorials/04_sources.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tutorials/06_xarray_examples.py` & `datatoolbox-0.7.0/datatoolbox/tutorials/06_xarray_examples.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tutorials/07_renewable_share_compuation.py` & `datatoolbox-0.7.0/datatoolbox/tutorials/07_renewable_share_compuation.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tutorials/08_low_carbon_fuel_computation.py` & `datatoolbox-0.7.0/datatoolbox/tutorials/08_low_carbon_fuel_computation.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tutorials/introduction_v1.ipynb` & `datatoolbox-0.7.0/datatoolbox/tutorials/introduction_v1.ipynb`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/tutorials/jump_start.py` & `datatoolbox-0.7.0/datatoolbox/tutorials/jump_start.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox/util.py` & `datatoolbox-0.7.0/datatoolbox/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,23 +60,14 @@
 #                                reason="please import from matplotlib toolkid",
 #                                version='0.4.0')
 # savefig = dp.deprecated(_plt.savefig,
 #                                reason="please import from matplotlib toolkid",
 #                                version='0.4.0')
 
 
-from .tools import html as _html
-
-
-def export_to_pdf(dataframe, fileName):
-    html = _html.export_to_html(dataframe)
-    import pdfkit
-
-    pdfkit.from_string(html, fileName)
-
 
 
 
 def diff_eps(df1, df2, eps=1e-6):
     """
     Identify differences between two Datatables higher than a defined treshold.
```

### Comparing `datatoolbox-0.6.9/datatoolbox/workflows.py` & `datatoolbox-0.7.0/datatoolbox/workflows.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/datatoolbox.egg-info/SOURCES.txt` & `datatoolbox-0.7.0/datatoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/doc/Makefile` & `datatoolbox-0.7.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/doc/conf.py` & `datatoolbox-0.7.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/doc/figures/ID_meta_data.svg` & `datatoolbox-0.7.0/doc/figures/ID_meta_data.svg`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/doc/figures/config_input.png` & `datatoolbox-0.7.0/doc/figures/config_input.png`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/doc/first_steps.md` & `datatoolbox-0.7.0/doc/first_steps.md`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/doc/installation.md` & `datatoolbox-0.7.0/doc/installation.md`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/doc/license.rst` & `datatoolbox-0.7.0/doc/license.rst`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/doc/make.bat` & `datatoolbox-0.7.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/documentation/Datatoolbox - First steps.md` & `datatoolbox-0.7.0/documentation/Datatoolbox - First steps.md`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/readthedocs.yml` & `datatoolbox-0.7.0/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/setup.py` & `datatoolbox-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/tests/test_calculations.py` & `datatoolbox-0.7.0/tests/test_calculations.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/tests/test_converters.py` & `datatoolbox-0.7.0/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/tests/test_database.py` & `datatoolbox-0.7.0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/tests/test_dataset.py` & `datatoolbox-0.7.0/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/tests/test_datatable.py` & `datatoolbox-0.7.0/tests/test_datatable.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/tests/test_io.py` & `datatoolbox-0.7.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/tests/test_pyam.py` & `datatoolbox-0.7.0/tests/test_pyam.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/tests/test_tableset.py` & `datatoolbox-0.7.0/tests/test_tableset.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/tests/test_tools.py` & `datatoolbox-0.7.0/tests/test_tools.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                   index = ['ARG', 'DEU', 'FRA', 'GBR'],
                   meta={'entity' : 'Emissions|CO2',
                        'scenario' : 'Historic',
                        'source' : 'XYZ_2020',
                        'unit' : 'm'}, )
 
 def test_interpolation():
-    from datatoolbox.tools.for_datatables import interpolate
+    from datatoolbox.data_structures import interpolate
     
     
     #interpolation to with columns as years
     resTable = interpolate(df1)
     
     assert (resTable.loc['DEU',2012] == 3)
     assert np.isnan(resTable.loc['GBR',2010])
@@ -44,30 +44,30 @@
     assert interpolated_table.loc['GBR', '2018-08-09 12:00:00'] == 11.
     assert interpolated_table.loc['GBR', '2018-08-09 13:00:00'] == 12.
     # test of linked method
     df1.interpolate()
    
 def test_aggregation():
     
-    from datatoolbox.tools.for_datatables import aggregate_region
+    from datatoolbox.data_structures import aggregate_region
     
     mapping= {'EU3': ['DEU', 'GBR', 'FRA']}
     res, missingCountries = aggregate_region(df1, mapping, skipna=True)
     
     npt.assert_array_almost_equal(res.loc['EU3',:].values, 
                                   np.array([2.3, 3.4, 6.4, 3.2]),
                                   decimal = 6)
     npt.assert_array_almost_equal(res.loc['GBR',:].values, 
                                   np.array([np.nan, 3.4, 2.4, 3.2]),
                                   decimal = 6)
     
     
 def test_growth_rates():
     
-    from datatoolbox.tools.for_datatables import growth_rate
+    from datatoolbox.data_structures import growth_rate
     
     res = growth_rate(df3)
     
     exp = np.array([[np.nan,  1.2 ,  0.36363636,  0.33333333,  0.25      ],
                     [np.nan, np.nan, np.nan, np.nan, np.nan],
                     [np.nan, np.nan, np.nan, np.nan, np.nan],
                     [np.nan, np.nan, -0.29411765,  0.33333333, np.nan]])
```

### Comparing `datatoolbox-0.6.9/tests/test_units.py` & `datatoolbox-0.7.0/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/tests/test_utilities.py` & `datatoolbox-0.7.0/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/tests/test_xarray.py` & `datatoolbox-0.7.0/tests/test_xarray.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.6.9/tests/util_for_testing.py` & `datatoolbox-0.7.0/tests/util_for_testing.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,9 +71,9 @@
                    'unit' : 'USD 2010',
                    '_timeformat' : '%Y-%m-%d %H:%M:%S'}
 
 df_datetime = dt.Datatable(data_datetime, 
                            meta=meta_datetime, 
                            columns = ['2018-08-09 11:00:00', '2018-08-09 12:00:00', '2018-08-09 13:00:00', '2018-08-10 12:00:00'], 
                            index = ['TUN', 'DEU', 'FRA', 'GBR'])
-from datatoolbox.tools.for_datatables import interpolate
+from datatoolbox.data_structures import interpolate
 # print(interpolate(df_datetime).values)
```

