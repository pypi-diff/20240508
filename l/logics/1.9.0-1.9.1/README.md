# Comparing `tmp/logics-1.9.0.tar.gz` & `tmp/logics-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logics-1.9.0.tar", last modified: Fri Feb 16 20:59:28 2024, max compression
+gzip compressed data, was "logics-1.9.1.tar", last modified: Wed Feb 21 18:12:23 2024, max compression
```

## Comparing `logics-1.9.0.tar` & `logics-1.9.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-16 20:59:28.962775 logics-1.9.0/
--rwxrwxrwx   0 root         (0) root         (0)     1079 2021-03-26 14:06:13.000000 logics-1.9.0/LICENSE.txt
--rwxrwxrwx   0 root         (0) root         (0)    12262 2024-02-16 20:59:28.962108 logics-1.9.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)    11457 2023-03-16 17:08:29.000000 logics-1.9.0/README.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-16 20:59:28.386733 logics-1.9.0/logics/
--rwxrwxrwx   0 root         (0) root         (0)       24 2021-01-04 20:43:46.000000 logics-1.9.0/logics/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-16 20:59:28.402472 logics-1.9.0/logics/classes/
--rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:17:26.000000 logics-1.9.0/logics/classes/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3109 2024-02-06 14:40:35.000000 logics-1.9.0/logics/classes/errors.py
--rwxrwxrwx   0 root         (0) root         (0)      919 2020-12-04 15:16:37.000000 logics-1.9.0/logics/classes/exceptions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-16 20:59:28.433057 logics-1.9.0/logics/classes/predicate/
--rwxrwxrwx   0 root         (0) root         (0)      243 2023-02-22 18:26:21.000000 logics-1.9.0/logics/classes/predicate/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    27795 2023-02-23 17:44:50.000000 logics-1.9.0/logics/classes/predicate/formula.py
--rwxrwxrwx   0 root         (0) root         (0)    19934 2024-02-16 18:55:30.000000 logics-1.9.0/logics/classes/predicate/language.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-16 20:59:28.440219 logics-1.9.0/logics/classes/predicate/proof_theories/
--rwxrwxrwx   0 root         (0) root         (0)      246 2023-02-22 18:26:21.000000 logics-1.9.0/logics/classes/predicate/proof_theories/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      418 2023-02-22 18:26:21.000000 logics-1.9.0/logics/classes/predicate/proof_theories/derivation.py
--rwxrwxrwx   0 root         (0) root         (0)    12369 2023-03-17 15:15:19.000000 logics-1.9.0/logics/classes/predicate/proof_theories/natural_deduction.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-16 20:59:28.445310 logics-1.9.0/logics/classes/predicate/semantics/
--rwxrwxrwx   0 root         (0) root         (0)       72 2021-03-24 14:39:07.000000 logics-1.9.0/logics/classes/predicate/semantics/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    35944 2021-03-25 15:15:23.000000 logics-1.9.0/logics/classes/predicate/semantics/models.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-16 20:59:28.479406 logics-1.9.0/logics/classes/propositional/
--rwxrwxrwx   0 root         (0) root         (0)      195 2020-11-21 15:41:12.000000 logics-1.9.0/logics/classes/propositional/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    19235 2023-02-22 18:26:21.000000 logics-1.9.0/logics/classes/propositional/formula.py
--rwxrwxrwx   0 root         (0) root         (0)    22170 2022-09-26 18:39:16.000000 logics-1.9.0/logics/classes/propositional/inference.py
--rwxrwxrwx   0 root         (0) root         (0)    10060 2022-02-03 20:01:19.000000 logics-1.9.0/logics/classes/propositional/language.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-16 20:59:28.579927 logics-1.9.0/logics/classes/propositional/proof_theories/
--rwxrwxrwx   0 root         (0) root         (0)      518 2020-11-12 22:59:54.000000 logics-1.9.0/logics/classes/propositional/proof_theories/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    10897 2023-03-17 15:15:19.000000 logics-1.9.0/logics/classes/propositional/proof_theories/axiom_system.py
--rwxrwxrwx   0 root         (0) root         (0)     6040 2021-03-27 16:24:15.000000 logics-1.9.0/logics/classes/propositional/proof_theories/derivation.py
--rwxrwxrwx   0 root         (0) root         (0)    17986 2024-02-02 14:30:39.000000 logics-1.9.0/logics/classes/propositional/proof_theories/metainferential_tableaux.py
--rwxrwxrwx   0 root         (0) root         (0)    37094 2023-08-31 13:57:52.000000 logics-1.9.0/logics/classes/propositional/proof_theories/natural_deduction.py
--rwxrwxrwx   0 root         (0) root         (0)    67490 2023-03-17 15:15:19.000000 logics-1.9.0/logics/classes/propositional/proof_theories/sequents.py
--rwxrwxrwx   0 root         (0) root         (0)    63575 2024-02-05 16:01:08.000000 logics-1.9.0/logics/classes/propositional/proof_theories/tableaux.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-16 20:59:28.642522 logics-1.9.0/logics/classes/propositional/semantics/
--rwxrwxrwx   0 root         (0) root         (0)      156 2020-12-02 15:23:39.000000 logics-1.9.0/logics/classes/propositional/semantics/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    45702 2022-08-29 18:21:06.000000 logics-1.9.0/logics/classes/propositional/semantics/many_valued.py
--rwxrwxrwx   0 root         (0) root         (0)    24328 2021-03-22 18:00:32.000000 logics-1.9.0/logics/classes/propositional/semantics/mapped_logic.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-16 20:59:28.644150 logics-1.9.0/logics/instances/
--rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:17:36.000000 logics-1.9.0/logics/instances/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-16 20:59:28.670582 logics-1.9.0/logics/instances/predicate/
--rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:18:38.000000 logics-1.9.0/logics/instances/predicate/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7074 2023-02-22 18:26:21.000000 logics-1.9.0/logics/instances/predicate/languages.py
--rwxrwxrwx   0 root         (0) root         (0)     5209 2021-03-25 14:49:21.000000 logics-1.9.0/logics/instances/predicate/model_semantics.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-16 20:59:28.681741 logics-1.9.0/logics/instances/predicate/model_subclasses/
--rwxrwxrwx   0 root         (0) root         (0)      109 2020-10-16 15:02:56.000000 logics-1.9.0/logics/instances/predicate/model_subclasses/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1606 2020-12-14 17:40:49.000000 logics-1.9.0/logics/instances/predicate/model_subclasses/arithmetic.py
--rwxrwxrwx   0 root         (0) root         (0)     2274 2023-02-22 18:26:21.000000 logics-1.9.0/logics/instances/predicate/natural_deduction.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-16 20:59:28.798366 logics-1.9.0/logics/instances/propositional/
--rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:18:54.000000 logics-1.9.0/logics/instances/propositional/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1022 2020-12-07 15:24:22.000000 logics-1.9.0/logics/instances/propositional/axiom_systems.py
--rwxrwxrwx   0 root         (0) root         (0)     4316 2022-08-29 18:21:06.000000 logics-1.9.0/logics/instances/propositional/languages.py
--rwxrwxrwx   0 root         (0) root         (0)    16665 2022-08-29 18:21:06.000000 logics-1.9.0/logics/instances/propositional/many_valued_semantics.py
--rwxrwxrwx   0 root         (0) root         (0)    12138 2021-03-18 16:02:34.000000 logics-1.9.0/logics/instances/propositional/mapped_logic_semantics.py
--rwxrwxrwx   0 root         (0) root         (0)    16069 2024-01-31 14:41:42.000000 logics-1.9.0/logics/instances/propositional/metainferential_tableaux.py
--rwxrwxrwx   0 root         (0) root         (0)     8493 2023-04-10 16:32:18.000000 logics-1.9.0/logics/instances/propositional/natural_deduction.py
--rwxrwxrwx   0 root         (0) root         (0)    17155 2022-02-03 19:56:56.000000 logics-1.9.0/logics/instances/propositional/sequents.py
--rwxrwxrwx   0 root         (0) root         (0)    17045 2023-02-28 16:31:49.000000 logics-1.9.0/logics/instances/propositional/tableaux.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-16 20:59:28.799442 logics-1.9.0/logics/utils/
--rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:17:53.000000 logics-1.9.0/logics/utils/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-16 20:59:28.802268 logics-1.9.0/logics/utils/formula_generators/
--rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:19:08.000000 logics-1.9.0/logics/utils/formula_generators/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    32445 2024-02-16 20:54:33.000000 logics-1.9.0/logics/utils/formula_generators/generators_biased.py
--rwxrwxrwx   0 root         (0) root         (0)       85 2021-03-26 15:35:46.000000 logics-1.9.0/logics/utils/formula_generators/generators_unbiased.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-16 20:59:28.832728 logics-1.9.0/logics/utils/parsers/
--rwxrwxrwx   0 root         (0) root         (0)      169 2023-03-16 17:08:29.000000 logics-1.9.0/logics/utils/parsers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    16572 2021-03-25 14:03:02.000000 logics-1.9.0/logics/utils/parsers/parser_utils.py
--rwxrwxrwx   0 root         (0) root         (0)    21937 2023-02-23 18:39:04.000000 logics-1.9.0/logics/utils/parsers/predicate_parser.py
--rwxrwxrwx   0 root         (0) root         (0)    28650 2022-08-29 18:21:06.000000 logics-1.9.0/logics/utils/parsers/standard_parser.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-16 20:59:28.899861 logics-1.9.0/logics/utils/solvers/
--rwxrwxrwx   0 root         (0) root         (0)      196 2022-11-15 18:01:45.000000 logics-1.9.0/logics/utils/solvers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    17735 2023-02-22 18:26:21.000000 logics-1.9.0/logics/utils/solvers/first_order_natural_deduction.py
--rwxrwxrwx   0 root         (0) root         (0)    65608 2023-02-22 18:26:21.000000 logics-1.9.0/logics/utils/solvers/natural_deduction.py
--rwxrwxrwx   0 root         (0) root         (0)    15790 2023-04-13 20:12:20.000000 logics-1.9.0/logics/utils/solvers/sequents.py
--rwxrwxrwx   0 root         (0) root         (0)    21035 2024-01-30 17:15:14.000000 logics-1.9.0/logics/utils/solvers/tableaux.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-16 20:59:28.955113 logics-1.9.0/logics/utils/upgrade/
--rwxrwxrwx   0 root         (0) root         (0)       88 2023-02-22 18:26:21.000000 logics-1.9.0/logics/utils/upgrade/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1916 2023-02-22 18:26:21.000000 logics-1.9.0/logics/utils/upgrade/upgrade.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-16 20:59:28.958549 logics-1.9.0/logics.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)    12262 2024-02-16 20:59:28.000000 logics-1.9.0/logics.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2761 2024-02-16 20:59:28.000000 logics-1.9.0/logics.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-02-16 20:59:28.000000 logics-1.9.0/logics.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       15 2024-02-16 20:59:28.000000 logics-1.9.0/logics.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2024-02-16 20:59:28.000000 logics-1.9.0/logics.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      104 2021-03-26 14:42:28.000000 logics-1.9.0/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)      906 2024-02-16 20:59:28.966506 logics-1.9.0/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 18:12:23.130009 logics-1.9.1/
+-rwxrwxrwx   0 root         (0) root         (0)     1079 2021-03-26 14:06:13.000000 logics-1.9.1/LICENSE.txt
+-rwxrwxrwx   0 root         (0) root         (0)    12262 2024-02-21 18:12:23.129639 logics-1.9.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)    11457 2023-03-16 17:08:29.000000 logics-1.9.1/README.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 18:12:22.651002 logics-1.9.1/logics/
+-rwxrwxrwx   0 root         (0) root         (0)       24 2021-01-04 20:43:46.000000 logics-1.9.1/logics/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 18:12:22.654643 logics-1.9.1/logics/classes/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:17:26.000000 logics-1.9.1/logics/classes/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3109 2024-02-16 21:00:29.000000 logics-1.9.1/logics/classes/errors.py
+-rwxrwxrwx   0 root         (0) root         (0)      919 2020-12-04 15:16:37.000000 logics-1.9.1/logics/classes/exceptions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 18:12:22.672667 logics-1.9.1/logics/classes/predicate/
+-rwxrwxrwx   0 root         (0) root         (0)      243 2023-02-22 18:26:21.000000 logics-1.9.1/logics/classes/predicate/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    27795 2023-02-23 17:44:50.000000 logics-1.9.1/logics/classes/predicate/formula.py
+-rwxrwxrwx   0 root         (0) root         (0)    19934 2024-02-16 21:00:29.000000 logics-1.9.1/logics/classes/predicate/language.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 18:12:22.674492 logics-1.9.1/logics/classes/predicate/proof_theories/
+-rwxrwxrwx   0 root         (0) root         (0)      246 2023-02-22 18:26:21.000000 logics-1.9.1/logics/classes/predicate/proof_theories/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      418 2023-02-22 18:26:21.000000 logics-1.9.1/logics/classes/predicate/proof_theories/derivation.py
+-rwxrwxrwx   0 root         (0) root         (0)    12369 2023-03-17 15:15:19.000000 logics-1.9.1/logics/classes/predicate/proof_theories/natural_deduction.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 18:12:22.678130 logics-1.9.1/logics/classes/predicate/semantics/
+-rwxrwxrwx   0 root         (0) root         (0)       72 2021-03-24 14:39:07.000000 logics-1.9.1/logics/classes/predicate/semantics/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    35946 2024-02-21 18:10:22.000000 logics-1.9.1/logics/classes/predicate/semantics/models.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 18:12:22.695578 logics-1.9.1/logics/classes/propositional/
+-rwxrwxrwx   0 root         (0) root         (0)      195 2020-11-21 15:41:12.000000 logics-1.9.1/logics/classes/propositional/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    19235 2023-02-22 18:26:21.000000 logics-1.9.1/logics/classes/propositional/formula.py
+-rwxrwxrwx   0 root         (0) root         (0)    22170 2022-09-26 18:39:16.000000 logics-1.9.1/logics/classes/propositional/inference.py
+-rwxrwxrwx   0 root         (0) root         (0)    10060 2022-02-03 20:01:19.000000 logics-1.9.1/logics/classes/propositional/language.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 18:12:22.789942 logics-1.9.1/logics/classes/propositional/proof_theories/
+-rwxrwxrwx   0 root         (0) root         (0)      518 2020-11-12 22:59:54.000000 logics-1.9.1/logics/classes/propositional/proof_theories/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    10897 2023-03-17 15:15:19.000000 logics-1.9.1/logics/classes/propositional/proof_theories/axiom_system.py
+-rwxrwxrwx   0 root         (0) root         (0)     6040 2021-03-27 16:24:15.000000 logics-1.9.1/logics/classes/propositional/proof_theories/derivation.py
+-rwxrwxrwx   0 root         (0) root         (0)    17986 2024-02-02 14:30:39.000000 logics-1.9.1/logics/classes/propositional/proof_theories/metainferential_tableaux.py
+-rwxrwxrwx   0 root         (0) root         (0)    37094 2023-08-31 13:57:52.000000 logics-1.9.1/logics/classes/propositional/proof_theories/natural_deduction.py
+-rwxrwxrwx   0 root         (0) root         (0)    67490 2023-03-17 15:15:19.000000 logics-1.9.1/logics/classes/propositional/proof_theories/sequents.py
+-rwxrwxrwx   0 root         (0) root         (0)    63575 2024-02-05 16:01:08.000000 logics-1.9.1/logics/classes/propositional/proof_theories/tableaux.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 18:12:22.837255 logics-1.9.1/logics/classes/propositional/semantics/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2020-12-02 15:23:39.000000 logics-1.9.1/logics/classes/propositional/semantics/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    45702 2022-08-29 18:21:06.000000 logics-1.9.1/logics/classes/propositional/semantics/many_valued.py
+-rwxrwxrwx   0 root         (0) root         (0)    24328 2021-03-22 18:00:32.000000 logics-1.9.1/logics/classes/propositional/semantics/mapped_logic.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 18:12:22.850916 logics-1.9.1/logics/instances/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:17:36.000000 logics-1.9.1/logics/instances/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 18:12:22.866319 logics-1.9.1/logics/instances/predicate/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:18:38.000000 logics-1.9.1/logics/instances/predicate/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7074 2023-02-22 18:26:21.000000 logics-1.9.1/logics/instances/predicate/languages.py
+-rwxrwxrwx   0 root         (0) root         (0)     5209 2021-03-25 14:49:21.000000 logics-1.9.1/logics/instances/predicate/model_semantics.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 18:12:22.885845 logics-1.9.1/logics/instances/predicate/model_subclasses/
+-rwxrwxrwx   0 root         (0) root         (0)      109 2020-10-16 15:02:56.000000 logics-1.9.1/logics/instances/predicate/model_subclasses/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1606 2020-12-14 17:40:49.000000 logics-1.9.1/logics/instances/predicate/model_subclasses/arithmetic.py
+-rwxrwxrwx   0 root         (0) root         (0)     2274 2023-02-22 18:26:21.000000 logics-1.9.1/logics/instances/predicate/natural_deduction.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 18:12:23.028566 logics-1.9.1/logics/instances/propositional/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:18:54.000000 logics-1.9.1/logics/instances/propositional/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1022 2020-12-07 15:24:22.000000 logics-1.9.1/logics/instances/propositional/axiom_systems.py
+-rwxrwxrwx   0 root         (0) root         (0)     4316 2022-08-29 18:21:06.000000 logics-1.9.1/logics/instances/propositional/languages.py
+-rwxrwxrwx   0 root         (0) root         (0)    16665 2022-08-29 18:21:06.000000 logics-1.9.1/logics/instances/propositional/many_valued_semantics.py
+-rwxrwxrwx   0 root         (0) root         (0)    12138 2021-03-18 16:02:34.000000 logics-1.9.1/logics/instances/propositional/mapped_logic_semantics.py
+-rwxrwxrwx   0 root         (0) root         (0)    16069 2024-01-31 14:41:42.000000 logics-1.9.1/logics/instances/propositional/metainferential_tableaux.py
+-rwxrwxrwx   0 root         (0) root         (0)     8493 2023-04-10 16:32:18.000000 logics-1.9.1/logics/instances/propositional/natural_deduction.py
+-rwxrwxrwx   0 root         (0) root         (0)    17155 2022-02-03 19:56:56.000000 logics-1.9.1/logics/instances/propositional/sequents.py
+-rwxrwxrwx   0 root         (0) root         (0)    17045 2023-02-28 16:31:49.000000 logics-1.9.1/logics/instances/propositional/tableaux.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 18:12:23.032376 logics-1.9.1/logics/utils/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:17:53.000000 logics-1.9.1/logics/utils/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 18:12:23.038812 logics-1.9.1/logics/utils/formula_generators/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2020-11-23 15:19:08.000000 logics-1.9.1/logics/utils/formula_generators/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    31856 2024-02-16 21:00:29.000000 logics-1.9.1/logics/utils/formula_generators/generators_biased.py
+-rwxrwxrwx   0 root         (0) root         (0)       85 2021-03-26 15:35:46.000000 logics-1.9.1/logics/utils/formula_generators/generators_unbiased.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 18:12:23.067541 logics-1.9.1/logics/utils/parsers/
+-rwxrwxrwx   0 root         (0) root         (0)      169 2023-03-16 17:08:29.000000 logics-1.9.1/logics/utils/parsers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    16572 2021-03-25 14:03:02.000000 logics-1.9.1/logics/utils/parsers/parser_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)    21937 2023-02-23 18:39:04.000000 logics-1.9.1/logics/utils/parsers/predicate_parser.py
+-rwxrwxrwx   0 root         (0) root         (0)    28650 2022-08-29 18:21:06.000000 logics-1.9.1/logics/utils/parsers/standard_parser.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 18:12:23.107699 logics-1.9.1/logics/utils/solvers/
+-rwxrwxrwx   0 root         (0) root         (0)      196 2022-11-15 18:01:45.000000 logics-1.9.1/logics/utils/solvers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    17735 2023-02-22 18:26:21.000000 logics-1.9.1/logics/utils/solvers/first_order_natural_deduction.py
+-rwxrwxrwx   0 root         (0) root         (0)    65608 2023-02-22 18:26:21.000000 logics-1.9.1/logics/utils/solvers/natural_deduction.py
+-rwxrwxrwx   0 root         (0) root         (0)    15790 2023-04-13 20:12:20.000000 logics-1.9.1/logics/utils/solvers/sequents.py
+-rwxrwxrwx   0 root         (0) root         (0)    21035 2024-01-30 17:15:14.000000 logics-1.9.1/logics/utils/solvers/tableaux.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 18:12:23.125505 logics-1.9.1/logics/utils/upgrade/
+-rwxrwxrwx   0 root         (0) root         (0)       88 2023-02-22 18:26:21.000000 logics-1.9.1/logics/utils/upgrade/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1916 2023-02-22 18:26:21.000000 logics-1.9.1/logics/utils/upgrade/upgrade.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 18:12:23.127627 logics-1.9.1/logics.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)    12262 2024-02-21 18:12:22.000000 logics-1.9.1/logics.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2761 2024-02-21 18:12:22.000000 logics-1.9.1/logics.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-02-21 18:12:22.000000 logics-1.9.1/logics.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       15 2024-02-21 18:12:22.000000 logics-1.9.1/logics.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        7 2024-02-21 18:12:22.000000 logics-1.9.1/logics.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      104 2021-03-26 14:42:28.000000 logics-1.9.1/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)      906 2024-02-21 18:12:23.132777 logics-1.9.1/setup.cfg
```

### Comparing `logics-1.9.0/LICENSE.txt` & `logics-1.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/PKG-INFO` & `logics-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logics
-Version: 1.9.0
+Version: 1.9.1
 Summary: Logics is a Python framework for mathematical logic
 Home-page: https://github.com/ariroffe/logics
 Author: Ariel Jonathan Roffé
 Author-email: arielroffe@filo.uba.ar
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `logics-1.9.0/README.rst` & `logics-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/classes/errors.py` & `logics-1.9.1/logics/classes/errors.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/classes/exceptions.py` & `logics-1.9.1/logics/classes/exceptions.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/classes/predicate/formula.py` & `logics-1.9.1/logics/classes/predicate/formula.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/classes/predicate/language.py` & `logics-1.9.1/logics/classes/predicate/language.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/classes/predicate/proof_theories/natural_deduction.py` & `logics-1.9.1/logics/classes/predicate/proof_theories/natural_deduction.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/classes/predicate/semantics/models.py` & `logics-1.9.1/logics/classes/predicate/semantics/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -453,21 +453,21 @@
             if self.language.is_sentential_constant_string(formula[0]):
                 return self.sentential_constant_values_dict[formula[0]]
 
             # n-ary predicate followed by n terms
             predicate = formula[0]
             predicate_denotation = model.denotation(predicate, free_variable_denotation_dict)
             # Denotations of the terms
-            # 1-ary
-            if self.language.arity(predicate) == 1:
+            # 1-ary predicate
+            if len(formula) == 2:
                 term_denotations = model.denotation(formula[1], free_variable_denotation_dict)
                 # Callable
                 if callable(predicate_denotation):
                     return predicate_denotation(term_denotations)
-            # >1-ary
+            # >1-ary predicate
             else:
                 term_denotations = tuple(model.denotation(x, free_variable_denotation_dict) for x in formula[1:])
                 # Callable
                 if callable(predicate_denotation):
                     return predicate_denotation(*term_denotations)
             # Non callable, apply the atomic valuation clause
             return self.apply_truth_function('atomic', predicate_denotation, term_denotations)
```

