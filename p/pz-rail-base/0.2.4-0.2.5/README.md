# Comparing `tmp/pz_rail_base-0.2.4.tar.gz` & `tmp/pz_rail_base-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz_rail_base-0.2.4.tar", last modified: Thu Apr 25 00:36:37 2024, max compression
+gzip compressed data, was "pz_rail_base-0.2.5.tar", last modified: Wed May  8 15:03:30 2024, max compression
```

## Comparing `pz_rail_base-0.2.4.tar` & `pz_rail_base-0.2.5.tar`

### file list

```diff
@@ -1,159 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.512645 pz_rail_base-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.484645 pz_rail_base-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.484645 pz_rail_base-0.2.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.488645 pz_rail_base-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-25 00:36:37.512645 pz_rail_base-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/rail_packages.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 00:36:37.512645 pz_rail_base-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.480645 pz_rail_base-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.512645 pz_rail_base-0.2.4/src/pz_rail_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-25 00:36:37.000000 pz_rail_base-0.2.4/src/pz_rail_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-25 00:36:37.000000 pz_rail_base-0.2.4/src/pz_rail_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 00:36:37.000000 pz_rail_base-0.2.4/src/pz_rail_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-25 00:36:37.000000 pz_rail_base-0.2.4/src/pz_rail_base.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-25 00:36:37.000000 pz_rail_base-0.2.4/src/pz_rail_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 00:36:37.000000 pz_rail_base-0.2.4/src/pz_rail_base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.484645 pz_rail_base-0.2.4/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.488645 pz_rail_base-0.2.4/src/rail/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/cli/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.488645 pz_rail_base-0.2.4/src/rail/core/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 00:36:37.000000 pz_rail_base-0.2.4/src/rail/core/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/core/algo_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/core/common_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    25183 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/core/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/core/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/core/point_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14637 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/core/stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/core/util_stages.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.488645 pz_rail_base-0.2.4/src/rail/creation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.492645 pz_rail_base-0.2.4/src/rail/creation/degradation/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/creation/degradation/addRandom.py
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/creation/degradation/quantityCut.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/creation/degrader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/creation/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/creation/noisifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/creation/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.492645 pz_rail_base-0.2.4/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.492645 pz_rail_base-0.2.4/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/estimation/algos/equal_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/estimation/algos/naive_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/estimation/algos/point_est_hist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/estimation/algos/random_gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/estimation/algos/train_z.py
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/estimation/algos/uniform_binning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/estimation/algos/var_inf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/estimation/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/estimation/estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/estimation/informer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/estimation/summarizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.492645 pz_rail_base-0.2.4/src/rail/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/evaluation/dist_to_dist_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/evaluation/dist_to_point_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    18658 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/evaluation/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.492645 pz_rail_base-0.2.4/src/rail/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/evaluation/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/evaluation/metrics/cdeloss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/evaluation/metrics/pointestimates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/evaluation/point_to_point_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21261 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/evaluation/single_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/evaluation/stats_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.492645 pz_rail_base-0.2.4/src/rail/examples_data/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.480645 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.492645 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/configs/flowModeler.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.492645 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.496645 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_I_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1000000 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)   431705 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.480645 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.496645 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.496645 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/AB/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/AB/dummy.txt
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/CWW_HDFN_prior.pkl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.500645 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/
--rw-r--r--   0 runner    (1001) docker     (127)    98003 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res
--rw-r--r--   0 runner    (1001) docker     (127)    95326 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res
--rw-r--r--   0 runner    (1001) docker     (127)    96635 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res
--rw-r--r--   0 runner    (1001) docker     (127)    90216 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res
--rw-r--r--   0 runner    (1001) docker     (127)   100126 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res
--rw-r--r--   0 runner    (1001) docker     (127)    93013 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.500645 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/
--rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/CWWSB4.list
--rwxr-xr-x   0 runner    (1001) docker     (127)    43750 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    42830 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    72228 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    68560 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    43351 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    42789 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)   179585 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)   179584 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.500645 pz_rail_base-0.2.4/src/rail/examples_data/goldenspike_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.500645 pz_rail_base-0.2.4/src/rail/examples_data/goldenspike_data/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.504645 pz_rail_base-0.2.4/src/rail/examples_data/goldenspike_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)  1158108 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   873947 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/goldenspike_data/goldenspike.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.512645 pz_rail_base-0.2.4/src/rail/examples_data/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    91936 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/lsst_filters.npy
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/make_rail_sample_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    43200 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/output_BPZ_lite.fits
--rw-r--r--   0 runner    (1001) docker     (127)    37192 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/output_BPZ_lite.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)    24574 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq
--rw-r--r--   0 runner    (1001) docker     (127)   662976 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)   873930 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/test_dc2_training_9816.pq
--rw-r--r--   0 runner    (1001) docker     (127)  1192254 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq
--rw-r--r--   0 runner    (1001) docker     (127)  1316984 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)    15192 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/training_100gal.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/examples_data/testdata/validation_10gal.hdf5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.512645 pz_rail_base-0.2.4/src/rail/stages/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/src/rail/stages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.484645 pz_rail_base-0.2.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.512645 pz_rail_base-0.2.4/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/cli/hello_world.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/cli/single_number.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/cli/test_scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.512645 pz_rail_base-0.2.4/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/core/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/core/test_introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/core/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/core/test_point_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.512645 pz_rail_base-0.2.4/tests/creation/
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/creation/test_degraders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.512645 pz_rail_base-0.2.4/tests/estimation/
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/estimation/test_algos.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/estimation/test_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/estimation/test_summarizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:36:37.512645 pz_rail_base-0.2.4/tests/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-25 00:36:27.000000 pz_rail_base-0.2.4/tests/evaluation/test_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.915544 pz_rail_base-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.883544 pz_rail_base-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.887544 pz_rail_base-0.2.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.887544 pz_rail_base-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-05-08 15:03:30.915544 pz_rail_base-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/rail_packages.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:03:30.915544 pz_rail_base-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.879544 pz_rail_base-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.915544 pz_rail_base-0.2.5/src/pz_rail_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-05-08 15:03:30.000000 pz_rail_base-0.2.5/src/pz_rail_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-08 15:03:30.000000 pz_rail_base-0.2.5/src/pz_rail_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:03:30.000000 pz_rail_base-0.2.5/src/pz_rail_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 15:03:30.000000 pz_rail_base-0.2.5/src/pz_rail_base.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-08 15:03:30.000000 pz_rail_base-0.2.5/src/pz_rail_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 15:03:30.000000 pz_rail_base-0.2.5/src/pz_rail_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.883544 pz_rail_base-0.2.5/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.887544 pz_rail_base-0.2.5/src/rail/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/cli/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.887544 pz_rail_base-0.2.5/src/rail/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 15:03:30.000000 pz_rail_base-0.2.5/src/rail/core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/core/common_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25297 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/core/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/core/point_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14637 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/core/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.891544 pz_rail_base-0.2.5/src/rail/creation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/creation/degrader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.891544 pz_rail_base-0.2.5/src/rail/creation/degraders/
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/creation/degraders/addRandom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/creation/degraders/quantityCut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/creation/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/creation/noisifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/creation/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.891544 pz_rail_base-0.2.5/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.891544 pz_rail_base-0.2.5/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/estimation/algos/equal_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/estimation/algos/naive_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/estimation/algos/point_est_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/estimation/algos/random_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/estimation/algos/train_z.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/estimation/algos/uniform_binning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/estimation/algos/var_inf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/estimation/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/estimation/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/estimation/informer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/estimation/summarizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.891544 pz_rail_base-0.2.5/src/rail/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/evaluation/dist_to_dist_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/evaluation/dist_to_point_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18658 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/evaluation/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.891544 pz_rail_base-0.2.5/src/rail/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/evaluation/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/evaluation/metrics/cdeloss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/evaluation/metrics/pointestimates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/evaluation/point_to_point_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21261 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/evaluation/single_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/evaluation/stats_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.891544 pz_rail_base-0.2.5/src/rail/examples_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.883544 pz_rail_base-0.2.5/src/rail/examples_data/creation_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.895544 pz_rail_base-0.2.5/src/rail/examples_data/creation_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/creation_data/configs/flowModeler.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.895544 pz_rail_base-0.2.5/src/rail/examples_data/creation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/creation_data/data/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.895544 pz_rail_base-0.2.5/src/rail/examples_data/creation_data/data/success_rate_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_I_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1000000 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   431705 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.883544 pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.895544 pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.895544 pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/AB/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/AB/dummy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/CWW_HDFN_prior.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.899544 pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/FILTER/
+-rw-r--r--   0 runner    (1001) docker     (127)    98003 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res
+-rw-r--r--   0 runner    (1001) docker     (127)    95326 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res
+-rw-r--r--   0 runner    (1001) docker     (127)    96635 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res
+-rw-r--r--   0 runner    (1001) docker     (127)    90216 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res
+-rw-r--r--   0 runner    (1001) docker     (127)   100126 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res
+-rw-r--r--   0 runner    (1001) docker     (127)    93013 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.899544 pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/SED/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/SED/CWWSB4.list
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43750 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42830 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    72228 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    68560 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43351 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42789 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179585 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179584 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.899544 pz_rail_base-0.2.5/src/rail/examples_data/goldenspike_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.899544 pz_rail_base-0.2.5/src/rail/examples_data/goldenspike_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.903544 pz_rail_base-0.2.5/src/rail/examples_data/goldenspike_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1158108 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   873947 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/goldenspike_data/goldenspike.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.911544 pz_rail_base-0.2.5/src/rail/examples_data/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/testdata/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    91936 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/testdata/lsst_filters.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/testdata/make_rail_sample_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    43200 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/testdata/output_BPZ_lite.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    37192 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/testdata/output_BPZ_lite.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)    24574 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq
+-rw-r--r--   0 runner    (1001) docker     (127)   662976 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)   873930 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/testdata/test_dc2_training_9816.pq
+-rw-r--r--   0 runner    (1001) docker     (127)  1192254 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq
+-rw-r--r--   0 runner    (1001) docker     (127)  1316984 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)    15192 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/testdata/training_100gal.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/examples_data/testdata/validation_10gal.hdf5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.911544 pz_rail_base-0.2.5/src/rail/stages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/stages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.911544 pz_rail_base-0.2.5/src/rail/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/tools/table_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.911544 pz_rail_base-0.2.5/src/rail/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/utils/path_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/src/rail/utils/testing_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.883544 pz_rail_base-0.2.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.911544 pz_rail_base-0.2.5/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/tests/cli/hello_world.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/tests/cli/single_number.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/tests/cli/test_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.911544 pz_rail_base-0.2.5/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     9301 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/tests/core/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/tests/core/test_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/tests/core/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/tests/core/test_point_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.911544 pz_rail_base-0.2.5/tests/creation/
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/tests/creation/test_degraders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.911544 pz_rail_base-0.2.5/tests/estimation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/tests/estimation/test_algos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/tests/estimation/test_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/tests/estimation/test_summarizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.915544 pz_rail_base-0.2.5/tests/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/tests/evaluation/test_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:03:30.915544 pz_rail_base-0.2.5/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-08 15:03:23.000000 pz_rail_base-0.2.5/tests/utils/test_utils.py
```

### Comparing `pz_rail_base-0.2.4/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_base-0.2.5/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_base-0.2.5/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/.github/pull_request_template.md` & `pz_rail_base-0.2.5/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/.github/workflows/linting.yml` & `pz_rail_base-0.2.5/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/.github/workflows/publish-to-pypi.yml` & `pz_rail_base-0.2.5/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/.github/workflows/smoke-test.yml` & `pz_rail_base-0.2.5/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/.github/workflows/testing-and-coverage.yml` & `pz_rail_base-0.2.5/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/.gitignore` & `pz_rail_base-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/.pre-commit-config.yaml` & `pz_rail_base-0.2.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/LICENSE` & `pz_rail_base-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/PKG-INFO` & `pz_rail_base-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-base
-Version: 0.2.4
+Version: 0.2.5
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_base-0.2.4/README.md` & `pz_rail_base-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/pyproject.toml` & `pz_rail_base-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/pz_rail_base.egg-info/PKG-INFO` & `pz_rail_base-0.2.5/src/pz_rail_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-base
-Version: 0.2.4
+Version: 0.2.5
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_base-0.2.4/src/pz_rail_base.egg-info/SOURCES.txt` & `pz_rail_base-0.2.5/src/pz_rail_base.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,28 +23,26 @@
 src/pz_rail_base.egg-info/requires.txt
 src/pz_rail_base.egg-info/top_level.txt
 src/rail/cli/commands.py
 src/rail/cli/options.py
 src/rail/cli/scripts.py
 src/rail/core/__init__.py
 src/rail/core/_version.py
