# Comparing `tmp/scores-0.6.tar.gz` & `tmp/scores-0.7.tar.gz`

## Comparing `scores-0.6.tar` & `scores-0.7.tar`

### file list

```diff
@@ -1,117 +1,52 @@
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 scores-0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 scores-0.6/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 scores-0.6/environment.yml
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scores-0.6/mkdocs.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.6/py.typed
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scores-0.6/readthedocs.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.6/setup.cfg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 scores-0.6/.binder/postBuild
--rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 scores-0.6/.binder/requirements.txt
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 scores-0.6/.github/pull_request_template.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 scores-0.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 scores-0.6/.github/ISSUE_TEMPLATE/new_score.md
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 scores-0.6/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 scores-0.6/.github/workflows/python-app.yml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 scores-0.6/.github/workflows/run-pre-commit.yml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scores-0.6/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/.gitignore
--rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_196c199763c487c9___init___py.html
--rw-r--r--   0        0        0   308776 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_196c199763c487c9_cdf_test_data_py.html
--rw-r--r--   0        0        0   231586 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_196c199763c487c9_crps_test_data_py.html
--rw-r--r--   0        0        0    13479 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_196c199763c487c9_functions_test_data_py.html
--rw-r--r--   0        0        0    53771 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_196c199763c487c9_roc_test_data_py.html
--rw-r--r--   0        0        0    45169 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_196c199763c487c9_test_brier_py.html
--rw-r--r--   0        0        0   157787 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_196c199763c487c9_test_crps_py.html
--rw-r--r--   0        0        0    65192 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_196c199763c487c9_test_functions_py.html
--rw-r--r--   0        0        0    50904 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_196c199763c487c9_test_roc_py.html
--rw-r--r--   0        0        0     7936 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_3421a23d4325477f___init___py.html
--rw-r--r--   0        0        0   114225 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_3421a23d4325477f_flip_flop_impl_py.html
--rw-r--r--   0        0        0   176515 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_3421a23d4325477f_isoreg_impl_py.html
--rw-r--r--   0        0        0   176359 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_3421a23d4325477f_isoreg_py.html
--rw-r--r--   0        0        0    79751 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_3421a23d4325477f_murphy_impl_py.html
--rw-r--r--   0        0        0    27743 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_3421a23d4325477f_quantile_loss_impl_py.html
--rw-r--r--   0        0        0    51058 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_3421a23d4325477f_standard_impl_py.html
--rw-r--r--   0        0        0     8307 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_77f509327f4cfccd___init___py.html
--rw-r--r--   0        0        0    19383 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_77f509327f4cfccd_brier_impl_py.html
--rw-r--r--   0        0        0    18057 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_77f509327f4cfccd_checks_py.html
--rw-r--r--   0        0        0   212629 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_77f509327f4cfccd_crps_impl_py.html
--rw-r--r--   0        0        0   105511 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_77f509327f4cfccd_functions_py.html
--rw-r--r--   0        0        0    38214 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_77f509327f4cfccd_roc_impl_py.html
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_9e03d4585d4ce690___init___py.html
--rw-r--r--   0        0        0    42739 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_9e03d4585d4ce690_binary_impl_py.html
--rw-r--r--   0        0        0    63835 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_9e03d4585d4ce690_multicategorical_impl_py.html
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_a44f0ac069e85531___init___py.html
--rw-r--r--   0        0        0    55964 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_a44f0ac069e85531_assertions_py.html
--rw-r--r--   0        0        0    26257 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_a44f0ac069e85531_test_functions_py.html
--rw-r--r--   0        0        0   283274 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_a44f0ac069e85531_test_processing_data_py.html
--rw-r--r--   0        0        0   161406 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_a44f0ac069e85531_test_processing_py.html
--rw-r--r--   0        0        0    18456 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_a44f0ac069e85531_test_sample_data_py.html
--rw-r--r--   0        0        0   192800 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_a44f0ac069e85531_test_utils_py.html
--rw-r--r--   0        0        0    56187 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_a44f0ac069e85531_test_weights_py.html
--rw-r--r--   0        0        0    17230 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_a44f0ac069e85531_utils_test_data_py.html
--rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_a837850aa7022bcf___init___py.html
--rw-r--r--   0        0        0    42497 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_a837850aa7022bcf_test_acovf_py.html
--rw-r--r--   0        0        0   118857 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_a837850aa7022bcf_test_diebold_mariano_py.html
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_b5d7082d1482d9f1___init___py.html
--rw-r--r--   0        0        0   193979 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_b5d7082d1482d9f1_multicategorical_test_data_py.html
--rw-r--r--   0        0        0    65796 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_b5d7082d1482d9f1_test_binary_py.html
--rw-r--r--   0        0        0   114760 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_b5d7082d1482d9f1_test_multicategorical_py.html
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_c9c9b489b8fbf792___init___py.html
--rw-r--r--   0        0        0    33973 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_c9c9b489b8fbf792_acovf_py.html
--rw-r--r--   0        0        0   106642 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_c9c9b489b8fbf792_diebold_mariano_impl_py.html
--rw-r--r--   0        0        0     5614 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_e9e7c70ce9e31b19___init___py.html
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_fa972d61f811bd58___init___py.html
--rw-r--r--   0        0        0   127244 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_fa972d61f811bd58_flip_flop_test_data_py.html
--rw-r--r--   0        0        0    91063 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_fa972d61f811bd58_isoreg_test_data_py.html
--rw-r--r--   0        0        0    43688 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_fa972d61f811bd58_quantile_loss_test_data_py.html
--rw-r--r--   0        0        0   126014 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_fa972d61f811bd58_test_flip_flop_py.html
--rw-r--r--   0        0        0   119047 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_fa972d61f811bd58_test_isoreg_py.html
--rw-r--r--   0        0        0   182217 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_fa972d61f811bd58_test_murphy_py.html
--rw-r--r--   0        0        0    44829 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_fa972d61f811bd58_test_quantile_loss_py.html
--rw-r--r--   0        0        0   204069 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_fa972d61f811bd58_test_standard_py.html
--rw-r--r--   0        0        0     7274 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_fe94c6366a0da9bc___init___py.html
--rw-r--r--   0        0        0    21762 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_fe94c6366a0da9bc_functions_py.html
--rw-r--r--   0        0        0    95641 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_fe94c6366a0da9bc_processing_py.html
--rw-r--r--   0        0        0    43505 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_fe94c6366a0da9bc_sample_data_py.html
--rw-r--r--   0        0        0    10098 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_fe94c6366a0da9bc_typing_py.html
--rw-r--r--   0        0        0    95582 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/d_fe94c6366a0da9bc_utils_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/favicon_32.png
--rw-r--r--   0        0        0    26225 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/keybd_open.png
--rw-r--r--   0        0        0    13704 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 scores-0.6/htmlcov/style.css
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 scores-0.6/src/scores/__init__.py
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 scores-0.6/src/scores/functions.py
--rw-r--r--   0        0        0    15335 2020-02-02 00:00:00.000000 scores-0.6/src/scores/processing.py
--rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 scores-0.6/src/scores/sample_data.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 scores-0.6/src/scores/typing.py
--rw-r--r--   0        0        0    14729 2020-02-02 00:00:00.000000 scores-0.6/src/scores/utils.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 scores-0.6/src/scores/categorical/__init__.py
--rw-r--r--   0        0        0     6602 2020-02-02 00:00:00.000000 scores-0.6/src/scores/categorical/binary_impl.py
--rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 scores-0.6/src/scores/categorical/multicategorical_impl.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 scores-0.6/src/scores/continuous/__init__.py
--rw-r--r--   0        0        0    17943 2020-02-02 00:00:00.000000 scores-0.6/src/scores/continuous/flip_flop_impl.py
--rw-r--r--   0        0        0    28478 2020-02-02 00:00:00.000000 scores-0.6/src/scores/continuous/isoreg_impl.py
--rw-r--r--   0        0        0    12424 2020-02-02 00:00:00.000000 scores-0.6/src/scores/continuous/murphy_impl.py
--rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 scores-0.6/src/scores/continuous/quantile_loss_impl.py
--rw-r--r--   0        0        0     9974 2020-02-02 00:00:00.000000 scores-0.6/src/scores/continuous/standard_impl.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 scores-0.6/src/scores/pandas/__init__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 scores-0.6/src/scores/pandas/continuous.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 scores-0.6/src/scores/pandas/typing.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 scores-0.6/src/scores/probability/__init__.py
--rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 scores-0.6/src/scores/probability/brier_impl.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 scores-0.6/src/scores/probability/checks.py
--rw-r--r--   0        0        0    36685 2020-02-02 00:00:00.000000 scores-0.6/src/scores/probability/crps_impl.py
--rw-r--r--   0        0        0    16016 2020-02-02 00:00:00.000000 scores-0.6/src/scores/probability/functions.py
--rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 scores-0.6/src/scores/probability/roc_impl.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 scores-0.6/src/scores/stats/__init__.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scores-0.6/src/scores/stats/statistical_tests/__init__.py
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 scores-0.6/src/scores/stats/statistical_tests/acovf.py
--rw-r--r--   0        0        0    17455 2020-02-02 00:00:00.000000 scores-0.6/src/scores/stats/statistical_tests/diebold_mariano_impl.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 scores-0.6/.gitignore
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 scores-0.6/LICENSE
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 scores-0.6/README.md
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 scores-0.6/pyproject.toml
--rw-r--r--   0        0        0     7340 2020-02-02 00:00:00.000000 scores-0.6/PKG-INFO
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 scores-0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 scores-0.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 scores-0.7/environment.yml
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scores-0.7/mkdocs.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.7/py.typed
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scores-0.7/readthedocs.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.7/setup.cfg
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 scores-0.7/.binder/postBuild
+-rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 scores-0.7/.binder/requirements.txt
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scores-0.7/.github/pull_request_template.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 scores-0.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 scores-0.7/.github/ISSUE_TEMPLATE/new_score.md
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scores-0.7/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 scores-0.7/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 scores-0.7/.github/workflows/run-pre-commit.yml
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 scores-0.7/src/scores/__init__.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 scores-0.7/src/scores/functions.py
+-rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 scores-0.7/src/scores/sample_data.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 scores-0.7/src/scores/typing.py
+-rw-r--r--   0        0        0    15729 2020-02-02 00:00:00.000000 scores-0.7/src/scores/utils.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 scores-0.7/src/scores/categorical/__init__.py
+-rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 scores-0.7/src/scores/categorical/binary_impl.py
+-rw-r--r--   0        0        0    14019 2020-02-02 00:00:00.000000 scores-0.7/src/scores/categorical/contingency_impl.py
+-rw-r--r--   0        0        0    11009 2020-02-02 00:00:00.000000 scores-0.7/src/scores/categorical/multicategorical_impl.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 scores-0.7/src/scores/continuous/__init__.py
+-rw-r--r--   0        0        0    18015 2020-02-02 00:00:00.000000 scores-0.7/src/scores/continuous/flip_flop_impl.py
+-rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 scores-0.7/src/scores/continuous/murphy_impl.py
+-rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 scores-0.7/src/scores/continuous/quantile_loss_impl.py
+-rw-r--r--   0        0        0    16768 2020-02-02 00:00:00.000000 scores-0.7/src/scores/continuous/standard_impl.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 scores-0.7/src/scores/pandas/__init__.py
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 scores-0.7/src/scores/pandas/continuous.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 scores-0.7/src/scores/pandas/typing.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 scores-0.7/src/scores/probability/__init__.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 scores-0.7/src/scores/probability/brier_impl.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 scores-0.7/src/scores/probability/checks.py
+-rw-r--r--   0        0        0    37852 2020-02-02 00:00:00.000000 scores-0.7/src/scores/probability/crps_impl.py
+-rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 scores-0.7/src/scores/probability/roc_impl.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 scores-0.7/src/scores/processing/__init__.py
+-rw-r--r--   0        0        0    12458 2020-02-02 00:00:00.000000 scores-0.7/src/scores/processing/discretise.py
+-rw-r--r--   0        0        0    29482 2020-02-02 00:00:00.000000 scores-0.7/src/scores/processing/isoreg_impl.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 scores-0.7/src/scores/processing/matching.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 scores-0.7/src/scores/processing/cdf/__init__.py
+-rw-r--r--   0        0        0    16430 2020-02-02 00:00:00.000000 scores-0.7/src/scores/processing/cdf/cdf_functions.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 scores-0.7/src/scores/stats/__init__.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scores-0.7/src/scores/stats/statistical_tests/__init__.py
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 scores-0.7/src/scores/stats/statistical_tests/acovf.py
+-rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 scores-0.7/src/scores/stats/statistical_tests/diebold_mariano_impl.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 scores-0.7/.gitignore
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 scores-0.7/LICENSE
+-rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 scores-0.7/README.md
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 scores-0.7/pyproject.toml
+-rw-r--r--   0        0        0     8856 2020-02-02 00:00:00.000000 scores-0.7/PKG-INFO
```

### Comparing `scores-0.6/.pre-commit-config.yaml` & `scores-0.7/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 ---
 repos:
-- repo: https://github.com/psf/black
-  rev: 23.3.0
-  hooks:
-    - id: black
-      name: black
-      entry: black --check
-# use local version of package with core deps to avoid import-errors from virtual env
-- repo: local
-  hooks:
-    - id: pylint
-      name: pylint
-      entry: pylint --reports=n
-      language: system
-      types: [python]
-      stages: [pre-commit]
-- repo: https://github.com/PyCQA/isort
-  rev: 5.11.5
-  hooks:
-    - id: isort
-      entry: isort --profile=black
-- repo: https://github.com/pre-commit/mirrors-mypy
-  rev: v1.3.0
-  hooks:
-    - id: mypy
-- repo: local
-  hooks:
-    - id: pytest
-      name: pytest
-      entry: pytest tests/ --cov=src/scores --cov-report term-missing
-      language: system
-      stages: [push]
-      always_run: true
-      pass_filenames: false
+  - repo: https://github.com/psf/black
+    rev: 23.3.0
+    hooks:
+      - id: black
+        name: black
+        entry: black --check
+  - repo: https://github.com/PyCQA/bandit
+    rev: 1.7.8
+    hooks:
+      - id: bandit
+        args: [--skip, "B101", --recursive, src/scores]
+  # use local version of package with core deps to avoid import-errors from virtual env
+  - repo: local
+    hooks:
+      - id: pylint
+        name: pylint
+        entry: pylint --reports=n
+        language: system
+        types: [python]
+        stages: [pre-commit]
+  - repo: https://github.com/PyCQA/isort
+    rev: 5.11.5
+    hooks:
+      - id: isort
+        entry: isort --profile=black
+  - repo: https://github.com/pre-commit/mirrors-mypy
+    rev: v1.3.0
+    hooks:
+      - id: mypy
+  - repo: local
+    hooks:
+      - id: pytest
+        name: pytest
+        entry: pytest tests/ --cov=src/scores --cov-report term-missing
+        language: system
+        stages: [push]
+        always_run: true
+        pass_filenames: false
```

### Comparing `scores-0.6/CODE_OF_CONDUCT.md` & `scores-0.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scores-0.6/readthedocs.yaml` & `scores-0.7/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `scores-0.6/.binder/requirements.txt` & `scores-0.7/.binder/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     # via scores (pyproject.toml)
 h5py==3.10.0
     # via h5netcdf
 httpcore==1.0.5
     # via httpx
 httpx==0.27.0
     # via jupyterlab
-idna==3.6
+idna==3.7
     # via
     #   anyio
     #   httpx
     #   jsonschema
     #   requests
 importlib-metadata==7.1.0
     # via
@@ -106,15 +106,15 @@
     # via jupyterlab
 ipython==8.18.1
     # via ipykernel
 isoduration==20.11.0
     # via jsonschema
 jedi==0.19.1
     # via ipython
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   jupyter-server
     #   jupyterlab
     #   jupyterlab-server
     #   nbconvert
 joblib==1.3.2
     # via scikit-learn
```

### Comparing `scores-0.6/.github/pull_request_template.md` & `scores-0.7/.github/ISSUE_TEMPLATE/new_score.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,22 @@
+---
+name: New Score or Metric
+about: Suggest a new score or metric which could be added to the repository
+title: ''
+labels: ''
+assignees: ''
+
+---
+
 A new score or metric should be developed on a separate feature branch, rebased against the main branch. Each merge request should include:
 
     The implementation of the new metric or score in xarray, ideally with support for pandas and dask
     100% unit test coverage
     A tutorial notebook showcasing the use of that metric or score, ideally based on the standard sample data
     API documentation (docstrings) using Napoleon (google) style, making sure to clearly explain the use of the metrics
     A reference to the paper which described the metrics, added to the API documentation
     For metrics which do not have a paper reference, an online source or reference should be provided
     For metrics which are still under development or which have not yet had an academic publication, they will be placed in a holding area within the API until the method has been properly published and peer reviewed (i.e. scores.emerging). The 'emerging' area of the API is subject to rapid change, still of sufficient community interest to include, similar to a 'preprint' of a score or metric.
