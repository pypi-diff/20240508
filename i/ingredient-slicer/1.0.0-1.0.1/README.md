# Comparing `tmp/ingredient_slicer-1.0.0.tar.gz` & `tmp/ingredient_slicer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ingredient_slicer-1.0.0.tar", last modified: Tue May  7 12:26:18 2024, max compression
+gzip compressed data, was "ingredient_slicer-1.0.1.tar", last modified: Wed May  8 17:35:47 2024, max compression
```

## Comparing `ingredient_slicer-1.0.0.tar` & `ingredient_slicer-1.0.1.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-07 12:26:18.653362 ingredient_slicer-1.0.0/
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-07 12:26:18.631990 ingredient_slicer-1.0.0/.github/
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-07 12:26:18.633497 ingredient_slicer-1.0.0/.github/workflows/
--rw-r--r--   0 anguswatters   (501) staff       (20)      782 2024-03-23 22:54:24.000000 ingredient_slicer-1.0.0/.github/workflows/run-unit-tests.yml
--rw-r--r--   0 anguswatters   (501) staff       (20)     3118 2024-03-17 16:59:19.000000 ingredient_slicer-1.0.0/.gitignore
--rw-r--r--   0 anguswatters   (501) staff       (20)     1075 2024-03-17 16:52:34.000000 ingredient_slicer-1.0.0/LICENSE
--rw-r--r--   0 anguswatters   (501) staff       (20)     3362 2024-05-07 12:26:18.653073 ingredient_slicer-1.0.0/PKG-INFO
--rw-r--r--   0 anguswatters   (501) staff       (20)     2389 2024-04-08 22:17:24.000000 ingredient_slicer-1.0.0/README.md
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-07 12:26:18.636817 ingredient_slicer-1.0.0/ingredient_slicer/
--rw-r--r--   0 anguswatters   (501) staff       (20)     1725 2024-05-06 13:28:44.000000 ingredient_slicer-1.0.0/ingredient_slicer/__init__.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   155546 2024-05-06 15:43:05.000000 ingredient_slicer-1.0.0/ingredient_slicer/_constants.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   102582 2024-05-06 17:09:54.000000 ingredient_slicer-1.0.0/ingredient_slicer/_ingredient_slicer.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    91104 2024-04-18 00:53:53.000000 ingredient_slicer-1.0.0/ingredient_slicer/_regex_patterns.py
--rw-r--r--   0 anguswatters   (501) staff       (20)   101437 2024-05-06 17:10:27.000000 ingredient_slicer-1.0.0/ingredient_slicer/_utils.py
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-07 12:26:18.652385 ingredient_slicer-1.0.0/ingredient_slicer.egg-info/
--rw-r--r--   0 anguswatters   (501) staff       (20)     3362 2024-05-07 12:26:18.000000 ingredient_slicer-1.0.0/ingredient_slicer.egg-info/PKG-INFO
--rw-r--r--   0 anguswatters   (501) staff       (20)     2070 2024-05-07 12:26:18.000000 ingredient_slicer-1.0.0/ingredient_slicer.egg-info/SOURCES.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)        1 2024-05-07 12:26:18.000000 ingredient_slicer-1.0.0/ingredient_slicer.egg-info/dependency_links.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-05-07 12:26:18.000000 ingredient_slicer-1.0.0/ingredient_slicer.egg-info/requires.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)       18 2024-05-07 12:26:18.000000 ingredient_slicer-1.0.0/ingredient_slicer.egg-info/top_level.txt
--rw-r--r--   0 anguswatters   (501) staff       (20)     1124 2024-05-06 13:29:01.000000 ingredient_slicer-1.0.0/pyproject.toml
--rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-05-07 12:26:18.653430 ingredient_slicer-1.0.0/setup.cfg
-drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-07 12:26:18.652019 ingredient_slicer-1.0.0/tests/
--rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 13:59:44.000000 ingredient_slicer-1.0.0/tests/__init__.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2402 2024-04-06 15:22:11.000000 ingredient_slicer-1.0.0/tests/test_avg_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5566 2024-04-10 14:53:42.000000 ingredient_slicer-1.0.0/tests/test_casual_ingredients.py
--rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:22:03.000000 ingredient_slicer-1.0.0/tests/test_clean_hyphen_padded_substrings.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5502 2024-04-06 15:27:00.000000 ingredient_slicer-1.0.0/tests/test_convert_fractions_to_decimals.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2145 2024-04-06 15:27:01.000000 ingredient_slicer-1.0.0/tests/test_convert_volumes_to_milliliters.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1182 2024-03-29 21:19:57.000000 ingredient_slicer-1.0.0/tests/test_duplicate_unit_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8507 2024-03-29 21:18:52.000000 ingredient_slicer-1.0.0/tests/test_extract_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3541 2024-03-29 21:19:50.000000 ingredient_slicer-1.0.0/tests/test_extract_quantities_utils.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3711 2024-03-29 21:19:48.000000 ingredient_slicer-1.0.0/tests/test_find_and_remove.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2842 2024-03-29 21:19:52.000000 ingredient_slicer-1.0.0/tests/test_find_and_remove_hyphen_substrings.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3352 2024-04-06 13:59:33.000000 ingredient_slicer-1.0.0/tests/test_fraction_str_to_decimal.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    26160 2024-05-06 14:16:39.000000 ingredient_slicer-1.0.0/tests/test_get_gram_weight.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2496 2024-05-06 15:32:33.000000 ingredient_slicer-1.0.0/tests/test_get_single_item_gram_weight.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    20386 2024-04-10 16:18:22.000000 ingredient_slicer-1.0.0/tests/test_ingredient_slicer.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3428 2024-04-08 13:04:03.000000 ingredient_slicer-1.0.0/tests/test_ingredient_slicer_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     4718 2024-04-10 14:52:58.000000 ingredient_slicer-1.0.0/tests/test_ingredient_slicer_fraction_conversions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1903 2024-05-06 17:14:21.000000 ingredient_slicer-1.0.0/tests/test_ingredient_slicer_gram_weights.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1515 2024-04-10 14:52:56.000000 ingredient_slicer-1.0.0/tests/test_ingredient_slicer_parenthesis.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     7502 2024-04-10 14:52:56.000000 ingredient_slicer-1.0.0/tests/test_ingredient_slicer_x_separators.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     4178 2024-04-10 14:52:54.000000 ingredient_slicer-1.0.0/tests/test_is_approximate_quantity_only_parenthesis.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2965 2024-04-10 14:52:54.000000 ingredient_slicer-1.0.0/tests/test_make_int_or_float_str.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2169 2024-04-06 15:26:57.000000 ingredient_slicer-1.0.0/tests/test_merge_misleading_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    14464 2024-03-29 21:19:43.000000 ingredient_slicer-1.0.0/tests/test_merge_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    43982 2024-04-06 14:42:17.000000 ingredient_slicer-1.0.0/tests/test_number_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    56318 2024-03-29 21:19:45.000000 ingredient_slicer-1.0.0/tests/test_number_ranges_separated_by_words.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5652 2024-04-06 13:59:36.000000 ingredient_slicer-1.0.0/tests/test_numbers_with_inch_symbols.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    15368 2024-03-29 21:19:20.000000 ingredient_slicer-1.0.0/tests/test_parenthesis.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    11036 2024-04-10 14:53:13.000000 ingredient_slicer-1.0.0/tests/test_parenthesis_utils.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     2512 2024-03-29 21:19:22.000000 ingredient_slicer-1.0.0/tests/test_percentages.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3547 2024-03-29 21:19:26.000000 ingredient_slicer-1.0.0/tests/test_prefixed_number_words_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5013 2024-03-29 21:19:28.000000 ingredient_slicer-1.0.0/tests/test_prep_words.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5261 2024-03-29 21:19:25.000000 ingredient_slicer-1.0.0/tests/test_quantity_range_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    27045 2024-04-06 13:59:38.000000 ingredient_slicer-1.0.0/tests/test_quantity_units_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     3571 2024-04-06 13:31:28.000000 ingredient_slicer-1.0.0/tests/test_remove_repeat_units_in_ranges.py
--rw-r--r--   0 anguswatters   (501) staff       (20)      633 2024-03-29 21:19:14.000000 ingredient_slicer-1.0.0/tests/test_remove_x_separators.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     6384 2024-03-29 21:19:12.000000 ingredient_slicer-1.0.0/tests/test_replace_a_or_an_quantities.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     6869 2024-03-29 21:19:08.000000 ingredient_slicer-1.0.0/tests/test_separate_dimensions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1808 2024-03-29 21:19:42.000000 ingredient_slicer-1.0.0/tests/test_size_modifiers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8974 2024-03-29 21:19:39.000000 ingredient_slicer-1.0.0/tests/test_spaced_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     5838 2024-03-29 21:19:40.000000 ingredient_slicer-1.0.0/tests/test_unit_regex.py
--rw-r--r--   0 anguswatters   (501) staff       (20)    16676 2024-04-06 15:22:15.000000 ingredient_slicer-1.0.0/tests/test_wild_ingredients.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     8022 2024-04-06 15:22:14.000000 ingredient_slicer-1.0.0/tests/test_word_fractions.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     7167 2024-03-29 21:19:33.000000 ingredient_slicer-1.0.0/tests/test_word_numbers.py
--rw-r--r--   0 anguswatters   (501) staff       (20)     1337 2024-04-06 14:42:17.000000 ingredient_slicer-1.0.0/tests/test_x_after_number_regex.py
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-08 17:35:47.783784 ingredient_slicer-1.0.1/
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-08 17:35:47.771068 ingredient_slicer-1.0.1/.github/
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-08 17:35:47.772807 ingredient_slicer-1.0.1/.github/workflows/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3289 2024-05-07 12:28:17.000000 ingredient_slicer-1.0.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 anguswatters   (501) staff       (20)      782 2024-03-23 22:54:24.000000 ingredient_slicer-1.0.1/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3118 2024-03-17 16:59:19.000000 ingredient_slicer-1.0.1/.gitignore
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1075 2024-03-17 16:52:34.000000 ingredient_slicer-1.0.1/LICENSE
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3362 2024-05-08 17:35:47.783512 ingredient_slicer-1.0.1/PKG-INFO
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2389 2024-04-08 22:17:24.000000 ingredient_slicer-1.0.1/README.md
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-08 17:35:47.774109 ingredient_slicer-1.0.1/ingredient_slicer/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1725 2024-05-08 17:34:45.000000 ingredient_slicer-1.0.1/ingredient_slicer/__init__.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   155567 2024-05-08 17:35:35.000000 ingredient_slicer-1.0.1/ingredient_slicer/_constants.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   102582 2024-05-06 17:09:54.000000 ingredient_slicer-1.0.1/ingredient_slicer/_ingredient_slicer.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    91104 2024-04-18 00:53:53.000000 ingredient_slicer-1.0.1/ingredient_slicer/_regex_patterns.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)   101437 2024-05-06 17:10:27.000000 ingredient_slicer-1.0.1/ingredient_slicer/_utils.py
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-08 17:35:47.782853 ingredient_slicer-1.0.1/ingredient_slicer.egg-info/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3362 2024-05-08 17:35:47.000000 ingredient_slicer-1.0.1/ingredient_slicer.egg-info/PKG-INFO
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2108 2024-05-08 17:35:47.000000 ingredient_slicer-1.0.1/ingredient_slicer.egg-info/SOURCES.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)        1 2024-05-08 17:35:47.000000 ingredient_slicer-1.0.1/ingredient_slicer.egg-info/dependency_links.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-05-08 17:35:47.000000 ingredient_slicer-1.0.1/ingredient_slicer.egg-info/requires.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)       18 2024-05-08 17:35:47.000000 ingredient_slicer-1.0.1/ingredient_slicer.egg-info/top_level.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1124 2024-05-08 17:34:40.000000 ingredient_slicer-1.0.1/pyproject.toml
+-rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-05-08 17:35:47.783847 ingredient_slicer-1.0.1/setup.cfg
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-08 17:35:47.782606 ingredient_slicer-1.0.1/tests/
+-rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 13:59:44.000000 ingredient_slicer-1.0.1/tests/__init__.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2402 2024-04-06 15:22:11.000000 ingredient_slicer-1.0.1/tests/test_avg_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5566 2024-04-10 14:53:42.000000 ingredient_slicer-1.0.1/tests/test_casual_ingredients.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)        0 2024-04-06 15:22:03.000000 ingredient_slicer-1.0.1/tests/test_clean_hyphen_padded_substrings.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5502 2024-04-06 15:27:00.000000 ingredient_slicer-1.0.1/tests/test_convert_fractions_to_decimals.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2145 2024-04-06 15:27:01.000000 ingredient_slicer-1.0.1/tests/test_convert_volumes_to_milliliters.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1182 2024-03-29 21:19:57.000000 ingredient_slicer-1.0.1/tests/test_duplicate_unit_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8507 2024-03-29 21:18:52.000000 ingredient_slicer-1.0.1/tests/test_extract_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3541 2024-03-29 21:19:50.000000 ingredient_slicer-1.0.1/tests/test_extract_quantities_utils.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3711 2024-03-29 21:19:48.000000 ingredient_slicer-1.0.1/tests/test_find_and_remove.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2842 2024-03-29 21:19:52.000000 ingredient_slicer-1.0.1/tests/test_find_and_remove_hyphen_substrings.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3352 2024-04-06 13:59:33.000000 ingredient_slicer-1.0.1/tests/test_fraction_str_to_decimal.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    26160 2024-05-06 14:16:39.000000 ingredient_slicer-1.0.1/tests/test_get_gram_weight.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2496 2024-05-06 15:32:33.000000 ingredient_slicer-1.0.1/tests/test_get_single_item_gram_weight.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    20386 2024-04-10 16:18:22.000000 ingredient_slicer-1.0.1/tests/test_ingredient_slicer.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3428 2024-04-08 13:04:03.000000 ingredient_slicer-1.0.1/tests/test_ingredient_slicer_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     4718 2024-04-10 14:52:58.000000 ingredient_slicer-1.0.1/tests/test_ingredient_slicer_fraction_conversions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1903 2024-05-06 17:14:21.000000 ingredient_slicer-1.0.1/tests/test_ingredient_slicer_gram_weights.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1515 2024-04-10 14:52:56.000000 ingredient_slicer-1.0.1/tests/test_ingredient_slicer_parenthesis.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     7502 2024-04-10 14:52:56.000000 ingredient_slicer-1.0.1/tests/test_ingredient_slicer_x_separators.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     4178 2024-04-10 14:52:54.000000 ingredient_slicer-1.0.1/tests/test_is_approximate_quantity_only_parenthesis.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2965 2024-04-10 14:52:54.000000 ingredient_slicer-1.0.1/tests/test_make_int_or_float_str.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2169 2024-04-06 15:26:57.000000 ingredient_slicer-1.0.1/tests/test_merge_misleading_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    14464 2024-03-29 21:19:43.000000 ingredient_slicer-1.0.1/tests/test_merge_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    43982 2024-04-06 14:42:17.000000 ingredient_slicer-1.0.1/tests/test_number_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    56318 2024-03-29 21:19:45.000000 ingredient_slicer-1.0.1/tests/test_number_ranges_separated_by_words.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5652 2024-04-06 13:59:36.000000 ingredient_slicer-1.0.1/tests/test_numbers_with_inch_symbols.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    15368 2024-03-29 21:19:20.000000 ingredient_slicer-1.0.1/tests/test_parenthesis.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    11036 2024-04-10 14:53:13.000000 ingredient_slicer-1.0.1/tests/test_parenthesis_utils.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     2512 2024-03-29 21:19:22.000000 ingredient_slicer-1.0.1/tests/test_percentages.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3547 2024-03-29 21:19:26.000000 ingredient_slicer-1.0.1/tests/test_prefixed_number_words_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5013 2024-03-29 21:19:28.000000 ingredient_slicer-1.0.1/tests/test_prep_words.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5261 2024-03-29 21:19:25.000000 ingredient_slicer-1.0.1/tests/test_quantity_range_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    27045 2024-04-06 13:59:38.000000 ingredient_slicer-1.0.1/tests/test_quantity_units_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     3571 2024-04-06 13:31:28.000000 ingredient_slicer-1.0.1/tests/test_remove_repeat_units_in_ranges.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)      633 2024-03-29 21:19:14.000000 ingredient_slicer-1.0.1/tests/test_remove_x_separators.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     6384 2024-03-29 21:19:12.000000 ingredient_slicer-1.0.1/tests/test_replace_a_or_an_quantities.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     6869 2024-03-29 21:19:08.000000 ingredient_slicer-1.0.1/tests/test_separate_dimensions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1808 2024-03-29 21:19:42.000000 ingredient_slicer-1.0.1/tests/test_size_modifiers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8974 2024-03-29 21:19:39.000000 ingredient_slicer-1.0.1/tests/test_spaced_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     5838 2024-03-29 21:19:40.000000 ingredient_slicer-1.0.1/tests/test_unit_regex.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    16676 2024-04-06 15:22:15.000000 ingredient_slicer-1.0.1/tests/test_wild_ingredients.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     8022 2024-04-06 15:22:14.000000 ingredient_slicer-1.0.1/tests/test_word_fractions.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     7167 2024-03-29 21:19:33.000000 ingredient_slicer-1.0.1/tests/test_word_numbers.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1337 2024-04-06 14:42:17.000000 ingredient_slicer-1.0.1/tests/test_x_after_number_regex.py
```

### Comparing `ingredient_slicer-1.0.0/.github/workflows/run-unit-tests.yml` & `ingredient_slicer-1.0.1/.github/workflows/run-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/.gitignore` & `ingredient_slicer-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/LICENSE` & `ingredient_slicer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/PKG-INFO` & `ingredient_slicer-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingredient_slicer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Parses unstructured recipe ingredient text into standardized quantities, units, and foods
 Author-email: Angus Watters <anguswatters@gmail.com>
 License: MIT License
 Keywords: ingredient,parser,recipe,text processing,food,cooking,grocery,shopping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ingredient_slicer-1.0.0/README.md` & `ingredient_slicer-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/ingredient_slicer/__init__.py` & `ingredient_slicer-1.0.1/ingredient_slicer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # __init__.py
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 from ._ingredient_slicer import IngredientSlicer
 
 from ._constants import UNITS, WEIGHT_UNITS, VOLUME_UNITS, DIMENSION_UNITS, \
     CASUAL_UNITS, CASUAL_QUANTITIES, PREP_WORDS, \
     FOOD_CATALOG, FOOD_CATEGORIES, FOOD_DENSITY_BY_GROUP, \
     PRIMARY_CATEGORIES, SECONDARY_CATEGORIES, \