-src/rail/core/algo_utils.py
 src/rail/core/common_params.py
 src/rail/core/data.py
 src/rail/core/introspection.py
 src/rail/core/point_estimation.py
 src/rail/core/stage.py
-src/rail/core/util_stages.py
 src/rail/core/utils.py
 src/rail/creation/degrader.py
 src/rail/creation/engine.py
 src/rail/creation/noisifier.py
 src/rail/creation/selector.py
-src/rail/creation/degradation/addRandom.py
-src/rail/creation/degradation/quantityCut.py
+src/rail/creation/degraders/addRandom.py
+src/rail/creation/degraders/quantityCut.py
 src/rail/estimation/classifier.py
 src/rail/estimation/estimator.py
 src/rail/estimation/informer.py
 src/rail/estimation/summarizer.py
 src/rail/estimation/algos/equal_count.py
 src/rail/estimation/algos/naive_stack.py
 src/rail/estimation/algos/point_est_hist.py
@@ -103,19 +101,23 @@
 src/rail/examples_data/testdata/test_dc2_training_9816.pq
 src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq
 src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq
 src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5
 src/rail/examples_data/testdata/training_100gal.hdf5
 src/rail/examples_data/testdata/validation_10gal.hdf5
 src/rail/stages/__init__.py
+src/rail/tools/table_tools.py
+src/rail/utils/path_utils.py
+src/rail/utils/testing_utils.py
 tests/cli/hello_world.ipynb
 tests/cli/single_number.ipynb
 tests/cli/test_scripts.py
 tests/core/test_core.py
 tests/core/test_introspection.py
 tests/core/test_pipeline.py
 tests/core/test_point_estimation.py
 tests/creation/test_degraders.py
 tests/estimation/test_algos.py
 tests/estimation/test_classifier.py
 tests/estimation/test_summarizers.py