-    Add your score to summary_table_of_scores.md in the documentation
 
 All merge requests should comply with the coding standards outlined in this document. Merge requests will undergo both a code review and a science review. The code review will focus on coding style, performance and test coverage. The science review will focus on the mathematical correctness of the implementation and the suitability of the method for inclusion within 'scores'.
 
 A github ticket should be created explaining the metric which is being implemented and why it is useful.
```

### Comparing `scores-0.6/.github/ISSUE_TEMPLATE/feature_request.md` & `scores-0.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `scores-0.6/.github/ISSUE_TEMPLATE/new_score.md` & `scores-0.7/.github/pull_request_template.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,13 @@
----
-name: New Score or Metric
-about: Suggest a new score or metric which could be added to the repository
-title: ''
-labels: ''
-assignees: ''
-
----
-
 A new score or metric should be developed on a separate feature branch, rebased against the main branch. Each merge request should include:
 
     The implementation of the new metric or score in xarray, ideally with support for pandas and dask
     100% unit test coverage
     A tutorial notebook showcasing the use of that metric or score, ideally based on the standard sample data
     API documentation (docstrings) using Napoleon (google) style, making sure to clearly explain the use of the metrics
     A reference to the paper which described the metrics, added to the API documentation
     For metrics which do not have a paper reference, an online source or reference should be provided
     For metrics which are still under development or which have not yet had an academic publication, they will be placed in a holding area within the API until the method has been properly published and peer reviewed (i.e. scores.emerging). The 'emerging' area of the API is subject to rapid change, still of sufficient community interest to include, similar to a 'preprint' of a score or metric.
-    Add your score to summary_table_of_scores.md in the documentation
 
 All merge requests should comply with the coding standards outlined in this document. Merge requests will undergo both a code review and a science review. The code review will focus on coding style, performance and test coverage. The science review will focus on the mathematical correctness of the implementation and the suitability of the method for inclusion within 'scores'.
 
 A github ticket should be created explaining the metric which is being implemented and why it is useful.
```

### Comparing `scores-0.6/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md` & `scores-0.7/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,12 +3,11 @@
     The implementation of the new metric or score in xarray, ideally with support for pandas and dask
     100% unit test coverage
     A tutorial notebook showcasing the use of that metric or score, ideally based on the standard sample data
     API documentation (docstrings) using Napoleon (google) style, making sure to clearly explain the use of the metrics
     A reference to the paper which described the metrics, added to the API documentation
     For metrics which do not have a paper reference, an online source or reference should be provided
     For metrics which are still under development or which have not yet had an academic publication, they will be placed in a holding area within the API until the method has been properly published and peer reviewed (i.e. scores.emerging). The 'emerging' area of the API is subject to rapid change, still of sufficient community interest to include, similar to a 'preprint' of a score or metric.
-    Add your score to summary_table_of_scores.md in the documentation
 
 All merge requests should comply with the coding standards outlined in this document. Merge requests will undergo both a code review and a science review. The code review will focus on coding style, performance and test coverage. The science review will focus on the mathematical correctness of the implementation and the suitability of the method for inclusion within 'scores'.
 
 A github ticket should be created explaining the metric which is being implemented and why it is useful.
```

### Comparing `scores-0.6/.github/workflows/python-app.yml` & `scores-0.7/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `scores-0.6/.github/workflows/run-pre-commit.yml` & `scores-0.7/.github/workflows/run-pre-commit.yml`

 * *Files identical despite different names*

### Comparing `scores-0.6/src/scores/__init__.py` & `scores-0.7/src/scores/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """
 The philosphy is to import the public API during the init phase rather than leaving it to the user
 """
+
 # pylint: disable=E0603
 
 import scores.categorical
 import scores.continuous
 import scores.functions
 import scores.pandas
 import scores.probability
+import scores.processing
 import scores.sample_data
 import scores.stats.statistical_tests  # noqa: F401
 
-__version__ = "v0.6"
+__version__ = "v0.7"
 
 __all__ = [
     "scores.categorical",
+    "scores.contingency",
     "scores.continuous",
     "scores.functions",
     "scores.pandas",
     "scores.probability",
+    "scores.processing",
     "scores.sample_data",
     "scores.stats.statistical_tests",
 ]
```

### Comparing `scores-0.6/src/scores/functions.py` & `scores-0.7/src/scores/functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Contains functions which transform data or perform calculations
 """
-from typing import overload
+from typing import Optional, overload
 
 import numpy as np
 import xarray as xr
 
 from scores.typing import XarrayLike
 
 
-def apply_weights(values, weights=None):
+def apply_weights(values, *, weights: Optional[XarrayLike] = None):
     """
     Returns:
         A new array with the elements of values multiplied by the specified weights.
 
     Args:
         - weights: The weightings to be used at every location in the values array. If weights contains additional
         dimensions, these will be taken to mean that multiple weightings are wanted simultaneoulsy, and these
@@ -72,9 +72,9 @@
         source_a: direction data in degrees, first source
         source_b: direction data in degrees, second source
 
     Returns:
         An array containing angles within the range [0, 180].
     """
     difference = np.abs(source_a - source_b) % 360
-    difference = difference.where(difference <= 180, 360 - difference)
-    return difference
+    difference = difference.where(difference <= 180, 360 - difference)  # type: ignore
+    return difference  # type: ignore
```

### Comparing `scores-0.6/src/scores/processing.py` & `scores-0.7/src/scores/processing/discretise.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Tools for processing data for verification"""
+"""Tools for discretising data for verification"""
 
 import operator
 from collections.abc import Iterable
 from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
@@ -18,47 +18,24 @@
     "<": (operator.lt, -1),
 }
 # '==' does not map to `operater.eq` and '!=' does not map to operator.ne on purpose.
 # This is because we wish to test within a tolerance.
 EQUALITY_MODES = {"==": (operator.le), "!=": (operator.gt)}
 
 
-def check_binary(data: XarrayLike, name: str):
-    """
-    Checks that data does not have any non-NaN values out of the set {0, 1}
-
-    Args:
-        data: The data to convert to check if only contains binary values
-    Raises:
-        ValueError: if there are values in `fcst` and `obs` that are not in the
-            set {0, 1, np.nan} and `check_args` is true.
-    """
-    if isinstance(data, xr.DataArray):
-        unique_values = pd.unique(data.values.flatten())
-    else:
-        unique_values = pd.unique(data.to_array().values.flatten())
-    unique_values = unique_values[~np.isnan(unique_values)]
-    binary_set = {0, 1}
-
-    if not set(unique_values).issubset(binary_set):
-        raise ValueError(f"`{name}` contains values that are not in the set {{0, 1, np.nan}}")
-
-
 def comparative_discretise(
-    data: XarrayLike, comparison: Union[xr.DataArray, float, int], mode: str, abs_tolerance: Optional[float] = None
+    data: XarrayLike, comparison: Union[xr.DataArray, float, int], mode: str, *, abs_tolerance: Optional[float] = None
 ) -> XarrayLike:
     """
     Converts the values of `data` to 0 or 1 based on how they relate to the specified
     values in `comparison` via the `mode` operator.
 
     Args:
-        data: The data to convert to
-            discrete values.
-        comparison: The values to which
-            to compare `data`.
+        data: The data to convert to discrete values.
+        comparison: The values to which to compare `data`.
         mode: Specifies the required relation of `data` to `thresholds`
             for a value to fall in the 'event' category (i.e. assigned to 1).
             Allowed modes are:
             - '>=' values in `data` greater than or equal to the
             corresponding threshold are assigned as 1.
             - '>' values in `data` greater than the corresponding threshold
             are assigned as 1.
@@ -111,33 +88,32 @@
         raise ValueError(
             f"'{mode}' is not a valid mode. Available modes are: "
             f"{sorted(INEQUALITY_MODES) + sorted(EQUALITY_MODES)}"
         )
     discrete_data.attrs["discretisation_tolerance"] = abs_tolerance
     discrete_data.attrs["discretisation_mode"] = mode
 
-    return discrete_data
+    return discrete_data  # type: ignore
 
 
 def binary_discretise(
     data: XarrayLike,
-    thresholds: FlexibleDimensionTypes,
+    thresholds: Optional[FlexibleDimensionTypes],
     mode: str,
+    *,  # Force keywords arguments to be keyword-only
     abs_tolerance: Optional[float] = None,
     autosqueeze: Optional[bool] = False,
 ):
     """
     Converts the values of `data` to 0 or 1 for each threshold in `thresholds`
     according to the operation defined by `mode`.
 
     Args:
-        data: The data to convert to
-            discrete values.
-        thresholds: Threshold(s) at which to convert the
-            values of `data` to 0 or 1.
+        data: The data to convert to discrete values.
+        thresholds: Threshold(s) at which to convert the values of `data` to 0 or 1.
         mode: Specifies the required relation of `data` to `thresholds`
             for a value to fall in the 'event' category (i.e. assigned to 1).
             Allowed modes are:
 
             - '>=' values in `data` greater than or equal to the
             corresponding threshold are assigned as 1.
             - '>' values in `data` greater than the corresponding threshold
@@ -166,29 +142,29 @@
         An xarray data object with the type and dimensions of `data`, plus an
         extra dimension 'threshold' if `autosqueeze` is False. The values of
         the output are either 0 or 1, depending on whether `data <mode> threshold`
         is True or not (although NaNs are preserved).
 
     Raises:
         ValueError: if 'threshold' is a dimension in `data`.
-        ValueError: if "Values in `thresholds` are not montonic increasing"
+        ValueError: if "Values in `thresholds` are not monotonic increasing"
     """
     if "threshold" in data.dims:
         raise ValueError("'threshold' must not be in the supplied data object dimensions")
 
     # if thresholds is 0-D, convert it to a length-1 1-D array
     # but autosqueeze=True so the 'threshold' dimension is dropped
     thresholds_np = np.array(thresholds)
     if thresholds_np.ndim == 0:
         thresholds_np = np.expand_dims(thresholds_np, 0)
         autosqueeze = True
 
     # sanitise thresholds
     if not (thresholds_np[1:] - thresholds_np[:-1] >= 0).all():
-        raise ValueError("Values in `thresholds` are not montonic increasing")
+        raise ValueError("Values in `thresholds` are not monotonic increasing")
 
     # make thresholds DataArray
     thresholds_da = xr.DataArray(thresholds_np, dims=["threshold"], coords={"threshold": thresholds_np})
 
     # do the discretisation
     discrete_data = comparative_discretise(data, thresholds_da, mode, abs_tolerance=abs_tolerance)
 
@@ -196,84 +172,20 @@
     if autosqueeze and len(thresholds_np) == 1:
         # squeeze out the 'threshold' dimension, but keep the coordinate
         discrete_data = discrete_data.squeeze(dim="threshold")
 
     return discrete_data
 
 
-def broadcast_and_match_nan(*args: XarrayLike) -> tuple[XarrayLike, ...]:
-    """
-    Input xarray data objects are 'matched' - they are broadcast against each
-    other (forced to have the same dimensions), and the position of nans are
-    forced onto all DataArrays. This matching process is applied across all
-    supplied DataArrays, as well as all DataArrays inside supplied Datasets.
-
-    Args:
-        *args: any number of xarray data objects supplied as positional arguments. See
-            examples below.
-
-    Returns:
-        A tuple of data objects of the same length as the number of data objects
-        supplied as input. Each returned object is the 'matched' version of the
-        input.
-
-    Raises:
-        ValueError: if any input args is not an xarray data
-            object.
-
-    Examples:
-
-        >>> # Matching xarray data objects
-        >>> da1_matched, ds_matched, da2_matched = xrtools.broadcast_and_match_nan(da1, ds, da2)
-
-        >>> # Matching a tuple of xarray data objects
-        >>> input_tuple = (da1, ds, da2)
-        >>> matched_tuple = broadcast_and_match_nan(*input_tuple)
-        >>> da1_matched = matched_tuple[0]
-        >>> ds_matched = matched_tuple[1]
-        >>> da2_matched = matched_tuple[2]
-    """
-
-    # sanitise inputs
-    for i, arg in enumerate(args):
-        if not isinstance(arg, (xr.Dataset, xr.DataArray)):
-            raise ValueError(
-                f"Argument {i} is not an xarray data object. (counting from 0, i.e. "
-                "argument 0 is the first argument)"
-            )
-
-    # internal function to update the mask
-    def update_mask(mask, data_array):
-        """
-        Perform the boolean AND operation on a mask (DataArray) and
-        data_array.notnull()
-        """
-        return mask & data_array.notnull()
-
-    # initialise the mask
-    mask = True
-    # generate the mask
-    for arg in args:
-        # update the mask for a DataArray
-        if isinstance(arg, xr.DataArray):
-            mask = update_mask(mask, arg)
-        # update the mask for Datasets
-        elif isinstance(arg, xr.Dataset):
-            for data_var in arg.data_vars:
-                mask = update_mask(mask, arg[data_var])
-
-    # return matched data objects
-    return tuple(arg.where(mask) for arg in args)
-
-
 def proportion_exceeding(
     data: XarrayLike,
     thresholds: Iterable,
-    reduce_dims: FlexibleDimensionTypes = None,
-    preserve_dims: FlexibleDimensionTypes = None,
+    *,  # Force keywords arguments to be keyword-only
+    reduce_dims: Optional[FlexibleDimensionTypes] = None,
+    preserve_dims: Optional[FlexibleDimensionTypes] = None,
 ):
     """
     Calculates the proportion of `data` equal to or exceeding `thresholds`.
 
     Args:
         data (xarray.Dataset or xarray.DataArray): The data from which
             to calculate the proportion exceeding `thresholds`
@@ -285,23 +197,24 @@
 
     Returns:
         An xarray data object with the type of `data` and dimensions
         `dims` + 'threshold'. The values are the proportion of `data`
         that are greater than or equal to the corresponding threshold.
 
     """