### Comparing `logics-1.9.0/logics/classes/propositional/formula.py` & `logics-1.9.1/logics/classes/propositional/formula.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/classes/propositional/inference.py` & `logics-1.9.1/logics/classes/propositional/inference.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/classes/propositional/language.py` & `logics-1.9.1/logics/classes/propositional/language.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/classes/propositional/proof_theories/__init__.py` & `logics-1.9.1/logics/classes/propositional/proof_theories/__init__.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/classes/propositional/proof_theories/axiom_system.py` & `logics-1.9.1/logics/classes/propositional/proof_theories/axiom_system.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/classes/propositional/proof_theories/derivation.py` & `logics-1.9.1/logics/classes/propositional/proof_theories/derivation.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/classes/propositional/proof_theories/metainferential_tableaux.py` & `logics-1.9.1/logics/classes/propositional/proof_theories/metainferential_tableaux.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/classes/propositional/proof_theories/natural_deduction.py` & `logics-1.9.1/logics/classes/propositional/proof_theories/natural_deduction.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/classes/propositional/proof_theories/sequents.py` & `logics-1.9.1/logics/classes/propositional/proof_theories/sequents.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/classes/propositional/proof_theories/tableaux.py` & `logics-1.9.1/logics/classes/propositional/proof_theories/tableaux.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/classes/propositional/semantics/many_valued.py` & `logics-1.9.1/logics/classes/propositional/semantics/many_valued.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/classes/propositional/semantics/mapped_logic.py` & `logics-1.9.1/logics/classes/propositional/semantics/mapped_logic.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/instances/predicate/languages.py` & `logics-1.9.1/logics/instances/predicate/languages.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/instances/predicate/model_semantics.py` & `logics-1.9.1/logics/instances/predicate/model_semantics.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/instances/predicate/model_subclasses/arithmetic.py` & `logics-1.9.1/logics/instances/predicate/model_subclasses/arithmetic.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/instances/predicate/natural_deduction.py` & `logics-1.9.1/logics/instances/predicate/natural_deduction.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/instances/propositional/axiom_systems.py` & `logics-1.9.1/logics/instances/propositional/axiom_systems.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/instances/propositional/languages.py` & `logics-1.9.1/logics/instances/propositional/languages.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/instances/propositional/many_valued_semantics.py` & `logics-1.9.1/logics/instances/propositional/many_valued_semantics.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/instances/propositional/mapped_logic_semantics.py` & `logics-1.9.1/logics/instances/propositional/mapped_logic_semantics.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/instances/propositional/metainferential_tableaux.py` & `logics-1.9.1/logics/instances/propositional/metainferential_tableaux.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/instances/propositional/natural_deduction.py` & `logics-1.9.1/logics/instances/propositional/natural_deduction.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/instances/propositional/sequents.py` & `logics-1.9.1/logics/instances/propositional/sequents.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/instances/propositional/tableaux.py` & `logics-1.9.1/logics/instances/propositional/tableaux.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/utils/formula_generators/generators_biased.py` & `logics-1.9.1/logics/utils/formula_generators/generators_biased.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,589 +1,589 @@
-import random
-from copy import copy
-
-from logics.classes.propositional import Formula, Inference
-from logics.classes.predicate import PredicateFormula
-from logics.classes.exceptions import FormulaGeneratorError
-
-
-class BiasedPropositionalGenerator:
-    """A biased random propositional generator.
-
-    It is biased because it will not return every formula/inference within the space asked with the same probability.
-    On the other hand, it is *much* faster than its non-biased counterpart.
-
-    Examples
-    --------
-    This generator takes no parameters, so to instantiate one you can simply do:
-
-    >>> from logics.utils.formula_generators.generators_biased import BiasedPropositionalGenerator
-    >>> random_generator = BiasedPropositionalGenerator()
-
-    There is also a predefined instance so there is even no need to instantiate it
-
-    >>> from logics.utils.formula_generators.generators_biased import random_formula_generator
-    """
-    # ------------------------------------------------------------------------------------------------------------------
-    # FORMULAE
-
-    def random_formula(self, depth, atomics, language, exact_depth=True, all_atomics=False):
-        """Generates a random formula for the language given.
-
-        Parameters
-        ----------
-        depth: int
-            A positive integer, representing the depth of the formula to obtain
-        atomics: list of str
-            The sublist of atomics of the language that the formula will be built of
-        language: logics.classes.propositional.Language or logics.classes.propositional.InfiniteLanguage
-            Instance of Language or InfiniteLanguage
-        exact_depth: bool
-            If true, the resulting formula will have *exactly* the depth given. Otherwise, will have *up to* that depth.
-            Defaults to True.
-        all_atomics: bool
-            If true, the resulting formula will contain *all* the atomics given. Otherwise, can contain *some* of them.
-            Defaults to False.
-
-        Returns
-        -------
-        logics.classes.propositional.Formula
-            A randomly generated formula of the given depth, containing some or all the atomics
-
-        Raises
-        ------
-        NotImplemented
-            If exact_depth is False and all_atomics is True
-        ValueError
-            If exact_depth is True, all_atomics is True and the number of atomics given > the maximum arity constant of
-            the language ** depth.
-            For example, it is not possible to build a formula of depth 1 with 3 atomics in a language that has
-            connectives of at most arity 2.
-
-        Examples
-        --------
-        Exact depth and not all atomics
-
-        >>> from logics.instances.propositional.languages import classical_language
-        >>> from logics.utils.formula_generators.generators_biased import random_formula_generator
-        >>> random_formula_generator.random_formula(depth=3, atomics=['p', 'q', 'r'],
-        ...                                         language=classical_language,
-        ...                                         exact_depth=True, all_atomics=False)
-        ['→', ['→', ['p'], ['↔', ['r'], ['p']]], ['~', ['r']]]
-        >>> random_formula_generator.random_formula(depth=3, atomics=['p', 'q', 'r'],
-        ...                                         language=classical_language,
-        ...                                         exact_depth=True, all_atomics=False)
-        ['↔', ['∨', ['~', ['r']], ['r']], ['↔', ['p'], ['q']]]
-
-        Not exact depth and not all atomics
-
-        >>> random_formula_generator.random_formula(depth=3, atomics=['p', 'q', 'r'],
-        ...                                         language=classical_language,
-        ...                                         exact_depth=False, all_atomics=False)
-        ['∨', ['r'], ['q']]
-        >>> random_formula_generator.random_formula(depth=3, atomics=['p', 'q', 'r'],
-        ...                                         language=classical_language,
-        ...                                         exact_depth=False, all_atomics=False)
-        ['→', ['r'], ['∨', ['p'], ['r']]]
-
-        Exact depth and all atomics
-
-        >>> random_formula_generator.random_formula(depth=3, atomics=['p', 'q', 'r'],
-        ...                                         language=classical_language,
-        ...                                         exact_depth=True, all_atomics=True)
-        ['~', ['∧', ['∧', ['r'], ['q']], ['p']]]
-        >>> random_formula_generator.random_formula(depth=3, atomics=['p', 'q', 'r'],
-        ...                                         language=classical_language,
-        ...                                         exact_depth=True, all_atomics=True)
-        ['∨', ['∨', ['∧', ['q'], ['r']], ['→', ['r'], ['q']]], ['p']]
-        """
-
-        if exact_depth and all_atomics:
-            return self._exact_depth_all_atomics(depth, atomics, language)
-        elif exact_depth and not all_atomics:
-            return self._exact_depth_some_atomics(depth, atomics, language)
-        elif not exact_depth and not all_atomics:
-            return self._upto_depth_some_atomics(depth, atomics, language)
-        else:
-            raise NotImplemented('This method does not yet accept a non-exact depth and all atomics')
-
-    def _exact_depth_some_atomics(self, depth, atomics, language):
-        """Generates a random formula of some *exact* depth, which includes *some* of the atomics given."""
-        if depth == 0:
-            return Formula([random.choice(atomics)])
-
-        else:
-            constant = random.choice(tuple(language.constants()))
-            arity = language.arity(constant)
-            formula = Formula([constant])
-            formula.extend([None] * arity)  # By now, formula is something like ['^', None, None]
-
-            # Randomly choose an index and put a formula of depth - 1 there
-            # (to ensure the formula reaches the depth given)
-            i = random.randint(1, arity)  # index 0 is the constant
-            formula[i] = self._exact_depth_some_atomics(depth-1, atomics, language)
-
-            # In the rest of the arguments put a formula of random depth
-            for x in set(range(1, arity+1)) - {i}:
-                j = random.randint(0, depth-1)
-                formula[x] = self._exact_depth_some_atomics(j, atomics, language)
-
-            return formula
-
-    def _upto_depth_some_atomics(self, depth, atomics, language):
-        """Generates a random formula of *up to* some depth, which includes *some* of the atomics given.
-        Works very similarly to the method above
-        """
-
-        # Choose a depth and then call the previous function
-        chosen_depth = random.randint(0, depth)
-        return self._exact_depth_some_atomics(chosen_depth, atomics, language)
-
-    def _exact_depth_all_atomics(self, depth, atomics, language):
-        """Generates a random formula of some *exact* depth, which includes *all* of the atomics given."""
-        # Brute force approach, will use g_ES and then check if all the atomics are present
-        # Tries up to 100 times, then raises an RuntimeError exception
-        # Should be possible to build a better function (see below).
-
-        # Validate that the request is possible
-        if len(atomics) > max(language.constant_arity_dict.values()) ** depth:
-            raise ValueError("len(atomics) can be at most the maximum arity of a constant of the language ** depth")
-
-        for x in range(100):
-            acceptable = True
-            formula = self._exact_depth_some_atomics(depth, atomics, language)
-            for at in atomics:
-                if at not in str(formula):
-                    acceptable = False
-            if acceptable:
-                return formula
-
-        raise FormulaGeneratorError('Could not generate a formula with the desired parameters')
-
-    def exact_depth_all_atomics2(self, depth, atomics, language):
-        # todo FIX THIS - for depth 1 and ['p', 'q'] the first part can return ~['$']
-
-        # Validate that the request is possible
-        if len(atomics) > max(language.constant_arity_dict.values()) ** depth:
-            raise ValueError("len(atomics) can be at most the maximum arity of a constant of the language ** depth")
-
-        # Generate a formula with placeholders where the atomics will be
-        formula_with_placeholders = self._exact_depth_some_atomics(depth, ['$'], language)
-
-        # For each atomic, replace at least one placeholder for it (so that every atomic appears at least once)
-        formula_string = str(formula_with_placeholders)
-        placeholder_indexes = [x for x in range(len(formula_string)) if formula_string[x] == '$']
-        for atomic in atomics:
-            # Choose an index and remove it from the list
-            chosen_index = random.choice(placeholder_indexes)
-            placeholder_indexes.remove(chosen_index)
-            # Replace the index with the atomic
-            formula_string = formula_string[:chosen_index] + atomic + formula_string[chosen_index+1:]
-
-        # The remaining placeholders replace them with a random choice of atomics
-        for index in placeholder_indexes:
-            chosen_atomic = random.choice(atomics)
-            formula_string = formula_string[:index] + chosen_atomic + formula_string[index+1:]
-
-        formula = Formula(eval(formula_string))
-        return formula
-
-    # ------------------------------------------------------------------------------------------------------------------
-    # INFERENCE
-
-    def random_inference(self, num_premises, num_conclusions, max_depth, atomics, language, level=1,
-                         exact_num_premises=True, exact_num_conclusions=True):
-        """Generates a random Inference.
-
-        Takes a number of premises and of conclusions (either exact or up to, see the `exact_num_premises` and
-        `exact_num_conclusions` parameters below), and populates them with formuale of *up to* the given `max_depth`
-        and *some* of the given `atomics`.
-
-        Can also be used to generate metainferences, if given a `level` > 1. In that case, the inferences in the
-        premises / conclusions will have *up to* that number of premises and conclusions. That is, if asked for an
-        inference of level 2 with exactly two premises, the premises will themselves be inferences, and they may contain
-        less than two premises.
-
-        Parameters
-        ----------
-        num_premises: int
-            The exact number of premises the inference will contain
-        num_conclusions: int
-            The exact number of conclusions the inference will contain
-        max_depth: int
-            The maximum depth that the formulae within the inference can contain
-        atomics: list of str
-            The sublist of atomics of the language that the formulae within the inference will be built of
-        language: logics.classes.propositional.Language or logics.classes.propositional.InfiniteLanguage
-            Instance of Language or InfiniteLanguage
-        level: int, optional
-            Level of the inference to be generated (1 is regular inference, 2 is metainference, 3 is metameta, ...).
-            level is 1 by default.
-        exact_num_premises: bool
-            If True, the resulting inference will contain will contain *exactly* that number of premises, otherwise will
-            contain *up to* that number of premises. Defaults to True.
-        exact_num_conclusions: bool
-            If True, the resulting inference will contain will contain *exactly* that number of premises, otherwise will
-            contain *up to* that number of premises. Defaults to True.
-
-        Returns
-        -------
-        logics.classes.propositional.Inference
-            A randomly generated inference of the given parameters.
-
-        Examples
-        --------
-        Random inferences with exactly two premises and one conclusion:
-
-        >>> from logics.instances.propositional.languages import classical_language
-        >>> from logics.utils.parsers import classical_parser
-        >>> from logics.utils.formula_generators.generators_biased import random_formula_generator
-        >>> inf = random_formula_generator.random_inference(num_premises=2, num_conclusions=1,
-        ...                                                 max_depth=2, atomics=['p', 'q'],
-        ...                                                 language=classical_language, level=1,
-        ...                                                 exact_num_premises=True,
-        ...                                                 exact_num_conclusions=True)
-        >>> classical_parser.unparse(inf)
-        '(p ∧ p), ((q ∨ q) ∧ (p ∨ p)) / ~q'
-        >>> inf = random_formula_generator.random_inference(num_premises=2, num_conclusions=1,
-        ...                                                 max_depth=2, atomics=['p', 'q'],
-        ...                                                 language=classical_language, level=1,
-        ...                                                 exact_num_premises=True,
-        ...                                                 exact_num_conclusions=True)
-        >>> classical_parser.unparse(inf)
-        '~(q ↔ q), q / (q ∧ (p → p))'
-
-        Random inferences with up to two premises and two conclusions
-
-        >>> inf = random_formula_generator.random_inference(num_premises=2, num_conclusions=2,
-        ...                                                 max_depth=2, atomics=['p', 'q'],
-        ...                                                 language=classical_language, level=1,
-        ...                                                 exact_num_premises=False,
-        ...                                                 exact_num_conclusions=False)
-        >>> classical_parser.unparse(inf)
-        '(p ↔ p) / ~q'
-        >>> inf = random_formula_generator.random_inference(num_premises=2, num_conclusions=2,
-        ...                                                 max_depth=2, atomics=['p', 'q'],
-        ...                                                 language=classical_language, level=1,
-        ...                                                 exact_num_premises=False,
-        ...                                                 exact_num_conclusions=False)
-        >>> classical_parser.unparse(inf)
-        '/'
-
-        Random metainferences with up to two premises and two conclusions
-
-        >>> inf = random_formula_generator.random_inference(num_premises=2, num_conclusions=2,
-        ...                                                 max_depth=2, atomics=['p', 'q'],
-        ...                                                 language=classical_language, level=2,
-        ...                                                 exact_num_premises=False,
-        ...                                                 exact_num_conclusions=False)
-        >>> classical_parser.unparse(inf)
-        '((q → (q → q)) /), ((p ↔ p), (q ∧ p) / (q ∨ q), p) //'
-        >>> inf = random_formula_generator.random_inference(num_premises=2, num_conclusions=2,
-        ...                                                 max_depth=2, atomics=['p', 'q'],
-        ...                                                 language=classical_language, level=2,
-        ...                                                 exact_num_premises=False,
-        ...                                                 exact_num_conclusions=False)
-        >>> classical_parser.unparse(inf)
-        '(/) //'
-        """
-        if level == 0:
-            raise ValueError('Inferences cannot have level 0')
-
-        # Premises
-        premises = list()
-        new_num_premises = num_premises
-        if not exact_num_premises:
-            new_num_premises = random.randint(0, num_premises)
-
-        for _ in range(new_num_premises):
-            if level == 1:
-                premises.append(self._upto_depth_some_atomics(max_depth, atomics, language))
-            else:
-                premises.append(self.random_inference(num_premises, num_conclusions, max_depth, atomics, language,
-                                                      level=level-1, exact_num_premises=False,
-                                                      exact_num_conclusions=False))
-
-        # Conclusions
-        conclusions = list()
-        new_num_conclusions = num_conclusions
-        if not exact_num_conclusions:
-            new_num_conclusions = random.randint(0, num_conclusions)
-
-        for _ in range(new_num_conclusions):
-            if level == 1:
-                conclusions.append(self._upto_depth_some_atomics(max_depth, atomics, language))
-            else:
-                conclusions.append(self.random_inference(num_premises, num_conclusions,
-                                                         max_depth, atomics, language, level=level-1))
-
-        return Inference(premises=premises, conclusions=conclusions, level=level)
-
-    # ------------------------------------------------------------------------------------------------------------------
-    # THINGS WITH VALIDITY APPARATUSES
-
-    def random_tautology(self, depth, atomics, language, validity_apparatus, exact_depth=True, all_atomics=False,
-                         attempts=100):
-        """Generates a random tautogy for the validity apparatus given.
-
-        Will generate a random formula and then test the inference ([] / [formula]) to see if it is valid. If it is,
-        returns it, otherwise generates another. Can fail for at most the number of `attempts` given.
-
-        The signature is very similar to that of random_formula but takes two extra parameters:
-
-            * validity_apparatus: any object with an is_valid method (which takes an inference as argument)
-            * attempts: an `int`, maximum number of formulae it generates and tests (defaults to 100)
-
-        Returns
-        -------
-        logics.classes.propositional.Formula
-            A randomly generated tautology of the given depth, containing some or all the atomics
-
-        Raises
-        ------
-        NotImplemented
-            If exact_depth is False and all_atomics is True
-        ValueError
-            If exact_depth is True, all_atomics is True and the number of atomics given > the maximum arity constant of
-            the language ** depth.
-        FormulaGeneratorError
-            If it cannot find a tautology in the given number of `attempts`
-
-        Examples
-        --------
-        >>> from logics.instances.propositional.languages import classical_language
-        >>> from logics.instances.propositional.many_valued_semantics import classical_mvl_semantics
-        >>> from logics.utils.formula_generators.generators_biased import random_formula_generator
-        >>> random_formula_generator.random_tautology(depth=2, atomics=['p', 'q'],
-        ...                                           language=classical_language,
-        ...                                           validity_apparatus=classical_mvl_semantics)
-        ['→', ['∧', ['q'], ['p']], ['∧', ['q'], ['q']]]
-        >>> random_formula_generator.random_tautology(depth=2, atomics=['p', 'q'],
-        ...                                           language=classical_language,
-        ...                                           validity_apparatus=classical_mvl_semantics)
-        ['→', ['p'], ['∨', ['p'], ['p']]]
-        """
-        for _ in range(attempts):
-            if exact_depth and all_atomics:
-                formula = self._exact_depth_all_atomics(depth, atomics, language)
-            elif exact_depth and not all_atomics:
-                formula = self._exact_depth_some_atomics(depth, atomics, language)
-            elif not exact_depth and not all_atomics:
-                formula = self._upto_depth_some_atomics(depth, atomics, language)
-            else:
-                raise NotImplemented('Not exact depth and all atomics generator not implemented yet')
-
-            inf = Inference(premises=[], conclusions=[formula])
-            if validity_apparatus.is_valid(inf):
-                return formula
-
-        raise FormulaGeneratorError('Could not generate tautology with the parameters given')
-
-    def random_valid_inference(self, num_premises, num_conclusions, max_depth, atomics, language, validity_apparatus,
-                               level=1, exact_num_premises=True, exact_num_conclusions=True, attempts=100):
-        """Generates a random *valid* inference for the validity apparatus given.
-
-        Similar to the random_inference method. The two new parameters are to the method above.
-        In particular, The object passed to `validity_apparatus` must have an `is_valid` method.
-        If `level` > 1 the validity apparatus must be able to handle metainferential validity.
-
-        Returns
-        -------
-        logics.classes.propositional.Inference
-            A randomly generated valid inference or metainference with the parameters given
-
-        Raises
-        ------
-        FormulaGeneratorError
-            If it cannot find a valid inference in the given number of `attempts`
-
-        Examples
-        --------
-        >>> from logics.instances.propositional.languages import classical_language
-        >>> from logics.utils.parsers import classical_parser
-        >>> from logics.instances.propositional.many_valued_semantics import classical_mvl_semantics
-        >>> from logics.utils.formula_generators.generators_biased import random_formula_generator
-        >>> inf = random_formula_generator.random_valid_inference(num_premises=2, num_conclusions=1,
-        ...                                                       max_depth=2, atomics=['p', 'q'],
-        ...                                                       language=classical_language, level=1,
-        ...                                                       validity_apparatus=classical_mvl_semantics)
-        >>> classical_parser.unparse(inf)
-        '(q ↔ p), p / (p ∨ q)'
-        >>> inf = random_formula_generator.random_valid_inference(num_premises=2, num_conclusions=1,
-        ...                                                       max_depth=2, atomics=['p', 'q'],
-        ...                                                       language=classical_language, level=2,
-        ...                                                       validity_apparatus=classical_mvl_semantics)
-        >>> classical_parser.unparse(inf)
-        '(p / p), (p, ((q → p) ∧ (p ∨ p)) / (p ↔ (q ↔ p))) // (((p ↔ p) ∨ p), ~q / (q ∨ ~p))'
-        """
-        for _ in range(attempts):
-            inf = self.random_inference(num_premises, num_conclusions, max_depth, atomics, language, level,
-                                        exact_num_premises, exact_num_conclusions)
-            if validity_apparatus.is_valid(inf):
-                return inf
-
-        raise FormulaGeneratorError('Could not generate valid inference with the parameters given')
-
-    def random_invalid_inference(self, num_premises, num_conclusions, max_depth, atomics, language, validity_apparatus,
-                                 level=1, exact_num_premises=True, exact_num_conclusions=True, attempts=100):
-        """Generates a random *invalid* inference for the validity apparatus given.
-
-        Identical to the method above, only that it returns an *invalid* inference.
-        """
-        for _ in range(attempts):
-            inf = self.random_inference(num_premises, num_conclusions, max_depth, atomics, language, level,
-                                        exact_num_premises, exact_num_conclusions)
-            if not validity_apparatus.is_valid(inf):
-                return inf
-
-        raise FormulaGeneratorError('Could not generate valid inference with the parameters given')
-
-
-random_formula_generator = BiasedPropositionalGenerator()
-
-
-# ----------------------------------------------------------------------------------------------------------------------
-# Predicate formula generator
-
-class BiasedPredicateGenerator:
-    """A biased random predicate generator.
-
-        It is biased because it will not return every formula/inference within the space asked with the same probability.
-        There is no non-biased generator implemented in this package yet.
-        This implementation does not yet work with function symbols.
-
-        Examples
-        --------
-        This generator takes no parameters, so to instantiate one you can simply do:
-
-        >>> from logics.utils.formula_generators.generators_biased import BiasedPredicateGenerator
-        >>> random_generator = BiasedPredicateGenerator()
-
-        There is also a predefined instance so there is even no need to instantiate it
-
-        >>> from logics.utils.formula_generators.generators_biased import random_predicate_formula_generator
-        """
-    def _random_term(self, ind_constants, variables):
-        # We select an ind_constant and a variable with equal probability, even if there is just 1 var and 5 ind_cts
-        if not variables or random.choice((True, False)):
-            return random.choice(ind_constants)
-        else:
-            return random.choice(variables)
-
-    def _random_atomic_formula(self, predicates, max_arity, ind_constants, variables, predicate_arities):
-        # Firstly, we must choose a predicate and set its arity
-        predicate = random.choice(predicates)
-        formula = PredicateFormula([predicate])
-        if predicate in predicate_arities:
-            arity = predicate_arities[predicate]
-        else:
-            arity = random.randint(1, max_arity)
-            predicate_arities[predicate] = arity  # Modify the dict, will be seen by the caller
-
-        for _ in range(arity):
-            formula.append(self._random_term(ind_constants, variables))
-
-        return formula
-
-    def random_formula(self, depth, predicates, max_predicate_arity, ind_constants, variables, language,
-                       remaining_depth=0, predicate_arities=None):
-        """Generates a random formula of some *exact* depth, which uses some of the predicates, variables and ind cts
-        provided
-
-        Because of the educational usecases I have in mind, I don't want it to output things like ∀x P(a) or like
-        ∀x ∀x P(x). More precisely, Its made so every quantifier binds at least one variable.
-
-        Assumes that the predicate arities can be random (i.e. will not respect the
-        predicate_letters={'P': 1, 'Q': 1, 'R': 2, 'S': 3} argument given to PredicateLanguage). If you want it to,
-        give it predicate_arities=language.predicate_letters
-
-        Examples
-        --------
-        >>> from logics.instances.predicate.languages import classical_predicate_language as lang
-        >>> from logics.utils.parsers import classical_predicate_parser
-        >>> from logics.utils.formula_generators.generators_biased import random_predicate_formula_generator
-        >>> for _ in range(5):
-        ...     formula = random_predicate_formula_generator.random_formula(depth=2, predicates=['P', 'Q'],
-        ...         max_predicate_arity=2, ind_constants=['a', 'b'], variables=['x', 'y'], language=lang)
-        ...     print(classical_predicate_parser.unparse(formula))
-        Q(b, a) → ∀x Q(x, x)
-        ∀y Q(y) ∧ Q(b)
-        ∀x (Q(b) ∧ P(x, a))
-        ∀y (Q(y, a) ∧ P(y, y))
-        ∃x P(x) ∨ P(b)
-        """
-        if predicate_arities is None:
-            predicate_arities = dict()
-
-        if depth == 0:
-            # We must make sure that the number of free variables in this atomic is not greater than the
-            # remaining depth, otherwise we cannot get to bind them all.
-            # E.g. if we originally asked for depth=1, when this clause is reached, remaining_depth==1
-            # and variables[:remaining_depth] will be ['x']
-            return self._random_atomic_formula(predicates, max_predicate_arity, ind_constants,
-                                               variables[:remaining_depth], predicate_arities)
-
-        else:
-            # We proceed recursively in the reverse direction than the other generator, that is, we go bottom-up
-            # First generate a subformula
-            first_argument = self.random_formula(depth-1, predicates, max_predicate_arity, ind_constants, variables,
-                                                 language, remaining_depth+1, predicate_arities)
-
-            # Check the free variables in the first arg
-            free_vars = first_argument.free_variables(language)
-            # If free_vars is ['x', 'y'], rem_depth must be at least 1
-            # since one quantifier can be introduced here, and the and another in the remaining top call
-            assert remaining_depth + 1 >= len(free_vars)
-            # if remaining_depth + 1 < len(free_vars):
-            #     print("ERROR", first_argument, depth, remaining_depth, free_vars)
-            #     raise ValueError("Fix this")
-
-            # Then choose a logical constant
-            if not free_vars:
-                # If there are no free variables, do not introduce quantifiers that bind nothing
-                constant = random.choice(tuple(language.constants()))
-            elif remaining_depth + 1 == len(free_vars):
-                # We MUST choose a quantifier
-                # e.g.  remaining depth is 0 (this is the last constant introduced) and we have 1 free variable
-                # e.g.2 remaining depth is 1 (we will introduce this + 1 ctt) and we have 2 free variables
-                constant = random.choice(language.quantifiers)
-            else:
-                # Otherwise can be either a quantifier or a logical constant, choose with equal prob so that
-                # there is no bias for all the quantifiers to be at the beginning of the formula
-                if random.choice((True, False)):
-                    constant = random.choice(tuple(language.constants()))
-                else:
-                    constant = random.choice(language.quantifiers)
-
-            arity = language.arity(constant)
-
-            # Quantified formula
-            if constant in language.quantifiers:
-                variable = random.choice(list(free_vars))
-                return PredicateFormula([constant, variable, first_argument])
-
-            # Unary connective formula
-            elif arity == 1:
-                return PredicateFormula([constant, first_argument])
-
-            # Binary connective formula
-            else:
-                # We must be careful here bc the second subformula could introduce more free variables
-                # We can use the free variables in the first_argument freely, though
-                # E.g. if x is already free here, and we have 2 remaining depth (will introduce 2 more cts--do not count
-                # this one bc it is not a quantifier) -- then the second subformula can contain one extra var
-                new_vars = list(free_vars)
-                extra_vars_allowed = remaining_depth - len(free_vars)
-                if extra_vars_allowed:
-                    extra_vars = [v for v in variables if v not in new_vars]
-                    new_vars.extend(extra_vars[:extra_vars_allowed])
-
-                second_argument = self.random_formula(random.randint(0, depth-1), predicates, max_predicate_arity,
-                                                      ind_constants, new_vars, language, remaining_depth+1,
-                                                      predicate_arities)
-                if random.choice((True, False)):
-                    return PredicateFormula([constant, first_argument, second_argument])
-                else:
-                    return PredicateFormula([constant, second_argument, first_argument])
-
-
-random_predicate_formula_generator = BiasedPredicateGenerator()
+import random
+from copy import copy
+
+from logics.classes.propositional import Formula, Inference
+from logics.classes.predicate import PredicateFormula
+from logics.classes.exceptions import FormulaGeneratorError
+
+
+class BiasedPropositionalGenerator:
+    """A biased random propositional generator.
+
+    It is biased because it will not return every formula/inference within the space asked with the same probability.
+    On the other hand, it is *much* faster than its non-biased counterpart.
+
+    Examples
+    --------
+    This generator takes no parameters, so to instantiate one you can simply do:
+
+    >>> from logics.utils.formula_generators.generators_biased import BiasedPropositionalGenerator
+    >>> random_generator = BiasedPropositionalGenerator()
+
+    There is also a predefined instance so there is even no need to instantiate it
+
+    >>> from logics.utils.formula_generators.generators_biased import random_formula_generator
+    """
+    # ------------------------------------------------------------------------------------------------------------------
+    # FORMULAE
+
+    def random_formula(self, depth, atomics, language, exact_depth=True, all_atomics=False):
+        """Generates a random formula for the language given.
+
+        Parameters
+        ----------
+        depth: int
+            A positive integer, representing the depth of the formula to obtain
+        atomics: list of str
+            The sublist of atomics of the language that the formula will be built of
+        language: logics.classes.propositional.Language or logics.classes.propositional.InfiniteLanguage
+            Instance of Language or InfiniteLanguage
+        exact_depth: bool
+            If true, the resulting formula will have *exactly* the depth given. Otherwise, will have *up to* that depth.
+            Defaults to True.
+        all_atomics: bool
+            If true, the resulting formula will contain *all* the atomics given. Otherwise, can contain *some* of them.
+            Defaults to False.
+
+        Returns
+        -------
+        logics.classes.propositional.Formula
+            A randomly generated formula of the given depth, containing some or all the atomics
+
+        Raises
+        ------
+        NotImplemented
+            If exact_depth is False and all_atomics is True
+        ValueError
+            If exact_depth is True, all_atomics is True and the number of atomics given > the maximum arity constant of
+            the language ** depth.
+            For example, it is not possible to build a formula of depth 1 with 3 atomics in a language that has
+            connectives of at most arity 2.
+
+        Examples
+        --------
+        Exact depth and not all atomics
+
+        >>> from logics.instances.propositional.languages import classical_language
+        >>> from logics.utils.formula_generators.generators_biased import random_formula_generator
+        >>> random_formula_generator.random_formula(depth=3, atomics=['p', 'q', 'r'],
+        ...                                         language=classical_language,
+        ...                                         exact_depth=True, all_atomics=False)
+        ['→', ['→', ['p'], ['↔', ['r'], ['p']]], ['~', ['r']]]
+        >>> random_formula_generator.random_formula(depth=3, atomics=['p', 'q', 'r'],
+        ...                                         language=classical_language,
+        ...                                         exact_depth=True, all_atomics=False)
+        ['↔', ['∨', ['~', ['r']], ['r']], ['↔', ['p'], ['q']]]
+
+        Not exact depth and not all atomics
+
+        >>> random_formula_generator.random_formula(depth=3, atomics=['p', 'q', 'r'],
+        ...                                         language=classical_language,
+        ...                                         exact_depth=False, all_atomics=False)
+        ['∨', ['r'], ['q']]
+        >>> random_formula_generator.random_formula(depth=3, atomics=['p', 'q', 'r'],
+        ...                                         language=classical_language,
+        ...                                         exact_depth=False, all_atomics=False)
+        ['→', ['r'], ['∨', ['p'], ['r']]]
+
+        Exact depth and all atomics
+
+        >>> random_formula_generator.random_formula(depth=3, atomics=['p', 'q', 'r'],
+        ...                                         language=classical_language,
+        ...                                         exact_depth=True, all_atomics=True)
+        ['~', ['∧', ['∧', ['r'], ['q']], ['p']]]
+        >>> random_formula_generator.random_formula(depth=3, atomics=['p', 'q', 'r'],
+        ...                                         language=classical_language,
+        ...                                         exact_depth=True, all_atomics=True)
+        ['∨', ['∨', ['∧', ['q'], ['r']], ['→', ['r'], ['q']]], ['p']]
+        """
+
+        if exact_depth and all_atomics:
+            return self._exact_depth_all_atomics(depth, atomics, language)
+        elif exact_depth and not all_atomics:
+            return self._exact_depth_some_atomics(depth, atomics, language)
+        elif not exact_depth and not all_atomics:
+            return self._upto_depth_some_atomics(depth, atomics, language)
+        else:
+            raise NotImplemented('This method does not yet accept a non-exact depth and all atomics')
+
+    def _exact_depth_some_atomics(self, depth, atomics, language):
+        """Generates a random formula of some *exact* depth, which includes *some* of the atomics given."""
+        if depth == 0:
+            return Formula([random.choice(atomics)])
+
+        else:
+            constant = random.choice(tuple(language.constants()))
+            arity = language.arity(constant)
+            formula = Formula([constant])
+            formula.extend([None] * arity)  # By now, formula is something like ['^', None, None]
+
+            # Randomly choose an index and put a formula of depth - 1 there
+            # (to ensure the formula reaches the depth given)
+            i = random.randint(1, arity)  # index 0 is the constant
+            formula[i] = self._exact_depth_some_atomics(depth-1, atomics, language)
+
+            # In the rest of the arguments put a formula of random depth
+            for x in set(range(1, arity+1)) - {i}:
+                j = random.randint(0, depth-1)
+                formula[x] = self._exact_depth_some_atomics(j, atomics, language)
+
+            return formula
+
+    def _upto_depth_some_atomics(self, depth, atomics, language):
+        """Generates a random formula of *up to* some depth, which includes *some* of the atomics given.
+        Works very similarly to the method above
+        """
+
+        # Choose a depth and then call the previous function
+        chosen_depth = random.randint(0, depth)
+        return self._exact_depth_some_atomics(chosen_depth, atomics, language)
+
+    def _exact_depth_all_atomics(self, depth, atomics, language):
+        """Generates a random formula of some *exact* depth, which includes *all* of the atomics given."""
+        # Brute force approach, will use g_ES and then check if all the atomics are present
+        # Tries up to 100 times, then raises an RuntimeError exception
+        # Should be possible to build a better function (see below).
+
+        # Validate that the request is possible
+        if len(atomics) > max(language.constant_arity_dict.values()) ** depth:
+            raise ValueError("len(atomics) can be at most the maximum arity of a constant of the language ** depth")
+
+        for x in range(100):
+            acceptable = True
+            formula = self._exact_depth_some_atomics(depth, atomics, language)
+            for at in atomics:
+                if at not in str(formula):
+                    acceptable = False
+            if acceptable:
+                return formula
+
+        raise FormulaGeneratorError('Could not generate a formula with the desired parameters')
+
+    def exact_depth_all_atomics2(self, depth, atomics, language):
+        # todo FIX THIS - for depth 1 and ['p', 'q'] the first part can return ~['$']
+
+        # Validate that the request is possible
+        if len(atomics) > max(language.constant_arity_dict.values()) ** depth:
+            raise ValueError("len(atomics) can be at most the maximum arity of a constant of the language ** depth")
+
+        # Generate a formula with placeholders where the atomics will be
+        formula_with_placeholders = self._exact_depth_some_atomics(depth, ['$'], language)
+
+        # For each atomic, replace at least one placeholder for it (so that every atomic appears at least once)
+        formula_string = str(formula_with_placeholders)
+        placeholder_indexes = [x for x in range(len(formula_string)) if formula_string[x] == '$']
+        for atomic in atomics:
+            # Choose an index and remove it from the list
+            chosen_index = random.choice(placeholder_indexes)
+            placeholder_indexes.remove(chosen_index)
+            # Replace the index with the atomic
+            formula_string = formula_string[:chosen_index] + atomic + formula_string[chosen_index+1:]
+
+        # The remaining placeholders replace them with a random choice of atomics
+        for index in placeholder_indexes:
+            chosen_atomic = random.choice(atomics)
+            formula_string = formula_string[:index] + chosen_atomic + formula_string[index+1:]
+
+        formula = Formula(eval(formula_string))
+        return formula
+
+    # ------------------------------------------------------------------------------------------------------------------
+    # INFERENCE
+
+    def random_inference(self, num_premises, num_conclusions, max_depth, atomics, language, level=1,
+                         exact_num_premises=True, exact_num_conclusions=True):
+        """Generates a random Inference.
+
+        Takes a number of premises and of conclusions (either exact or up to, see the `exact_num_premises` and
+        `exact_num_conclusions` parameters below), and populates them with formuale of *up to* the given `max_depth`
+        and *some* of the given `atomics`.
+
+        Can also be used to generate metainferences, if given a `level` > 1. In that case, the inferences in the
+        premises / conclusions will have *up to* that number of premises and conclusions. That is, if asked for an
+        inference of level 2 with exactly two premises, the premises will themselves be inferences, and they may contain
+        less than two premises.
+
+        Parameters
+        ----------
+        num_premises: int
+            The exact number of premises the inference will contain
+        num_conclusions: int
+            The exact number of conclusions the inference will contain
+        max_depth: int
+            The maximum depth that the formulae within the inference can contain
+        atomics: list of str
+            The sublist of atomics of the language that the formulae within the inference will be built of
+        language: logics.classes.propositional.Language or logics.classes.propositional.InfiniteLanguage
+            Instance of Language or InfiniteLanguage
+        level: int, optional
+            Level of the inference to be generated (1 is regular inference, 2 is metainference, 3 is metameta, ...).
+            level is 1 by default.
+        exact_num_premises: bool
+            If True, the resulting inference will contain will contain *exactly* that number of premises, otherwise will
+            contain *up to* that number of premises. Defaults to True.
+        exact_num_conclusions: bool
+            If True, the resulting inference will contain will contain *exactly* that number of premises, otherwise will
+            contain *up to* that number of premises. Defaults to True.
+
+        Returns
+        -------
+        logics.classes.propositional.Inference
+            A randomly generated inference of the given parameters.
+
+        Examples
+        --------
+        Random inferences with exactly two premises and one conclusion:
+
+        >>> from logics.instances.propositional.languages import classical_language
+        >>> from logics.utils.parsers import classical_parser
+        >>> from logics.utils.formula_generators.generators_biased import random_formula_generator
+        >>> inf = random_formula_generator.random_inference(num_premises=2, num_conclusions=1,
+        ...                                                 max_depth=2, atomics=['p', 'q'],
+        ...                                                 language=classical_language, level=1,
+        ...                                                 exact_num_premises=True,
+        ...                                                 exact_num_conclusions=True)
+        >>> classical_parser.unparse(inf)
+        '(p ∧ p), ((q ∨ q) ∧ (p ∨ p)) / ~q'
+        >>> inf = random_formula_generator.random_inference(num_premises=2, num_conclusions=1,
+        ...                                                 max_depth=2, atomics=['p', 'q'],
+        ...                                                 language=classical_language, level=1,
+        ...                                                 exact_num_premises=True,
+        ...                                                 exact_num_conclusions=True)
+        >>> classical_parser.unparse(inf)
+        '~(q ↔ q), q / (q ∧ (p → p))'
+
+        Random inferences with up to two premises and two conclusions
+
+        >>> inf = random_formula_generator.random_inference(num_premises=2, num_conclusions=2,
+        ...                                                 max_depth=2, atomics=['p', 'q'],
+        ...                                                 language=classical_language, level=1,
+        ...                                                 exact_num_premises=False,
+        ...                                                 exact_num_conclusions=False)
+        >>> classical_parser.unparse(inf)
+        '(p ↔ p) / ~q'
+        >>> inf = random_formula_generator.random_inference(num_premises=2, num_conclusions=2,
+        ...                                                 max_depth=2, atomics=['p', 'q'],
+        ...                                                 language=classical_language, level=1,
+        ...                                                 exact_num_premises=False,
+        ...                                                 exact_num_conclusions=False)
+        >>> classical_parser.unparse(inf)
+        '/'
+
+        Random metainferences with up to two premises and two conclusions
+
+        >>> inf = random_formula_generator.random_inference(num_premises=2, num_conclusions=2,
+        ...                                                 max_depth=2, atomics=['p', 'q'],
+        ...                                                 language=classical_language, level=2,
+        ...                                                 exact_num_premises=False,
+        ...                                                 exact_num_conclusions=False)
+        >>> classical_parser.unparse(inf)
+        '((q → (q → q)) /), ((p ↔ p), (q ∧ p) / (q ∨ q), p) //'
+        >>> inf = random_formula_generator.random_inference(num_premises=2, num_conclusions=2,
+        ...                                                 max_depth=2, atomics=['p', 'q'],
+        ...                                                 language=classical_language, level=2,
+        ...                                                 exact_num_premises=False,
+        ...                                                 exact_num_conclusions=False)
+        >>> classical_parser.unparse(inf)
+        '(/) //'
+        """
+        if level == 0:
+            raise ValueError('Inferences cannot have level 0')
+
+        # Premises
+        premises = list()
+        new_num_premises = num_premises
+        if not exact_num_premises:
+            new_num_premises = random.randint(0, num_premises)
+
+        for _ in range(new_num_premises):
+            if level == 1:
+                premises.append(self._upto_depth_some_atomics(max_depth, atomics, language))
+            else:
+                premises.append(self.random_inference(num_premises, num_conclusions, max_depth, atomics, language,
+                                                      level=level-1, exact_num_premises=False,
+                                                      exact_num_conclusions=False))
+
+        # Conclusions
+        conclusions = list()
+        new_num_conclusions = num_conclusions
+        if not exact_num_conclusions:
+            new_num_conclusions = random.randint(0, num_conclusions)
+
+        for _ in range(new_num_conclusions):
+            if level == 1:
+                conclusions.append(self._upto_depth_some_atomics(max_depth, atomics, language))
+            else:
+                conclusions.append(self.random_inference(num_premises, num_conclusions,
+                                                         max_depth, atomics, language, level=level-1))
+
+        return Inference(premises=premises, conclusions=conclusions, level=level)
+
+    # ------------------------------------------------------------------------------------------------------------------
+    # THINGS WITH VALIDITY APPARATUSES
+
+    def random_tautology(self, depth, atomics, language, validity_apparatus, exact_depth=True, all_atomics=False,
+                         attempts=100):
+        """Generates a random tautogy for the validity apparatus given.
+
+        Will generate a random formula and then test the inference ([] / [formula]) to see if it is valid. If it is,
+        returns it, otherwise generates another. Can fail for at most the number of `attempts` given.
+
+        The signature is very similar to that of random_formula but takes two extra parameters:
+
+            * validity_apparatus: any object with an is_valid method (which takes an inference as argument)
+            * attempts: an `int`, maximum number of formulae it generates and tests (defaults to 100)
+
+        Returns
+        -------
+        logics.classes.propositional.Formula
+            A randomly generated tautology of the given depth, containing some or all the atomics
+
+        Raises
+        ------
+        NotImplemented
+            If exact_depth is False and all_atomics is True
+        ValueError
+            If exact_depth is True, all_atomics is True and the number of atomics given > the maximum arity constant of
+            the language ** depth.
+        FormulaGeneratorError
+            If it cannot find a tautology in the given number of `attempts`
+
+        Examples
+        --------
+        >>> from logics.instances.propositional.languages import classical_language
+        >>> from logics.instances.propositional.many_valued_semantics import classical_mvl_semantics
+        >>> from logics.utils.formula_generators.generators_biased import random_formula_generator
+        >>> random_formula_generator.random_tautology(depth=2, atomics=['p', 'q'],
+        ...                                           language=classical_language,
+        ...                                           validity_apparatus=classical_mvl_semantics)
+        ['→', ['∧', ['q'], ['p']], ['∧', ['q'], ['q']]]
+        >>> random_formula_generator.random_tautology(depth=2, atomics=['p', 'q'],
+        ...                                           language=classical_language,
+        ...                                           validity_apparatus=classical_mvl_semantics)
+        ['→', ['p'], ['∨', ['p'], ['p']]]
+        """
+        for _ in range(attempts):
+            if exact_depth and all_atomics:
+                formula = self._exact_depth_all_atomics(depth, atomics, language)
+            elif exact_depth and not all_atomics:
+                formula = self._exact_depth_some_atomics(depth, atomics, language)
+            elif not exact_depth and not all_atomics:
+                formula = self._upto_depth_some_atomics(depth, atomics, language)
+            else:
+                raise NotImplemented('Not exact depth and all atomics generator not implemented yet')
+
+            inf = Inference(premises=[], conclusions=[formula])
+            if validity_apparatus.is_valid(inf):
+                return formula
+
+        raise FormulaGeneratorError('Could not generate tautology with the parameters given')
+
+    def random_valid_inference(self, num_premises, num_conclusions, max_depth, atomics, language, validity_apparatus,
+                               level=1, exact_num_premises=True, exact_num_conclusions=True, attempts=100):
+        """Generates a random *valid* inference for the validity apparatus given.
+
+        Similar to the random_inference method. The two new parameters are to the method above.
+        In particular, The object passed to `validity_apparatus` must have an `is_valid` method.
+        If `level` > 1 the validity apparatus must be able to handle metainferential validity.
+
+        Returns
+        -------
+        logics.classes.propositional.Inference
+            A randomly generated valid inference or metainference with the parameters given
+
+        Raises
+        ------
+        FormulaGeneratorError
+            If it cannot find a valid inference in the given number of `attempts`
+
+        Examples
+        --------
+        >>> from logics.instances.propositional.languages import classical_language
+        >>> from logics.utils.parsers import classical_parser
+        >>> from logics.instances.propositional.many_valued_semantics import classical_mvl_semantics
+        >>> from logics.utils.formula_generators.generators_biased import random_formula_generator
+        >>> inf = random_formula_generator.random_valid_inference(num_premises=2, num_conclusions=1,
+        ...                                                       max_depth=2, atomics=['p', 'q'],
+        ...                                                       language=classical_language, level=1,
+        ...                                                       validity_apparatus=classical_mvl_semantics)
+        >>> classical_parser.unparse(inf)
+        '(q ↔ p), p / (p ∨ q)'
+        >>> inf = random_formula_generator.random_valid_inference(num_premises=2, num_conclusions=1,
+        ...                                                       max_depth=2, atomics=['p', 'q'],
+        ...                                                       language=classical_language, level=2,
+        ...                                                       validity_apparatus=classical_mvl_semantics)
+        >>> classical_parser.unparse(inf)
+        '(p / p), (p, ((q → p) ∧ (p ∨ p)) / (p ↔ (q ↔ p))) // (((p ↔ p) ∨ p), ~q / (q ∨ ~p))'
+        """
+        for _ in range(attempts):
+            inf = self.random_inference(num_premises, num_conclusions, max_depth, atomics, language, level,
+                                        exact_num_premises, exact_num_conclusions)
+            if validity_apparatus.is_valid(inf):
+                return inf
+
+        raise FormulaGeneratorError('Could not generate valid inference with the parameters given')
+
+    def random_invalid_inference(self, num_premises, num_conclusions, max_depth, atomics, language, validity_apparatus,
+                                 level=1, exact_num_premises=True, exact_num_conclusions=True, attempts=100):
+        """Generates a random *invalid* inference for the validity apparatus given.
+
+        Identical to the method above, only that it returns an *invalid* inference.
+        """
+        for _ in range(attempts):
+            inf = self.random_inference(num_premises, num_conclusions, max_depth, atomics, language, level,
+                                        exact_num_premises, exact_num_conclusions)
+            if not validity_apparatus.is_valid(inf):
+                return inf
+
+        raise FormulaGeneratorError('Could not generate valid inference with the parameters given')
+
+
+random_formula_generator = BiasedPropositionalGenerator()
+
+
+# ----------------------------------------------------------------------------------------------------------------------
+# Predicate formula generator
+
+class BiasedPredicateGenerator:
+    """A biased random predicate generator.
+
+        It is biased because it will not return every formula/inference within the space asked with the same probability.
+        There is no non-biased generator implemented in this package yet.
+        This implementation does not yet work with function symbols.
+
+        Examples
+        --------
+        This generator takes no parameters, so to instantiate one you can simply do:
+
+        >>> from logics.utils.formula_generators.generators_biased import BiasedPredicateGenerator
+        >>> random_generator = BiasedPredicateGenerator()
+
+        There is also a predefined instance so there is even no need to instantiate it
+
+        >>> from logics.utils.formula_generators.generators_biased import random_predicate_formula_generator
+        """
+    def _random_term(self, ind_constants, variables):
+        # We select an ind_constant and a variable with equal probability, even if there is just 1 var and 5 ind_cts
+        if not variables or random.choice((True, False)):
+            return random.choice(ind_constants)
+        else:
+            return random.choice(variables)
+
+    def _random_atomic_formula(self, predicates, max_arity, ind_constants, variables, predicate_arities):
+        # Firstly, we must choose a predicate and set its arity
+        predicate = random.choice(predicates)
+        formula = PredicateFormula([predicate])
+        if predicate in predicate_arities:
+            arity = predicate_arities[predicate]
+        else:
+            arity = random.randint(1, max_arity)
+            predicate_arities[predicate] = arity  # Modify the dict, will be seen by the caller
+
+        for _ in range(arity):
+            formula.append(self._random_term(ind_constants, variables))
+
+        return formula
+
+    def random_formula(self, depth, predicates, max_predicate_arity, ind_constants, variables, language,
+                       remaining_depth=0, predicate_arities=None):
+        """Generates a random formula of some *exact* depth, which uses some of the predicates, variables and ind cts
+        provided
+
+        Because of the educational usecases I have in mind, I don't want it to output things like ∀x P(a) or like
+        ∀x ∀x P(x). More precisely, Its made so every quantifier binds at least one variable.
+
+        Assumes that the predicate arities can be random (i.e. will not respect the
+        predicate_letters={'P': 1, 'Q': 1, 'R': 2, 'S': 3} argument given to PredicateLanguage). If you want it to,
+        give it predicate_arities=language.predicate_letters
+
+        Examples
+        --------
+        >>> from logics.instances.predicate.languages import classical_predicate_language as lang
+        >>> from logics.utils.parsers import classical_predicate_parser
+        >>> from logics.utils.formula_generators.generators_biased import random_predicate_formula_generator
+        >>> for _ in range(5):
+        ...     formula = random_predicate_formula_generator.random_formula(depth=2, predicates=['P', 'Q'],
+        ...         max_predicate_arity=2, ind_constants=['a', 'b'], variables=['x', 'y'], language=lang)
+        ...     print(classical_predicate_parser.unparse(formula))
+        Q(b, a) → ∀x Q(x, x)
+        ∀y Q(y) ∧ Q(b)
+        ∀x (Q(b) ∧ P(x, a))
+        ∀y (Q(y, a) ∧ P(y, y))
+        ∃x P(x) ∨ P(b)
+        """
+        if predicate_arities is None:
+            predicate_arities = dict()
+
+        if depth == 0:
+            # We must make sure that the number of free variables in this atomic is not greater than the
+            # remaining depth, otherwise we cannot get to bind them all.
+            # E.g. if we originally asked for depth=1, when this clause is reached, remaining_depth==1
+            # and variables[:remaining_depth] will be ['x']
+            return self._random_atomic_formula(predicates, max_predicate_arity, ind_constants,
+                                               variables[:remaining_depth], predicate_arities)
+
+        else:
+            # We proceed recursively in the reverse direction than the other generator, that is, we go bottom-up
+            # First generate a subformula
+            first_argument = self.random_formula(depth-1, predicates, max_predicate_arity, ind_constants, variables,
+                                                 language, remaining_depth+1, predicate_arities)
+
+            # Check the free variables in the first arg
+            free_vars = first_argument.free_variables(language)
+            # If free_vars is ['x', 'y'], rem_depth must be at least 1
+            # since one quantifier can be introduced here, and the and another in the remaining top call
+            assert remaining_depth + 1 >= len(free_vars)
+            # if remaining_depth + 1 < len(free_vars):
+            #     print("ERROR", first_argument, depth, remaining_depth, free_vars)
+            #     raise ValueError("Fix this")
+
+            # Then choose a logical constant
+            if not free_vars:
+                # If there are no free variables, do not introduce quantifiers that bind nothing
+                constant = random.choice(tuple(language.constants()))
+            elif remaining_depth + 1 == len(free_vars):
+                # We MUST choose a quantifier
+                # e.g.  remaining depth is 0 (this is the last constant introduced) and we have 1 free variable
+                # e.g.2 remaining depth is 1 (we will introduce this + 1 ctt) and we have 2 free variables
+                constant = random.choice(language.quantifiers)
+            else:
+                # Otherwise can be either a quantifier or a logical constant, choose with equal prob so that
+                # there is no bias for all the quantifiers to be at the beginning of the formula
+                if random.choice((True, False)):
+                    constant = random.choice(tuple(language.constants()))
+                else:
+                    constant = random.choice(language.quantifiers)
+
+            arity = language.arity(constant)
+
+            # Quantified formula
+            if constant in language.quantifiers:
+                variable = random.choice(list(free_vars))
+                return PredicateFormula([constant, variable, first_argument])
+
+            # Unary connective formula
+            elif arity == 1:
+                return PredicateFormula([constant, first_argument])
+
+            # Binary connective formula
+            else:
+                # We must be careful here bc the second subformula could introduce more free variables
+                # We can use the free variables in the first_argument freely, though
+                # E.g. if x is already free here, and we have 2 remaining depth (will introduce 2 more cts--do not count
+                # this one bc it is not a quantifier) -- then the second subformula can contain one extra var
+                new_vars = list(free_vars)
+                extra_vars_allowed = remaining_depth - len(free_vars)
+                if extra_vars_allowed:
+                    extra_vars = [v for v in variables if v not in new_vars]
+                    new_vars.extend(extra_vars[:extra_vars_allowed])
+
+                second_argument = self.random_formula(random.randint(0, depth-1), predicates, max_predicate_arity,
+                                                      ind_constants, new_vars, language, remaining_depth+1,
+                                                      predicate_arities)
+                if random.choice((True, False)):
+                    return PredicateFormula([constant, first_argument, second_argument])
+                else:
+                    return PredicateFormula([constant, second_argument, first_argument])
+
+
+random_predicate_formula_generator = BiasedPredicateGenerator()
```

### Comparing `logics-1.9.0/logics/utils/parsers/parser_utils.py` & `logics-1.9.1/logics/utils/parsers/parser_utils.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/utils/parsers/predicate_parser.py` & `logics-1.9.1/logics/utils/parsers/predicate_parser.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/utils/parsers/standard_parser.py` & `logics-1.9.1/logics/utils/parsers/standard_parser.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/utils/solvers/first_order_natural_deduction.py` & `logics-1.9.1/logics/utils/solvers/first_order_natural_deduction.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/utils/solvers/natural_deduction.py` & `logics-1.9.1/logics/utils/solvers/natural_deduction.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/utils/solvers/sequents.py` & `logics-1.9.1/logics/utils/solvers/sequents.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/utils/solvers/tableaux.py` & `logics-1.9.1/logics/utils/solvers/tableaux.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics/utils/upgrade/upgrade.py` & `logics-1.9.1/logics/utils/upgrade/upgrade.py`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/logics.egg-info/PKG-INFO` & `logics-1.9.1/logics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logics
-Version: 1.9.0
+Version: 1.9.1
 Summary: Logics is a Python framework for mathematical logic
 Home-page: https://github.com/ariroffe/logics
 Author: Ariel Jonathan Roffé
 Author-email: arielroffe@filo.uba.ar
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `logics-1.9.0/logics.egg-info/SOURCES.txt` & `logics-1.9.1/logics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logics-1.9.0/setup.cfg` & `logics-1.9.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = logics
-version = 1.9.0
+version = 1.9.1
 author = Ariel Jonathan Roffé
 author_email = arielroffe@filo.uba.ar
 url = https://github.com/ariroffe/logics
 description = Logics is a Python framework for mathematical logic
 license = MIT
 license_files = LICENSE.txt
 long_description = file: README.rst
```