-tests/evaluation/test_evaluation.py
+tests/evaluation/test_evaluation.py
+tests/utils/test_utils.py
```

### Comparing `pz_rail_base-0.2.4/src/rail/cli/commands.py` & `pz_rail_base-0.2.5/src/rail/cli/commands.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/cli/options.py` & `pz_rail_base-0.2.5/src/rail/cli/options.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/cli/scripts.py` & `pz_rail_base-0.2.5/src/rail/cli/scripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import yaml
 
 import rail.stages
 from rail.core import RailEnv
 from rail.cli.options import GitMode
-from rail.core.utils import RAILDIR
+from rail.utils.path_utils import RAILDIR
 
 
 def render_nb(outdir, clear_output, dry_run, inputs, skip, **_kwargs):
     command = "jupyter nbconvert"
     options = "--to html"
 
     status = {}
```

### Comparing `pz_rail_base-0.2.4/src/rail/core/__init__.py` & `pz_rail_base-0.2.5/src/rail/core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import setuptools
 import rail
 
 from .stage import RailPipeline, RailStage
 
 # from .utilPhotometry import PhotormetryManipulator, HyperbolicSmoothing, HyperbolicMagnitudes
-from .util_stages import ColumnMapper, RowSelector, TableConverter
+# from .util_stages import ColumnMapper, RowSelector, TableConverter
 from .introspection import RailEnv
 from .point_estimation import PointEstimationMixin
 
 
 def find_version():
     """Find the version"""
     # setuptools_scm should install a