-    return _binary_discretise_proportion(data, thresholds, ">=", reduce_dims=reduce_dims, preserve_dims=preserve_dims)
+    return binary_discretise_proportion(data, thresholds, ">=", reduce_dims=reduce_dims, preserve_dims=preserve_dims)
 
 
-def _binary_discretise_proportion(
+def binary_discretise_proportion(
     data: XarrayLike,
     thresholds: Iterable,
     mode: str,
-    reduce_dims: FlexibleDimensionTypes = None,
-    preserve_dims: FlexibleDimensionTypes = None,
+    *,  # Force keywords arguments to be keyword-only
+    reduce_dims: Optional[FlexibleDimensionTypes] = None,
+    preserve_dims: Optional[FlexibleDimensionTypes] = None,
     abs_tolerance: Optional[bool] = None,
     autosqueeze: bool = False,
 ):
     """
     Returns the proportion of `data` in each category. The categories are
     defined by the relationship of data to threshold as specified by
     the operation `mode`.
```

### Comparing `scores-0.6/src/scores/sample_data.py` & `scores-0.7/src/scores/sample_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 """
 Module to generate simple sample data for users (not tests). Supports tutorials and demos.
 """
 
 import numpy as np
 import pandas as pd
 import xarray as xr
-from scipy.stats import skewnorm
+from scipy.stats import skewnorm  # type: ignore
 
 
 def simple_forecast() -> xr.DataArray:
     """Generate a simple series of prediction values"""
     return xr.DataArray(data=[10, 10, 11, 13, 14, 17, 15, 14])
 
 
 def simple_observations() -> xr.DataArray:
     """Generate a simple series of observation values"""
     return xr.DataArray(data=[11, 11, 12, 14, 11, 14, 12, 11])
 
 
-def continuous_observations(large_size: bool = False) -> xr.DataArray:
+def simple_forecast_pandas() -> pd.Series:
+    """Generate a simple series of prediction values"""
+    return pd.Series([10, 10, 11, 13, 14, 17, 15, 14])
+
+
+def simple_observations_pandas() -> pd.Series:
+    """Generate a simple series of observation values"""
+    return pd.Series([11, 11, 12, 14, 11, 14, 12, 11])
+
+
+def continuous_observations(*, large_size: bool = False) -> xr.DataArray:
     """Creates a obs array with continuous values.
 
     Args:
         large_size (bool): If True, then returns a large global array with ~0.5 degree
             grid spacing, otherwise returns a cut down, lower resolution array.
 
     Returns:
@@ -49,36 +59,36 @@
     np.random.seed(42)
     data = 10 * np.random.rand(len(lat), len(lon), len(time_series))
     obs = xr.DataArray(coords={"lat": lat, "lon": lon, "time": time_series}, data=data)
 
     return obs
 
 
-def continuous_forecast(large_size: bool = False, lead_days: bool = False) -> xr.DataArray:
+def continuous_forecast(*, large_size: bool = False, lead_days: bool = False) -> xr.DataArray:
     """Creates a forecast array with continuous values.
 
     Args:
         large_size (bool): If True, then returns a large global array with ~0.5 degree
             grid spacing, otherwise returns a cut down, lower resolution array.
         lead_days (bool): If True, returns an array with a "lead_day" dimension.
 
     Returns:
         xr.Datarray: Containing synthetic forecast data.
     """
-    obs = continuous_observations(large_size)
+    obs = continuous_observations(large_size=large_size)
     np.random.seed(42)
     forecast = obs + np.random.normal(0, 2, obs.shape)
     if lead_days:
         forecast2 = obs + np.random.normal(0, 3, obs.shape)
         forecast = xr.concat([forecast, forecast2], dim="lead_time")
         forecast = forecast.assign_coords(lead_time=[1, 2])
     return forecast
 
 
-def cdf_forecast(lead_days: bool = False) -> xr.DataArray:
+def cdf_forecast(*, lead_days: bool = False) -> xr.DataArray:
     """
     Creates a forecast array with a CDF at each point.
 
     Args:
         lead_days (bool): If True, returns an array with a "lead_day" dimension.
 
     Returns:
```

### Comparing `scores-0.6/src/scores/typing.py` & `scores-0.7/src/scores/typing.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 This module contains various compound or union types which can be used across the codebase to ensure
 a consistent approach to typing is handled.
 """
 from collections.abc import Hashable, Iterable
-from typing import Optional, Union
+from typing import Union
 
 import pandas as pd
 import xarray as xr
 
 # Flexible Dimension Types should be used for preserve_dims and reduce_dims in all
 # cases across the repository
-FlexibleDimensionTypes = Optional[Iterable[Hashable]]
+FlexibleDimensionTypes = Iterable[Hashable]
 
 # Xarraylike data types should be used for all forecast, observed and weights
 # However currently some are specified as DataArray only
 XarrayLike = Union[xr.DataArray, xr.Dataset]
 
 # These type hint values *may* be used for various arguments across the
 # scores repository but are not establishing a standard or expectation beyond
```

### Comparing `scores-0.6/src/scores/utils.py` & `scores-0.7/src/scores/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """
 Contains frequently-used functions of a general nature within scores
 """
+
 import warnings
 from collections.abc import Hashable, Iterable, Sequence
 from typing import Optional, Union
 
+import numpy as np
+import pandas as pd
 import xarray as xr
 
 from scores.typing import FlexibleDimensionTypes, XarrayLike
 
 WARN_ALL_DATA_CONFLICT_MSG = """
 You are requesting to reduce or preserve every dimension by specifying the string 'all'.
 In this case, 'all' is also a named dimension in your data, leading to an ambiguity.
@@ -52,16 +55,16 @@
     """
 
 
 def gather_dimensions(  # pylint: disable=too-many-branches
     fcst_dims: Iterable[Hashable],
     obs_dims: Iterable[Hashable],
     *,  # Force keywords arguments to be keyword-only
-    reduce_dims: FlexibleDimensionTypes = None,
-    preserve_dims: FlexibleDimensionTypes = None,
+    reduce_dims: Optional[FlexibleDimensionTypes] = None,
+    preserve_dims: Optional[FlexibleDimensionTypes] = None,
 ) -> set[Hashable]:
     """
     Establish which dimensions to reduce when calculating errors but before taking means.
 
     Note: `scores.utils.gather_dimensions` and `scores.utils.gather_dimensions2` will be
     integrated at some point in the future. `scores.utils.gather_dimensions2` offers
     more comprehensive and less restrictive dimension checking and should be preferred in
@@ -122,29 +125,29 @@
         reduce_dims = set(all_dims)
 
     # Handle reduce by string
     elif isinstance(reduce_dims, str):
         reduce_dims = set([reduce_dims])
 
     # Turn into a set if needed
-    assert reduce_dims is not None
+    assert reduce_dims is not None  # nosec - this is just to modify type hinting
     reduce_dims = set(reduce_dims)
 
     # Reduce by list is the default so no handling needed
     return reduce_dims
 
 
 def gather_dimensions2(  # pylint: disable=too-many-branches
     fcst: xr.DataArray,
     obs: xr.DataArray,
     *,  # Force keywords arguments to be keyword-only
-    weights: xr.DataArray = None,
-    reduce_dims: FlexibleDimensionTypes = None,
-    preserve_dims: FlexibleDimensionTypes = None,
-    special_fcst_dims: FlexibleDimensionTypes = None,
+    weights: Optional[xr.DataArray] = None,
+    reduce_dims: Optional[FlexibleDimensionTypes] = None,
+    preserve_dims: Optional[FlexibleDimensionTypes] = None,
+    special_fcst_dims: Optional[FlexibleDimensionTypes] = None,
 ) -> set[Hashable]:
     """
     Performs standard dimensions checks for inputs of functions that calculate (mean) scores.
     Returns a set of the dimensions to reduce.
 
     Note: `scores.utils.gather_dimensions` and `scores.utils.gather_dimensions2` will be
     integrated at some point in the future. `scores.utils.gather_dimensions2` offers
@@ -228,15 +231,15 @@
             return all_scoring_dims
         return set(specified_dims)
     if preserve_dims == "all":
         return set([])
     return all_scoring_dims.difference(set(specified_dims))
 
 
-def dims_complement(data, dims=None) -> list[str]:
+def dims_complement(data, *, dims=None) -> list[str]:
     """Returns the complement of data.dims and dims
 
     Args:
         data: Input xarray object
         dims: an Iterable of strings corresponding to dimension names
 
     Returns:
@@ -249,15 +252,15 @@
     # check that dims is in data.dims, and that dims is a of a valid form
     check_dims(data, dims, mode="superset")
 
     complement = set(data.dims) - set(dims)
     return sorted(list(complement))
 
 
-def check_dims(xr_data: XarrayLike, expected_dims: Sequence[str], mode: Optional[str] = None):
+def check_dims(xr_data: XarrayLike, expected_dims: Iterable[Hashable], *, mode: Optional[str] = None):
     """
     Checks the dimensions xr_data with expected_dims, according to `mode`.
 
     Args:
         xr_data: if a Dataset is supplied,
             all of its data variables (DataArray objects) are checked.
         expected_dims: an Iterable of dimension names.
@@ -293,15 +296,15 @@
     try:
         dims_set = set(expected_dims)
     except Exception as exc:
         raise ValueError(
             f"Cannot convert supplied dims {expected_dims} into a set. Check debug log for more information."
         ) from exc
 
-    if len(dims_set) != len(expected_dims):
+    if len(list(dims_set)) != len(list(expected_dims)):
         raise ValueError(f"Supplied dimensions {expected_dims} contains duplicate values.")
 
     if not hasattr(xr_data, "dims"):
         raise DimensionError("Supplied object has no dimensions")
 
     # internal functions to check a data array
     check_modes = {
@@ -320,42 +323,63 @@
 
     check_fn = check_modes[mode]
 
     # check the dims
     if not check_fn(xr_data, dims_set):
         raise DimensionError(
             f"Dimensions {list(xr_data.dims)} of data object are not {mode} to the "
-            f"dimensions {sorted(list(dims_set))}."
+            f"dimensions {sorted([str(d) for d in dims_set])}."
         )
 
     if isinstance(xr_data, xr.Dataset):
         # every data variable must pass the dims check too!
         for data_var in xr_data.data_vars:
             if not check_fn(xr_data[data_var], dims_set):
                 raise DimensionError(
                     f"Dimensions {list(xr_data[data_var].dims)} of data variable "
-                    f"'{data_var}' are not {mode} to the dimensions {sorted(dims_set)}"
+                    f"'{data_var}' are not {mode} to the dimensions {sorted([str(d) for d in dims_set])}"
                 )
 
 
-def tmp_coord_name(xr_data: xr.DataArray, count=1) -> Union[str, list[str]]:
+def tmp_coord_name(xr_data: xr.DataArray, *, count=1) -> Union[str, list[str]]:
     """
     Generates temporary coordinate names that are not among the coordinate or dimension
     names of `xr_data`.
 
     Args:
         xr_data: Input xarray data array
         count: Number of unique names to generate
 
     Returns:
         If count = 1, a string which is the concatenation of 'new' with all coordinate and
         dimension names in the input array. (this is the default)
         If count > 1, a list of such strings, each unique from one another
     """
     all_names = ["new"] + list(xr_data.dims) + list(xr_data.coords)
-    result = "".join(all_names)
+    result = "".join(all_names)  # type: ignore
 
     if count == 1:
         return result
 
     results = [str(i) + result for i in range(count)]
     return results
+
+
+def check_binary(data: XarrayLike, name: str):
+    """
+    Checks that data does not have any non-NaN values out of the set {0, 1}
+
+    Args:
+        data: The data to convert to check if only contains binary values
+    Raises:
+        ValueError: if there are values in `fcst` and `obs` that are not in the
+            set {0, 1, np.nan} and `check_args` is true.
+    """
+    if isinstance(data, xr.DataArray):
+        unique_values = pd.unique(data.values.flatten())
+    else:
+        unique_values = pd.unique(data.to_array().values.flatten())
+    unique_values = unique_values[~np.isnan(unique_values)]
+    binary_set = {0, 1}
+
+    if not set(unique_values).issubset(binary_set):
+        raise ValueError(f"`{name}` contains values that are not in the set {{0, 1, np.nan}}")
```

### Comparing `scores-0.6/src/scores/categorical/binary_impl.py` & `scores-0.7/src/scores/categorical/binary_impl.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 This module contains methods for binary categories
 """
+
 from typing import Optional
 
 import numpy as np
 import xarray as xr
 
 from scores.functions import apply_weights
-from scores.processing import check_binary
 from scores.typing import FlexibleDimensionTypes, XarrayLike
-from scores.utils import gather_dimensions
+from scores.utils import check_binary, gather_dimensions
 
 
 def probability_of_detection(
     fcst: XarrayLike,
     obs: XarrayLike,
     *,  # Force keywords arguments to be keyword-only
-    reduce_dims: FlexibleDimensionTypes = None,
-    preserve_dims: FlexibleDimensionTypes = None,
+    reduce_dims: Optional[FlexibleDimensionTypes] = None,
+    preserve_dims: Optional[FlexibleDimensionTypes] = None,
     weights: Optional[xr.DataArray] = None,
     check_args: Optional[bool] = True,
 ) -> XarrayLike:
     """
     Calculates the Probability of Detection (POD), also known as the Hit Rate.
     This is the proportion of observed events (obs = 1) that were correctly
     forecast as an event (fcst = 1).
@@ -66,30 +66,30 @@
     misses = (obs == 1) & (fcst == 0)
     hits = (obs == 1) & (fcst == 1)
 
     # preserve NaNs
     misses = misses.where((~np.isnan(fcst)) & (~np.isnan(obs)))
     hits = hits.where((~np.isnan(fcst)) & (~np.isnan(obs)))
 
-    misses = apply_weights(misses, weights)
-    hits = apply_weights(hits, weights)
+    misses = apply_weights(misses, weights=weights)
+    hits = apply_weights(hits, weights=weights)
 
     misses = misses.sum(dim=dims_to_sum)
     hits = hits.sum(dim=dims_to_sum)
 
     pod = hits / (hits + misses)
     return pod
 
 
 def probability_of_false_detection(
     fcst: XarrayLike,
     obs: XarrayLike,
     *,  # Force keywords arguments to be keyword-only
-    reduce_dims: FlexibleDimensionTypes = None,
-    preserve_dims: FlexibleDimensionTypes = None,
+    reduce_dims: Optional[FlexibleDimensionTypes] = None,
+    preserve_dims: Optional[FlexibleDimensionTypes] = None,
     weights: Optional[xr.DataArray] = None,
     check_args: Optional[bool] = True,
 ) -> XarrayLike:
     """
     Calculates the Probability of False Detection (POFD), also known as False
     Alarm Rate (not to be confused with the False Alarm Ratio). The POFD is
     the proportion of observed non-events (obs = 0) that were incorrectly
@@ -134,15 +134,15 @@
     false_alarms = (obs == 0) & (fcst == 1)
     correct_negatives = (obs == 0) & (fcst == 0)
 
     # preserve NaNs
     false_alarms = false_alarms.where((~np.isnan(fcst)) & (~np.isnan(obs)))
     correct_negatives = correct_negatives.where((~np.isnan(fcst)) & (~np.isnan(obs)))
 
-    false_alarms = apply_weights(false_alarms, weights)
-    correct_negatives = apply_weights(correct_negatives, weights)
+    false_alarms = apply_weights(false_alarms, weights=weights)
+    correct_negatives = apply_weights(correct_negatives, weights=weights)
 
     false_alarms = false_alarms.sum(dim=dims_to_sum)
     correct_negatives = correct_negatives.sum(dim=dims_to_sum)
 
     pofd = false_alarms / (false_alarms + correct_negatives)
     return pofd
```

### Comparing `scores-0.6/src/scores/categorical/multicategorical_impl.py` & `scores-0.7/src/scores/categorical/multicategorical_impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 
 def firm(  # pylint: disable=too-many-arguments
     fcst: xr.DataArray,
     obs: xr.DataArray,
     risk_parameter: float,
     categorical_thresholds: Sequence[float],
     threshold_weights: Sequence[Union[float, xr.DataArray]],
+    *,  # Force keywords arguments to be keyword-only
     discount_distance: Optional[float] = 0,
-    reduce_dims: FlexibleDimensionTypes = None,
-    preserve_dims: FlexibleDimensionTypes = None,
+    reduce_dims: Optional[FlexibleDimensionTypes] = None,
+    preserve_dims: Optional[FlexibleDimensionTypes] = None,
     weights: Optional[xr.DataArray] = None,
     threshold_assignment: Optional[str] = "lower",
 ) -> xr.Dataset:
     """
     Calculates the FIxed Risk Multicategorical (FIRM) score including the
     underforecast and overforecast penalties.
 
@@ -104,25 +105,30 @@
     """
     _check_firm_inputs(
         obs, risk_parameter, categorical_thresholds, threshold_weights, discount_distance, threshold_assignment
     )
     total_score = []
     for categorical_threshold, weight in zip(categorical_thresholds, threshold_weights):
         score = weight * _single_category_score(
-            fcst, obs, risk_parameter, categorical_threshold, discount_distance, threshold_assignment
+            fcst,
+            obs,
+            risk_parameter,
+            categorical_threshold,
+            discount_distance=discount_distance,
+            threshold_assignment=threshold_assignment,
         )
         total_score.append(score)
     summed_score = sum(total_score)
     reduce_dims = gather_dimensions(
         fcst.dims, obs.dims, reduce_dims=reduce_dims, preserve_dims=preserve_dims
     )  # type: ignore[assignment]
-    summed_score = apply_weights(summed_score, weights)
-    score = summed_score.mean(dim=reduce_dims)
+    summed_score = apply_weights(summed_score, weights=weights)  # type: ignore
+    score = summed_score.mean(dim=reduce_dims)  # type: ignore
 
-    return score
+    return score  # type: ignore
 
 
 def _check_firm_inputs(
     obs, risk_parameter, categorical_thresholds, threshold_weights, discount_distance, threshold_assignment
 ):
     """
     Checks that the FIRM inputs are suitable
@@ -133,15 +139,15 @@
     if not len(categorical_thresholds) == len(threshold_weights):
         raise ValueError("The length of `categorical_thresholds` and `weights` must be equal")
     if risk_parameter <= 0 or risk_parameter >= 1:
         raise ValueError("0 < `risk_parameter` < 1 must be satisfied")
 
     for count, weight in enumerate(threshold_weights):
         if isinstance(weight, xr.DataArray):
-            check_dims(weight, obs.dims, "subset")
+            check_dims(weight, obs.dims, mode="subset")
             if np.any(weight <= 0):
                 raise ValueError(
                     f"""
                     No values <= 0 are allowed in `weights`. At least one
                     negative value was found in index {count} of `weights`
                     """
                 )
@@ -156,14 +162,15 @@
 
 
 def _single_category_score(
     fcst: xr.DataArray,
     obs: xr.DataArray,
     risk_parameter: float,
     categorical_threshold: float,
+    *,  # Force keywords arguments to be keyword-only
     discount_distance: Optional[float] = None,
     threshold_assignment: Optional[str] = "lower",
 ) -> xr.Dataset:
     """
     Calculates the score for a single category for the `firm` metric at each
     coord. Under-forecast and over-forecast penalties are also calculated
 
@@ -212,16 +219,16 @@
     condition2 = condition2.where(~np.isnan(fcst))
     condition2 = condition2.where(~np.isnan(obs))
 
     if discount_distance:
         scale_1 = np.minimum(categorical_threshold - obs, discount_distance)
         scale_2 = np.minimum(obs - categorical_threshold, discount_distance)
     else:
-        scale_1 = 1
-        scale_2 = 1
+        scale_1 = 1  # type: ignore
+        scale_2 = 1  # type: ignore
 
     overforecast_penalty = (1 - risk_parameter) * scale_1 * condition1
     underforecast_penalty = risk_parameter * scale_2 * condition2
     firm_score = overforecast_penalty + underforecast_penalty
 
     score = xr.Dataset(
         {
```

### Comparing `scores-0.6/src/scores/continuous/flip_flop_impl.py` & `scores-0.7/src/scores/continuous/flip_flop_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module contains functions for calculating flip flop indices
+This module contains functions for calculating Flip-Flop indices
 """
 
 from collections.abc import Generator, Iterable, Sequence
 from typing import Optional, Union, overload
 
 import numpy as np
 import xarray as xr
@@ -14,26 +14,26 @@
 from scores.utils import DimensionError, check_dims, dims_complement
 
 
 def _flip_flop_index(
     data: xr.DataArray, sampling_dim: str, *, is_angular: bool = False  # Force keywords arguments to be keyword-only
 ) -> xr.DataArray:
     """
-    Calculates the flip-flop index by collapsing the dimension specified by
+    Calculates the Flip-Flop Index by collapsing the dimension specified by
     `sampling_dim`.
 
     Args:
         data: Data from which to draw subsets.
         sampling_dim: The name of the dimension along which to calculate
-            the flip-flop index.
+            the Flip-Flop Index.
         is_angular: specifies whether `data` is directional data (e.g. wind
             direction).
 
     Returns:
-        A xarray.DataArray of the flip-flop index with the dimensions of
+        A xarray.DataArray of the Flip-Flop Index with the dimensions of
         `data`, except for the `sampling_dim` dimension which is collapsed.
 
     See also:
         `scores.continuous.flip_flop.flip_flop_index`
     """
     # check that `sampling_dim` is in `data`.
     check_dims(data, [sampling_dim], mode="superset")
@@ -43,24 +43,24 @@
 
     # calculate the range
     # skip_na=False guarantees that if there is a nan in that row,
     # it will show up as nan in the end
     if is_angular:
         # get complementary dimensions as `encompassing_sector_size` takes
         # dimensions to be preserved, not collapsed
-        dims_to_preserve = dims_complement(data, [sampling_dim])
+        dims_to_preserve = dims_complement(data, dims=[sampling_dim])
         # get maximum forecast range, if > 180 then clip to 180 as this is the
         # maximum possible angular difference between two forecasts
         enc_size = encompassing_sector_size(data=data, dims=dims_to_preserve)
         range_val = np.clip(enc_size, a_min=None, a_max=180.0)
         flip_flop = angular_difference(data.shift({sampling_dim: 1}), data)
     else:
         max_val = data.max(dim=sampling_dim, skipna=False)
         min_val = data.min(dim=sampling_dim, skipna=False)
-        range_val = max_val - min_val
+        range_val = max_val - min_val  # type: ignore
         # subtract each consecutive 'row' from eachother
         flip_flop = data.shift({sampling_dim: 1}) - data
 
     # take the absolute value and sum.
     # I don't do skipna=False here because .shift makes a row of nan
     flip_flop = abs(flip_flop).sum(dim=sampling_dim)
     # adjust based on the range. This is where nan will be introduced.
@@ -98,33 +98,33 @@
     data: xr.DataArray,
     sampling_dim: str,
     *,  # Force keywords arguments to be keyword-only
     is_angular: bool = False,
     **selections: Optional[Iterable[int]],
 ) -> XarrayLike:
     """
-    Calculates the Flip-flop Index along the dimensions `sampling_dim`.
+    Calculates the Flip-Flop Index along the dimensions `sampling_dim`.
 
     Args:
         data: Data from which to draw subsets.
         sampling_dim: The name of the dimension along which to calculate
-            the flip-flop index.
+            the Flip-Flop Index.
         is_angular: specifies whether `data` is directional data (e.g. wind
             direction).
         **selections: Additional keyword arguments specify
             subsets to draw from the dimension `sampling_dim` of the supplied `data`
-            before calculation of the flip_flop index. e.g. days123=[1, 2, 3]
+            before calculation of the Flip_Flop Index. e.g. days123=[1, 2, 3]
 
     Returns:
-        If `selections` are not supplied: An xarray.DataArray, the Flip-flop
+        If `selections` are not supplied: An xarray.DataArray, the Flip-Flop
         Index by collapsing the dimension `sampling_dim`.
 
         If `selections` are supplied: An xarray.Dataset. Each data variable
         is a supplied key-word argument, and corresponds to selecting the
-        values specified from `sampling_dim` of `data`. The Flip-flop Index
+        values specified from `sampling_dim` of `data`. The Flip-Flop Index
         is calculated for each of these selections.
 
     Notes:
 
         .. math::
 
             \\text{{Flip-Flop Index}} = \\frac{{1}}{{N-2}}
@@ -158,15 +158,15 @@
             sampling_dim: lead_day
 
     """
 
     if not selections and isinstance(data, xr.DataArray):
         result = _flip_flop_index(data, sampling_dim, is_angular=is_angular)
     else:
-        result = xr.Dataset()
+        result = xr.Dataset()  # type: ignore
         result.attrs["selections"] = selections
         for key, data_subset in iter_selections(data, sampling_dim, **selections):
             result[key] = _flip_flop_index(data_subset, sampling_dim, is_angular=is_angular)
     result.attrs["sampling_dim"] = sampling_dim
 
     return result
 
@@ -224,15 +224,15 @@
           * lead_day  (lead_day) int64 1 2 3 4 5 6 7
         days123 : <xarray.DataArray (lead_day: 3)>
         array([ 0. ,  0.1,  0.2])
         Coordinates:
           * lead_day  (lead_day) int64 1 2 3
 
     """
-    check_dims(data, [sampling_dim], "superset")
+    check_dims(data, [sampling_dim], mode="superset")
 
     for key, values in selections.items():
         try:
             # Need copy so that attributes added in _iter_selections_with_attrs
             # don't affect the whole dataframe but just the subset
             data_subset = data.sel({sampling_dim: values}).copy(deep=False)
         except KeyError as ex:
@@ -268,16 +268,16 @@
 
     Raises:
         scores.utils.DimensionError: raised if
 
             - the set of data dimensions is not a proper superset of `dims`
             - dimension to be collapsed isn't 1
     """
-    check_dims(data, dims, "proper superset")
-    dims_to_collapse = dims_complement(data, dims)
+    check_dims(data, dims, mode="proper superset")
+    dims_to_collapse = dims_complement(data, dims=dims)
     if len(dims_to_collapse) != 1:
         raise DimensionError("can only collapse one dimension")
     dim_to_collapse = dims_to_collapse[0]
     axis_to_collapse = data.get_axis_num(dim_to_collapse)
     values = _encompassing_sector_size_np(
         data=data.values,
         axis_to_collapse=axis_to_collapse,
@@ -371,38 +371,38 @@
 
 def flip_flop_index_proportion_exceeding(
     data: xr.DataArray,
     sampling_dim: str,
     thresholds: Iterable,
     *,  # Force keywords arguments to be keyword-only
     is_angular: bool = False,
-    preserve_dims: FlexibleDimensionTypes = None,
-    reduce_dims: FlexibleDimensionTypes = None,
+    preserve_dims: Optional[FlexibleDimensionTypes] = None,
+    reduce_dims: Optional[FlexibleDimensionTypes] = None,
     **selections: Iterable[int],
 ):
     """
-    Calculates the flip-flop index and returns the proportion exceeding
+    Calculates the Flip-Flop Index and returns the proportion exceeding
     (or equal to) each of the supplied `thresholds`.
 
     Args:
         data: Data from which to draw subsets.
         sampling_dim: The name of the dimension along which to calculate
-        thresholds: The proportion of Flip-Flop index results
+        thresholds: The proportion of Flip-Flop Index results
             equal to or exceeding these thresholds will be calculated.
-            the flip-flop index.
+            the Flip-Flop Index.
         is_angular: specifies whether `data` is directional data (e.g. wind
             direction).
         reduce_dims: Dimensions to reduce.
         preserve_dims: Dimensions to preserve.
         **selections: Additional keyword arguments specify
             subsets to draw from the dimension `sampling_dim` of the supplied `data`
-            before calculation of the flip_flop index. e.g. days123=[1, 2, 3]
+            before calculation of the Flip_Flop Index. e.g. days123=[1, 2, 3]
     Returns:
         If `selections` are not supplied - An xarray.DataArray with dimensions
-        `dims` + 'threshold'. The DataArray is the proportion of the Flip-flop
+        `dims` + 'threshold'. The DataArray is the proportion of the Flip-Flop
         Index calculated by collapsing dimension `sampling_dim` exceeding or
         equal to `thresholds`.
 
         If `selections` are supplied - An xarray.Dataset with dimensions `dims`
         + 'threshold'. There is a data variable for each keyword in
         `selections`, and corresponds to the Flip-Flop Index proportion
         exceeding for the subset of data specified by the keyword values.
@@ -446,15 +446,15 @@
             f"`preserve_dims`: {list(preserve_dims)}"
         )
     if reduce_dims is not None and sampling_dim in list(reduce_dims):
         raise DimensionError(
             f"`sampling_dim`: '{sampling_dim}' must not be in dimensions to reduce "
             f"`reduce_dims`: {list(reduce_dims)}"
         )
-    # calculate the flip-flop index
+    # calculate the Flip-Flop Index
     flip_flop_data = flip_flop_index(data, sampling_dim, is_angular=is_angular, **selections)
     # calculate the proportion exceeding each threshold
     flip_flop_exceeding = proportion_exceeding(
         flip_flop_data, thresholds, reduce_dims=reduce_dims, preserve_dims=preserve_dims
     )
     # overwrite the attributes
     flip_flop_exceeding.attrs = flip_flop_data.attrs
```

### Comparing `scores-0.6/src/scores/continuous/isoreg_impl.py` & `scores-0.7/src/scores/processing/isoreg_impl.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from scipy import interpolate
 from sklearn.isotonic import IsotonicRegression
 
 
 def isotonic_fit(  # pylint: disable=too-many-locals, too-many-arguments
     fcst: Union[np.ndarray, xr.DataArray],
     obs: Union[np.ndarray, xr.DataArray],
+    *,  # Force keywords arguments to be keyword-only
     weight: Optional[Union[np.ndarray, xr.DataArray]] = None,
     functional: Optional[Literal["mean", "quantile"]] = "mean",
     bootstraps: Optional[int] = None,
     quantile_level: Optional[float] = None,
     solver: Optional[Union[Callable[[np.ndarray, np.ndarray], float], Callable[[np.ndarray], float]]] = None,
     confidence_level: Optional[float] = 0.9,
     min_non_nan: Optional[int] = 1,
@@ -141,29 +142,36 @@
         - Dimitriadis, Gneiting and Jordan. "Stable reliability diagrams for probabilistic classifiers",
           PNAS, Vol. 118 No. 8, 2020. Available at https://www.pnas.org/doi/10.1073/pnas.2016191118
         - Jordan, Mühlemann, and Ziegel. "Optimal solutions to the isotonic regression problem",
           2020 (version 2), available on arxiv at https://arxiv.org/abs/1904.04761
     """
 
     if isinstance(fcst, xr.DataArray):
-        fcst, obs, weight = _xr_to_np(fcst, obs, weight)
+        fcst, obs, weight = _xr_to_np(fcst, obs, weight)  # type: ignore
     # now fcst, obs and weight (unless None) are np.arrays
 
     _iso_arg_checks(
-        fcst,
-        obs,
-        weight,
-        functional,
-        quantile_level,
-        solver,
-        bootstraps,
-        confidence_level,
+        fcst,  # type: ignore
+        obs,  # type: ignore
+        weight=weight,  # type: ignore
+        functional=functional,
+        quantile_level=quantile_level,
+        solver=solver,
+        bootstraps=bootstraps,
+        confidence_level=confidence_level,
+    )
+    fcst_tidied, obs_tidied, weight_tidied = _tidy_ir_inputs(fcst, obs, weight=weight)  # type: ignore
+    y_out = _do_ir(
+        fcst_tidied,
+        obs_tidied,
+        weight=weight_tidied,
+        functional=functional,
+        quantile_level=quantile_level,
+        solver=solver,
     )
-    fcst_tidied, obs_tidied, weight_tidied = _tidy_ir_inputs(fcst, obs, weight)
-    y_out = _do_ir(fcst_tidied, obs_tidied, weight_tidied, functional, quantile_level, solver)
 
     # calculate the fitting function
     ir_func = interpolate.interp1d(fcst_tidied, y_out, bounds_error=False)
 
     if bootstraps is not None:
         boot_results = _bootstrap_ir(
             fcst=fcst_tidied,
@@ -179,15 +187,15 @@
 
         lower_func = interpolate.interp1d(fcst_tidied, lower_pts, bounds_error=False)
         upper_func = interpolate.interp1d(fcst_tidied, upper_pts, bounds_error=False)
 
         confband_levels = ((1 - confidence_level) / 2, 1 - (1 - confidence_level) / 2)  # type: ignore
 
     else:
-        boot_results = lower_pts = upper_pts = None
+        boot_results = lower_pts = upper_pts = None  # type: ignore
         lower_func = upper_func = partial(np.full_like, fill_value=np.nan)
         confband_levels = (None, None)  # type: ignore
     # To reduce the size of output dictionary, we only keep the unique values of
     # forecasts and accordingly regression and confidence band values calculate by using
     # unique forecast values. We also calculate forecast counts that can be used to create
     # the forecast histogram.
     unique_fcst_sorted, fcst_counts = np.unique(fcst_tidied, return_counts=True)
@@ -237,28 +245,29 @@
     if set(fcst_dims) != set(obs.dims):
         raise ValueError("`fcst` and `obs` must have same dimensions.")
 
     if weight is not None:
         if set(fcst_dims) != set(weight.dims):
             raise ValueError("`fcst` and `weight` must have same dimensions.")
         merged_ds = xr.merge([fcst.rename("fcst"), obs.rename("obs"), weight.rename("weight")])
-        weight = merged_ds["weight"].transpose(*fcst_dims).values
+        weight = merged_ds["weight"].transpose(*fcst_dims).values  # type: ignore
     else:
         merged_ds = xr.merge([fcst.rename("fcst"), obs.rename("obs")])
 
-    fcst = merged_ds["fcst"].transpose(*fcst_dims).values
-    obs = merged_ds["obs"].transpose(*fcst_dims).values
+    fcst = merged_ds["fcst"].transpose(*fcst_dims).values  # type: ignore
+    obs = merged_ds["obs"].transpose(*fcst_dims).values  # type: ignore
 
-    return fcst, obs, weight
+    return fcst, obs, weight  # type: ignore
 
 
 def _iso_arg_checks(  # pylint: disable=too-many-arguments, too-many-branches
     fcst: np.ndarray,
     obs: np.ndarray,
-    weight: np.ndarray,
+    *,  # Force keywords arguments to be keyword-only
+    weight: Optional[Union[np.ndarray, xr.DataArray]] = None,
     functional: Optional[str] = None,
     quantile_level: Optional[float] = None,
     solver: Optional[Union[Callable[[np.ndarray, np.ndarray], float], Callable[[np.ndarray], float]]] = None,
     bootstraps: Optional[int] = None,
     confidence_level: Optional[float] = None,
 ) -> None:
     """Raises ValueError if isotonic_fit arguments are invalid."""
@@ -305,14 +314,15 @@
         if not 0 < confidence_level < 1:  # type: ignore
             raise ValueError("`confidence_level` must be strictly between 0 and 1.")
 
 
 def _tidy_ir_inputs(
     fcst: np.ndarray,
     obs: np.ndarray,
+    *,  # Force keywords arguments to be keyword-only
     weight: Optional[np.ndarray] = None,
 ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
     """
     Tidies array inputs to `isotonic_fit` in preparation for the regression routine.
 
     Arrays are flattened to 1D arrays. NaNs are jointly removed from fcst, obs, weights.
     The array data is then sorted by fcst (ascending) then by obs (descending).
@@ -355,24 +365,25 @@
 
     if weight is None:
         new_weight = None
     else:
         new_weight = weight[~nan_locs]
         new_weight = new_weight[sorter]
 
-    return new_fcst, new_obs, new_weight
+    return new_fcst, new_obs, new_weight  # type: ignore
 
 
 def _do_ir(  # pylint: disable=too-many-arguments
     fcst: np.ndarray,
     obs: np.ndarray,
-    weight: Optional[np.ndarray],
-    functional: Optional[Literal["mean", "quantile"]],
-    quantile_level: Optional[float],
-    solver: Optional[Union[Callable[[np.ndarray, np.ndarray], float], Callable[[np.ndarray], float]]],
+    *,  # Force keywords arguments to be keyword-only
+    weight: Optional[np.ndarray] = None,
+    functional: Optional[Literal["mean", "quantile"]] = None,
+    quantile_level: Optional[float] = None,
+    solver: Optional[Union[Callable[[np.ndarray, np.ndarray], float], Callable[[np.ndarray], float]]] = None,
 ) -> np.ndarray:
     """
     Returns the isotonic regression (IR) fit for specified functional or solver,
     by passing the inputs to the appropriate IR algorithm.
 
     The inputs `fcst`, `obs` and `weight` are 1D numpy arrays assumed to have been
     mutually tidied via `_tidy_ir_inputs`.
@@ -387,26 +398,27 @@
         solver: solver function as described in docstring of `isotonic_fit`, or `None`.
             Cannot be `None` if `functional` is `None`.
 
     Returns:
         1D numpy array of values fitted using isotonic regression.
     """
     if functional == "mean":
-        y_out = _contiguous_mean_ir(fcst, obs, weight)
+        y_out = _contiguous_mean_ir(fcst, obs, weight=weight)
     elif functional == "quantile":
         y_out = _contiguous_quantile_ir(obs, quantile_level)  # type: ignore
     else:
-        y_out = _contiguous_ir(obs, solver, weight)  # type: ignore
+        y_out = _contiguous_ir(obs, solver, weight=weight)  # type: ignore
 
     return y_out
 
 
 def _contiguous_ir(
     y: np.ndarray,
     solver: Union[Callable[[np.ndarray, np.ndarray], float], Callable[[np.ndarray], float]],
+    *,  # Force keywords arguments to be keyword-only
     weight: Optional[np.ndarray] = None,
 ) -> np.ndarray:
     """
     Given a 1D numpy array `y` of response values, returns fitted isotonic regression
     with values for each valid regression block determined by `solver`.
 
     This implementation uses the pool adjacent violators (PAV) algorithm, and is based on the squared loss
@@ -479,34 +491,37 @@
         index = idx_next_block
 
     return y_out
 
 
 def _contiguous_quantile_ir(y: np.ndarray, alpha: float) -> np.ndarray:
     """Performs contiguous quantile IR on tidied data y, for quantile-level alpha, with no weights."""
-    return _contiguous_ir(y, partial(np.quantile, q=alpha))
+    return _contiguous_ir(y, partial(np.quantile, q=alpha))  # type: ignore
 
 
-def _contiguous_mean_ir(x: np.ndarray, y: np.ndarray, weight: Optional[np.ndarray]) -> np.ndarray:
+def _contiguous_mean_ir(
+    x: np.ndarray, y: np.ndarray, *, weight: Optional[np.ndarray] = None  # Force keywords arguments to be keyword-only
+) -> np.ndarray:
     """
     Performs classical (i.e. for mean functional) contiguous quantile IR on tidied data x, y.
     Uses sklearn implementation rather than supplying the mean solver function to `_contiguous_ir`,
     as it is about 4 times faster (since it is optimised for mean).
     """
-    return IsotonicRegression().fit_transform(x, y, sample_weight=weight)
+    return IsotonicRegression().fit_transform(x, y, sample_weight=weight)  # type: ignore
 
 
 def _bootstrap_ir(  # pylint: disable=too-many-arguments, too-many-locals
     fcst: np.ndarray,
     obs: np.ndarray,
     bootstraps: int,
-    weight: Optional[np.ndarray],
-    functional: Optional[Literal["mean", "quantile"]],
-    quantile_level: Optional[float],
-    solver: Optional[Union[Callable[[np.ndarray, np.ndarray], float], Callable[[np.ndarray], float]]],
+    *,  # Force keywords arguments to be keyword-only
+    weight: Optional[np.ndarray] = None,
+    functional: Optional[Literal["mean", "quantile"]] = None,
+    quantile_level: Optional[float] = None,
+    solver: Optional[Union[Callable[[np.ndarray, np.ndarray], float], Callable[[np.ndarray], float]]] = None,
 ):
     """
     Gives the isotonic fits of bootstrapped samples.
 
     Args:
         fcst: 1D numpy array of forecast values.
         obs: 1D numpy array of observed values corresponding to `fcst`.
@@ -531,16 +546,24 @@
         fcst_sample = fcst[selection]
         obs_sample = obs[selection]
         if weight is None:
             weight_sample = None
         else:
             weight_sample = weight[selection]
 
-        fcst_sample, obs_sample, weight_sample = _tidy_ir_inputs(fcst_sample, obs_sample, weight_sample)
-        ir_results = _do_ir(fcst_sample, obs_sample, weight_sample, functional, quantile_level, solver)
+        fcst_sample, obs_sample, weight_sample = _tidy_ir_inputs(fcst_sample, obs_sample, weight=weight_sample)
+
+        ir_results = _do_ir(
+            fcst_sample,
+            obs_sample,
+            weight=weight_sample,
+            functional=functional,
+            quantile_level=quantile_level,
+            solver=solver,
+        )
 
         approximation_func = interpolate.interp1d(fcst_sample, ir_results, bounds_error=False)
 
         result[boostrap_sample_num] = approximation_func(fcst)
 
     return result
```

### Comparing `scores-0.6/src/scores/continuous/murphy_impl.py` & `scores-0.7/src/scores/continuous/murphy_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,21 @@
 SCORING_FUNC_DOCSTRING_PARAMS = {fun.upper(): fun for fun in VALID_SCORING_FUNC_NAMES}
 
 
 def murphy_score(  # pylint: disable=R0914
     fcst: xr.DataArray,
     obs: xr.DataArray,
     thetas: Union[Sequence[float], xr.DataArray],
+    *,  # Force keywords arguments to be keyword-only
     functional: Literal["quantile", "huber", "expectile"],
     alpha: float,
     huber_a: Optional[float] = None,
     decomposition: bool = False,
-    reduce_dims: FlexibleDimensionTypes = None,
-    preserve_dims: FlexibleDimensionTypes = None,
+    reduce_dims: Optional[FlexibleDimensionTypes] = None,
+    preserve_dims: Optional[FlexibleDimensionTypes] = None,
 ) -> xr.Dataset:
     """Returns the mean elementary score (Ehm et. al. 2016), also known as Murphy score,
     evaluated at decision thresholds specified by thetas. Optionally returns a decomposition
     of the score in terms of penalties for over- and under-forecasting.
 
     Select `functional="quantile"` and `alpha=0.5` for the median functional.
     Select `functional="expectile"` and `alpha=0.5` for the mean (i.e., expectation) functional.
@@ -95,15 +96,15 @@
     """
     functional_lower = functional.lower()
     _check_murphy_inputs(alpha=alpha, functional=functional_lower, huber_a=huber_a)
     if isinstance(thetas, xr.DataArray):
         theta1 = thetas
     else:
         theta1 = xr.DataArray(data=thetas, dims=["theta"], coords={"theta": thetas})
-    theta1, fcst1, obs1 = broadcast_and_match_nan(theta1, fcst, obs)
+    theta1, fcst1, obs1 = broadcast_and_match_nan(theta1, fcst, obs)  # type: ignore
 
     over, under = exposed_functions()[f"_{functional_lower}_elementary_score"](
         fcst1, obs1, theta1, alpha, huber_a=huber_a
     )
     # Align dimensions, this is required in cases such as when the station numbers
     # are not in the same order in `obs` and `fcst` to prevent an exception on the next
     # line that combines the scores
@@ -144,15 +145,15 @@
 def _expectile_elementary_score(fcst: FlexibleArrayType, obs: FlexibleArrayType, theta, alpha, **_):
     """Return over and under forecast vs obs penalties relative to theta for {EXPECTILE}."""
     over = (1 - alpha) * np.abs(obs - theta).where((fcst > theta) & (obs <= theta))
     under = alpha * np.abs(obs - theta).where((fcst <= theta) & (obs > theta))
     return over, under
 
 
-def _check_murphy_inputs(alpha=None, functional=None, huber_a=None, left_limit_delta=None):
+def _check_murphy_inputs(*, alpha=None, functional=None, huber_a=None, left_limit_delta=None):
     """Raise ValueError if the arguments have unexpected values."""
     if (alpha is not None) and not (0 < alpha < 1):  # pylint: disable=C0325
         err = f"alpha (={alpha}) argument for Murphy scoring function should be strictly " "between 0 and 1."
         raise ValueError(err)
     if (functional is not None) and (functional not in VALID_SCORING_FUNC_NAMES):
         err = (
             f"Functional option '{functional}' for Murphy scoring function is "
@@ -167,14 +168,15 @@
         raise ValueError(err)
 
 
 def murphy_thetas(
     forecasts: list[xr.DataArray],
     obs: xr.DataArray,
     functional: Literal["quantile", "huber", "expectile"],
+    *,  # Force keywords arguments to be keyword-only
     huber_a: Optional[float] = None,
     left_limit_delta: Optional[float] = None,
 ) -> list[float]:
     """Return the decision thresholds (theta values) at which to evaluate
     elementary scores for the construction of Murphy diagrams.
 
     This function may generate a very large number of theta thresholds if the forecast
```

### Comparing `scores-0.6/src/scores/continuous/quantile_loss_impl.py` & `scores-0.7/src/scores/continuous/quantile_loss_impl.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 Implementation of quantile loss (score)
 """
 from typing import Optional, Sequence
 
 import xarray as xr
 
 from scores.functions import apply_weights
-from scores.typing import XarrayLike
+from scores.typing import FlexibleDimensionTypes, XarrayLike
 from scores.utils import check_dims, gather_dimensions
 
 
 def quantile_score(
     fcst: XarrayLike,
     obs: XarrayLike,
     alpha: float,
-    reduce_dims: Optional[Sequence[str]] = None,
-    preserve_dims: Optional[Sequence[str]] = None,
-    weights: XarrayLike = None,
+    *,  # Force keywords arguments to be keyword-only
+    reduce_dims: Optional[FlexibleDimensionTypes] = None,
+    preserve_dims: Optional[FlexibleDimensionTypes] = None,
+    weights: Optional[XarrayLike] = None,
 ) -> XarrayLike:
     """
     Calculates a score that targets alpha-quantiles.
     Use with alpha = 0.5 for forecasts of the median.
     Use with alpha = 0.9 for forecasts of the 90th percentile.
 
     Args:
@@ -52,34 +53,34 @@
     Raises:
         ValueError: if `alpha` is not between 0 and 1.
 
     Notes:
 
         .. math::
 
-            gpl(x) = \\begin{{cases}}\\alpha * (-x) & x \\leq 0\\\\
-           (1-\\alpha) x & x > 0\\end{{cases}}
+            gpl(x) = \\begin{cases}\\alpha * (-x) & x \\leq 0\\\\
+           (1-\\alpha) x & x > 0\\end{cases}
 
         where:
 
             - :math:`\\alpha` is the targeted quantile.
             - :math:`x` is the difference, fcst - obs
 
     References:
-        T. Geinting, "Making and evaluating point forecasts",
+        T. Gneiting, "Making and evaluating point forecasts",
         J. Amer. Stat. Assoc., Vol. 106 No. 494 (June 2011), pp. 754--755,
         Theorem 9
 
     """
     specified_dims = reduce_dims or preserve_dims
     # check requested dims are a subset of fcst dimensions
     if specified_dims is not None:
         check_dims(xr_data=fcst, expected_dims=specified_dims, mode="superset")
     # check obs dimensions are a subset of fcst dimensions
-    check_dims(xr_data=obs, expected_dims=fcst.dims, mode="subset")
+    check_dims(xr_data=obs, expected_dims=fcst.dims, mode="subset")  # type: ignore
 
     # check that alpha is between 0 and 1 as required
     if (alpha <= 0) or (alpha >= 1):
         raise ValueError("alpha is not between 0 and 1")
 
     # Do this operation once to save compute time
     diff = fcst - obs
@@ -89,11 +90,11 @@
 
     # calculate the score applicable when fcst > obs
     score_fcst_ge_obs = (1 - alpha) * diff
 
     result = xr.where(diff > 0, score_fcst_ge_obs, score_fcst_lte_obs)
 
     reduce_dims = gather_dimensions(fcst.dims, obs.dims, reduce_dims=reduce_dims, preserve_dims=preserve_dims)  # type: ignore[assignment]
-    results = apply_weights(result, weights)
+    results = apply_weights(result, weights=weights)
     score = results.mean(dim=reduce_dims)
 
-    return score
+    return score  # type: ignore
```

### Comparing `scores-0.6/src/scores/pandas/continuous.py` & `scores-0.7/src/scores/pandas/continuous.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,96 +6,96 @@
 from scores.pandas.typing import PandasType
 
 
 def mse(
     fcst: PandasType,
     obs: PandasType,
     *,  # Force keywords arguments to be keyword-only
-    angular: bool = False,
+    is_angular: bool = False,
 ) -> PandasType:
     """Calculates the mean squared error from forecast and observed data.
 
     A detailed explanation is on [Wikipedia](https://en.wikipedia.org/wiki/Mean_squared_error)
 
 
     Dimensional reduction is not supported for pandas and the user should
     convert their data to xarray to formulate the call to the base metric, `scores.continuous.mse`.
 
     Args:
         fcst: Forecast or predicted variables in pandas.
         obs: Observed variables in pandas.
-        angular: specifies whether `fcst` and `obs` are angular
+        is_angular: specifies whether `fcst` and `obs` are angular
             data (e.g. wind direction). If True, a different function is used
             to calculate the difference between `fcst` and `obs`, which
             accounts for circularity. Angular `fcst` and `obs` data should be in
             degrees rather than radians.
 
     Returns:
         An object containing
             a single floating point number representing the mean squared
             error for the supplied data. All dimensions will be reduced.
 
     """
-    return __continuous.mse(fcst, obs, angular=angular)  # type: ignore  # mypy is wrong, I think
+    return __continuous.mse(fcst, obs, is_angular=is_angular)  # type: ignore  # mypy is wrong, I think
 
 
 def rmse(
     fcst: PandasType,
     obs: PandasType,
     *,  # Force keywords arguments to be keyword-only
-    angular: bool = False,
+    is_angular: bool = False,
 ) -> PandasType:
     """Calculate the Root Mean Squared Error from xarray or pandas objects.
 
     A detailed explanation is on [Wikipedia](https://en.wikipedia.org/wiki/Root-mean-square_deviation)
 
     Dimensional reduction is not supported for pandas and the user should
     convert their data to xarray to formulate the call to the base metric, `scores.continuous.rmse`.
 
     Args:
         fcst: Forecast or predicted variables in pandas.
         obs: Observed variables in pandas.
-        angular: specifies whether `fcst` and `obs` are angular
+        is_angular: specifies whether `fcst` and `obs` are angular
             data (e.g. wind direction). If True, a different function is used
             to calculate the difference between `fcst` and `obs`, which
             accounts for circularity. Angular `fcst` and `obs` data should be in
             degrees rather than radians.
 
     Returns:
         An object containing
             a single floating point number representing the root mean squared
             error for the supplied data. All dimensions will be reduced.
 
     """
-    return __continuous.rmse(fcst, obs, angular=angular)  # type: ignore  # mypy is wrong, I think
+    return __continuous.rmse(fcst, obs, is_angular=is_angular)  # type: ignore  # mypy is wrong, I think
 
 
 def mae(
     fcst: PandasType,
     obs: PandasType,
     *,  # Force keywords arguments to be keyword-only
-    angular: bool = False,
+    is_angular: bool = False,
 ) -> PandasType:
     """Calculates the mean absolute error from forecast and observed data.
 
     A detailed explanation is on [Wikipedia](https://en.wikipedia.org/wiki/Mean_absolute_error)
 
 
     Dimensional reduction is not supported for pandas and the user should
     convert their data to xarray to formulate the call to the base metric, `scores.continuous.mae`.
 
     Args:
         fcst: Forecast or predicted variables in pandas.
         obs: Observed variables in pandas.
-        angular: specifies whether `fcst` and `obs` are angular
+        is_angular: specifies whether `fcst` and `obs` are angular
             data (e.g. wind direction). If True, a different function is used
             to calculate the difference between `fcst` and `obs`, which
             accounts for circularity. Angular `fcst` and `obs` data should be in
             degrees rather than radians.
 
     Returns:
         An object containing
             a single floating point number representing the mean absolute
             error for the supplied data. All dimensions will be reduced.
 
     """
-    return __continuous.mae(fcst, obs, angular=angular)  # type: ignore  # mypy is wrong, I think
+    return __continuous.mae(fcst, obs, is_angular=is_angular)  # type: ignore  # mypy is wrong, I think
```

### Comparing `scores-0.6/src/scores/probability/__init__.py` & `scores-0.7/src/scores/probability/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 Import the functions from the implementations into the public API
 """
 
-from scores.continuous.isoreg_impl import isotonic_fit
 from scores.continuous.murphy_impl import murphy_score, murphy_thetas
 from scores.probability.brier_impl import brier_score
 from scores.probability.crps_impl import (
     adjust_fcst_for_crps,
     crps_cdf,
     crps_cdf_brier_decomposition,
     crps_for_ensemble,
 )
 from scores.probability.roc_impl import roc_curve_data
+from scores.processing.isoreg_impl import isotonic_fit
 
 __all__ = [
-    "isotonic_fit",
     "murphy_score",
     "murphy_thetas",
     "brier_score",
     "adjust_fcst_for_crps",
     "crps_cdf",
     "crps_cdf_brier_decomposition",
     "crps_for_ensemble",
     "roc_curve_data",
+    "isotonic_fit",
 ]
```

### Comparing `scores-0.6/src/scores/probability/brier_impl.py` & `scores-0.7/src/scores/probability/brier_impl.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """
 This module contains methods related to the Brier score
 """
 
+from typing import Optional
+
 import xarray as xr
 
 from scores.continuous import mse
-from scores.processing import check_binary
 from scores.typing import FlexibleDimensionTypes, XarrayLike
+from scores.utils import check_binary
 
 
 def brier_score(
     fcst: XarrayLike,
     obs: XarrayLike,
-    reduce_dims: FlexibleDimensionTypes = None,
-    preserve_dims: FlexibleDimensionTypes = None,
-    weights: xr.DataArray = None,
+    *,  # Force keywords arguments to be keyword-only
+    reduce_dims: Optional[FlexibleDimensionTypes] = None,
+    preserve_dims: Optional[FlexibleDimensionTypes] = None,
+    weights: Optional[xr.DataArray] = None,
     check_args: bool = True,
 ):
     """
     Calculates the Brier score for forecast and observed data. For an explanation of the
     Brier score, see [Wikipedia](https://en.wikipedia.org/wiki/Brier_score).
 
     If you want to speed up performance with Dask and are confident of your input data,
@@ -49,8 +52,8 @@
             if fcst.to_array().max().values.item() > 1 or fcst.to_array().min().values.item() < 0:
                 raise error_msg
         else:
             if fcst.max().values.item() > 1 or fcst.min().values.item() < 0:
                 raise error_msg
         check_binary(obs, "obs")
 
-    return mse(fcst, obs, reduce_dims, preserve_dims, weights)
+    return mse(fcst, obs, reduce_dims=reduce_dims, preserve_dims=preserve_dims, weights=weights)
```

### Comparing `scores-0.6/src/scores/probability/checks.py` & `scores-0.7/src/scores/probability/checks.py`

 * *Files identical despite different names*

### Comparing `scores-0.6/src/scores/probability/crps_impl.py` & `scores-0.7/src/scores/probability/crps_impl.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 This module supports the implementation of the CRPS scoring function, drawing from additional functions.
 The two primary methods, `crps_cdf` and `crps_for_ensemble` are imported into 
 the probability module to be part of the probability API.
 """
+
 from collections.abc import Iterable
 from typing import Literal, Optional, Sequence
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 
 import scores.utils
 from scores.probability.checks import coords_increasing
-from scores.probability.functions import (
+from scores.processing.cdf import (
     add_thresholds,
     cdf_envelope,
     decreasing_cdfs,
     integrate_square_piecewise_linear,
     observed_cdf,
     propagate_nan,
 )
@@ -82,18 +83,19 @@
         raise ValueError("`threshold_weight` has negative values")
 
 
 def crps_cdf_reformat_inputs(
     fcst: xr.DataArray,
     obs: xr.DataArray,
     threshold_dim: str,
-    threshold_weight: Optional[xr.DataArray],
-    additional_thresholds: Optional[Iterable[float]],
-    fcst_fill_method: Literal["linear", "step", "forward", "backward"],
-    threshold_weight_fill_method: Literal["linear", "step", "forward", "backward"],
+    *,  # Force keywords arguments to be keyword-only
+    threshold_weight: Optional[xr.DataArray] = None,
+    additional_thresholds: Optional[Iterable[float]] = None,
+    fcst_fill_method: Literal["linear", "step", "forward", "backward"] = "linear",
+    threshold_weight_fill_method: Literal["linear", "step", "forward", "backward"] = "forward",
 ) -> tuple[xr.DataArray, xr.DataArray, xr.DataArray]:
     """
     Takes `fcst`, `obs` and `threshold_weight` inputs from `crps_cdf` and reformats them
     for use in `crps_cdf`; that is, `cdf_fcst`, `cdf_obs` and `threshold_weight` are
     returned with matching dimensions and coordinates.
 
     `additional_thresholds` contains additional thresholds to use.
@@ -102,22 +104,22 @@
     NaNs are filled, unless there are too few non-NaNs for filling.
     """
     # will use all thresholds from fcst, obs and (if applicable) weight
 
     fcst_thresholds = fcst[threshold_dim].values
     obs_thresholds = pd.unique(obs.values.flatten())
 
-    weight_thresholds = []
+    weight_thresholds = []  # type: ignore
     if threshold_weight is not None:
-        weight_thresholds = threshold_weight[threshold_dim].values
+        weight_thresholds = threshold_weight[threshold_dim].values  # type: ignore
 
     if additional_thresholds is None:
         additional_thresholds = []
 
-    thresholds = np.concatenate((weight_thresholds, fcst_thresholds, obs_thresholds, additional_thresholds))
+    thresholds = np.concatenate((weight_thresholds, fcst_thresholds, obs_thresholds, additional_thresholds))  # type: ignore
     thresholds = np.sort(pd.unique(thresholds))
     thresholds = thresholds[~np.isnan(thresholds)]
 
     # get obs in cdf form with correct thresholds
     obs_cdf = observed_cdf(
         obs,
         threshold_dim,
@@ -141,14 +143,15 @@
     return fcst_cdf, obs_cdf, weight_cdf
 
 
 # pylint: disable=too-many-locals
 def crps_cdf(
     fcst: xr.DataArray,
     obs: xr.DataArray,
+    *,  # Force keywords arguments to be keyword-only
     threshold_dim: str = "threshold",
     threshold_weight: Optional[xr.DataArray] = None,
     additional_thresholds: Optional[Iterable[float]] = None,
     propagate_nans: bool = True,
     fcst_fill_method: Literal["linear", "step", "forward", "backward"] = "linear",
     threshold_weight_fill_method: Literal["linear", "step", "forward", "backward"] = "forward",
     integration_method: Literal["exact", "trapz"] = "exact",
@@ -307,26 +310,26 @@
         fcst_fill_method,
         threshold_weight_fill_method,
         integration_method,
         dims,
     )
 
     if propagate_nans:
-        fcst = propagate_nan(fcst, threshold_dim)
+        fcst = propagate_nan(fcst, threshold_dim)  # type: ignore
         if threshold_weight is not None:
-            threshold_weight = propagate_nan(threshold_weight, threshold_dim)
+            threshold_weight = propagate_nan(threshold_weight, threshold_dim)  # type: ignore
 
     fcst, obs, threshold_weight = crps_cdf_reformat_inputs(
         fcst,
         obs,
         threshold_dim,
-        threshold_weight,
-        additional_thresholds,
-        fcst_fill_method,
-        threshold_weight_fill_method,
+        threshold_weight=threshold_weight,
+        additional_thresholds=additional_thresholds,
+        fcst_fill_method=fcst_fill_method,
+        threshold_weight_fill_method=threshold_weight_fill_method,
     )
 
     if integration_method == "exact":
         result = crps_cdf_exact(
             fcst,
             obs,
             threshold_weight,
@@ -339,28 +342,29 @@
             fcst,
             obs,
             threshold_weight,
             threshold_dim,
             include_components=include_components,
         )
 
-    weighted = scores.functions.apply_weights(result, weights)
+    weighted = scores.functions.apply_weights(result, weights=weights)
 
     dims.remove(threshold_dim)  # type: ignore
 
-    result = weighted.mean(dim=dims)
+    result = weighted.mean(dim=dims)  # type: ignore
 
     return result
 
 
 def crps_cdf_exact(
     cdf_fcst: xr.DataArray,
     cdf_obs: xr.DataArray,
     threshold_weight: xr.DataArray,
     threshold_dim: str,
+    *,  # Force keywords arguments to be keyword-only
     include_components=False,
 ) -> xr.Dataset:
     """
     Calculates exact value of CRPS assuming that:
         - the forecast CDF is continuous piecewise linear, with join points given by
           values in `cdf_fcst`,
         - the observation CDF is right continuous with values in {0,1} given by `cdf_obs`,
@@ -377,29 +381,30 @@
         (xr.Dataset): Dataset with `threshold_dim` collapsed containing DataArrays with
         CRPS and its decomposition, labelled "total", "underforecast_penalty" and
         "overforecast_penalty". NaN is returned if there is a NaN in the corresponding
         `cdf_fcst`, `cdf_obs` or `threshold_weight`.
     """
 
     # identify where input arrays have no NaN, collapsing `threshold_dim`
+    # Mypy doesn't realise the isnan and any come from xarray not numpy
     inputs_without_nan = (
-        ~np.isnan(cdf_fcst).any(threshold_dim)
-        & ~np.isnan(cdf_obs).any(threshold_dim)
-        & ~np.isnan(threshold_weight).any(threshold_dim)
+        ~np.isnan(cdf_fcst).any(threshold_dim)  # type: ignore
+        & ~np.isnan(cdf_obs).any(threshold_dim)  # type: ignore
+        & ~np.isnan(threshold_weight).any(threshold_dim)  # type: ignore
     )
 
     # thresholds in the closure of the interval (i.e. including endpoints) where
     # weight is 1
-    interval_where_weight_one = (threshold_weight == 1) | ((threshold_weight.shift(**{threshold_dim: 1})) == 1)
+    interval_where_weight_one = (threshold_weight == 1) | ((threshold_weight.shift(**{threshold_dim: 1})) == 1)  # type: ignore
 
     # thresholds in the closure of the interval where cdf_obs is 1
     interval_where_obs_one = cdf_obs == 1
 
     # thresholds in the closure of the interval where obs cdf is 0
-    interval_where_obs_zero = (cdf_obs == 0) | ((cdf_obs.shift(**{threshold_dim: 1})) == 0)
+    interval_where_obs_zero = (cdf_obs == 0) | ((cdf_obs.shift(**{threshold_dim: 1})) == 0)  # type: ignore
 
     # over-forecast penalty contribution to CRPS: integral(w(x) * (F(x) - 1)^2) where x >= obs
     over = (cdf_fcst - 1).where(interval_where_obs_one).where(interval_where_weight_one)
     over = integrate_square_piecewise_linear(over, threshold_dim)
     # If zero penalty, could be NaN. Replace with 0, then NaN using inputs_without_nan
     over = over.where(~np.isnan(over), 0).where(inputs_without_nan)
 
@@ -423,14 +428,15 @@
 
     return result
 
 
 def crps_cdf_brier_decomposition(
     fcst: xr.DataArray,
     obs: xr.DataArray,
+    *,  # Force keywords arguments to be keyword-only
     threshold_dim: str = "threshold",
     additional_thresholds: Optional[Iterable[float]] = None,
     fcst_fill_method: Literal["linear", "step", "forward", "backward"] = "linear",
     reduce_dims: Optional[Iterable[str]] = None,
     preserve_dims: Optional[Iterable[str]] = None,
 ) -> xr.Dataset:
     """
@@ -486,24 +492,24 @@
         obs.dims,
         reduce_dims=reduce_dims,
         preserve_dims=preserve_dims,
     )
 
     check_crps_cdf_brier_inputs(fcst, obs, threshold_dim, fcst_fill_method, dims)
 
-    fcst = propagate_nan(fcst, threshold_dim)
+    fcst = propagate_nan(fcst, threshold_dim)  # type: ignore
 
     fcst, obs, _ = crps_cdf_reformat_inputs(
         fcst,
         obs,
         threshold_dim,
-        None,
-        additional_thresholds,
-        fcst_fill_method,
-        "forward",
+        threshold_weight=None,
+        additional_thresholds=additional_thresholds,
+        fcst_fill_method=fcst_fill_method,
+        threshold_weight_fill_method="forward",
     )
 
     dims.remove(threshold_dim)  # type: ignore
 
     # brier score for each forecast case
     bscore = (fcst - obs) ** 2
     not_nan = ~np.isnan(bscore)
@@ -548,14 +554,15 @@
         raise ValueError("`threshold_dim` coordinates in `fcst` must be increasing")
 
 
 def adjust_fcst_for_crps(
     fcst: xr.DataArray,
     threshold_dim: str,
     obs: xr.DataArray,
+    *,  # Force keywords arguments to be keyword-only
     decreasing_tolerance: float = 0,
     additional_thresholds: Optional[Iterable[float]] = None,
     fcst_fill_method: Literal["linear", "step", "forward", "backward"] = "linear",
     integration_method: Literal["exact", "trapz"] = "exact",
 ) -> xr.DataArray:
     """
     This function takes a forecast cumulative distribution functions (CDF) `fcst`.
@@ -612,34 +619,34 @@
     """
     if threshold_dim not in fcst.dims:
         raise ValueError(f"'{threshold_dim}' is not a dimension of `fcst`")
 
     if decreasing_tolerance < 0:
         raise ValueError("`decreasing_tolerance` must be nonnegative")
 
-    fcst = propagate_nan(fcst, threshold_dim)
+    fcst = propagate_nan(fcst, threshold_dim)  # type: ignore
 
     is_decreasing = decreasing_cdfs(fcst, threshold_dim, decreasing_tolerance)
 
     if not is_decreasing.any():
         return fcst
 
     fcst_env = cdf_envelope(fcst, threshold_dim)
 
     # dimensions to preserve when calculating CRPS
     crps_dims = [x for x in fcst_env.dims if x != threshold_dim]
 
     crps_fcst_env = crps_cdf(
         fcst_env,
         obs,
-        threshold_dim,
+        threshold_dim=threshold_dim,
         additional_thresholds=additional_thresholds,
         fcst_fill_method=fcst_fill_method,
         integration_method=integration_method,
-        preserve_dims=crps_dims,
+        preserve_dims=crps_dims,  # type: ignore
     )
 
     fcst_type_to_use = crps_fcst_env["total"].idxmax("cdf_type")
 
     fcst_to_return = fcst_env.where(fcst_env["cdf_type"] == fcst_type_to_use).max("cdf_type")
 
     fcst_to_return = fcst_to_return.where(is_decreasing).combine_first(fcst)
@@ -648,14 +655,15 @@
 
 
 def crps_cdf_trapz(
     cdf_fcst: xr.DataArray,
     cdf_obs: xr.DataArray,
     threshold_weight: xr.DataArray,
     threshold_dim: str,
+    *,  # Force keywords arguments to be keyword-only
     include_components=False,
 ) -> xr.Dataset:
     """
     Returns dataset with CRPS estimate and decomposition using a trapezoidal rule on
     points from the integrand
         threshold_weight(x) * (cdf_fcst(x) - cdf_obs(x)) ** 2
 
@@ -663,18 +671,19 @@
     `threshold_dim` approaches zero.
 
     NaN is returned if there is a NaN in the corresponding `cdf_fcst`, `cdf_obs` or
     `threshold_weight`.
     """
 
     # identify where input arrays have no NaN, collapsing `threshold_dim`
+    # mypy doesn't realise the isnan and any come from xarray not numpy
     inputs_without_nan = (
-        ~np.isnan(cdf_fcst).any(threshold_dim)
-        & ~np.isnan(cdf_obs).any(threshold_dim)
-        & ~np.isnan(threshold_weight).any(threshold_dim)
+        ~np.isnan(cdf_fcst).any(dim=threshold_dim)  # type: ignore
+        & ~np.isnan(cdf_obs).any(dim=threshold_dim)  # type: ignore
+        & ~np.isnan(threshold_weight).any(dim=threshold_dim)  # type: ignore
     )
 
     # total error measured by CRPS
     total = (threshold_weight * (cdf_fcst - cdf_obs) ** 2).integrate(threshold_dim).where(inputs_without_nan)
 
     over = (cdf_obs * threshold_weight * (cdf_fcst - cdf_obs) ** 2).integrate(threshold_dim).where(inputs_without_nan)
 
@@ -693,14 +702,15 @@
 
     return result
 
 
 def crps_step_threshold_weight(
     step_points: xr.DataArray,
     threshold_dim: str,
+    *,  # Force keywords arguments to be keyword-only
     threshold_values: Optional[Iterable[float]] = None,
     steppoints_in_thresholds: bool = True,
     steppoint_precision: float = 0,
     weight_upper: bool = True,
 ) -> xr.DataArray:
     """Generates an array of weights based on DataArray step points.
 
@@ -739,18 +749,19 @@
     return weight
 
 
 def crps_for_ensemble(
     fcst: xr.DataArray,
     obs: xr.DataArray,
     ensemble_member_dim: str,
+    *,  # Force keywords arguments to be keyword-only
     method: Literal["ecdf", "fair"] = "ecdf",
     reduce_dims: Optional[Sequence[str]] = None,
     preserve_dims: Optional[Sequence[str]] = None,
-    weights: xr.DataArray = None,
+    weights: Optional[xr.DataArray] = None,
 ) -> xr.DataArray:
     """Calculates the CRPS probabilistic metric given ensemble input.
 
     Calculates the continuous ranked probability score (CRPS) given an ensemble of forecasts.
     An ensemble of forecasts can also be thought of as a random sample from the predictive
     distribution.
 
@@ -811,24 +822,24 @@
         preserve_dims=preserve_dims,
         special_fcst_dims=ensemble_member_dim,
     )
 
     ensemble_member_dim1 = scores.utils.tmp_coord_name(fcst)
 
     # calculate forecast spread contribution
-    fcst_copy = fcst.rename({ensemble_member_dim: ensemble_member_dim1})
+    fcst_copy = fcst.rename({ensemble_member_dim: ensemble_member_dim1})  # type: ignore
 
-    fcst_spread_term = np.abs(fcst - fcst_copy).sum([ensemble_member_dim, ensemble_member_dim1])
+    fcst_spread_term = abs(fcst - fcst_copy).sum(dim=[ensemble_member_dim, ensemble_member_dim1])  # type: ignore
     ens_count = fcst.count(ensemble_member_dim)
     if method == "ecdf":
         fcst_spread_term = fcst_spread_term / (2 * ens_count**2)
     if method == "fair":
         fcst_spread_term = fcst_spread_term / (2 * ens_count * (ens_count - 1))
 
     # calculate final CRPS for each forecast case
-    fcst_obs_term = np.abs(fcst - obs).mean(ensemble_member_dim)
+    fcst_obs_term = abs(fcst - obs).mean(dim=ensemble_member_dim)
     result = fcst_obs_term - fcst_spread_term
 
     # apply weights and take means across specified dims
-    result = scores.functions.apply_weights(result, weights).mean(dim=dims_for_mean)
+    result = scores.functions.apply_weights(result, weights=weights).mean(dim=dims_for_mean)  # type: ignore
 
-    return result
+    return result  # type: ignore
```

### Comparing `scores-0.6/src/scores/probability/functions.py` & `scores-0.7/src/scores/processing/cdf/cdf_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """
 This module contains a variety of functions which modify data in various ways to process data structures
-to support probablistic verification.
+to support probabilistic verification.
 """
+
 from collections.abc import Iterable
 from typing import Literal, Optional
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 
 from scores.probability.checks import (
     cdf_values_within_bounds,
     check_nan_decreasing_inputs,
 )
 from scores.typing import XarrayLike
 
 
-def round_values(array: xr.DataArray, rounding_precision: float, final_round_decpl: int = 7) -> xr.DataArray:
+def round_values(array: xr.DataArray, rounding_precision: float, *, final_round_decpl: int = 7) -> xr.DataArray:
     """Round data array to specified precision.
 
     Rounding is done differently to `xarray.DataArray.round` or `numpy.round` where
     the number of decimal places is specified in those cases. Instead, here the rounding
     precision is specified as a float. The value is rounded to the nearest value that is
     divisible by `rounding_precision`.
 
@@ -74,14 +75,15 @@
     result = cdf.where(~where_nan, np.nan)
     return result
 
 
 def observed_cdf(
     obs: xr.DataArray,
     threshold_dim: str,
+    *,  # Force keywords arguments to be keyword-only
     threshold_values: Optional[Iterable[float]] = None,
     include_obs_in_thresholds: bool = True,
     precision: float = 0,
 ) -> xr.DataArray:
     """Returns a data array of observations converted into CDF format.
 
     Such that:
@@ -114,20 +116,23 @@
 
     if precision > 0:
         obs = round_values(obs, precision)
 
     thresholds = threshold_values_as_array if threshold_values is not None else []
 
     if include_obs_in_thresholds:
-        thresholds = np.concatenate((obs.values.flatten(), thresholds))
+        thresholds = np.concatenate((obs.values.flatten(), thresholds))  # type: ignore
 
     # remove any NaN
-    thresholds = [x for x in thresholds if not np.isnan(x)]
+    thresholds = [x for x in thresholds if not np.isnan(x)]  # type: ignore
 
-    thresholds = np.sort(pd.unique(thresholds))
+    # pandas.unique retains the original ordering whereas set() may not
+    # pandas.unique no longer accepts a simple array as input
+    thresholds = pd.Series(thresholds)
+    thresholds = np.sort(pd.unique(thresholds))  # type: ignore
 
     da_thresholds = xr.DataArray(
         thresholds,
         dims=[threshold_dim],
         coords={threshold_dim: thresholds},
     )
 
@@ -164,24 +169,24 @@
         xr.DataArray: Integral values and `threshold_dim` collapsed.
     """
 
     # notation: Since F is piecewise linear we have
     # F(t) = mt + b, whenever x[i-1] <= t <= x[i].
 
     # difference in x
-    diff_xs = function_values[threshold_dim] - function_values[threshold_dim].shift(**{threshold_dim: 1})
+    diff_xs = function_values[threshold_dim] - function_values[threshold_dim].shift(**{threshold_dim: 1})  # type: ignore
 
     # difference in function values
-    diff_ys = function_values - function_values.shift(**{threshold_dim: 1})
+    diff_ys = function_values - function_values.shift(**{threshold_dim: 1})  # type: ignore
 
     # gradients m
     m_values = diff_ys / diff_xs
 
     # y intercepts b
-    b_values = function_values.shift(**{threshold_dim: 1})
+    b_values = function_values.shift(**{threshold_dim: 1})  # type: ignore
 
     # integral for x[i-1] <= t <= x[i]
     piece_integral = (
         (m_values**2) * (diff_xs**3) / 3 + m_values * b_values * (diff_xs**2) + (b_values**2) * diff_xs
     )
 
     # Need at least one non-NaN piece_integral to return float.
@@ -190,14 +195,15 @@
 
 
 def add_thresholds(
     cdf: xr.DataArray,
     threshold_dim: str,
     new_thresholds: Iterable[float],
     fill_method: Literal["linear", "step", "forward", "backward", "none"],
+    *,  # Force keywords arguments to be keyword-only
     min_nonnan: int = 2,
 ) -> xr.DataArray:
     """Takes a CDF data array with dimension `threshold_dim` and adds values from `new_thresholds`.
 
     The CDF is then filled to replace any NaN values.
     The array `cdf` requires at least 2 non-NaN values along `threshold_dim`.
 
@@ -210,15 +216,15 @@
         min_nonnan (int): passed onto `fill_cdf` for performing filling.
 
     Returns:
         xr.DataArray: Additional thresholds, and values at those thresholds
         determined by the specified fill method.
     """
 
-    thresholds = np.concatenate((cdf[threshold_dim].values, new_thresholds))
+    thresholds = np.concatenate((cdf[threshold_dim].values, new_thresholds))  # type: ignore
     thresholds = np.sort(pd.unique(thresholds))
     thresholds = thresholds[~np.isnan(thresholds)]
 
     da_thresholds = xr.DataArray(data=thresholds, dims=[threshold_dim], coords={threshold_dim: thresholds})
 
     da_cdf = xr.broadcast(cdf, da_thresholds)[0]
 
@@ -327,15 +333,15 @@
         ValueError: If `tolerance` is negative.
         ValueError: If coordinates are not increasing along `threshold_dim`.
         ValueError: If some, but not all, CDF values in `cdf` along `threshold_dim` are NaN.
     """
     check_nan_decreasing_inputs(cdf, threshold_dim, tolerance)
 
     # difference between consecutive terms along threshold_dim
-    diff = cdf - cdf.shift(**{threshold_dim: 1})
+    diff = cdf - cdf.shift(**{threshold_dim: 1})  # type: ignore
 
     result = diff.clip(max=0).sum(dim=threshold_dim) < -tolerance
 
     return result
 
 
 def cdf_envelope(
```

### Comparing `scores-0.6/src/scores/probability/roc_impl.py` & `scores-0.7/src/scores/probability/roc_impl.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Implementation of Reciever Operating Characteristic (ROC) calculations
 """
+
 from collections.abc import Iterable, Sequence
 from typing import Optional
 
 import numpy as np
 import xarray as xr
 
 from scores.categorical import probability_of_detection, probability_of_false_detection
@@ -12,14 +13,15 @@
 from scores.utils import gather_dimensions
 
 
 def roc_curve_data(  # pylint: disable=too-many-arguments
     fcst: xr.DataArray,
     obs: xr.DataArray,
     thresholds: Iterable[float],
+    *,  # Force keywords arguments to be keyword-only
     reduce_dims: Optional[Sequence[str]] = None,
     preserve_dims: Optional[Sequence[str]] = None,
     weights: Optional[xr.DataArray] = None,
     check_args: bool = True,
 ) -> xr.Dataset:
     """
     Calculates data required for plotting a Receiver (Relative) Operating Characteristic (ROC)
@@ -76,22 +78,22 @@
         Ideally concave ROC curves should be generated rather than traditional
         ROC curves.
 
     Raises:
         ValueError: if `fcst` contains values outside of the range [0, 1]
         ValueError: if `obs` contains non-nan values not in the set {0, 1}
         ValueError: if 'threshold' is a dimension in `fcst`.
-        ValueError: if values in `thresholds` are not montonic increasing or are outside
+        ValueError: if values in `thresholds` are not monotonic increasing or are outside
           the range [0, 1]
     """
     if check_args:
         if fcst.max().item() > 1 or fcst.min().item() < 0:
             raise ValueError("`fcst` contains values outside of the range [0, 1]")
 
-        if np.max(thresholds) > 1 or np.min(thresholds) < 0:
+        if np.max(thresholds) > 1 or np.min(thresholds) < 0:  # type: ignore
             raise ValueError("`thresholds` contains values outside of the range [0, 1]")
 
         if not np.all(np.array(thresholds)[1:] >= np.array(thresholds)[:-1]):
             raise ValueError("`thresholds` is not monotonic increasing between 0 and 1")
 
     # make a discrete forecast for each threshold in thresholds
     # discrete_fcst has an extra dimension 'threshold'
@@ -115,13 +117,13 @@
     pod = pod.transpose(*final_preserve_dims)
     pofd = pofd.transpose(*final_preserve_dims)
 
     auc = -1 * xr.apply_ufunc(
         np.trapz,
         pod,
         pofd,
-        input_core_dims=[pod.dims, pofd.dims],
+        input_core_dims=[pod.dims, pofd.dims],  # type: ignore
         output_core_dims=[auc_dims],
         dask="parallelized",
     )
 
     return xr.Dataset({"POD": pod, "POFD": pofd, "AUC": auc})
```

### Comparing `scores-0.6/src/scores/stats/statistical_tests/acovf.py` & `scores-0.7/src/scores/stats/statistical_tests/acovf.py`

 * *Files identical despite different names*

### Comparing `scores-0.6/src/scores/stats/statistical_tests/diebold_mariano_impl.py` & `scores-0.7/src/scores/stats/statistical_tests/diebold_mariano_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from scores.utils import dims_complement
 
 
 def diebold_mariano(  # pylint: disable=R0914
     da_timeseries: xr.DataArray,
     ts_dim: str,
     h_coord: str,
+    *,  # Force keywords arguments to be keyword-only
     method: Literal["HG", "HLN"] = "HG",
     confidence_level: float = 0.95,
     statistic_distribution: Literal["normal", "t"] = "normal",
 ) -> xr.Dataset:
     """
     Given an array of (multiple) timeseries, with each timeseries consisting of score
     differences for h-step ahead forecasts, calculates a modified Diebold-Mariano test
@@ -154,29 +155,29 @@
     # It allows values like 7.0 to pass, which is OK for the application.
     if any(da_timeseries[h_coord].values % 1 != 0):
         raise ValueError("Every value in `da_timeseries[h_coord]` must be an integer.")
 
     if (da_timeseries[h_coord] <= 0).any():
         raise ValueError("Every value in `da_timeseries[h_coord]` must be positive.")
 
-    other_dim = dims_complement(da_timeseries, [ts_dim])[0]
+    other_dim = dims_complement(da_timeseries, dims=[ts_dim])[0]
     da_timeseries_len = da_timeseries.count(other_dim)
 
     if (da_timeseries_len <= da_timeseries[h_coord]).any():
         msg = "Each `h_coord` value must be less than the length of the corresponding timeseries"
         raise ValueError(msg + " after NaNs are removed")
 
     ts_dim_len = len(da_timeseries[ts_dim])
     test_stats = np.empty([ts_dim_len])
     ts_mean = da_timeseries.mean(other_dim).values
 
     for i in range(ts_dim_len):
         timeseries = da_timeseries.isel({ts_dim: i})
         h = int(timeseries[h_coord])
-        test_stats[i] = _dm_test_statistic(timeseries.values, h, method)
+        test_stats[i] = _dm_test_statistic(timeseries.values, h, method=method)
 
     if statistic_distribution == "normal":
         pvals = sp.stats.norm.cdf(test_stats)
         ci_quantile = sp.stats.norm.ppf(1 - (1 - confidence_level) / 2)
     else:
         pvals = sp.stats.t.cdf(test_stats, da_timeseries_len.values - 1)
         ci_quantile = sp.stats.t.ppf(1 - (1 - confidence_level) / 2, da_timeseries_len.values - 1)
@@ -192,15 +193,15 @@
         },
         coords={ts_dim: da_timeseries[ts_dim].values},
     )
 
     return result
 
 
-def _dm_test_statistic(diffs: np.ndarray, h: int, method: Literal["HG", "HLN"] = "HG") -> float:
+def _dm_test_statistic(diffs: np.ndarray, h: int, *, method: Literal["HG", "HLN"] = "HG") -> float:
     """
     Given a timeseries of score differences for h-step ahead forecasts, as a 1D numpy
     array, returns a modified Diebold-Mariano test statistic. NaNs are removed prior
     to computing the statistic.
 
     Two methods for computing the test statistic can be used: either the "HLN" method of
     Harvey, Leybourne and Newbold (1997), or "HG" method of Hering and Genton (2011).
@@ -289,15 +290,15 @@
     Returns:
         Difference between modelled and empirical autocoveriances.
 
     References:
         Hering and Genton, 'Comparing spatial predictions',
         Technometrics 53 no. 4 (2011), 414-425.
     """
-    return (pars[0] ** 2) * np.exp(-3 * lag / pars[1]) - acv  # ignore: type
+    return (pars[0] ** 2) * np.exp(-3 * lag / pars[1]) - acv  # type: ignore
 
 
 def _hg_method_stat(diffs: np.ndarray, h: int) -> float:
     """
     Calculates the modified Diebold-Mariano test statistic using the "HG" method.
     Assumes that h < len(diffs).
 
@@ -391,10 +392,10 @@
     summands = np.empty(h - 1)
     for k in range(h - 1):
         summands[k] = _dm_gamma_hat_k(diffs, diffs_bar, n, k + 1)
 
     result = (_dm_gamma_hat_k(diffs, diffs_bar, n, 0) + 2 * np.sum(summands)) / n**2
 
     if result <= 0:
-        result = np.nan
+        result = np.nan  # type: ignore
 
     return result  # type: ignore
```

### Comparing `scores-0.6/LICENSE` & `scores-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scores-0.6/README.md` & `scores-0.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 # About the Scores Project
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nci/scores/HEAD?labpath=tutorials%2FExplanation.ipynb)
 
-One-line intro: xarray based verification (accuracy) scoring that can scale with Dask if needed. Pandas supported where possible.
+One-line intro: xarray based verification scores and tools that can scale with Dask if needed. Pandas supported where possible.
 Why use it: trusted implementations, novel metrics, performance, one-stop-shop.
 
-Currently Included Metrics and Tools:
+A **complete list** of the 47 included Metrics, Statistical Techniques and Data Processing Tools is: [available here](https://scores.readthedocs.io/en/develop/included.html).
+
+Here is a **curated selection** of the Metrics and Tools included in `scores`:
 
 | continuous                      | probability | categorical      | statistical tests |
 | ----------                      | ----------- | -----------      | ----------------- |
-| MAE, MSE, RMSE, Flip Flop Index, Quantile Score, Isotonic Regression, Pearsons correlation coefficient  | CRPS for CDF, CRPS for ensemble, ROC, Brier score   | FIRM, POD, POFD  |  Diebold Mariano (with the Harvey et al. 1997 and the Hering and Genton 2011 modifications) |
+| MAE, MSE, RMSE, Flip-Flop Index, Quantile Score, Murphy score, Pearson's Correlation Coefficient, Additive Bias, Multiplicative Bias  | CRPS for CDF, CRPS for ensemble, ROC, Brier Score, Isotonic Regression (reliability diagrams)   | FIRM, Hit Rate, Probability of False Detection, Success Ratio, Peirce's Skill Score  |  Diebold Mariano (with the Harvey et al. 1997 and the Hering and Genton 2011 modifications) |
 
 **Notice -- This repository is currently undergoing initial construction and maintenance. It is getting much closer to our goals for version one, but there are a few more things to add. This notice will be removed after the first feature release. In the meantime, please feel free to look around, and don't hesitate to get in touch with any questions (see the contributing guide for how).**
 
 Documentation is hosted at [scores.readthedocs.io](https://scores.readthedocs.io).  
 Source code is hosted at [github.com/nci/scores](https://github.com/nci/scores).  
 The tutorial gallery is hosted at [as part of the documentation, here](https://scores.readthedocs.io/en/latest/tutorials/Explanation.html).
 
-`scores` is a Python package containing mathematical functions for the verification, evaluation, and optimisation of model outputs and predictions. It primarily supports the geoscience and earth system science communities. It also has wide potential application in machine learning, and in domains other than meteorology, geoscience and weather.
+`scores` is a Python package containing mathematical functions for the verification, evaluation, and optimisation of forecasts, predictions or models. It primarily supports the geoscience and earth system science communities. It also has wide potential application in machine learning, and in domains other than meteorology, geoscience and weather.
 
-`scores` includes novel scores not commonly found elsewhere (e.g. FIRM, FlipFlop Index), complex scores (e.g. CRPS), more common scores (e.g. MAE, RMSE) and statistical tests (such as the Diebold Mariano test). `scores` provides its own implementations where relevant to avoid extensive dependencies.
+`scores` includes novel scores not commonly found elsewhere (e.g. FIRM, Flip-Flop Index), complex scores (e.g. threshold weighted CRPS), more common scores (e.g. MAE, RMSE) and statistical tests (such as the Diebold Mariano test). Additionally, it provides pre-processing tools for preparing data for scores in a variety of formats including Cumulative Density Functions (CDF). `scores` provides its own implementations where relevant to avoid extensive dependencies.
 
-`scores` is focused on supporting xarray datatypes for earth system data. It also aims to be compatible with pandas, geopandas, pangeo and work with NetCDF4, hdf5, Zarr and GRIB data sources among others. `scores` is designed to utilise Dask for scaling and performance.
+`scores` is focused on supporting xarray datatypes for earth system data. It also aims to be compatible with pandas, geopandas, pangeo and work with NetCDF4, hdf5, Zarr and GRIB data sources among others. `scores` is designed to use Dask for scaling and performance.
 
 All of the scores and metrics in this package have undergone a thorough statistical and scientific review. Every score has a companion Jupyter Notebook tutorial demonstrating its use in practice.
 
+## Contributing
+To find out more about contributing, see our [contributor's guide](https://github.com/nci/scores/blob/develop/docs/contributing.md).
+
 All interactions in discussions, issues, emails and code (e.g. merge requests, code comments) will be managed according to the expectations outlined in the [ code of conduct ](https://github.com/nci/scores/blob/main/CODE_OF_CONDUCT.md) and in accordance with all relevant laws and obligations. This project is an inclusive, respectful and open project with high standards for respectful behaviour and language. The code of conduct is the Contributor Covenant, adopted by over 40, 000 open source projects. Any concerns will be dealt with fairly and respectfully, with the processes described in the code of conduct.
 
 ## Using This Package
 
 The [installation guide](https://scores.readthedocs.io/en/latest/installation.html) describes four different use cases for installing, using and working with this package.
 
 Most users currently want the *all* installation option. This includes the mathematical functions (scores, metrics, statistical tests etc.), the tutorial notebooks and development libraries.
```

### Comparing `scores-0.6/pyproject.toml` & `scores-0.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     "pytest",
     "pytest-watch",
     "pytest-cov",
     "pre-commit",
     "black == 23.3.0",
     "mypy == 1.3.0",
     "pylint == 3.0.1",
+    "bandit == 1.7.8",
     "dask",
     "h5netcdf",
     "pandas-stubs",
     "nbmake"
 ]
 tutorial = [
     "jupyterlab",
@@ -50,15 +51,18 @@
     "plotly"
 ]
 maintainer = ["build",
               "hatch",
               "sphinx",
               "myst-parser",
               "sphinx-book-theme",
+              "nbsphinx",
+              "sphinx_gallery",
               "twine",
+              "pandoc",
               "pip-tools",
 ]
 all = ["scores[dev,tutorial]"]
 
 [project.urls]
 "Homepage" = "http://www.bom.gov.au"
 
@@ -78,15 +82,21 @@
 [tool.black]
 line-length = 120
 
 [tool.mypy]
 warn_return_any = true
 warn_unused_configs = true
 
-#ignore_missing_imports = true
+[[tool.mypy.overrides]]
+module = "scipy.*"
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = "sklearn.*"
+ignore_missing_imports = true
 
 [tool.coverage.paths]
 source = ["/src/"]
 
 [tool.coverage.report]
 exclude_also = [
     "@overload",
@@ -104,15 +114,16 @@
     '--cov-report=term-missing',
     '--junitxml=report.xml',
     # Ignore notebooks which depend on external data for E2E tests
     '--ignore=tutorials/First_Data_Fetching.ipynb',
     '--ignore=tutorials/Mean_Squared_Error.ipynb',
     '--ignore=tutorials/Root_Mean_Squared_Error.ipynb',
     '--ignore=tutorials/Weighting_Results.ipynb',
-    '--ignore=tutorials/Mean_Absolute_Error.ipynb'
+    '--ignore=tutorials/Mean_Absolute_Error.ipynb',
+    '--ignore=tutorials/Additive_and_multiplicative_bias.ipynb'
 ]
 
 [tool.pylint.master]
 # https://github.com/PyCQA/pylint/issues/4081#issuecomment-778242554
 init-hook = 'import sys; sys.setrecursionlimit(3 * sys.getrecursionlimit())'
 fail-under=9.8
 ignore-paths = [
```

### Comparing `scores-0.6/PKG-INFO` & `scores-0.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,43 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: scores
-Version: 0.6
+Version: 0.7
 Summary: Scores is a package containing mathematical functions for the verification, evaluation and optimisation of model outputs and predictions.
 Project-URL: Homepage, http://www.bom.gov.au
 Author-email: Tennessee Leeuwenburg <tennessee.leeuwenburg@bom.gov.au>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: bottleneck
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: xarray
 Provides-Extra: all
-Requires-Dist: scores[dev,tutorial]; extra == 'all'
+Requires-Dist: bandit==1.7.8; extra == 'all'
+Requires-Dist: black==23.3.0; extra == 'all'
+Requires-Dist: dask; extra == 'all'
+Requires-Dist: h5netcdf; extra == 'all'
+Requires-Dist: jupyterlab; extra == 'all'
+Requires-Dist: matplotlib; extra == 'all'
+Requires-Dist: mypy==1.3.0; extra == 'all'
+Requires-Dist: nbmake; extra == 'all'
+Requires-Dist: pandas-stubs; extra == 'all'
+Requires-Dist: plotly; extra == 'all'
+Requires-Dist: pre-commit; extra == 'all'
+Requires-Dist: pylint==3.0.1; extra == 'all'
+Requires-Dist: pytest; extra == 'all'
+Requires-Dist: pytest-cov; extra == 'all'
+Requires-Dist: pytest-watch; extra == 'all'
+Requires-Dist: rasterio; extra == 'all'
+Requires-Dist: rioxarray; extra == 'all'
 Provides-Extra: dev
+Requires-Dist: bandit==1.7.8; extra == 'dev'
 Requires-Dist: black==23.3.0; extra == 'dev'
 Requires-Dist: dask; extra == 'dev'
 Requires-Dist: h5netcdf; extra == 'dev'
 Requires-Dist: mypy==1.3.0; extra == 'dev'
 Requires-Dist: nbmake; extra == 'dev'
 Requires-Dist: pandas-stubs; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
@@ -28,54 +45,62 @@
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: pytest-watch; extra == 'dev'
 Provides-Extra: maintainer
 Requires-Dist: build; extra == 'maintainer'
 Requires-Dist: hatch; extra == 'maintainer'
 Requires-Dist: myst-parser; extra == 'maintainer'
+Requires-Dist: nbsphinx; extra == 'maintainer'
+Requires-Dist: pandoc; extra == 'maintainer'
 Requires-Dist: pip-tools; extra == 'maintainer'
 Requires-Dist: sphinx; extra == 'maintainer'
 Requires-Dist: sphinx-book-theme; extra == 'maintainer'
+Requires-Dist: sphinx-gallery; extra == 'maintainer'
 Requires-Dist: twine; extra == 'maintainer'
 Provides-Extra: tutorial
 Requires-Dist: h5netcdf; extra == 'tutorial'
 Requires-Dist: jupyterlab; extra == 'tutorial'
 Requires-Dist: matplotlib; extra == 'tutorial'
 Requires-Dist: plotly; extra == 'tutorial'
 Requires-Dist: rasterio; extra == 'tutorial'
 Requires-Dist: rioxarray; extra == 'tutorial'
 Description-Content-Type: text/markdown
 
 # About the Scores Project
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nci/scores/HEAD?labpath=tutorials%2FExplanation.ipynb)
 
-One-line intro: xarray based verification (accuracy) scoring that can scale with Dask if needed. Pandas supported where possible.
+One-line intro: xarray based verification scores and tools that can scale with Dask if needed. Pandas supported where possible.
 Why use it: trusted implementations, novel metrics, performance, one-stop-shop.
 
-Currently Included Metrics and Tools:
+A **complete list** of the 47 included Metrics, Statistical Techniques and Data Processing Tools is: [available here](https://scores.readthedocs.io/en/develop/included.html).
+
+Here is a **curated selection** of the Metrics and Tools included in `scores`:
 
 | continuous                      | probability | categorical      | statistical tests |
 | ----------                      | ----------- | -----------      | ----------------- |
-| MAE, MSE, RMSE, Flip Flop Index, Quantile Score, Isotonic Regression, Pearsons correlation coefficient  | CRPS for CDF, CRPS for ensemble, ROC, Brier score   | FIRM, POD, POFD  |  Diebold Mariano (with the Harvey et al. 1997 and the Hering and Genton 2011 modifications) |
+| MAE, MSE, RMSE, Flip-Flop Index, Quantile Score, Murphy score, Pearson's Correlation Coefficient, Additive Bias, Multiplicative Bias  | CRPS for CDF, CRPS for ensemble, ROC, Brier Score, Isotonic Regression (reliability diagrams)   | FIRM, Hit Rate, Probability of False Detection, Success Ratio, Peirce's Skill Score  |  Diebold Mariano (with the Harvey et al. 1997 and the Hering and Genton 2011 modifications) |
 
 **Notice -- This repository is currently undergoing initial construction and maintenance. It is getting much closer to our goals for version one, but there are a few more things to add. This notice will be removed after the first feature release. In the meantime, please feel free to look around, and don't hesitate to get in touch with any questions (see the contributing guide for how).**
 
 Documentation is hosted at [scores.readthedocs.io](https://scores.readthedocs.io).  
 Source code is hosted at [github.com/nci/scores](https://github.com/nci/scores).  
 The tutorial gallery is hosted at [as part of the documentation, here](https://scores.readthedocs.io/en/latest/tutorials/Explanation.html).
 
-`scores` is a Python package containing mathematical functions for the verification, evaluation, and optimisation of model outputs and predictions. It primarily supports the geoscience and earth system science communities. It also has wide potential application in machine learning, and in domains other than meteorology, geoscience and weather.
+`scores` is a Python package containing mathematical functions for the verification, evaluation, and optimisation of forecasts, predictions or models. It primarily supports the geoscience and earth system science communities. It also has wide potential application in machine learning, and in domains other than meteorology, geoscience and weather.
 
-`scores` includes novel scores not commonly found elsewhere (e.g. FIRM, FlipFlop Index), complex scores (e.g. CRPS), more common scores (e.g. MAE, RMSE) and statistical tests (such as the Diebold Mariano test). `scores` provides its own implementations where relevant to avoid extensive dependencies.
+`scores` includes novel scores not commonly found elsewhere (e.g. FIRM, Flip-Flop Index), complex scores (e.g. threshold weighted CRPS), more common scores (e.g. MAE, RMSE) and statistical tests (such as the Diebold Mariano test). Additionally, it provides pre-processing tools for preparing data for scores in a variety of formats including Cumulative Density Functions (CDF). `scores` provides its own implementations where relevant to avoid extensive dependencies.
 
-`scores` is focused on supporting xarray datatypes for earth system data. It also aims to be compatible with pandas, geopandas, pangeo and work with NetCDF4, hdf5, Zarr and GRIB data sources among others. `scores` is designed to utilise Dask for scaling and performance.
+`scores` is focused on supporting xarray datatypes for earth system data. It also aims to be compatible with pandas, geopandas, pangeo and work with NetCDF4, hdf5, Zarr and GRIB data sources among others. `scores` is designed to use Dask for scaling and performance.
 
 All of the scores and metrics in this package have undergone a thorough statistical and scientific review. Every score has a companion Jupyter Notebook tutorial demonstrating its use in practice.
 
+## Contributing
+To find out more about contributing, see our [contributor's guide](https://github.com/nci/scores/blob/develop/docs/contributing.md).
+
 All interactions in discussions, issues, emails and code (e.g. merge requests, code comments) will be managed according to the expectations outlined in the [ code of conduct ](https://github.com/nci/scores/blob/main/CODE_OF_CONDUCT.md) and in accordance with all relevant laws and obligations. This project is an inclusive, respectful and open project with high standards for respectful behaviour and language. The code of conduct is the Contributor Covenant, adopted by over 40, 000 open source projects. Any concerns will be dealt with fairly and respectfully, with the processes described in the code of conduct.
 
 ## Using This Package
 
 The [installation guide](https://scores.readthedocs.io/en/latest/installation.html) describes four different use cases for installing, using and working with this package.
 
 Most users currently want the *all* installation option. This includes the mathematical functions (scores, metrics, statistical tests etc.), the tutorial notebooks and development libraries.
```

