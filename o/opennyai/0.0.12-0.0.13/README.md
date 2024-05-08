# Comparing `tmp/opennyai-0.0.12.tar.gz` & `tmp/opennyai-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opennyai-0.0.12.tar", max compression
+gzip compressed data, was "opennyai-0.0.13.tar", max compression
```

## Comparing `opennyai-0.0.12.tar` & `opennyai-0.0.13.tar`

### file list

```diff
@@ -1,241 +1,241 @@
--rw-r--r--   0        0        0     1096 2022-12-01 20:08:59.808342 opennyai-0.0.12/LICENSE
--rw-r--r--   0        0        0     5069 2023-11-09 17:52:00.567874 opennyai-0.0.12/README.md
--rw-r--r--   0        0        0      330 2023-11-09 17:35:19.017196 opennyai-0.0.12/opennyai/__init__.py
--rw-r--r--   0        0        0     5719 2022-12-07 05:10:07.210614 opennyai-0.0.12/opennyai/ner/InLegalNER/InLegalNER.py
--rw-r--r--   0        0        0        0 2022-11-10 10:57:46.006446 opennyai-0.0.12/opennyai/ner/InLegalNER/__init__.py
--rw-r--r--   0        0        0     4215 2023-11-09 17:22:42.274538 opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/InLegalNER.cpython-310.pyc
--rw-r--r--   0        0        0     6323 2023-11-09 16:42:27.015474 opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/InLegalNER.cpython-311.pyc
--rw-r--r--   0        0        0     4237 2023-11-09 15:48:08.054676 opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/InLegalNER.cpython-38.pyc
--rw-r--r--   0        0        0     4237 2022-12-21 05:08:43.888318 opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/InLegalNER.cpython-39.pyc
--rw-r--r--   0        0        0      164 2023-11-09 17:22:42.272549 opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      180 2023-11-09 16:42:27.012417 opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      162 2023-11-09 15:48:08.053503 opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      162 2022-11-10 11:04:23.353830 opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1259 2023-11-09 17:23:10.202604 opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/entity_recognizer_utils.cpython-310.pyc
--rw-r--r--   0        0        0     1231 2023-11-09 15:51:07.096047 opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/entity_recognizer_utils.cpython-38.pyc
--rw-r--r--   0        0        0     1247 2022-11-11 05:17:23.178038 opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/entity_recognizer_utils.cpython-39.pyc
--rw-r--r--   0        0        0    27867 2023-11-09 17:23:10.212242 opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/postprocessing_utils.cpython-310.pyc
--rw-r--r--   0        0        0    28203 2023-11-09 15:51:07.104504 opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/postprocessing_utils.cpython-38.pyc
--rw-r--r--   0        0        0    28079 2023-11-09 17:16:27.130090 opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/postprocessing_utils.cpython-39.pyc
--rw-r--r--   0        0        0     1195 2022-11-11 05:15:03.882432 opennyai-0.0.12/opennyai/ner/InLegalNER/entity_recognizer_utils.py
--rw-r--r--   0        0        0    44209 2023-11-09 15:26:19.714769 opennyai-0.0.12/opennyai/ner/InLegalNER/postprocessing_utils.py
--rw-r--r--   0        0        0      171 2022-11-10 10:57:46.007110 opennyai-0.0.12/opennyai/ner/__init__.py
--rw-r--r--   0        0        0      382 2023-11-09 17:22:21.648342 opennyai-0.0.12/opennyai/ner/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      488 2023-11-09 16:42:18.604183 opennyai-0.0.12/opennyai/ner/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      380 2023-11-09 15:45:23.707942 opennyai-0.0.12/opennyai/ner/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      380 2022-11-10 11:04:21.860264 opennyai-0.0.12/opennyai/ner/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5197 2023-11-09 17:22:21.650927 opennyai-0.0.12/opennyai/ner/__pycache__/ner_utils.cpython-310.pyc
--rw-r--r--   0        0        0     9578 2023-11-09 16:42:18.607212 opennyai-0.0.12/opennyai/ner/__pycache__/ner_utils.cpython-311.pyc
--rw-r--r--   0        0        0     5355 2023-11-09 15:45:23.709738 opennyai-0.0.12/opennyai/ner/__pycache__/ner_utils.cpython-38.pyc
--rw-r--r--   0        0        0     5345 2023-11-09 17:15:40.566344 opennyai-0.0.12/opennyai/ner/__pycache__/ner_utils.cpython-39.pyc
--rw-r--r--   0        0        0     6868 2023-11-09 15:26:19.716495 opennyai-0.0.12/opennyai/ner/ner_utils.py
--rw-r--r--   0        0        0     7055 2022-12-01 20:04:30.660403 opennyai-0.0.12/opennyai/pipeline.py
--rw-r--r--   0        0        0        0 2022-11-10 10:57:46.007640 opennyai-0.0.12/opennyai/rhetorical_roles/__init__.py
--rw-r--r--   0        0        0      166 2023-11-09 17:23:12.176935 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      164 2023-11-09 16:05:06.517614 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      164 2022-11-10 11:04:26.100434 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3561 2023-11-09 17:23:42.168397 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/batch_creator.cpython-310.pyc
--rw-r--r--   0        0        0     3553 2023-11-09 16:05:08.531732 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/batch_creator.cpython-38.pyc
--rw-r--r--   0        0        0     3549 2022-12-01 19:34:02.997994 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/batch_creator.cpython-39.pyc
--rw-r--r--   0        0        0     4506 2023-11-09 17:23:42.170541 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/bucketing.cpython-310.pyc
--rw-r--r--   0        0        0     4500 2023-11-09 16:05:08.532780 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/bucketing.cpython-38.pyc
--rw-r--r--   0        0        0     4486 2022-11-10 11:04:26.484136 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/bucketing.cpython-39.pyc
--rw-r--r--   0        0        0     2327 2023-11-09 17:23:42.172583 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/dataset_reader.cpython-310.pyc
--rw-r--r--   0        0        0     2295 2023-11-09 16:05:08.533552 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/dataset_reader.cpython-38.pyc
--rw-r--r--   0        0        0     2319 2022-11-10 11:04:26.485087 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/dataset_reader.cpython-39.pyc
--rw-r--r--   0        0        0     1486 2023-11-09 17:23:13.758512 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/eval.cpython-310.pyc
--rw-r--r--   0        0        0     1474 2023-11-09 16:05:07.222366 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/eval.cpython-38.pyc
--rw-r--r--   0        0        0     1478 2022-11-10 11:04:26.468026 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/eval.cpython-39.pyc
--rw-r--r--   0        0        0     3410 2023-11-09 17:23:13.757100 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/infer_data_prep.cpython-310.pyc
--rw-r--r--   0        0        0     3292 2023-11-09 16:05:07.221555 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/infer_data_prep.cpython-38.pyc
--rw-r--r--   0        0        0     3392 2022-11-10 11:04:26.467171 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/infer_data_prep.cpython-39.pyc
--rw-r--r--   0        0        0    12466 2023-11-09 17:23:13.543350 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/models.cpython-310.pyc
--rw-r--r--   0        0        0    12534 2023-11-09 16:05:07.088215 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/models.cpython-38.pyc
--rw-r--r--   0        0        0    12499 2022-12-06 11:29:27.242731 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/models.cpython-39.pyc
--rw-r--r--   0        0        0     4486 2023-11-09 17:23:12.179713 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/rhetorical_roles.cpython-310.pyc
--rw-r--r--   0        0        0     4438 2023-11-09 16:05:06.519678 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/rhetorical_roles.cpython-38.pyc
--rw-r--r--   0        0        0     4482 2022-12-01 06:22:58.082509 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/rhetorical_roles.cpython-39.pyc
--rw-r--r--   0        0        0     6270 2023-11-09 17:23:13.821659 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     6388 2023-11-09 16:05:07.267886 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/task.cpython-38.pyc
--rw-r--r--   0        0        0     6305 2022-11-10 11:04:26.481407 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/task.cpython-39.pyc
--rw-r--r--   0        0        0     2946 2023-11-09 17:23:13.760022 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0     2836 2023-11-09 16:05:07.223308 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0     2888 2022-11-10 11:04:26.469021 opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0        0        0        0 2022-11-10 10:57:46.007803 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/__init__.py
--rw-r--r--   0        0        0      182 2023-11-09 17:23:13.648172 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      180 2023-11-09 16:05:07.182556 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      180 2022-11-10 11:04:26.420268 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0        0 2022-11-10 10:57:46.007971 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__init__.py
--rw-r--r--   0        0        0      189 2023-11-09 17:23:13.648898 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      187 2023-11-09 16:05:07.183358 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      187 2022-11-10 11:04:26.421226 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4328 2023-11-09 17:23:13.655707 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/checks.cpython-310.pyc
--rw-r--r--   0        0        0     4315 2023-11-09 16:05:07.187600 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/checks.cpython-38.pyc
--rw-r--r--   0        0        0     4315 2022-11-10 11:04:26.427373 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/checks.cpython-39.pyc
--rw-r--r--   0        0        0    16225 2023-11-09 17:23:13.749669 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/from_params.cpython-310.pyc
--rw-r--r--   0        0        0    16279 2023-11-09 16:05:07.216893 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/from_params.cpython-38.pyc
--rw-r--r--   0        0        0    16283 2022-11-10 11:04:26.462397 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/from_params.cpython-39.pyc
--rw-r--r--   0        0        0     3552 2023-11-09 17:23:13.750899 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/lazy.cpython-310.pyc
--rw-r--r--   0        0        0     3527 2023-11-09 16:05:07.217647 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/lazy.cpython-38.pyc
--rw-r--r--   0        0        0     3539 2022-11-10 11:04:26.463264 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/lazy.cpython-39.pyc
--rw-r--r--   0        0        0    19817 2023-11-09 17:23:13.663796 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/params.cpython-310.pyc
--rw-r--r--   0        0        0    19958 2023-11-09 16:05:07.190384 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/params.cpython-38.pyc
--rw-r--r--   0        0        0    19906 2022-11-10 11:04:26.431090 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/params.cpython-39.pyc
--rw-r--r--   0        0        0    10941 2023-11-09 17:23:13.745773 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/registrable.cpython-310.pyc
--rw-r--r--   0        0        0    10943 2023-11-09 16:05:07.214084 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/registrable.cpython-38.pyc
--rw-r--r--   0        0        0    10943 2022-11-10 11:04:26.459237 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/registrable.cpython-39.pyc
--rw-r--r--   0        0        0    18857 2023-11-09 17:23:13.653111 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/util.cpython-310.pyc
--rw-r--r--   0        0        0    18802 2023-11-09 16:05:07.186489 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/util.cpython-38.pyc
--rw-r--r--   0        0        0    18875 2022-11-10 11:04:26.425885 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/util.cpython-39.pyc
--rw-r--r--   0        0        0     3891 2022-11-10 10:57:46.008135 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/checks.py
--rw-r--r--   0        0        0    27842 2022-11-10 10:57:46.008377 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/from_params.py
--rw-r--r--   0        0        0     3323 2022-11-10 10:57:46.008546 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/lazy.py
--rw-r--r--   0        0        0    22823 2022-11-10 10:57:46.008780 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/params.py
--rw-r--r--   0        0        0    13490 2022-11-10 10:57:46.008995 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/registrable.py
--rw-r--r--   0        0        0    24090 2022-11-10 10:57:46.009238 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/util.py
--rw-r--r--   0        0        0        0 2022-11-10 10:57:46.009410 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/__init__.py
--rw-r--r--   0        0        0      190 2023-11-09 17:23:13.721009 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      188 2023-11-09 16:05:07.194479 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      188 2022-11-10 11:04:26.440044 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    12015 2023-11-09 17:23:13.753860 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/__pycache__/encoder_base.cpython-310.pyc
--rw-r--r--   0        0        0    12020 2023-11-09 16:05:07.219999 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/__pycache__/encoder_base.cpython-38.pyc
--rw-r--r--   0        0        0    11980 2022-11-10 11:04:26.465422 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/__pycache__/encoder_base.cpython-39.pyc
--rw-r--r--   0        0        0      557 2022-11-10 10:57:46.009661 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/__init__.py
--rw-r--r--   0        0        0      215 2023-11-09 17:23:13.722636 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      213 2023-11-09 16:05:07.196011 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      213 2022-11-10 11:04:26.440831 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    12076 2023-11-09 17:23:13.726850 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/__pycache__/conditional_random_field.cpython-310.pyc
--rw-r--r--   0        0        0    12063 2023-11-09 16:05:07.200249 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/__pycache__/conditional_random_field.cpython-38.pyc
--rw-r--r--   0        0        0    12019 2022-11-10 11:04:26.443377 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/__pycache__/conditional_random_field.cpython-39.pyc
--rw-r--r--   0        0        0    20123 2022-11-10 10:57:46.009915 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/conditional_random_field.py
--rw-r--r--   0        0        0     4003 2022-11-10 10:57:46.010099 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/conditional_random_field_wemission.py
--rw-r--r--   0        0        0    10785 2022-11-10 10:57:46.010289 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/conditional_random_field_wlannoy.py
--rw-r--r--   0        0        0     4304 2022-11-10 10:57:46.010463 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/conditional_random_field_wtrans.py
--rw-r--r--   0        0        0    17002 2022-11-10 10:57:46.010678 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/encoder_base.py
--rw-r--r--   0        0        0     4316 2022-11-10 10:57:46.010861 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/feedforward.py
--rw-r--r--   0        0        0     1074 2022-11-10 10:57:46.011082 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__init__.py
--rw-r--r--   0        0        0     1289 2023-11-09 17:23:13.741310 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1287 2023-11-09 16:05:07.210746 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1287 2022-11-10 11:04:26.455670 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5078 2023-11-09 17:23:13.743033 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/pytorch_seq2seq_wrapper.cpython-310.pyc
--rw-r--r--   0        0        0     5050 2023-11-09 16:05:07.211969 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/pytorch_seq2seq_wrapper.cpython-38.pyc
--rw-r--r--   0        0        0     5032 2022-11-10 11:04:26.456939 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/pytorch_seq2seq_wrapper.cpython-39.pyc
--rw-r--r--   0        0        0     2206 2023-11-09 17:23:13.743937 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/seq2seq_encoder.cpython-310.pyc
--rw-r--r--   0        0        0     2229 2023-11-09 16:05:07.212587 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/seq2seq_encoder.cpython-38.pyc
--rw-r--r--   0        0        0     2229 2022-11-10 11:04:26.457598 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/seq2seq_encoder.cpython-39.pyc
--rw-r--r--   0        0        0     2381 2022-11-10 10:57:46.011238 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/compose_encoder.py
--rw-r--r--   0        0        0     1436 2022-11-10 10:57:46.011406 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/feedforward_encoder.py
--rw-r--r--   0        0        0     8293 2022-11-10 10:57:46.011578 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/gated_cnn_encoder.py
--rw-r--r--   0        0        0     1539 2022-11-10 10:57:46.011733 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/pass_through_encoder.py
--rw-r--r--   0        0        0     6250 2022-11-10 10:57:46.011894 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/pytorch_seq2seq_wrapper.py
--rw-r--r--   0        0        0     5147 2022-11-10 10:57:46.012067 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/pytorch_transformer_wrapper.py
--rw-r--r--   0        0        0     1652 2022-11-10 10:57:46.012219 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/seq2seq_encoder.py
--rw-r--r--   0        0        0        0 2022-11-10 10:57:46.012369 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/nn/__init__.py
--rw-r--r--   0        0        0      185 2023-11-09 17:23:13.727869 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/nn/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      183 2023-11-09 16:05:07.200912 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/nn/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      183 2022-11-10 11:04:26.444160 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/nn/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    78488 2023-11-09 17:23:13.739289 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/nn/__pycache__/util.cpython-310.pyc
--rw-r--r--   0        0        0    78826 2023-11-09 16:05:07.209508 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/nn/__pycache__/util.cpython-38.pyc
--rw-r--r--   0        0        0    78632 2022-11-10 11:04:26.454339 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/nn/__pycache__/util.cpython-39.pyc
--rw-r--r--   0        0        0     4301 2022-11-10 10:57:46.012534 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/nn/activations.py
--rw-r--r--   0        0        0   102552 2022-11-10 10:57:46.013090 opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/nn/util.py
--rw-r--r--   0        0        0     4314 2022-12-01 06:29:36.792873 opennyai-0.0.12/opennyai/rhetorical_roles/batch_creator.py
--rw-r--r--   0        0        0     3523 2022-11-10 10:57:46.013441 opennyai-0.0.12/opennyai/rhetorical_roles/bucketing.py
--rw-r--r--   0        0        0     2027 2022-11-10 10:57:46.013588 opennyai-0.0.12/opennyai/rhetorical_roles/dataset_reader.py
--rw-r--r--   0        0        0     1819 2022-11-10 10:57:46.013747 opennyai-0.0.12/opennyai/rhetorical_roles/eval.py
--rw-r--r--   0        0        0     5670 2022-11-10 10:57:46.013911 opennyai-0.0.12/opennyai/rhetorical_roles/infer_data_prep.py
--rw-r--r--   0        0        0    17880 2022-12-06 11:27:39.240884 opennyai-0.0.12/opennyai/rhetorical_roles/models.py
--rw-r--r--   0        0        0     5471 2022-12-01 06:21:18.093400 opennyai-0.0.12/opennyai/rhetorical_roles/rhetorical_roles.py
--rw-r--r--   0        0        0     8264 2022-11-10 10:57:46.014503 opennyai-0.0.12/opennyai/rhetorical_roles/task.py
--rw-r--r--   0        0        0     1895 2022-11-10 10:57:46.014654 opennyai-0.0.12/opennyai/rhetorical_roles/utils.py
--rw-r--r--   0        0        0     6537 2022-12-01 20:04:30.661122 opennyai-0.0.12/opennyai/summarizer/ExtractiveSummarizer.py
--rw-r--r--   0        0        0        0 2022-11-10 10:57:46.014993 opennyai-0.0.12/opennyai/summarizer/__init__.py
--rw-r--r--   0        0        0     5398 2023-11-09 17:23:42.177650 opennyai-0.0.12/opennyai/summarizer/__pycache__/ExtractiveSummarizer.cpython-310.pyc
--rw-r--r--   0        0        0     5372 2023-11-09 16:05:08.536634 opennyai-0.0.12/opennyai/summarizer/__pycache__/ExtractiveSummarizer.cpython-38.pyc
--rw-r--r--   0        0        0     5388 2022-12-05 12:46:45.889366 opennyai-0.0.12/opennyai/summarizer/__pycache__/ExtractiveSummarizer.cpython-39.pyc
--rw-r--r--   0        0        0      160 2023-11-09 17:23:42.174275 opennyai-0.0.12/opennyai/summarizer/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      158 2023-11-09 16:05:08.535183 opennyai-0.0.12/opennyai/summarizer/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      158 2022-11-10 11:04:26.485816 opennyai-0.0.12/opennyai/summarizer/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0        0 2022-11-10 10:57:46.015162 opennyai-0.0.12/opennyai/summarizer/models/__init__.py
--rw-r--r--   0        0        0      167 2023-11-09 17:23:42.192312 opennyai-0.0.12/opennyai/summarizer/models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      165 2023-11-09 16:05:08.548771 opennyai-0.0.12/opennyai/summarizer/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      165 2022-11-10 11:04:26.497927 opennyai-0.0.12/opennyai/summarizer/models/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     8783 2023-11-09 17:23:42.195576 opennyai-0.0.12/opennyai/summarizer/models/__pycache__/data_loader.cpython-310.pyc
--rw-r--r--   0        0        0     8948 2023-11-09 16:05:08.551289 opennyai-0.0.12/opennyai/summarizer/models/__pycache__/data_loader.cpython-38.pyc
--rw-r--r--   0        0        0     8871 2022-11-10 11:04:26.500686 opennyai-0.0.12/opennyai/summarizer/models/__pycache__/data_loader.cpython-39.pyc
--rw-r--r--   0        0        0     8537 2023-11-09 17:23:43.302225 opennyai-0.0.12/opennyai/summarizer/models/__pycache__/decoder.cpython-310.pyc
--rw-r--r--   0        0        0     8561 2023-11-09 16:45:44.977244 opennyai-0.0.12/opennyai/summarizer/models/__pycache__/decoder.cpython-38.pyc
--rw-r--r--   0        0        0     8517 2022-11-10 11:04:26.726204 opennyai-0.0.12/opennyai/summarizer/models/__pycache__/decoder.cpython-39.pyc
--rw-r--r--   0        0        0     4163 2023-11-09 17:23:43.303890 opennyai-0.0.12/opennyai/summarizer/models/__pycache__/encoder.cpython-310.pyc
--rw-r--r--   0        0        0     4191 2023-11-09 16:45:44.978624 opennyai-0.0.12/opennyai/summarizer/models/__pycache__/encoder.cpython-38.pyc
--rw-r--r--   0        0        0     4187 2022-11-10 11:04:26.727612 opennyai-0.0.12/opennyai/summarizer/models/__pycache__/encoder.cpython-39.pyc
--rw-r--r--   0        0        0     8166 2023-11-09 17:23:42.199005 opennyai-0.0.12/opennyai/summarizer/models/__pycache__/model_builder.cpython-310.pyc
--rw-r--r--   0        0        0     8212 2023-11-09 16:05:08.554218 opennyai-0.0.12/opennyai/summarizer/models/__pycache__/model_builder.cpython-38.pyc
--rw-r--r--   0        0        0     8184 2022-11-10 11:04:26.502956 opennyai-0.0.12/opennyai/summarizer/models/__pycache__/model_builder.cpython-39.pyc
--rw-r--r--   0        0        0    12454 2023-11-09 17:23:43.307428 opennyai-0.0.12/opennyai/summarizer/models/__pycache__/neural.cpython-310.pyc
--rw-r--r--   0        0        0    12479 2023-11-09 16:45:44.981524 opennyai-0.0.12/opennyai/summarizer/models/__pycache__/neural.cpython-38.pyc
--rw-r--r--   0        0        0    12429 2022-11-10 11:04:26.730043 opennyai-0.0.12/opennyai/summarizer/models/__pycache__/neural.cpython-39.pyc
--rw-r--r--   0        0        0     6726 2023-11-09 17:23:43.309854 opennyai-0.0.12/opennyai/summarizer/models/__pycache__/optimizers.cpython-310.pyc
--rw-r--r--   0        0        0     6776 2023-11-09 16:45:44.983377 opennyai-0.0.12/opennyai/summarizer/models/__pycache__/optimizers.cpython-38.pyc
--rw-r--r--   0        0        0     6732 2022-11-10 11:04:26.731892 opennyai-0.0.12/opennyai/summarizer/models/__pycache__/optimizers.cpython-39.pyc
--rw-r--r--   0        0        0    12988 2022-11-10 10:57:46.015428 opennyai-0.0.12/opennyai/summarizer/models/data_loader.py
--rw-r--r--   0        0        0     9907 2022-11-10 10:57:46.015633 opennyai-0.0.12/opennyai/summarizer/models/decoder.py
--rw-r--r--   0        0        0     3507 2022-11-10 10:57:46.015791 opennyai-0.0.12/opennyai/summarizer/models/encoder.py
--rw-r--r--   0        0        0    11280 2022-11-10 10:57:46.015961 opennyai-0.0.12/opennyai/summarizer/models/model_builder.py
--rw-r--r--   0        0        0    15813 2022-11-10 10:57:46.016163 opennyai-0.0.12/opennyai/summarizer/models/neural.py
--rw-r--r--   0        0        0     7737 2022-11-10 10:57:46.016339 opennyai-0.0.12/opennyai/summarizer/models/optimizers.py
--rw-r--r--   0        0        0        0 2022-11-10 10:57:46.016561 opennyai-0.0.12/opennyai/summarizer/others/__init__.py
--rw-r--r--   0        0        0      167 2023-11-09 17:23:43.310563 opennyai-0.0.12/opennyai/summarizer/others/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      165 2023-11-09 16:45:44.983988 opennyai-0.0.12/opennyai/summarizer/others/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      165 2022-11-10 11:04:26.732755 opennyai-0.0.12/opennyai/summarizer/others/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3001 2023-11-09 17:23:43.311929 opennyai-0.0.12/opennyai/summarizer/others/__pycache__/args.cpython-310.pyc
--rw-r--r--   0        0        0     2997 2023-11-09 16:45:44.985134 opennyai-0.0.12/opennyai/summarizer/others/__pycache__/args.cpython-38.pyc
--rw-r--r--   0        0        0     2997 2022-11-10 11:04:26.733996 opennyai-0.0.12/opennyai/summarizer/others/__pycache__/args.cpython-39.pyc
--rw-r--r--   0        0        0     3752 2023-11-09 17:23:43.313772 opennyai-0.0.12/opennyai/summarizer/others/__pycache__/postprocessing_utils.cpython-310.pyc
--rw-r--r--   0        0        0     3754 2023-11-09 16:45:44.986606 opennyai-0.0.12/opennyai/summarizer/others/__pycache__/postprocessing_utils.cpython-38.pyc
--rw-r--r--   0        0        0     3736 2022-12-05 12:46:46.185189 opennyai-0.0.12/opennyai/summarizer/others/__pycache__/postprocessing_utils.cpython-39.pyc
--rw-r--r--   0        0        0    10665 2023-11-09 17:23:43.335343 opennyai-0.0.12/opennyai/summarizer/others/__pycache__/tokenization.cpython-310.pyc
--rw-r--r--   0        0        0    10663 2023-11-09 16:45:45.005132 opennyai-0.0.12/opennyai/summarizer/others/__pycache__/tokenization.cpython-38.pyc
--rw-r--r--   0        0        0    10658 2022-11-10 11:04:26.748220 opennyai-0.0.12/opennyai/summarizer/others/__pycache__/tokenization.cpython-39.pyc
--rw-r--r--   0        0        0     3297 2023-11-09 17:23:43.315726 opennyai-0.0.12/opennyai/summarizer/others/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0     3351 2023-11-09 16:45:44.988072 opennyai-0.0.12/opennyai/summarizer/others/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0     3321 2022-11-10 11:04:26.736639 opennyai-0.0.12/opennyai/summarizer/others/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0        0        0     4087 2022-11-10 10:57:46.016796 opennyai-0.0.12/opennyai/summarizer/others/args.py
--rw-r--r--   0        0        0     5762 2022-12-01 20:04:30.661653 opennyai-0.0.12/opennyai/summarizer/others/postprocessing_utils.py
--rw-r--r--   0        0        0    15126 2022-11-10 10:57:46.017198 opennyai-0.0.12/opennyai/summarizer/others/tokenization.py
--rw-r--r--   0        0        0     5090 2022-11-10 10:57:46.017381 opennyai-0.0.12/opennyai/summarizer/others/utils.py
--rw-r--r--   0        0        0        0 2022-11-10 10:57:46.017547 opennyai-0.0.12/opennyai/summarizer/prepro/__init__.py
--rw-r--r--   0        0        0      167 2023-11-09 17:23:43.316353 opennyai-0.0.12/opennyai/summarizer/prepro/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      165 2023-11-09 16:45:44.988594 opennyai-0.0.12/opennyai/summarizer/prepro/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      165 2022-11-10 11:04:26.737364 opennyai-0.0.12/opennyai/summarizer/prepro/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    15280 2023-11-09 17:23:43.321043 opennyai-0.0.12/opennyai/summarizer/prepro/__pycache__/data_builder.cpython-310.pyc
--rw-r--r--   0        0        0    15638 2023-11-09 16:45:44.992536 opennyai-0.0.12/opennyai/summarizer/prepro/__pycache__/data_builder.cpython-38.pyc
--rw-r--r--   0        0        0    15548 2022-11-10 11:04:26.741222 opennyai-0.0.12/opennyai/summarizer/prepro/__pycache__/data_builder.cpython-39.pyc
--rw-r--r--   0        0        0      819 2023-11-09 17:23:43.332880 opennyai-0.0.12/opennyai/summarizer/prepro/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0      833 2023-11-09 16:45:45.002802 opennyai-0.0.12/opennyai/summarizer/prepro/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0      817 2022-11-10 11:04:26.745976 opennyai-0.0.12/opennyai/summarizer/prepro/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0        0        0    16680 2022-11-10 10:57:46.017771 opennyai-0.0.12/opennyai/summarizer/prepro/data_builder.py
--rw-r--r--   0        0        0     3719 2022-11-10 10:57:46.017954 opennyai-0.0.12/opennyai/summarizer/prepro/smart_common_words.txt
--rw-r--r--   0        0        0      870 2022-11-10 10:57:46.018097 opennyai-0.0.12/opennyai/summarizer/prepro/utils.py
--rw-r--r--   0        0        0       86 2022-11-10 10:57:46.018306 opennyai-0.0.12/opennyai/utils/__init__.py
--rw-r--r--   0        0        0      261 2023-11-09 17:23:10.076962 opennyai-0.0.12/opennyai/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      259 2023-11-09 15:48:09.020308 opennyai-0.0.12/opennyai/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      259 2022-11-10 11:04:24.648069 opennyai-0.0.12/opennyai/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2186 2023-11-09 17:23:10.078911 opennyai-0.0.12/opennyai/utils/__pycache__/_ikscrapper_.cpython-310.pyc
--rw-r--r--   0        0        0     2190 2023-11-09 15:48:09.021378 opennyai-0.0.12/opennyai/utils/__pycache__/_ikscrapper_.cpython-38.pyc
--rw-r--r--   0        0        0     2188 2022-11-10 11:04:24.649129 opennyai-0.0.12/opennyai/utils/__pycache__/_ikscrapper_.cpython-39.pyc
--rw-r--r--   0        0        0     2388 2023-11-09 17:23:10.198033 opennyai-0.0.12/opennyai/utils/__pycache__/download.cpython-310.pyc
--rw-r--r--   0        0        0     2394 2023-11-09 15:49:07.513008 opennyai-0.0.12/opennyai/utils/__pycache__/download.cpython-38.pyc
--rw-r--r--   0        0        0     2390 2022-11-10 11:04:24.789991 opennyai-0.0.12/opennyai/utils/__pycache__/download.cpython-39.pyc
--rw-r--r--   0        0        0     6860 2023-11-09 17:23:10.196928 opennyai-0.0.12/opennyai/utils/__pycache__/preprocess.cpython-310.pyc
--rw-r--r--   0        0        0     6944 2023-11-09 15:49:07.512413 opennyai-0.0.12/opennyai/utils/__pycache__/preprocess.cpython-38.pyc
--rw-r--r--   0        0        0     6912 2022-12-21 05:08:49.018014 opennyai-0.0.12/opennyai/utils/__pycache__/preprocess.cpython-39.pyc
--rw-r--r--   0        0        0     5111 2023-11-09 17:23:10.200619 opennyai-0.0.12/opennyai/utils/__pycache__/sentencizer.cpython-310.pyc
--rw-r--r--   0        0        0     5177 2023-11-09 15:51:07.095004 opennyai-0.0.12/opennyai/utils/__pycache__/sentencizer.cpython-38.pyc
--rw-r--r--   0        0        0     5169 2022-12-21 05:08:49.020512 opennyai-0.0.12/opennyai/utils/__pycache__/sentencizer.cpython-39.pyc
--rw-r--r--   0        0        0     3810 2022-11-10 10:57:46.019300 opennyai-0.0.12/opennyai/utils/_ikscrapper_.py
--rw-r--r--   0        0        0     2290 2022-11-10 10:57:46.019465 opennyai-0.0.12/opennyai/utils/download.py
--rw-r--r--   0        0        0     8185 2022-12-21 05:08:18.974601 opennyai-0.0.12/opennyai/utils/preprocess.py
--rw-r--r--   0        0        0     6829 2022-12-21 05:08:18.975142 opennyai-0.0.12/opennyai/utils/sentencizer.py
--rw-r--r--   0        0        0      634 2023-11-09 17:44:02.169376 opennyai-0.0.12/pyproject.toml
--rw-r--r--   0        0        0     6054 1970-01-01 00:00:00.000000 opennyai-0.0.12/PKG-INFO
+-rw-r--r--   0        0        0     1096 2022-12-01 20:08:59.808342 opennyai-0.0.13/LICENSE
+-rw-r--r--   0        0        0     5237 2024-05-08 12:03:54.134541 opennyai-0.0.13/README.md
+-rw-r--r--   0        0        0      330 2024-05-08 12:09:29.964725 opennyai-0.0.13/opennyai/__init__.py
+-rw-r--r--   0        0        0     5719 2022-12-07 05:10:07.210614 opennyai-0.0.13/opennyai/ner/InLegalNER/InLegalNER.py
+-rw-r--r--   0        0        0        0 2022-11-10 10:57:46.006446 opennyai-0.0.13/opennyai/ner/InLegalNER/__init__.py
+-rw-r--r--   0        0        0     4215 2023-11-09 17:22:42.274538 opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/InLegalNER.cpython-310.pyc
+-rw-r--r--   0        0        0     6323 2023-11-09 16:42:27.015474 opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/InLegalNER.cpython-311.pyc
+-rw-r--r--   0        0        0     4237 2023-11-09 15:48:08.054676 opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/InLegalNER.cpython-38.pyc
+-rw-r--r--   0        0        0     4237 2022-12-21 05:08:43.888318 opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/InLegalNER.cpython-39.pyc
+-rw-r--r--   0        0        0      164 2023-11-09 17:22:42.272549 opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      180 2023-11-09 16:42:27.012417 opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      162 2023-11-09 15:48:08.053503 opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      162 2022-11-10 11:04:23.353830 opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1259 2023-11-09 17:23:10.202604 opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/entity_recognizer_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     1231 2023-11-09 15:51:07.096047 opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/entity_recognizer_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     1247 2022-11-11 05:17:23.178038 opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/entity_recognizer_utils.cpython-39.pyc
+-rw-r--r--   0        0        0    27867 2023-11-09 17:23:10.212242 opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/postprocessing_utils.cpython-310.pyc
+-rw-r--r--   0        0        0    28203 2023-11-09 15:51:07.104504 opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/postprocessing_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    28079 2023-11-09 17:16:27.130090 opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/postprocessing_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     1195 2022-11-11 05:15:03.882432 opennyai-0.0.13/opennyai/ner/InLegalNER/entity_recognizer_utils.py
+-rw-r--r--   0        0        0    44209 2023-11-09 15:26:19.714769 opennyai-0.0.13/opennyai/ner/InLegalNER/postprocessing_utils.py
+-rw-r--r--   0        0        0      171 2022-11-10 10:57:46.007110 opennyai-0.0.13/opennyai/ner/__init__.py
+-rw-r--r--   0        0        0      382 2023-11-09 17:22:21.648342 opennyai-0.0.13/opennyai/ner/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      488 2023-11-09 16:42:18.604183 opennyai-0.0.13/opennyai/ner/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      380 2023-11-09 15:45:23.707942 opennyai-0.0.13/opennyai/ner/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      380 2022-11-10 11:04:21.860264 opennyai-0.0.13/opennyai/ner/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5197 2023-11-09 17:22:21.650927 opennyai-0.0.13/opennyai/ner/__pycache__/ner_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     9578 2023-11-09 16:42:18.607212 opennyai-0.0.13/opennyai/ner/__pycache__/ner_utils.cpython-311.pyc
+-rw-r--r--   0        0        0     5355 2023-11-09 15:45:23.709738 opennyai-0.0.13/opennyai/ner/__pycache__/ner_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     5345 2023-11-09 17:15:40.566344 opennyai-0.0.13/opennyai/ner/__pycache__/ner_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     6868 2023-11-09 15:26:19.716495 opennyai-0.0.13/opennyai/ner/ner_utils.py
+-rw-r--r--   0        0        0     7055 2022-12-01 20:04:30.660403 opennyai-0.0.13/opennyai/pipeline.py
+-rw-r--r--   0        0        0        0 2022-11-10 10:57:46.007640 opennyai-0.0.13/opennyai/rhetorical_roles/__init__.py
+-rw-r--r--   0        0        0      166 2023-11-09 17:23:12.176935 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      164 2023-11-09 16:05:06.517614 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      164 2022-11-10 11:04:26.100434 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3561 2023-11-09 17:23:42.168397 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/batch_creator.cpython-310.pyc
+-rw-r--r--   0        0        0     3553 2023-11-09 16:05:08.531732 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/batch_creator.cpython-38.pyc
+-rw-r--r--   0        0        0     3549 2022-12-01 19:34:02.997994 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/batch_creator.cpython-39.pyc
+-rw-r--r--   0        0        0     4506 2023-11-09 17:23:42.170541 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/bucketing.cpython-310.pyc
+-rw-r--r--   0        0        0     4500 2023-11-09 16:05:08.532780 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/bucketing.cpython-38.pyc
+-rw-r--r--   0        0        0     4486 2022-11-10 11:04:26.484136 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/bucketing.cpython-39.pyc
+-rw-r--r--   0        0        0     2327 2023-11-09 17:23:42.172583 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/dataset_reader.cpython-310.pyc
+-rw-r--r--   0        0        0     2295 2023-11-09 16:05:08.533552 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/dataset_reader.cpython-38.pyc
+-rw-r--r--   0        0        0     2319 2022-11-10 11:04:26.485087 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/dataset_reader.cpython-39.pyc
+-rw-r--r--   0        0        0     1486 2023-11-09 17:23:13.758512 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/eval.cpython-310.pyc
+-rw-r--r--   0        0        0     1474 2023-11-09 16:05:07.222366 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/eval.cpython-38.pyc
+-rw-r--r--   0        0        0     1478 2022-11-10 11:04:26.468026 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/eval.cpython-39.pyc
+-rw-r--r--   0        0        0     3410 2023-11-09 17:23:13.757100 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/infer_data_prep.cpython-310.pyc
+-rw-r--r--   0        0        0     3292 2023-11-09 16:05:07.221555 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/infer_data_prep.cpython-38.pyc
+-rw-r--r--   0        0        0     3392 2022-11-10 11:04:26.467171 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/infer_data_prep.cpython-39.pyc
+-rw-r--r--   0        0        0    12466 2023-11-09 17:23:13.543350 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/models.cpython-310.pyc
+-rw-r--r--   0        0        0    12534 2023-11-09 16:05:07.088215 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/models.cpython-38.pyc
+-rw-r--r--   0        0        0    12499 2022-12-06 11:29:27.242731 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0        0        0     4486 2023-11-09 17:23:12.179713 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/rhetorical_roles.cpython-310.pyc
+-rw-r--r--   0        0        0     4438 2023-11-09 16:05:06.519678 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/rhetorical_roles.cpython-38.pyc
+-rw-r--r--   0        0        0     4482 2022-12-01 06:22:58.082509 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/rhetorical_roles.cpython-39.pyc
+-rw-r--r--   0        0        0     6270 2023-11-09 17:23:13.821659 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     6388 2023-11-09 16:05:07.267886 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/task.cpython-38.pyc
+-rw-r--r--   0        0        0     6305 2022-11-10 11:04:26.481407 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/task.cpython-39.pyc
+-rw-r--r--   0        0        0     2946 2023-11-09 17:23:13.760022 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0     2836 2023-11-09 16:05:07.223308 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0     2888 2022-11-10 11:04:26.469021 opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0        0        0        0 2022-11-10 10:57:46.007803 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/__init__.py
+-rw-r--r--   0        0        0      182 2023-11-09 17:23:13.648172 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      180 2023-11-09 16:05:07.182556 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      180 2022-11-10 11:04:26.420268 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0        0 2022-11-10 10:57:46.007971 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__init__.py
+-rw-r--r--   0        0        0      189 2023-11-09 17:23:13.648898 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      187 2023-11-09 16:05:07.183358 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      187 2022-11-10 11:04:26.421226 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4328 2023-11-09 17:23:13.655707 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/checks.cpython-310.pyc
+-rw-r--r--   0        0        0     4315 2023-11-09 16:05:07.187600 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/checks.cpython-38.pyc
+-rw-r--r--   0        0        0     4315 2022-11-10 11:04:26.427373 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/checks.cpython-39.pyc
+-rw-r--r--   0        0        0    16225 2023-11-09 17:23:13.749669 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/from_params.cpython-310.pyc
+-rw-r--r--   0        0        0    16279 2023-11-09 16:05:07.216893 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/from_params.cpython-38.pyc
+-rw-r--r--   0        0        0    16283 2022-11-10 11:04:26.462397 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/from_params.cpython-39.pyc
+-rw-r--r--   0        0        0     3552 2023-11-09 17:23:13.750899 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/lazy.cpython-310.pyc
+-rw-r--r--   0        0        0     3527 2023-11-09 16:05:07.217647 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/lazy.cpython-38.pyc
+-rw-r--r--   0        0        0     3539 2022-11-10 11:04:26.463264 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/lazy.cpython-39.pyc
+-rw-r--r--   0        0        0    19817 2023-11-09 17:23:13.663796 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/params.cpython-310.pyc
+-rw-r--r--   0        0        0    19958 2023-11-09 16:05:07.190384 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/params.cpython-38.pyc
+-rw-r--r--   0        0        0    19906 2022-11-10 11:04:26.431090 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/params.cpython-39.pyc
+-rw-r--r--   0        0        0    10941 2023-11-09 17:23:13.745773 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/registrable.cpython-310.pyc
+-rw-r--r--   0        0        0    10943 2023-11-09 16:05:07.214084 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/registrable.cpython-38.pyc
+-rw-r--r--   0        0        0    10943 2022-11-10 11:04:26.459237 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/registrable.cpython-39.pyc
+-rw-r--r--   0        0        0    18857 2023-11-09 17:23:13.653111 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/util.cpython-310.pyc
+-rw-r--r--   0        0        0    18802 2023-11-09 16:05:07.186489 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/util.cpython-38.pyc
+-rw-r--r--   0        0        0    18875 2022-11-10 11:04:26.425885 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0        0        0     3891 2022-11-10 10:57:46.008135 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/checks.py
+-rw-r--r--   0        0        0    27842 2022-11-10 10:57:46.008377 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/from_params.py
+-rw-r--r--   0        0        0     3323 2022-11-10 10:57:46.008546 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/lazy.py
+-rw-r--r--   0        0        0    22823 2022-11-10 10:57:46.008780 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/params.py
+-rw-r--r--   0        0        0    13490 2022-11-10 10:57:46.008995 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/registrable.py
+-rw-r--r--   0        0        0    24090 2022-11-10 10:57:46.009238 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/util.py
+-rw-r--r--   0        0        0        0 2022-11-10 10:57:46.009410 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/__init__.py
+-rw-r--r--   0        0        0      190 2023-11-09 17:23:13.721009 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      188 2023-11-09 16:05:07.194479 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      188 2022-11-10 11:04:26.440044 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    12015 2023-11-09 17:23:13.753860 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/__pycache__/encoder_base.cpython-310.pyc
+-rw-r--r--   0        0        0    12020 2023-11-09 16:05:07.219999 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/__pycache__/encoder_base.cpython-38.pyc
+-rw-r--r--   0        0        0    11980 2022-11-10 11:04:26.465422 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/__pycache__/encoder_base.cpython-39.pyc
+-rw-r--r--   0        0        0      557 2022-11-10 10:57:46.009661 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/__init__.py
+-rw-r--r--   0        0        0      215 2023-11-09 17:23:13.722636 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      213 2023-11-09 16:05:07.196011 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      213 2022-11-10 11:04:26.440831 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    12076 2023-11-09 17:23:13.726850 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/__pycache__/conditional_random_field.cpython-310.pyc
+-rw-r--r--   0        0        0    12063 2023-11-09 16:05:07.200249 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/__pycache__/conditional_random_field.cpython-38.pyc
+-rw-r--r--   0        0        0    12019 2022-11-10 11:04:26.443377 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/__pycache__/conditional_random_field.cpython-39.pyc
+-rw-r--r--   0        0        0    20123 2022-11-10 10:57:46.009915 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/conditional_random_field.py
+-rw-r--r--   0        0        0     4003 2022-11-10 10:57:46.010099 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/conditional_random_field_wemission.py
+-rw-r--r--   0        0        0    10785 2022-11-10 10:57:46.010289 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/conditional_random_field_wlannoy.py
+-rw-r--r--   0        0        0     4304 2022-11-10 10:57:46.010463 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/conditional_random_field_wtrans.py
+-rw-r--r--   0        0        0    17002 2022-11-10 10:57:46.010678 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/encoder_base.py
+-rw-r--r--   0        0        0     4316 2022-11-10 10:57:46.010861 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/feedforward.py
+-rw-r--r--   0        0        0     1074 2022-11-10 10:57:46.011082 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__init__.py
+-rw-r--r--   0        0        0     1289 2023-11-09 17:23:13.741310 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1287 2023-11-09 16:05:07.210746 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1287 2022-11-10 11:04:26.455670 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5078 2023-11-09 17:23:13.743033 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/pytorch_seq2seq_wrapper.cpython-310.pyc
+-rw-r--r--   0        0        0     5050 2023-11-09 16:05:07.211969 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/pytorch_seq2seq_wrapper.cpython-38.pyc
+-rw-r--r--   0        0        0     5032 2022-11-10 11:04:26.456939 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/pytorch_seq2seq_wrapper.cpython-39.pyc
+-rw-r--r--   0        0        0     2206 2023-11-09 17:23:13.743937 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/seq2seq_encoder.cpython-310.pyc
+-rw-r--r--   0        0        0     2229 2023-11-09 16:05:07.212587 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/seq2seq_encoder.cpython-38.pyc
+-rw-r--r--   0        0        0     2229 2022-11-10 11:04:26.457598 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/seq2seq_encoder.cpython-39.pyc
+-rw-r--r--   0        0        0     2381 2022-11-10 10:57:46.011238 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/compose_encoder.py
+-rw-r--r--   0        0        0     1436 2022-11-10 10:57:46.011406 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/feedforward_encoder.py
+-rw-r--r--   0        0        0     8293 2022-11-10 10:57:46.011578 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/gated_cnn_encoder.py
+-rw-r--r--   0        0        0     1539 2022-11-10 10:57:46.011733 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/pass_through_encoder.py
+-rw-r--r--   0        0        0     6250 2022-11-10 10:57:46.011894 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/pytorch_seq2seq_wrapper.py
+-rw-r--r--   0        0        0     5147 2022-11-10 10:57:46.012067 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/pytorch_transformer_wrapper.py
+-rw-r--r--   0        0        0     1652 2022-11-10 10:57:46.012219 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/seq2seq_encoder.py
+-rw-r--r--   0        0        0        0 2022-11-10 10:57:46.012369 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/nn/__init__.py
+-rw-r--r--   0        0        0      185 2023-11-09 17:23:13.727869 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/nn/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      183 2023-11-09 16:05:07.200912 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/nn/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      183 2022-11-10 11:04:26.444160 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/nn/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    78488 2023-11-09 17:23:13.739289 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/nn/__pycache__/util.cpython-310.pyc
+-rw-r--r--   0        0        0    78826 2023-11-09 16:05:07.209508 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/nn/__pycache__/util.cpython-38.pyc
+-rw-r--r--   0        0        0    78632 2022-11-10 11:04:26.454339 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/nn/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0        0        0     4301 2022-11-10 10:57:46.012534 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/nn/activations.py
+-rw-r--r--   0        0        0   102552 2022-11-10 10:57:46.013090 opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/nn/util.py
+-rw-r--r--   0        0        0     4314 2022-12-01 06:29:36.792873 opennyai-0.0.13/opennyai/rhetorical_roles/batch_creator.py
+-rw-r--r--   0        0        0     3523 2022-11-10 10:57:46.013441 opennyai-0.0.13/opennyai/rhetorical_roles/bucketing.py
+-rw-r--r--   0        0        0     2027 2022-11-10 10:57:46.013588 opennyai-0.0.13/opennyai/rhetorical_roles/dataset_reader.py
+-rw-r--r--   0        0        0     1819 2022-11-10 10:57:46.013747 opennyai-0.0.13/opennyai/rhetorical_roles/eval.py
+-rw-r--r--   0        0        0     5670 2022-11-10 10:57:46.013911 opennyai-0.0.13/opennyai/rhetorical_roles/infer_data_prep.py
+-rw-r--r--   0        0        0    17880 2022-12-06 11:27:39.240884 opennyai-0.0.13/opennyai/rhetorical_roles/models.py
+-rw-r--r--   0        0        0     5471 2022-12-01 06:21:18.093400 opennyai-0.0.13/opennyai/rhetorical_roles/rhetorical_roles.py
+-rw-r--r--   0        0        0     8264 2022-11-10 10:57:46.014503 opennyai-0.0.13/opennyai/rhetorical_roles/task.py
+-rw-r--r--   0        0        0     1895 2022-11-10 10:57:46.014654 opennyai-0.0.13/opennyai/rhetorical_roles/utils.py
+-rw-r--r--   0        0        0     6537 2022-12-01 20:04:30.661122 opennyai-0.0.13/opennyai/summarizer/ExtractiveSummarizer.py
+-rw-r--r--   0        0        0        0 2022-11-10 10:57:46.014993 opennyai-0.0.13/opennyai/summarizer/__init__.py
+-rw-r--r--   0        0        0     5398 2023-11-09 17:23:42.177650 opennyai-0.0.13/opennyai/summarizer/__pycache__/ExtractiveSummarizer.cpython-310.pyc
+-rw-r--r--   0        0        0     5372 2023-11-09 16:05:08.536634 opennyai-0.0.13/opennyai/summarizer/__pycache__/ExtractiveSummarizer.cpython-38.pyc
+-rw-r--r--   0        0        0     5388 2022-12-05 12:46:45.889366 opennyai-0.0.13/opennyai/summarizer/__pycache__/ExtractiveSummarizer.cpython-39.pyc
+-rw-r--r--   0        0        0      160 2023-11-09 17:23:42.174275 opennyai-0.0.13/opennyai/summarizer/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      158 2023-11-09 16:05:08.535183 opennyai-0.0.13/opennyai/summarizer/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      158 2022-11-10 11:04:26.485816 opennyai-0.0.13/opennyai/summarizer/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0        0 2022-11-10 10:57:46.015162 opennyai-0.0.13/opennyai/summarizer/models/__init__.py
+-rw-r--r--   0        0        0      167 2023-11-09 17:23:42.192312 opennyai-0.0.13/opennyai/summarizer/models/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      165 2023-11-09 16:05:08.548771 opennyai-0.0.13/opennyai/summarizer/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      165 2022-11-10 11:04:26.497927 opennyai-0.0.13/opennyai/summarizer/models/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     8783 2023-11-09 17:23:42.195576 opennyai-0.0.13/opennyai/summarizer/models/__pycache__/data_loader.cpython-310.pyc
+-rw-r--r--   0        0        0     8948 2023-11-09 16:05:08.551289 opennyai-0.0.13/opennyai/summarizer/models/__pycache__/data_loader.cpython-38.pyc
+-rw-r--r--   0        0        0     8871 2022-11-10 11:04:26.500686 opennyai-0.0.13/opennyai/summarizer/models/__pycache__/data_loader.cpython-39.pyc
+-rw-r--r--   0        0        0     8537 2023-11-09 17:23:43.302225 opennyai-0.0.13/opennyai/summarizer/models/__pycache__/decoder.cpython-310.pyc
+-rw-r--r--   0        0        0     8561 2023-11-09 16:45:44.977244 opennyai-0.0.13/opennyai/summarizer/models/__pycache__/decoder.cpython-38.pyc
+-rw-r--r--   0        0        0     8517 2022-11-10 11:04:26.726204 opennyai-0.0.13/opennyai/summarizer/models/__pycache__/decoder.cpython-39.pyc
+-rw-r--r--   0        0        0     4163 2023-11-09 17:23:43.303890 opennyai-0.0.13/opennyai/summarizer/models/__pycache__/encoder.cpython-310.pyc
+-rw-r--r--   0        0        0     4191 2023-11-09 16:45:44.978624 opennyai-0.0.13/opennyai/summarizer/models/__pycache__/encoder.cpython-38.pyc
+-rw-r--r--   0        0        0     4187 2022-11-10 11:04:26.727612 opennyai-0.0.13/opennyai/summarizer/models/__pycache__/encoder.cpython-39.pyc
+-rw-r--r--   0        0        0     8166 2023-11-09 17:23:42.199005 opennyai-0.0.13/opennyai/summarizer/models/__pycache__/model_builder.cpython-310.pyc
+-rw-r--r--   0        0        0     8212 2023-11-09 16:05:08.554218 opennyai-0.0.13/opennyai/summarizer/models/__pycache__/model_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     8184 2022-11-10 11:04:26.502956 opennyai-0.0.13/opennyai/summarizer/models/__pycache__/model_builder.cpython-39.pyc
+-rw-r--r--   0        0        0    12454 2023-11-09 17:23:43.307428 opennyai-0.0.13/opennyai/summarizer/models/__pycache__/neural.cpython-310.pyc
+-rw-r--r--   0        0        0    12479 2023-11-09 16:45:44.981524 opennyai-0.0.13/opennyai/summarizer/models/__pycache__/neural.cpython-38.pyc
+-rw-r--r--   0        0        0    12429 2022-11-10 11:04:26.730043 opennyai-0.0.13/opennyai/summarizer/models/__pycache__/neural.cpython-39.pyc
+-rw-r--r--   0        0        0     6726 2023-11-09 17:23:43.309854 opennyai-0.0.13/opennyai/summarizer/models/__pycache__/optimizers.cpython-310.pyc
+-rw-r--r--   0        0        0     6776 2023-11-09 16:45:44.983377 opennyai-0.0.13/opennyai/summarizer/models/__pycache__/optimizers.cpython-38.pyc
+-rw-r--r--   0        0        0     6732 2022-11-10 11:04:26.731892 opennyai-0.0.13/opennyai/summarizer/models/__pycache__/optimizers.cpython-39.pyc
+-rw-r--r--   0        0        0    12988 2022-11-10 10:57:46.015428 opennyai-0.0.13/opennyai/summarizer/models/data_loader.py
+-rw-r--r--   0        0        0     9907 2022-11-10 10:57:46.015633 opennyai-0.0.13/opennyai/summarizer/models/decoder.py
+-rw-r--r--   0        0        0     3507 2022-11-10 10:57:46.015791 opennyai-0.0.13/opennyai/summarizer/models/encoder.py
+-rw-r--r--   0        0        0    11280 2022-11-10 10:57:46.015961 opennyai-0.0.13/opennyai/summarizer/models/model_builder.py
+-rw-r--r--   0        0        0    15813 2022-11-10 10:57:46.016163 opennyai-0.0.13/opennyai/summarizer/models/neural.py
+-rw-r--r--   0        0        0     7737 2022-11-10 10:57:46.016339 opennyai-0.0.13/opennyai/summarizer/models/optimizers.py
+-rw-r--r--   0        0        0        0 2022-11-10 10:57:46.016561 opennyai-0.0.13/opennyai/summarizer/others/__init__.py
+-rw-r--r--   0        0        0      167 2023-11-09 17:23:43.310563 opennyai-0.0.13/opennyai/summarizer/others/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      165 2023-11-09 16:45:44.983988 opennyai-0.0.13/opennyai/summarizer/others/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      165 2022-11-10 11:04:26.732755 opennyai-0.0.13/opennyai/summarizer/others/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3001 2023-11-09 17:23:43.311929 opennyai-0.0.13/opennyai/summarizer/others/__pycache__/args.cpython-310.pyc
+-rw-r--r--   0        0        0     2997 2023-11-09 16:45:44.985134 opennyai-0.0.13/opennyai/summarizer/others/__pycache__/args.cpython-38.pyc
+-rw-r--r--   0        0        0     2997 2022-11-10 11:04:26.733996 opennyai-0.0.13/opennyai/summarizer/others/__pycache__/args.cpython-39.pyc
+-rw-r--r--   0        0        0     3752 2023-11-09 17:23:43.313772 opennyai-0.0.13/opennyai/summarizer/others/__pycache__/postprocessing_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     3754 2023-11-09 16:45:44.986606 opennyai-0.0.13/opennyai/summarizer/others/__pycache__/postprocessing_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     3736 2022-12-05 12:46:46.185189 opennyai-0.0.13/opennyai/summarizer/others/__pycache__/postprocessing_utils.cpython-39.pyc
+-rw-r--r--   0        0        0    10665 2023-11-09 17:23:43.335343 opennyai-0.0.13/opennyai/summarizer/others/__pycache__/tokenization.cpython-310.pyc
+-rw-r--r--   0        0        0    10663 2023-11-09 16:45:45.005132 opennyai-0.0.13/opennyai/summarizer/others/__pycache__/tokenization.cpython-38.pyc
+-rw-r--r--   0        0        0    10658 2022-11-10 11:04:26.748220 opennyai-0.0.13/opennyai/summarizer/others/__pycache__/tokenization.cpython-39.pyc
+-rw-r--r--   0        0        0     3297 2023-11-09 17:23:43.315726 opennyai-0.0.13/opennyai/summarizer/others/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0     3351 2023-11-09 16:45:44.988072 opennyai-0.0.13/opennyai/summarizer/others/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0     3321 2022-11-10 11:04:26.736639 opennyai-0.0.13/opennyai/summarizer/others/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0        0        0     4087 2022-11-10 10:57:46.016796 opennyai-0.0.13/opennyai/summarizer/others/args.py
+-rw-r--r--   0        0        0     5762 2022-12-01 20:04:30.661653 opennyai-0.0.13/opennyai/summarizer/others/postprocessing_utils.py
+-rw-r--r--   0        0        0    15126 2022-11-10 10:57:46.017198 opennyai-0.0.13/opennyai/summarizer/others/tokenization.py
+-rw-r--r--   0        0        0     5090 2022-11-10 10:57:46.017381 opennyai-0.0.13/opennyai/summarizer/others/utils.py
+-rw-r--r--   0        0        0        0 2022-11-10 10:57:46.017547 opennyai-0.0.13/opennyai/summarizer/prepro/__init__.py
+-rw-r--r--   0        0        0      167 2023-11-09 17:23:43.316353 opennyai-0.0.13/opennyai/summarizer/prepro/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      165 2023-11-09 16:45:44.988594 opennyai-0.0.13/opennyai/summarizer/prepro/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      165 2022-11-10 11:04:26.737364 opennyai-0.0.13/opennyai/summarizer/prepro/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    15280 2023-11-09 17:23:43.321043 opennyai-0.0.13/opennyai/summarizer/prepro/__pycache__/data_builder.cpython-310.pyc
+-rw-r--r--   0        0        0    15638 2023-11-09 16:45:44.992536 opennyai-0.0.13/opennyai/summarizer/prepro/__pycache__/data_builder.cpython-38.pyc
+-rw-r--r--   0        0        0    15548 2022-11-10 11:04:26.741222 opennyai-0.0.13/opennyai/summarizer/prepro/__pycache__/data_builder.cpython-39.pyc
+-rw-r--r--   0        0        0      819 2023-11-09 17:23:43.332880 opennyai-0.0.13/opennyai/summarizer/prepro/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0      833 2023-11-09 16:45:45.002802 opennyai-0.0.13/opennyai/summarizer/prepro/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0      817 2022-11-10 11:04:26.745976 opennyai-0.0.13/opennyai/summarizer/prepro/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0        0        0    16680 2022-11-10 10:57:46.017771 opennyai-0.0.13/opennyai/summarizer/prepro/data_builder.py
+-rw-r--r--   0        0        0     3719 2022-11-10 10:57:46.017954 opennyai-0.0.13/opennyai/summarizer/prepro/smart_common_words.txt
+-rw-r--r--   0        0        0      870 2022-11-10 10:57:46.018097 opennyai-0.0.13/opennyai/summarizer/prepro/utils.py
+-rw-r--r--   0        0        0       86 2022-11-10 10:57:46.018306 opennyai-0.0.13/opennyai/utils/__init__.py
+-rw-r--r--   0        0        0      261 2023-11-09 17:23:10.076962 opennyai-0.0.13/opennyai/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      259 2023-11-09 15:48:09.020308 opennyai-0.0.13/opennyai/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      259 2022-11-10 11:04:24.648069 opennyai-0.0.13/opennyai/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2186 2023-11-09 17:23:10.078911 opennyai-0.0.13/opennyai/utils/__pycache__/_ikscrapper_.cpython-310.pyc
+-rw-r--r--   0        0        0     2190 2023-11-09 15:48:09.021378 opennyai-0.0.13/opennyai/utils/__pycache__/_ikscrapper_.cpython-38.pyc
+-rw-r--r--   0        0        0     2188 2022-11-10 11:04:24.649129 opennyai-0.0.13/opennyai/utils/__pycache__/_ikscrapper_.cpython-39.pyc
+-rw-r--r--   0        0        0     2388 2023-11-09 17:23:10.198033 opennyai-0.0.13/opennyai/utils/__pycache__/download.cpython-310.pyc
+-rw-r--r--   0        0        0     2394 2023-11-09 15:49:07.513008 opennyai-0.0.13/opennyai/utils/__pycache__/download.cpython-38.pyc
+-rw-r--r--   0        0        0     2390 2022-11-10 11:04:24.789991 opennyai-0.0.13/opennyai/utils/__pycache__/download.cpython-39.pyc
+-rw-r--r--   0        0        0     6860 2023-11-09 17:23:10.196928 opennyai-0.0.13/opennyai/utils/__pycache__/preprocess.cpython-310.pyc
+-rw-r--r--   0        0        0     6944 2023-11-09 15:49:07.512413 opennyai-0.0.13/opennyai/utils/__pycache__/preprocess.cpython-38.pyc
+-rw-r--r--   0        0        0     6912 2022-12-21 05:08:49.018014 opennyai-0.0.13/opennyai/utils/__pycache__/preprocess.cpython-39.pyc
+-rw-r--r--   0        0        0     5111 2023-11-09 17:23:10.200619 opennyai-0.0.13/opennyai/utils/__pycache__/sentencizer.cpython-310.pyc
+-rw-r--r--   0        0        0     5177 2023-11-09 15:51:07.095004 opennyai-0.0.13/opennyai/utils/__pycache__/sentencizer.cpython-38.pyc
+-rw-r--r--   0        0        0     5169 2022-12-21 05:08:49.020512 opennyai-0.0.13/opennyai/utils/__pycache__/sentencizer.cpython-39.pyc
+-rw-r--r--   0        0        0     3810 2022-11-10 10:57:46.019300 opennyai-0.0.13/opennyai/utils/_ikscrapper_.py
+-rw-r--r--   0        0        0     2200 2024-05-08 12:07:02.324751 opennyai-0.0.13/opennyai/utils/download.py
+-rw-r--r--   0        0        0     8185 2022-12-21 05:08:18.974601 opennyai-0.0.13/opennyai/utils/preprocess.py
+-rw-r--r--   0        0        0     6829 2022-12-21 05:08:18.975142 opennyai-0.0.13/opennyai/utils/sentencizer.py
+-rw-r--r--   0        0        0      631 2024-05-08 12:09:59.032784 opennyai-0.0.13/pyproject.toml
+-rw-r--r--   0        0        0     6219 1970-01-01 00:00:00.000000 opennyai-0.0.13/PKG-INFO
```

### Comparing `opennyai-0.0.12/LICENSE` & `opennyai-0.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/README.md` & `opennyai-0.0.13/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 Opennyai is a python library for natural language preprocessing on Indian legal texts.
 
 This library provides unified access to the following 3 pre-trained AI models developed by OpenNyAI which focus on
 Indian court
 judgments:
 
 * Named Entity Recognition (NER): [GitHub](https://github.com/Legal-NLP-EkStep/legal_NER)
-  , [paper](https://arxiv.org/pdf/2211.03442.pdf)
+  , [paper](https://arxiv.org/pdf/2211.03442.pdf), [Huggingface Datasets](https://huggingface.co/datasets/opennyaiorg/InLegalNER)
 * Judgment Structuring using Sentence Rhetorical
-  Roles: [GitHub](https://github.com/Legal-NLP-EkStep/rhetorical-role-baseline)
-  , [paper](http://www.lrec-conf.org/proceedings/lrec2022/pdf/2022.lrec-1.470.pdf)
+  Roles: [GitHub](https://github.com/Legal-NLP-EkStep/rhetorical-role-baseline) 
+  , [paper](http://www.lrec-conf.org/proceedings/lrec2022/pdf/2022.lrec-1.470.pdf), [Huggingface Datasets](https://huggingface.co/datasets/opennyaiorg/InRhetoricalRoles)
 * Extractive Summarizer: [GitHub](https://github.com/Legal-NLP-EkStep/judgment_extractive_summarizer)
 
 This library is mainly for running the pretrained models on your custom input judgments text. For more details about
 data and model training, please refer to individual git repo links.
 
 # 🔧 1. Installation
```

#### html2text {}

```diff
@@ -8,19 +8,21 @@
 %3E=3.8-blue)](https://github.com/OpenNyAI/Opennyai) [![python version](https:/
 /img.shields.io/badge/Python-<3.11-blue)](https://github.com/OpenNyAI/Opennyai)
 [![Downloads](https://pepy.tech/badge/opennyai)](https://github.com/OpenNyAI/
 Opennyai) Opennyai is a python library for natural language preprocessing on
 Indian legal texts. This library provides unified access to the following 3
 pre-trained AI models developed by OpenNyAI which focus on Indian court
 judgments: * Named Entity Recognition (NER): [GitHub](https://github.com/Legal-
-NLP-EkStep/legal_NER) , [paper](https://arxiv.org/pdf/2211.03442.pdf) *
-Judgment Structuring using Sentence Rhetorical Roles: [GitHub](https://
+NLP-EkStep/legal_NER) , [paper](https://arxiv.org/pdf/2211.03442.pdf),
+[Huggingface Datasets](https://huggingface.co/datasets/opennyaiorg/InLegalNER)
+* Judgment Structuring using Sentence Rhetorical Roles: [GitHub](https://
 github.com/Legal-NLP-EkStep/rhetorical-role-baseline) , [paper](http://
-www.lrec-conf.org/proceedings/lrec2022/pdf/2022.lrec-1.470.pdf) * Extractive
-Summarizer: [GitHub](https://github.com/Legal-NLP-EkStep/
+www.lrec-conf.org/proceedings/lrec2022/pdf/2022.lrec-1.470.pdf), [Huggingface
+Datasets](https://huggingface.co/datasets/opennyaiorg/InRhetoricalRoles) *
+Extractive Summarizer: [GitHub](https://github.com/Legal-NLP-EkStep/
 judgment_extractive_summarizer) This library is mainly for running the
 pretrained models on your custom input judgments text. For more details about
 data and model training, please refer to individual git repo links. # ð§ 1.
 Installation To get started using opennyai first create a new python virtual
 environment using [conda](https://www.anaconda.com/): Supports python 3.8, 3.9,
 3.10 ```bash conda create -n opennyai python=3.8 conda activate opennyai ```
 Install it using pip by running the following line in your terminal ```bash pip
```

### Comparing `opennyai-0.0.12/opennyai/ner/InLegalNER/InLegalNER.py` & `opennyai-0.0.13/opennyai/ner/InLegalNER/InLegalNER.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/InLegalNER.cpython-310.pyc` & `opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/InLegalNER.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/InLegalNER.cpython-311.pyc` & `opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/InLegalNER.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/InLegalNER.cpython-38.pyc` & `opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/InLegalNER.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/InLegalNER.cpython-39.pyc` & `opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/InLegalNER.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/entity_recognizer_utils.cpython-310.pyc` & `opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/entity_recognizer_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/entity_recognizer_utils.cpython-38.pyc` & `opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/entity_recognizer_utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/entity_recognizer_utils.cpython-39.pyc` & `opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/entity_recognizer_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/postprocessing_utils.cpython-310.pyc` & `opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/postprocessing_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/postprocessing_utils.cpython-38.pyc` & `opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/postprocessing_utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/ner/InLegalNER/__pycache__/postprocessing_utils.cpython-39.pyc` & `opennyai-0.0.13/opennyai/ner/InLegalNER/__pycache__/postprocessing_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/ner/InLegalNER/entity_recognizer_utils.py` & `opennyai-0.0.13/opennyai/ner/InLegalNER/entity_recognizer_utils.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/ner/InLegalNER/postprocessing_utils.py` & `opennyai-0.0.13/opennyai/ner/InLegalNER/postprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/ner/__pycache__/ner_utils.cpython-310.pyc` & `opennyai-0.0.13/opennyai/ner/__pycache__/ner_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/ner/__pycache__/ner_utils.cpython-311.pyc` & `opennyai-0.0.13/opennyai/ner/__pycache__/ner_utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/ner/__pycache__/ner_utils.cpython-38.pyc` & `opennyai-0.0.13/opennyai/ner/__pycache__/ner_utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/ner/__pycache__/ner_utils.cpython-39.pyc` & `opennyai-0.0.13/opennyai/ner/__pycache__/ner_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/ner/ner_utils.py` & `opennyai-0.0.13/opennyai/ner/ner_utils.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/pipeline.py` & `opennyai-0.0.13/opennyai/pipeline.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/batch_creator.cpython-310.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/batch_creator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/batch_creator.cpython-38.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/batch_creator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/batch_creator.cpython-39.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/batch_creator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/bucketing.cpython-310.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/bucketing.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/bucketing.cpython-38.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/bucketing.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/bucketing.cpython-39.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/bucketing.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/dataset_reader.cpython-310.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/dataset_reader.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/dataset_reader.cpython-38.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/dataset_reader.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/dataset_reader.cpython-39.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/dataset_reader.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/eval.cpython-310.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/eval.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/eval.cpython-38.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/eval.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/eval.cpython-39.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/eval.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/infer_data_prep.cpython-310.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/infer_data_prep.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/infer_data_prep.cpython-38.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/infer_data_prep.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/infer_data_prep.cpython-39.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/infer_data_prep.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/models.cpython-310.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/models.cpython-38.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/models.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/models.cpython-39.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/models.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/rhetorical_roles.cpython-310.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/rhetorical_roles.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/rhetorical_roles.cpython-38.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/rhetorical_roles.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/rhetorical_roles.cpython-39.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/rhetorical_roles.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/task.cpython-310.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/task.cpython-38.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/task.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/task.cpython-39.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/task.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/utils.cpython-310.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/utils.cpython-38.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/__pycache__/utils.cpython-39.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/checks.cpython-310.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/checks.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/checks.cpython-38.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/checks.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/checks.cpython-39.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/checks.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/from_params.cpython-310.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/from_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/from_params.cpython-38.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/from_params.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/from_params.cpython-39.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/from_params.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/lazy.cpython-310.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/lazy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/lazy.cpython-38.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/lazy.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/lazy.cpython-39.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/lazy.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/params.cpython-310.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/params.cpython-38.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/params.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/params.cpython-39.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/params.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/registrable.cpython-310.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/registrable.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/registrable.cpython-38.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/registrable.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/registrable.cpython-39.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/registrable.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/util.cpython-310.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/util.cpython-38.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/util.cpython-39.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/__pycache__/util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/checks.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/checks.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/from_params.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/from_params.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/lazy.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/lazy.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/params.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/params.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/registrable.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/registrable.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/common/util.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/common/util.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/__pycache__/encoder_base.cpython-310.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/__pycache__/encoder_base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/__pycache__/encoder_base.cpython-38.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/__pycache__/encoder_base.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/__pycache__/encoder_base.cpython-39.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/__pycache__/encoder_base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/__init__.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/__init__.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/__pycache__/conditional_random_field.cpython-310.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/__pycache__/conditional_random_field.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/__pycache__/conditional_random_field.cpython-38.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/__pycache__/conditional_random_field.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/__pycache__/conditional_random_field.cpython-39.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/__pycache__/conditional_random_field.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/conditional_random_field.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/conditional_random_field.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/conditional_random_field_wemission.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/conditional_random_field_wemission.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/conditional_random_field_wlannoy.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/conditional_random_field_wlannoy.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/conditional_random_field_wtrans.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/conditional_random_field/conditional_random_field_wtrans.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/encoder_base.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/encoder_base.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/feedforward.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/feedforward.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__init__.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/__init__.cpython-310.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/__init__.cpython-38.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/__init__.cpython-39.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/pytorch_seq2seq_wrapper.cpython-310.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/pytorch_seq2seq_wrapper.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/pytorch_seq2seq_wrapper.cpython-38.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/pytorch_seq2seq_wrapper.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/pytorch_seq2seq_wrapper.cpython-39.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/pytorch_seq2seq_wrapper.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/seq2seq_encoder.cpython-310.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/seq2seq_encoder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/seq2seq_encoder.cpython-38.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/seq2seq_encoder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/seq2seq_encoder.cpython-39.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/__pycache__/seq2seq_encoder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/compose_encoder.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/compose_encoder.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/feedforward_encoder.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/feedforward_encoder.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/gated_cnn_encoder.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/gated_cnn_encoder.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/pass_through_encoder.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/pass_through_encoder.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/pytorch_seq2seq_wrapper.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/pytorch_seq2seq_wrapper.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/pytorch_transformer_wrapper.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/pytorch_transformer_wrapper.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/seq2seq_encoder.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/modules/seq2seq_encoders/seq2seq_encoder.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/nn/__pycache__/util.cpython-310.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/nn/__pycache__/util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/nn/__pycache__/util.cpython-38.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/nn/__pycache__/util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/nn/__pycache__/util.cpython-39.pyc` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/nn/__pycache__/util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/nn/activations.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/nn/activations.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/allennlp_helper/nn/util.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/allennlp_helper/nn/util.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/batch_creator.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/batch_creator.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/bucketing.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/bucketing.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/dataset_reader.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/dataset_reader.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/eval.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/eval.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/infer_data_prep.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/infer_data_prep.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/models.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/models.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/rhetorical_roles.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/rhetorical_roles.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/task.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/task.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/rhetorical_roles/utils.py` & `opennyai-0.0.13/opennyai/rhetorical_roles/utils.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/ExtractiveSummarizer.py` & `opennyai-0.0.13/opennyai/summarizer/ExtractiveSummarizer.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/__pycache__/ExtractiveSummarizer.cpython-310.pyc` & `opennyai-0.0.13/opennyai/summarizer/__pycache__/ExtractiveSummarizer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/__pycache__/ExtractiveSummarizer.cpython-38.pyc` & `opennyai-0.0.13/opennyai/summarizer/__pycache__/ExtractiveSummarizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/__pycache__/ExtractiveSummarizer.cpython-39.pyc` & `opennyai-0.0.13/opennyai/summarizer/__pycache__/ExtractiveSummarizer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/__pycache__/data_loader.cpython-310.pyc` & `opennyai-0.0.13/opennyai/summarizer/models/__pycache__/data_loader.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/__pycache__/data_loader.cpython-38.pyc` & `opennyai-0.0.13/opennyai/summarizer/models/__pycache__/data_loader.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/__pycache__/data_loader.cpython-39.pyc` & `opennyai-0.0.13/opennyai/summarizer/models/__pycache__/data_loader.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/__pycache__/decoder.cpython-310.pyc` & `opennyai-0.0.13/opennyai/summarizer/models/__pycache__/decoder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/__pycache__/decoder.cpython-38.pyc` & `opennyai-0.0.13/opennyai/summarizer/models/__pycache__/decoder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/__pycache__/decoder.cpython-39.pyc` & `opennyai-0.0.13/opennyai/summarizer/models/__pycache__/decoder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/__pycache__/encoder.cpython-310.pyc` & `opennyai-0.0.13/opennyai/summarizer/models/__pycache__/encoder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/__pycache__/encoder.cpython-38.pyc` & `opennyai-0.0.13/opennyai/summarizer/models/__pycache__/encoder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/__pycache__/encoder.cpython-39.pyc` & `opennyai-0.0.13/opennyai/summarizer/models/__pycache__/encoder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/__pycache__/model_builder.cpython-310.pyc` & `opennyai-0.0.13/opennyai/summarizer/models/__pycache__/model_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/__pycache__/model_builder.cpython-38.pyc` & `opennyai-0.0.13/opennyai/summarizer/models/__pycache__/model_builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/__pycache__/model_builder.cpython-39.pyc` & `opennyai-0.0.13/opennyai/summarizer/models/__pycache__/model_builder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/__pycache__/neural.cpython-310.pyc` & `opennyai-0.0.13/opennyai/summarizer/models/__pycache__/neural.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/__pycache__/neural.cpython-38.pyc` & `opennyai-0.0.13/opennyai/summarizer/models/__pycache__/neural.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/__pycache__/neural.cpython-39.pyc` & `opennyai-0.0.13/opennyai/summarizer/models/__pycache__/neural.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/__pycache__/optimizers.cpython-310.pyc` & `opennyai-0.0.13/opennyai/summarizer/models/__pycache__/optimizers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/__pycache__/optimizers.cpython-38.pyc` & `opennyai-0.0.13/opennyai/summarizer/models/__pycache__/optimizers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/__pycache__/optimizers.cpython-39.pyc` & `opennyai-0.0.13/opennyai/summarizer/models/__pycache__/optimizers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/data_loader.py` & `opennyai-0.0.13/opennyai/summarizer/models/data_loader.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/decoder.py` & `opennyai-0.0.13/opennyai/summarizer/models/decoder.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/encoder.py` & `opennyai-0.0.13/opennyai/summarizer/models/encoder.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/model_builder.py` & `opennyai-0.0.13/opennyai/summarizer/models/model_builder.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/neural.py` & `opennyai-0.0.13/opennyai/summarizer/models/neural.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/models/optimizers.py` & `opennyai-0.0.13/opennyai/summarizer/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/others/__pycache__/args.cpython-310.pyc` & `opennyai-0.0.13/opennyai/summarizer/others/__pycache__/args.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/others/__pycache__/args.cpython-38.pyc` & `opennyai-0.0.13/opennyai/summarizer/others/__pycache__/args.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/others/__pycache__/args.cpython-39.pyc` & `opennyai-0.0.13/opennyai/summarizer/others/__pycache__/args.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/others/__pycache__/postprocessing_utils.cpython-310.pyc` & `opennyai-0.0.13/opennyai/summarizer/others/__pycache__/postprocessing_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/others/__pycache__/postprocessing_utils.cpython-38.pyc` & `opennyai-0.0.13/opennyai/summarizer/others/__pycache__/postprocessing_utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/others/__pycache__/postprocessing_utils.cpython-39.pyc` & `opennyai-0.0.13/opennyai/summarizer/others/__pycache__/postprocessing_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/others/__pycache__/tokenization.cpython-310.pyc` & `opennyai-0.0.13/opennyai/summarizer/others/__pycache__/tokenization.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/others/__pycache__/tokenization.cpython-38.pyc` & `opennyai-0.0.13/opennyai/summarizer/others/__pycache__/tokenization.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/others/__pycache__/tokenization.cpython-39.pyc` & `opennyai-0.0.13/opennyai/summarizer/others/__pycache__/tokenization.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/others/__pycache__/utils.cpython-310.pyc` & `opennyai-0.0.13/opennyai/summarizer/others/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/others/__pycache__/utils.cpython-38.pyc` & `opennyai-0.0.13/opennyai/summarizer/others/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/others/__pycache__/utils.cpython-39.pyc` & `opennyai-0.0.13/opennyai/summarizer/others/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/others/args.py` & `opennyai-0.0.13/opennyai/summarizer/others/args.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/others/postprocessing_utils.py` & `opennyai-0.0.13/opennyai/summarizer/others/postprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/others/tokenization.py` & `opennyai-0.0.13/opennyai/summarizer/others/tokenization.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/others/utils.py` & `opennyai-0.0.13/opennyai/summarizer/others/utils.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/prepro/__pycache__/data_builder.cpython-310.pyc` & `opennyai-0.0.13/opennyai/summarizer/prepro/__pycache__/data_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/prepro/__pycache__/data_builder.cpython-38.pyc` & `opennyai-0.0.13/opennyai/summarizer/prepro/__pycache__/data_builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/prepro/__pycache__/data_builder.cpython-39.pyc` & `opennyai-0.0.13/opennyai/summarizer/prepro/__pycache__/data_builder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/prepro/__pycache__/utils.cpython-310.pyc` & `opennyai-0.0.13/opennyai/summarizer/prepro/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/prepro/__pycache__/utils.cpython-38.pyc` & `opennyai-0.0.13/opennyai/summarizer/prepro/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/prepro/__pycache__/utils.cpython-39.pyc` & `opennyai-0.0.13/opennyai/summarizer/prepro/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/prepro/data_builder.py` & `opennyai-0.0.13/opennyai/summarizer/prepro/data_builder.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/prepro/smart_common_words.txt` & `opennyai-0.0.13/opennyai/summarizer/prepro/smart_common_words.txt`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/summarizer/prepro/utils.py` & `opennyai-0.0.13/opennyai/summarizer/prepro/utils.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/utils/__pycache__/_ikscrapper_.cpython-310.pyc` & `opennyai-0.0.13/opennyai/utils/__pycache__/_ikscrapper_.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/utils/__pycache__/_ikscrapper_.cpython-38.pyc` & `opennyai-0.0.13/opennyai/utils/__pycache__/_ikscrapper_.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/utils/__pycache__/_ikscrapper_.cpython-39.pyc` & `opennyai-0.0.13/opennyai/utils/__pycache__/_ikscrapper_.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/utils/__pycache__/download.cpython-310.pyc` & `opennyai-0.0.13/opennyai/utils/__pycache__/download.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/utils/__pycache__/download.cpython-38.pyc` & `opennyai-0.0.13/opennyai/utils/__pycache__/download.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/utils/__pycache__/download.cpython-39.pyc` & `opennyai-0.0.13/opennyai/utils/__pycache__/download.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/utils/__pycache__/preprocess.cpython-310.pyc` & `opennyai-0.0.13/opennyai/utils/__pycache__/preprocess.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/utils/__pycache__/preprocess.cpython-38.pyc` & `opennyai-0.0.13/opennyai/utils/__pycache__/preprocess.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/utils/__pycache__/preprocess.cpython-39.pyc` & `opennyai-0.0.13/opennyai/utils/__pycache__/preprocess.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/utils/__pycache__/sentencizer.cpython-310.pyc` & `opennyai-0.0.13/opennyai/utils/__pycache__/sentencizer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/utils/__pycache__/sentencizer.cpython-38.pyc` & `opennyai-0.0.13/opennyai/utils/__pycache__/sentencizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/utils/__pycache__/sentencizer.cpython-39.pyc` & `opennyai-0.0.13/opennyai/utils/__pycache__/sentencizer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/utils/_ikscrapper_.py` & `opennyai-0.0.13/opennyai/utils/_ikscrapper_.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/utils/preprocess.py` & `opennyai-0.0.13/opennyai/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/opennyai/utils/sentencizer.py` & `opennyai-0.0.13/opennyai/utils/sentencizer.py`

 * *Files identical despite different names*

### Comparing `opennyai-0.0.12/pyproject.toml` & `opennyai-0.0.13/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "opennyai"
-version = "0.0.12"
+version = "0.0.13"
 description = "A SpaCy pipeline and models for NLP on indian legal text."
-authors = ["Aman Tiwari <aman.tiwari@thoughtworks.com>"]
+authors = ["Aman Tiwari <work.amantiwari@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8 || ^3.9 || ^3.10"
 
 spacy = ">=3.2.2,<3.3.0"
 pandas = ">1.2.4"
```

### Comparing `opennyai-0.0.12/PKG-INFO` & `opennyai-0.0.13/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: opennyai
-Version: 0.0.12
+Version: 0.0.13
 Summary: A SpaCy pipeline and models for NLP on indian legal text.
 Author: Aman Tiwari
-Author-email: aman.tiwari@thoughtworks.com
+Author-email: work.amantiwari@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.10.0)
@@ -37,18 +37,18 @@
 Opennyai is a python library for natural language preprocessing on Indian legal texts.
 
 This library provides unified access to the following 3 pre-trained AI models developed by OpenNyAI which focus on
 Indian court
 judgments:
 
 * Named Entity Recognition (NER): [GitHub](https://github.com/Legal-NLP-EkStep/legal_NER)
-  , [paper](https://arxiv.org/pdf/2211.03442.pdf)
+  , [paper](https://arxiv.org/pdf/2211.03442.pdf), [Huggingface Datasets](https://huggingface.co/datasets/opennyaiorg/InLegalNER)
 * Judgment Structuring using Sentence Rhetorical
-  Roles: [GitHub](https://github.com/Legal-NLP-EkStep/rhetorical-role-baseline)
-  , [paper](http://www.lrec-conf.org/proceedings/lrec2022/pdf/2022.lrec-1.470.pdf)
+  Roles: [GitHub](https://github.com/Legal-NLP-EkStep/rhetorical-role-baseline) 
+  , [paper](http://www.lrec-conf.org/proceedings/lrec2022/pdf/2022.lrec-1.470.pdf), [Huggingface Datasets](https://huggingface.co/datasets/opennyaiorg/InRhetoricalRoles)
 * Extractive Summarizer: [GitHub](https://github.com/Legal-NLP-EkStep/judgment_extractive_summarizer)
 
 This library is mainly for running the pretrained models on your custom input judgments text. For more details about
 data and model training, please refer to individual git repo links.
 
 # 🔧 1. Installation
```

#### html2text {}

```diff
@@ -1,39 +1,41 @@
-Metadata-Version: 2.1 Name: opennyai Version: 0.0.12 Summary: A SpaCy pipeline
+Metadata-Version: 2.1 Name: opennyai Version: 0.0.13 Summary: A SpaCy pipeline
 and models for NLP on indian legal text. Author: Aman Tiwari Author-email:
-aman.tiwari@thoughtworks.com Requires-Python: >=3.8,<4.0 Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Requires-Dist: beautifulsoup4 (>=4.10.0) Requires-Dist:
-levenshtein (>=0.23.0,<0.24.0) Requires-Dist: multiprocess (>=0.70.15,<0.71.0)
-Requires-Dist: nltk (>=3.6) Requires-Dist: pandas (>1.2.4) Requires-Dist:
-prettytable (>=3.1.1) Requires-Dist: pytest (>=7.4.3,<8.0.0) Requires-Dist:
-pytorch-transformers (>=1.2.0,<2.0.0) Requires-Dist: scikit-learn
-(>=1.3.2,<2.0.0) Requires-Dist: spacy (>=3.2.2,<3.3.0) Requires-Dist: spacy-
-transformers (>=1.1.4) Requires-Dist: torch (>=1.12.1) Description-Content-
-Type: text/markdown _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_O_p_e_n_N_y_A_I_/_O_p_e_n_n_y_a_i_/_r_a_w_/_m_a_s_t_e_r_/_a_s_s_e_t_/
-_f_i_n_a_l_-_l_o_g_o_-_0_1_._j_p_e_g_]# Opennyai : An efficient NLP Pipeline for Indian Legal
-documents [![Current Release Version](https://img.shields.io/github/release/
-OpenNyAI/opennyai.svg?style=flat-square&logo=github)](https://github.com/
-OpenNyAI/Opennyai/releases) [![PyPI version](https://img.shields.io/pypi/v/
+work.amantiwari@gmail.com Requires-Python: >=3.8,<4.0 Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: beautifulsoup4 (>=4.10.0) Requires-Dist: levenshtein
+(>=0.23.0,<0.24.0) Requires-Dist: multiprocess (>=0.70.15,<0.71.0) Requires-
+Dist: nltk (>=3.6) Requires-Dist: pandas (>1.2.4) Requires-Dist: prettytable
+(>=3.1.1) Requires-Dist: pytest (>=7.4.3,<8.0.0) Requires-Dist: pytorch-
+transformers (>=1.2.0,<2.0.0) Requires-Dist: scikit-learn (>=1.3.2,<2.0.0)
+Requires-Dist: spacy (>=3.2.2,<3.3.0) Requires-Dist: spacy-transformers
+(>=1.1.4) Requires-Dist: torch (>=1.12.1) Description-Content-Type: text/
+markdown _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_O_p_e_n_N_y_A_I_/_O_p_e_n_n_y_a_i_/_r_a_w_/_m_a_s_t_e_r_/_a_s_s_e_t_/_f_i_n_a_l_-_l_o_g_o_-
+_0_1_._j_p_e_g_]# Opennyai : An efficient NLP Pipeline for Indian Legal documents [!
+[Current Release Version](https://img.shields.io/github/release/OpenNyAI/
+opennyai.svg?style=flat-square&logo=github)](https://github.com/OpenNyAI/
+Opennyai/releases) [![PyPI version](https://img.shields.io/pypi/v/
 opennyai.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/
 project/opennyai/) [![python version](https://img.shields.io/badge/Python-
 %3E=3.8-blue)](https://github.com/OpenNyAI/Opennyai) [![python version](https:/
 /img.shields.io/badge/Python-<3.11-blue)](https://github.com/OpenNyAI/Opennyai)
 [![Downloads](https://pepy.tech/badge/opennyai)](https://github.com/OpenNyAI/
 Opennyai) Opennyai is a python library for natural language preprocessing on
 Indian legal texts. This library provides unified access to the following 3
 pre-trained AI models developed by OpenNyAI which focus on Indian court
 judgments: * Named Entity Recognition (NER): [GitHub](https://github.com/Legal-
-NLP-EkStep/legal_NER) , [paper](https://arxiv.org/pdf/2211.03442.pdf) *
-Judgment Structuring using Sentence Rhetorical Roles: [GitHub](https://
+NLP-EkStep/legal_NER) , [paper](https://arxiv.org/pdf/2211.03442.pdf),
+[Huggingface Datasets](https://huggingface.co/datasets/opennyaiorg/InLegalNER)
+* Judgment Structuring using Sentence Rhetorical Roles: [GitHub](https://
 github.com/Legal-NLP-EkStep/rhetorical-role-baseline) , [paper](http://
-www.lrec-conf.org/proceedings/lrec2022/pdf/2022.lrec-1.470.pdf) * Extractive
-Summarizer: [GitHub](https://github.com/Legal-NLP-EkStep/
+www.lrec-conf.org/proceedings/lrec2022/pdf/2022.lrec-1.470.pdf), [Huggingface
+Datasets](https://huggingface.co/datasets/opennyaiorg/InRhetoricalRoles) *
+Extractive Summarizer: [GitHub](https://github.com/Legal-NLP-EkStep/
 judgment_extractive_summarizer) This library is mainly for running the
 pretrained models on your custom input judgments text. For more details about
 data and model training, please refer to individual git repo links. # ð§ 1.
 Installation To get started using opennyai first create a new python virtual
 environment using [conda](https://www.anaconda.com/): Supports python 3.8, 3.9,
 3.10 ```bash conda create -n opennyai python=3.8 conda activate opennyai ```
 Install it using pip by running the following line in your terminal ```bash pip
```