```

### Comparing `pz_rail_base-0.2.4/src/rail/core/algo_utils.py` & `pz_rail_base-0.2.5/src/rail/utils/testing_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Utility functions to test alogrithms"""
 import os
 import scipy.special
 from rail.core.stage import RailStage
-from rail.core.utils import RAILDIR
+from rail.utils.path_utils import RAILDIR
 from rail.core.data import TableHandle
 
 
 traindata = os.path.join(RAILDIR, "rail/examples_data/testdata/training_100gal.hdf5")
 validdata = os.path.join(RAILDIR, "rail/examples_data/testdata/validation_10gal.hdf5")
 DS = RailStage.data_store
 DS.__class__.allow_overwrite = True
```

### Comparing `pz_rail_base-0.2.4/src/rail/core/common_params.py` & `pz_rail_base-0.2.5/src/rail/core/common_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """ Parameters that are shared between stages """
 
 from ceci.config import StageParameter as Param
 from ceci.config import StageConfig
 
+
+
+
 lsst_bands = "ugrizy"
 lsst_mag_cols = [f"mag_{band}_lsst" for band in lsst_bands]
 lsst_mag_err_cols = [f"mag_err_{band}_lsst" for band in lsst_bands]
 lsst_def_maglims = dict(
     mag_u_lsst=27.79,
     mag_g_lsst=29.04,
     mag_r_lsst=29.06,
```

### Comparing `pz_rail_base-0.2.4/src/rail/core/data.py` & `pz_rail_base-0.2.5/src/rail/core/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,15 +278,15 @@
         """Write the data to the associated file"""
         return tables_io.write(data, path, **kwargs)
 
     def _size(self, path, **kwargs):
         if path in [None, 'none', 'None']:  # pragma: no cover
             return 0
         try:
-            return tables_io.io.getInputDataLengthHdf5(path, **kwargs)
+            return tables_io.io.getInputDataLength(path, **kwargs)
         except Exception:
             return 0
 
     def _data_size(self, data, **kwargs):
         group_name = kwargs.get('groupname', None)
         if group_name:
             try:
@@ -363,14 +363,17 @@
 
 
 class PqHandle(TableHandle):
     """DataHandle for a parquet table"""
 
     suffix = "pq"
 
+    @classmethod
+    def _size(cls, path, **kwargs):
+        return tables_io.io.getInputDataLengthPq(path, **kwargs)
 
 class QPHandle(DataHandle):
     """DataHandle for qp ensembles"""
 
     suffix = "hdf5"
 
     @classmethod
```

### Comparing `pz_rail_base-0.2.4/src/rail/core/introspection.py` & `pz_rail_base-0.2.5/src/rail/core/introspection.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/core/point_estimation.py` & `pz_rail_base-0.2.5/src/rail/core/point_estimation.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/core/stage.py` & `pz_rail_base-0.2.5/src/rail/core/stage.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/core/util_stages.py` & `pz_rail_base-0.2.5/src/rail/tools/table_tools.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/core/utils.py` & `pz_rail_base-0.2.5/src/rail/utils/path_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import os
 import rail
 import rail.core
 
 RAILDIR = os.path.abspath(os.path.join(os.path.dirname(rail.core.__file__), "..", ".."))
 
-
 def find_rail_file(relpath):
     """Find a file somewhere in rail by searching the namespace path
 
     This lets us avoid issues that the paths can be different depending
     on if we have installed things from source or not
     """
     for path_ in rail.__path__:
```

### Comparing `pz_rail_base-0.2.4/src/rail/creation/degradation/addRandom.py` & `pz_rail_base-0.2.5/src/rail/creation/degraders/addRandom.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/creation/degradation/quantityCut.py` & `pz_rail_base-0.2.5/src/rail/creation/degraders/quantityCut.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/creation/degrader.py` & `pz_rail_base-0.2.5/src/rail/creation/degrader.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/creation/engine.py` & `pz_rail_base-0.2.5/src/rail/creation/engine.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/creation/noisifier.py` & `pz_rail_base-0.2.5/src/rail/creation/noisifier.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/creation/selector.py` & `pz_rail_base-0.2.5/src/rail/creation/selector.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/estimation/algos/equal_count.py` & `pz_rail_base-0.2.5/src/rail/estimation/algos/equal_count.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/estimation/algos/naive_stack.py` & `pz_rail_base-0.2.5/src/rail/estimation/algos/naive_stack.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/estimation/algos/point_est_hist.py` & `pz_rail_base-0.2.5/src/rail/estimation/algos/point_est_hist.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/estimation/algos/random_gauss.py` & `pz_rail_base-0.2.5/src/rail/estimation/algos/random_gauss.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/estimation/algos/train_z.py` & `pz_rail_base-0.2.5/src/rail/estimation/algos/train_z.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/estimation/algos/uniform_binning.py` & `pz_rail_base-0.2.5/src/rail/estimation/algos/uniform_binning.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/estimation/algos/var_inf.py` & `pz_rail_base-0.2.5/src/rail/estimation/algos/var_inf.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/estimation/classifier.py` & `pz_rail_base-0.2.5/src/rail/estimation/classifier.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/estimation/estimator.py` & `pz_rail_base-0.2.5/src/rail/estimation/estimator.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/estimation/informer.py` & `pz_rail_base-0.2.5/src/rail/estimation/informer.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/estimation/summarizer.py` & `pz_rail_base-0.2.5/src/rail/estimation/summarizer.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/evaluation/dist_to_dist_evaluator.py` & `pz_rail_base-0.2.5/src/rail/evaluation/dist_to_dist_evaluator.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/evaluation/dist_to_point_evaluator.py` & `pz_rail_base-0.2.5/src/rail/evaluation/dist_to_point_evaluator.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/evaluation/evaluator.py` & `pz_rail_base-0.2.5/src/rail/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/evaluation/metrics/base.py` & `pz_rail_base-0.2.5/src/rail/evaluation/metrics/base.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/evaluation/metrics/cdeloss.py` & `pz_rail_base-0.2.5/src/rail/evaluation/metrics/cdeloss.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/evaluation/metrics/pointestimates.py` & `pz_rail_base-0.2.5/src/rail/evaluation/metrics/pointestimates.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/evaluation/point_to_point_evaluator.py` & `pz_rail_base-0.2.5/src/rail/evaluation/point_to_point_evaluator.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/evaluation/single_evaluator.py` & `pz_rail_base-0.2.5/src/rail/evaluation/single_evaluator.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt` & `pz_rail_base-0.2.5/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt` & `pz_rail_base-0.2.5/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt` & `pz_rail_base-0.2.5/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt` & `pz_rail_base-0.2.5/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt` & `pz_rail_base-0.2.5/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res` & `pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res` & `pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res` & `pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res` & `pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res` & `pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res` & `pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed` & `pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed` & `pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed` & `pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed` & `pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed` & `pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed` & `pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed` & `pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed` & `pz_rail_base-0.2.5/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml` & `pz_rail_base-0.2.5/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl` & `pz_rail_base-0.2.5/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq` & `pz_rail_base-0.2.5/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/goldenspike_data/goldenspike.yml` & `pz_rail_base-0.2.5/src/rail/examples_data/goldenspike_data/goldenspike.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/testdata/README.md` & `pz_rail_base-0.2.5/src/rail/examples_data/testdata/README.md`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/testdata/lsst_filters.npy` & `pz_rail_base-0.2.5/src/rail/examples_data/testdata/lsst_filters.npy`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/testdata/make_rail_sample_data.ipynb` & `pz_rail_base-0.2.5/src/rail/examples_data/testdata/make_rail_sample_data.ipynb`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/testdata/output_BPZ_lite.fits` & `pz_rail_base-0.2.5/src/rail/examples_data/testdata/output_BPZ_lite.fits`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/testdata/output_BPZ_lite.hdf5` & `pz_rail_base-0.2.5/src/rail/examples_data/testdata/output_BPZ_lite.hdf5`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq` & `pz_rail_base-0.2.5/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5` & `pz_rail_base-0.2.5/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/testdata/test_dc2_training_9816.pq` & `pz_rail_base-0.2.5/src/rail/examples_data/testdata/test_dc2_training_9816.pq`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq` & `pz_rail_base-0.2.5/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq` & `pz_rail_base-0.2.5/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5` & `pz_rail_base-0.2.5/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/testdata/training_100gal.hdf5` & `pz_rail_base-0.2.5/src/rail/examples_data/testdata/training_100gal.hdf5`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/examples_data/testdata/validation_10gal.hdf5` & `pz_rail_base-0.2.5/src/rail/examples_data/testdata/validation_10gal.hdf5`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/src/rail/stages/__init__.py` & `pz_rail_base-0.2.5/src/rail/stages/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,29 +10,30 @@
 from rail.estimation.algos.train_z import *
 from rail.estimation.algos.var_inf import *
 from rail.estimation.algos.uniform_binning import *
 from rail.estimation.algos.equal_count import *
 
 
 from rail.creation.degrader import *
-#from rail.creation.degradation.spectroscopic_degraders import *
-# from rail.creation.degradation.spectroscopic_selections import *
-from rail.creation.degradation.quantityCut import *
+#from rail.creation.degraders.spectroscopic_degraders import *
+# from rail.creation.degraders.spectroscopic_selections import *
+from rail.creation.degraders.quantityCut import *
 
 from rail.creation.engine import *
 
 # from rail.creation.engines.flowEngine import *
 # from rail.creation.engines.galaxy_population_components import *
 # from rail.creation.engines.dsps_photometry_creator import *
 # from rail.creation.engines.dsps_sed_modeler import *
 
 from rail.evaluation.dist_to_dist_evaluator import DistToDistEvaluator
 from rail.evaluation.dist_to_point_evaluator import DistToPointEvaluator
 from rail.evaluation.evaluator import Evaluator, OldEvaluator
 from rail.evaluation.point_to_point_evaluator import PointToPointEvaluator
 from rail.evaluation.single_evaluator import SingleEvaluator
 
+from rail.tools.table_tools import ColumnMapper, RowSelector, TableConverter
 
 def import_and_attach_all():
     """Import all the packages in the rail ecosystem and attach them to this module"""
     RailEnv.import_all_packages()
     RailEnv.attach_stages(rail.stages)
```

### Comparing `pz_rail_base-0.2.4/tests/cli/hello_world.ipynb` & `pz_rail_base-0.2.5/tests/cli/hello_world.ipynb`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/tests/cli/single_number.ipynb` & `pz_rail_base-0.2.5/tests/cli/single_number.ipynb`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/tests/cli/test_scripts.py` & `pz_rail_base-0.2.5/tests/cli/test_scripts.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/tests/core/test_core.py` & `pz_rail_base-0.2.5/tests/core/test_core.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,63 +14,21 @@
     ModelHandle,
     PqHandle,
     QPHandle,
     QPOrTableHandle,
     TableHandle,
 )
 from rail.core.stage import RailStage
-from rail.core.utils import RAILDIR, find_rail_file
-from rail.core.util_stages import (
-    ColumnMapper,
-    RowSelector,
-    TableConverter,
-)
+from rail.utils.path_utils import RAILDIR
 
 
 # def test_data_file():
 #    with pytest.raises(ValueError) as errinfo:
 #        df = DataFile('dummy', 'x')
 
-def test_find_rail_file():
-    afile = find_rail_file(os.path.join("examples_data", "testdata", "test_dc2_training_9816.pq"))
-    assert afile
-    with pytest.raises(ValueError):
-        _not_a_file = find_rail_file("not_a_file")
-
-
-def test_util_stages():
-    DS = RailStage.data_store
-    DS.clear()
-    datapath = os.path.join(
-        RAILDIR, "rail", "examples_data", "testdata", "test_dc2_training_9816.pq"
-    )
-
-    data = DS.read_file("data", TableHandle, datapath)
-
-    table_conv = TableConverter.make_stage(name="conv", output_format="numpyDict")
-    col_map = ColumnMapper.make_stage(name="col_map", columns={})
-    row_sel = RowSelector.make_stage(name="row_sel", start=1, stop=15)
-
-    with pytest.raises(KeyError) as _errinfo:
-        table_conv.get_handle("nope", allow_missing=False)
-
-    _conv_data = table_conv(data)
-    mapped_data = col_map(data)
-    _sel_data = row_sel(mapped_data)
-
-    row_sel_2 = RowSelector.make_stage(name="row_sel_2", start=1, stop=15)
-    row_sel_2.set_data("input", mapped_data.data)
-    handle = row_sel_2.get_handle("input")
-
-    row_sel_3 = RowSelector.make_stage(
-        name="row_sel_3", input=handle.path, start=1, stop=15
-    )
-    row_sel_3.set_data("input", None, do_read=True)
-
-
 def do_data_handle(datapath, handle_class):
     _DS = RailStage.data_store
 
     th = handle_class("data", path=datapath)
 
     with pytest.raises(ValueError) as _errinfo:
         th.write()
@@ -287,48 +245,14 @@
     assert model2 is model3
 
     mh3 = ModelHandle("model3", path=model_path_copy, data=model1)
     with mh3.open(mode="w") as fout:
         pickle.dump(obj=mh3.data, file=fout, protocol=pickle.HIGHEST_PROTOCOL)
     os.remove(model_path_copy)
 
-
-def test_data_hdf5_iter():
-    DS = RailStage.data_store
-    DS.clear()
-
-    datapath = os.path.join(
-        RAILDIR, "rail", "examples_data", "testdata", "test_dc2_training_9816.hdf5"
-    )
-
-    # data = DS.read_file('data', TableHandle, datapath)
-    th = Hdf5Handle("data", path=datapath)
-    x = th.iterator(groupname="photometry", chunk_size=1000)
-
-    assert isinstance(x, GeneratorType)
-    for i, xx in enumerate(x):
-        assert xx[0] == i * 1000
-        assert xx[1] - xx[0] <= 1000
-
-    _data = DS.read_file("input", TableHandle, datapath)
-    cm = ColumnMapper.make_stage(
-        input=datapath,
-        chunk_size=1000,
-        hdf5_groupname="photometry",
-        columns=dict(id="bob"),
-    )
-    x = cm.input_iterator("input")
-
-    assert isinstance(x, GeneratorType)
-
-    for i, xx in enumerate(x):
-        assert xx[0] == i * 1000
-        assert xx[1] - xx[0] <= 1000
-
-
 def test_data_store():
     DS = RailStage.data_store
     DS.clear()
     DS.__class__.allow_overwrite = False
 
     datapath_hdf5 = os.path.join(
         RAILDIR, "rail", "examples_data", "testdata", "test_dc2_training_9816.hdf5"
@@ -399,41 +323,7 @@
 
     set_param_default("zmin", 0.1)
     par = copy_param("zmin")
     assert par.default == 0.1
     assert par.value == 0.1
     assert par.dtype == float
 
-
-def test_set_data_nonexistent_file():
-    """Create an instance of a child class of RailStage. Exercise the `set_data`
-    method and pass in a path to a nonexistent file. A `FileNotFound` exception
-    should be raised.
-    """
-
-    col_map = ColumnMapper.make_stage(name="col_map", columns={})
-    with pytest.raises(FileNotFoundError) as err:
-        col_map.set_data("model", None, path="./bad_directory/no_file.py")
-        assert "Unable to find file" in err.context
-
-
-def test_set_data_real_file():
-    """Create an instance of a child class of RailStage. Exercise the `set_data`
-    method and pass in a path to model. The output of set_data should be `None`.
-    """
-    DS = RailStage.data_store
-    DS.clear()
-    model_path = os.path.join(
-        RAILDIR,
-        "rail",
-        "examples_data",
-        "estimation_data",
-        "data",
-        "CWW_HDFN_prior.pkl",
-    )
-    DS.add_data("model", None, ModelHandle, path=model_path)
-
-    col_map = ColumnMapper.make_stage(name="col_map", columns={})
-
-    ret_val = col_map.set_data("model", None, path=model_path, do_read=False)
-
-    assert ret_val is None
```

### Comparing `pz_rail_base-0.2.4/tests/core/test_introspection.py` & `pz_rail_base-0.2.5/tests/core/test_introspection.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/tests/core/test_pipeline.py` & `pz_rail_base-0.2.5/tests/core/test_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 import ceci
 import numpy as np
 
 from rail.core.stage import RailPipeline, RailStage
-from rail.core.utils import RAILDIR
-from rail.core.util_stages import ColumnMapper, TableConverter
+from rail.utils.path_utils import RAILDIR
+from rail.tools.table_tools import ColumnMapper, TableConverter
 
 
 def test_pipeline():
     DS = RailStage.data_store
     DS.__class__.allow_overwrite = True
     DS.clear()
```

### Comparing `pz_rail_base-0.2.4/tests/core/test_point_estimation.py` & `pz_rail_base-0.2.5/tests/core/test_point_estimation.py`

 * *Files identical despite different names*

### Comparing `pz_rail_base-0.2.4/tests/creation/test_degraders.py` & `pz_rail_base-0.2.5/tests/creation/test_degraders.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from typing import Type
 
 import numpy as np
 import pandas as pd
 import pytest
 
 from rail.core.data import DATA_STORE, TableHandle
-from rail.core.util_stages import ColumnMapper
-from rail.creation.degradation.quantityCut import QuantityCut
-from rail.creation.degradation.addRandom import AddColumnOfRandom
+from rail.tools.table_tools import ColumnMapper
+from rail.creation.degraders.quantityCut import QuantityCut
+from rail.creation.degraders.addRandom import AddColumnOfRandom
 
 
 @pytest.fixture
 def data():
     """Some dummy data to use below."""
 
     DS = DATA_STORE()
```

### Comparing `pz_rail_base-0.2.4/tests/estimation/test_algos.py` & `pz_rail_base-0.2.5/tests/estimation/test_algos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import scipy.special
 
-from rail.core.algo_utils import one_algo
+from rail.utils.testing_utils import one_algo
 from rail.core.stage import RailStage
 from rail.estimation.algos import random_gauss, train_z
 
 sci_ver_str = scipy.__version__.split(".")
 
 
 DS = RailStage.data_store
```

### Comparing `pz_rail_base-0.2.4/tests/estimation/test_classifier.py` & `pz_rail_base-0.2.5/tests/estimation/test_classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import numpy as np
 import pytest
 
-from rail.core.utils import RAILDIR
+from rail.utils.path_utils import RAILDIR
 from rail.core.stage import RailStage
 from rail.core.data import QPHandle
 from rail.estimation.algos.uniform_binning import UniformBinningClassifier
 from rail.estimation.algos.equal_count import EqualCountClassifier
 
 
 DS = RailStage.data_store
```

### Comparing `pz_rail_base-0.2.4/tests/estimation/test_summarizers.py` & `pz_rail_base-0.2.5/tests/estimation/test_summarizers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from rail.core.data import QPHandle
 from rail.core.stage import RailStage
-from rail.core.utils import RAILDIR
+from rail.utils.path_utils import RAILDIR
 from rail.estimation.algos import naive_stack, point_est_hist, var_inf
 
 testdata = os.path.join(RAILDIR, "rail/examples_data/testdata/output_BPZ_lite.hdf5")
 DS = RailStage.data_store
 
 
 def one_algo(key, summarizer_class, summary_kwargs):
```

### Comparing `pz_rail_base-0.2.4/tests/evaluation/test_evaluation.py` & `pz_rail_base-0.2.5/tests/evaluation/test_evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import numpy as np
 import qp
 
 import rail.evaluation.metrics.pointestimates as pe
 from rail.core.data import QPHandle, TableHandle,  QPOrTableHandle
 from rail.core.stage import RailStage
-from rail.core.utils import find_rail_file
+from rail.utils.path_utils import find_rail_file
 from rail.evaluation.evaluator import OldEvaluator
 from rail.evaluation.dist_to_dist_evaluator import DistToDistEvaluator
 from rail.evaluation.dist_to_point_evaluator import DistToPointEvaluator
 from rail.evaluation.point_to_point_evaluator import PointToPointEvaluator
 from rail.evaluation.single_evaluator import SingleEvaluator
 
 # values for metrics
```