```

### Comparing `ingredient_slicer-1.0.0/ingredient_slicer/_constants.py` & `ingredient_slicer-1.0.1/ingredient_slicer/_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,16 +241,17 @@
     # print(f"key: {key}, pattern: {pattern}")
     for val in pattern:
         UNIT_TO_STANDARD_UNIT[val] = key
 
 # Only the core basic imperial and metric units (Excludes the more specific units like "stalk", "fillet", "slices", etc.)
 BASIC_UNITS = {
     # Imperial volume units
-    'teaspoon': ('teaspoon', 'teaspoons', 'tsp', 'tsps', "tsp", "tspn", "tspns", "tspn." "tspns." , "ts", "t", "t."), # 'teaspoon': ('teaspoon', 'teaspoons', 'tsp', 'tsps', "tsp", "t"),
-    'tablespoon': ('tablespoon', 'tablespoons', 'tbsp', 'tbsps', "tbsp", "tbsps", "tbsp.", "tbsps.", "tbl", "tbls", "tbl.", "tbls.", "T", "tbs", "tbs."),
+    'teaspoon': ('teaspoon', 'teaspoons', 'tsp', 'tsps', "tsp", "tspn", "tspns", "tspn.", "tspns." , "ts", "t", "t."), # 'teaspoon': ('teaspoon', 'teaspoons', 'tsp', 'tsps', "tsp", "t"),
+    'tablespoon': ('tablespoon', 'tablespoons', 'tbsp', 'tbsps', "tbsp", "tbsps", "tbsp.", "tbsps.", "tbl", "tbls", "tbl.", 
+                   "tbls.", "T", "tbs", "tbs."),
     'tablespoonful': ('tablespoonful', 'tablespoonfuls'),
     'teaspoonful': ('teaspoonful', 'teaspoonfuls'),
     'cup': ('cup', 'cups', "C", "c"),
     'pint': ('pint', 'pints', "pt", "pts"),
     'quart': ('quart', 'quarts', "qt", "qts"),
     'gallon': ('gallon', 'gallons', "gals", "gal"),
     'fluid ounce': ('fluid ounce', 'fluid ounces', 'fl oz', 'fl ozs',
```

### Comparing `ingredient_slicer-1.0.0/ingredient_slicer/_ingredient_slicer.py` & `ingredient_slicer-1.0.1/ingredient_slicer/_ingredient_slicer.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/ingredient_slicer/_regex_patterns.py` & `ingredient_slicer-1.0.1/ingredient_slicer/_regex_patterns.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/ingredient_slicer/_utils.py` & `ingredient_slicer-1.0.1/ingredient_slicer/_utils.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/ingredient_slicer.egg-info/PKG-INFO` & `ingredient_slicer-1.0.1/ingredient_slicer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingredient_slicer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Parses unstructured recipe ingredient text into standardized quantities, units, and foods
 Author-email: Angus Watters <anguswatters@gmail.com>
 License: MIT License
 Keywords: ingredient,parser,recipe,text processing,food,cooking,grocery,shopping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ingredient_slicer-1.0.0/ingredient_slicer.egg-info/SOURCES.txt` & `ingredient_slicer-1.0.1/ingredient_slicer.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitignore
 LICENSE
 README.md
 pyproject.toml
+.github/workflows/publish-to-pypi.yml
 .github/workflows/run-unit-tests.yml
 ingredient_slicer/__init__.py
 ingredient_slicer/_constants.py
 ingredient_slicer/_ingredient_slicer.py
 ingredient_slicer/_regex_patterns.py
 ingredient_slicer/_utils.py
 ingredient_slicer.egg-info/PKG-INFO
```

### Comparing `ingredient_slicer-1.0.0/pyproject.toml` & `ingredient_slicer-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = ["setuptools", "setuptools-scm"]
 
 [project]
 name = "ingredient_slicer"
 authors = [
   {name = "Angus Watters", email = "anguswatters@gmail.com"},
 ]
-version = "1.0.0"
+version = "1.0.1"
 description = "Parses unstructured recipe ingredient text into standardized quantities, units, and foods"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: Unix",
```

### Comparing `ingredient_slicer-1.0.0/tests/test_avg_ranges.py` & `ingredient_slicer-1.0.1/tests/test_avg_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_casual_ingredients.py` & `ingredient_slicer-1.0.1/tests/test_casual_ingredients.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_convert_fractions_to_decimals.py` & `ingredient_slicer-1.0.1/tests/test_convert_fractions_to_decimals.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_convert_volumes_to_milliliters.py` & `ingredient_slicer-1.0.1/tests/test_convert_volumes_to_milliliters.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_duplicate_unit_ranges.py` & `ingredient_slicer-1.0.1/tests/test_duplicate_unit_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_extract_dimensions.py` & `ingredient_slicer-1.0.1/tests/test_extract_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_extract_quantities_utils.py` & `ingredient_slicer-1.0.1/tests/test_extract_quantities_utils.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_find_and_remove.py` & `ingredient_slicer-1.0.1/tests/test_find_and_remove.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_find_and_remove_hyphen_substrings.py` & `ingredient_slicer-1.0.1/tests/test_find_and_remove_hyphen_substrings.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_fraction_str_to_decimal.py` & `ingredient_slicer-1.0.1/tests/test_fraction_str_to_decimal.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_get_gram_weight.py` & `ingredient_slicer-1.0.1/tests/test_get_gram_weight.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_get_single_item_gram_weight.py` & `ingredient_slicer-1.0.1/tests/test_get_single_item_gram_weight.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_ingredient_slicer.py` & `ingredient_slicer-1.0.1/tests/test_ingredient_slicer.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_ingredient_slicer_dimensions.py` & `ingredient_slicer-1.0.1/tests/test_ingredient_slicer_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_ingredient_slicer_fraction_conversions.py` & `ingredient_slicer-1.0.1/tests/test_ingredient_slicer_fraction_conversions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_ingredient_slicer_gram_weights.py` & `ingredient_slicer-1.0.1/tests/test_ingredient_slicer_gram_weights.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_ingredient_slicer_parenthesis.py` & `ingredient_slicer-1.0.1/tests/test_ingredient_slicer_parenthesis.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_ingredient_slicer_x_separators.py` & `ingredient_slicer-1.0.1/tests/test_ingredient_slicer_x_separators.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_is_approximate_quantity_only_parenthesis.py` & `ingredient_slicer-1.0.1/tests/test_is_approximate_quantity_only_parenthesis.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_make_int_or_float_str.py` & `ingredient_slicer-1.0.1/tests/test_make_int_or_float_str.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_merge_misleading_ranges.py` & `ingredient_slicer-1.0.1/tests/test_merge_misleading_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_merge_numbers.py` & `ingredient_slicer-1.0.1/tests/test_merge_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_number_ranges.py` & `ingredient_slicer-1.0.1/tests/test_number_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_number_ranges_separated_by_words.py` & `ingredient_slicer-1.0.1/tests/test_number_ranges_separated_by_words.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_numbers_with_inch_symbols.py` & `ingredient_slicer-1.0.1/tests/test_numbers_with_inch_symbols.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_parenthesis.py` & `ingredient_slicer-1.0.1/tests/test_parenthesis.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_parenthesis_utils.py` & `ingredient_slicer-1.0.1/tests/test_parenthesis_utils.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_percentages.py` & `ingredient_slicer-1.0.1/tests/test_percentages.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_prefixed_number_words_regex.py` & `ingredient_slicer-1.0.1/tests/test_prefixed_number_words_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_prep_words.py` & `ingredient_slicer-1.0.1/tests/test_prep_words.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_quantity_range_regex.py` & `ingredient_slicer-1.0.1/tests/test_quantity_range_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_quantity_units_regex.py` & `ingredient_slicer-1.0.1/tests/test_quantity_units_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_remove_repeat_units_in_ranges.py` & `ingredient_slicer-1.0.1/tests/test_remove_repeat_units_in_ranges.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_remove_x_separators.py` & `ingredient_slicer-1.0.1/tests/test_remove_x_separators.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_replace_a_or_an_quantities.py` & `ingredient_slicer-1.0.1/tests/test_replace_a_or_an_quantities.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_separate_dimensions.py` & `ingredient_slicer-1.0.1/tests/test_separate_dimensions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_size_modifiers.py` & `ingredient_slicer-1.0.1/tests/test_size_modifiers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_spaced_numbers.py` & `ingredient_slicer-1.0.1/tests/test_spaced_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_unit_regex.py` & `ingredient_slicer-1.0.1/tests/test_unit_regex.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_wild_ingredients.py` & `ingredient_slicer-1.0.1/tests/test_wild_ingredients.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_word_fractions.py` & `ingredient_slicer-1.0.1/tests/test_word_fractions.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_word_numbers.py` & `ingredient_slicer-1.0.1/tests/test_word_numbers.py`

 * *Files identical despite different names*

### Comparing `ingredient_slicer-1.0.0/tests/test_x_after_number_regex.py` & `ingredient_slicer-1.0.1/tests/test_x_after_number_regex.py`

 * *Files identical despite different names*

