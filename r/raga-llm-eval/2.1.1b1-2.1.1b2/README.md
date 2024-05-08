# Comparing `tmp/raga_llm_eval-2.1.1b1.tar.gz` & `tmp/raga_llm_eval-2.1.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raga_llm_eval-2.1.1b1.tar", last modified: Wed May  8 11:34:03 2024, max compression
+gzip compressed data, was "raga_llm_eval-2.1.1b2.tar", last modified: Wed May  8 11:54:56 2024, max compression
```

## Comparing `raga_llm_eval-2.1.1b1.tar` & `raga_llm_eval-2.1.1b2.tar`

### file list

```diff
@@ -1,359 +1,359 @@
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.944239 raga_llm_eval-2.1.1b1/
--rw-r--r--   0 kiran-raga   (501) staff       (20)        0 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/LICENSE
--rw-r--r--   0 kiran-raga   (501) staff       (20)      777 2024-04-18 11:24:07.000000 raga_llm_eval-2.1.1b1/MANIFEST.in
--rw-r--r--   0 kiran-raga   (501) staff       (20)    13102 2024-05-08 11:34:03.943889 raga_llm_eval-2.1.1b1/PKG-INFO
--rw-r--r--   0 kiran-raga   (501) staff       (20)    10122 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/README.md
--rw-r--r--   0 kiran-raga   (501) staff       (20)     3628 2024-05-08 09:57:57.000000 raga_llm_eval-2.1.1b1/pyproject.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)       38 2024-05-08 11:34:03.944298 raga_llm_eval-2.1.1b1/setup.cfg
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.868059 raga_llm_eval-2.1.1b1/src/
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.871164 raga_llm_eval-2.1.1b1/src/raga_llm_eval/
--rw-r--r--   0 kiran-raga   (501) staff       (20)      431 2024-04-16 16:29:47.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/__init__.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1599 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/api_client_manager.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4085 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/db_manager.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.881562 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1526 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/__init__.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)    14106 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.883802 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/
--rw-r--r--   0 kiran-raga   (501) staff       (20)      582 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/__init__.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4687 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/analyzer.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)       51 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/exception.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2277 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/faker.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     7851 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/ner_mapping.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.884229 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/predefined_recognizers/
--rw-r--r--   0 kiran-raga   (501) staff       (20)      483 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/predefined_recognizers/__init__.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      233 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/predefined_recognizers/phone_recognizer.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.885666 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/predefined_recognizers/zh/
--rw-r--r--   0 kiran-raga   (501) staff       (20)      380 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/predefined_recognizers/zh/__init__.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      288 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/predefined_recognizers/zh/crypto_recognizer.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      626 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/predefined_recognizers/zh/custom_pattern_recognizer.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      359 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/predefined_recognizers/zh/email_recognizer.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1282 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/predefined_recognizers/zh/ip_recognizer.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     9500 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/regex_patterns.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     7006 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/transformers_helpers.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)    14149 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/transformers_recognizer.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     3670 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/ban_competitors.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4168 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/ban_substrings.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4402 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/ban_topics.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     5980 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/code.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     5040 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/deanonymize.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2668 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/factual_consistency.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1401 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/gibberish.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1817 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/invisible_text.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1178 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/ir_metrics_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     3085 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/json_verify.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     6611 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/language.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     3192 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/language_same.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2573 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/malicious_url.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      324 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/match_type.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     3324 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/no_refusal.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1397 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/nsfw.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1293 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/politeness.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2047 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/profanity.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1595 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/reading_time.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4141 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/regex.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.885810 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.902894 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/
--rw-r--r--   0 kiran-raga   (501) staff       (20)        0 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/__init__.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      477 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/adafruit.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      621 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/adobe.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      349 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/age_secret_key.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      486 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/airtable_api_key.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      353 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/algolia_api_key.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      652 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/alibaba.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      761 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/asana.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      549 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/atlassian_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      571 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/authress_access_key.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      521 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/beamer_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      812 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/bitbucket.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      786 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/bittrex.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      361 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/clojars_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      534 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/codecov_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      542 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/coinbase_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      827 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/confluent.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      525 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/contentful_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      370 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/databricks_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      502 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/datadog_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      558 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/defined_networking_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      631 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/digitalocean.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1009 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/discord.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      361 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/doppler_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      534 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/droneci_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1046 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/dropbox.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      371 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/duffel_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      385 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/dynatrace_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      437 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/easypost.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      516 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/etsy_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      540 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/facebook_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      507 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/fastly_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      802 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/finicity.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      534 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/finnhub_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      528 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/flickr_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      563 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/flutterwave.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      367 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/frameio_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      552 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/freshbooks_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      366 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/gcp_api_key.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      637 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/github_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      539 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/gitlab.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      530 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/gitter_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      570 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/gocardless_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      682 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/grafana.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      462 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/hashicorp_tf_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      526 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/heroku_api_key.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      567 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/hubspot_api_key.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      557 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/huggingface.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      500 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/intercom_api_key.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      827 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/jfrog.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1145 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/jwt.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      539 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/kraken_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      829 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/kucoin.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      531 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/launchdarkly_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      609 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/linear.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      804 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/linkedin.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      778 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/lob.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1099 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/mailgun.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      531 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/mapbox_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      552 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/mattermost_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      891 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/messagebird.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      608 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/microsoft_teams_webhook.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      541 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/netlify_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1115 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/new_relic.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      556 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/nytimes_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      491 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/okta_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      395 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/openai_api_key.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      689 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/planetscale.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      374 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/postman_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      346 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/prefect_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      342 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/pulumi_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      337 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/pypi_upload_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      509 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/rapidapi_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      343 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/readme_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      352 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/rubygems_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      325 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/scalingo_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      832 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/sendbird.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      356 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/sendgrid_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      389 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/sendinblue_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      497 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/sentry_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      371 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/shippo_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      766 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/shopify.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      804 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/sidekiq.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1217 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/slack.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      523 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/snyk_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      570 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/squarespace_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      652 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/sumologic.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      397 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/telegram_bot_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      508 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/travisci_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      485 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/twitch_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1512 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/twitter.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      505 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/typeform_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      470 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/vault.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1028 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/yandex.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      494 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/zendesk_secret_key.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     9444 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/sensitive_patterns.json
--rw-r--r--   0 kiran-raga   (501) staff       (20)    16818 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/secrets.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     6377 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/sensitive.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2772 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/sentiment.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2112 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/token_limit.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2441 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/url_reachability.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     6341 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/utils.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1754 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/valid_csv.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1384 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/valid_python.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      603 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/valid_sql.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1063 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/vault.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.903083 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/
--rw-r--r--   0 kiran-raga   (501) staff       (20)      312 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/base_metrics.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.909387 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/
--rw-r--r--   0 kiran-raga   (501) staff       (20)      677 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/__init__.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      749 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/accuracy.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      699 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/ap.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1073 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/bpm.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      574 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/bpref.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      652 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/compat.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1888 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/f1_at_k.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2291 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/f1_score.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      574 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/infAP.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      832 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/insq.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      832 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/inst.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      854 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/iprec.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      597 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/judged.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      998 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/ndcg.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      839 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/nerr10.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      839 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/nerr11.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      950 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/nerr8.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      950 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/nerr9.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      514 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/numq.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      661 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/numrel.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      576 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/numret.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      752 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/p.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1525 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/precision.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1580 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/precision_at_k.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      752 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/r.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      716 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/rbp.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1528 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/recall.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1580 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/recall_at_k.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1019 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/retrieval_metrics.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      688 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/rprec.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1085 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/sdcg.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      688 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/setap.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      750 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/setf.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      829 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/setp.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      572 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/setr.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      764 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/success.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.909669 raga_llm_eval-2.1.1b1/src/raga_llm_eval/observer/
--rw-r--r--   0 kiran-raga   (501) staff       (20)      116 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/observer/__init__.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2405 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/observer/raga_observer.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4150 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/raga_llm_eval.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2848 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/raga_llm_observer.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4773 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/result_manager.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)    10745 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/test_manager.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.922037 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2929 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/__init__.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2009 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/bias_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2087 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/chunk_impact_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     3398 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/coherence_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2741 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/complexity_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4200 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/conciseness_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     6496 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/consistency_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4096 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/context_retrieval_metrics_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     5505 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/contextual_precision_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     5313 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/contextual_recall_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     5211 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/contextual_relevancy_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4540 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/correctness_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1593 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/cosine_similarity_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      913 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/cost_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1856 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/cover_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     8479 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/dan_detectors.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)    55600 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/dan_probes.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4493 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/dan_vulnerability_scanner.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     6258 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/faithfulness_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     5343 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/generic_evaluation_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1371 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/grade_score_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     5070 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/hallucination_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4122 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/harmless_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4978 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/ir_metrics_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      953 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/latency_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1293 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/length_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     8011 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/lmrc_detectors.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     8540 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/lmrc_probes.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4832 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/lmrc_vulnerability_scanner.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2748 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/maliciousness_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1731 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/matcher.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2777 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/overall_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1873 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/pos_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     6679 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/prompt_injection_modeleval.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1068 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/prompt_injection_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)    34353 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/prompt_template.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     3342 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/readability_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1994 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/refusal_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     6157 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/relevancy_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     3056 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/response_toxicity_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1367 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/sentiment_analysis_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     5739 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/summarisation_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     5657 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/template.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.922394 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/
--rw-r--r--   0 kiran-raga   (501) staff       (20)       66 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/__init__.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.931532 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1387 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/anonymize_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      791 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/ban_competitors_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1032 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/ban_substrings_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1290 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/ban_topics_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1371 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/bias_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      997 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/chunk_impact_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2057 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/code.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2703 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/coherence_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      881 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/complexity_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2841 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/conciseness_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1236 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/consistency_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     6415 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/context_retrieval_metrics_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2829 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/contextual_precision_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1525 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/contextual_recall_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2629 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/contextual_relevancy_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      940 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/correctness_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1951 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/cosine_similarity_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)       75 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/cost_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1162 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/cover_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2263 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/factual_consistency_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2195 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/faithfulness_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2801 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/generic_evaluation_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1297 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/grade_score_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1695 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/hallucination_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1467 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/harmful_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1467 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/harmless_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      772 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/invisible_text_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      865 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/ir_metrics_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      526 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/json_verify_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      664 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/language_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1341 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/language_same_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)       92 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/latency_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      300 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/length_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)        0 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/lmrc_vulnerability_scanner.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      334 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/malicious_url_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2005 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/maliciousness_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2933 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/no_refusal_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1914 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/overall_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1343 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/pos_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)       23 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/prompt_injection_modeleval_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1322 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/prompt_injection_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)       23 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/promptinject_modelcompare_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1319 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/readability_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2732 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/reading_time_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1113 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/refusal_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      129 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/regex_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2296 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/relevancy_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1086 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/response_toxicity_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)       97 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/secrets_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1739 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/sensitive_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      843 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/sentiment_analysis_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      223 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/sentiment_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4780 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/summarisation_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1035 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/tokenlimit_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      299 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/toxicity_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      192 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/url_reachability_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1019 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/winner_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1494 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/test_data.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)    28078 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_details.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)    52555 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_executor.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     5266 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_utils.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2857 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/toxicity_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2378 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/winner_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     3719 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/track_manager.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.931790 raga_llm_eval-2.1.1b1/src/raga_llm_eval/utils/
--rw-r--r--   0 kiran-raga   (501) staff       (20)        0 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/utils/__init__.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.934913 raga_llm_eval-2.1.1b1/src/raga_llm_eval/utils/data_files/
--rw-r--r--   0 kiran-raga   (501) staff       (20)  1331765 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/utils/data_files/inthewild_jailbreak_llms.txt
--rw-r--r--   0 kiran-raga   (501) staff       (20)     3777 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/utils/data_files/ldnoobw-en.txt
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2839 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/utils/data_files/ofcom-potentially-offensive.txt
--rw-r--r--   0 kiran-raga   (501) staff       (20)   104116 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/utils/data_files/profanity_en.csv
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1609 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval/utils/utils.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.942775 raga_llm_eval-2.1.1b1/src/raga_llm_eval.egg-info/
--rw-r--r--   0 kiran-raga   (501) staff       (20)    13102 2024-05-08 11:34:03.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval.egg-info/PKG-INFO
--rw-r--r--   0 kiran-raga   (501) staff       (20)    19187 2024-05-08 11:34:03.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval.egg-info/SOURCES.txt
--rw-r--r--   0 kiran-raga   (501) staff       (20)        1 2024-05-08 11:34:03.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval.egg-info/dependency_links.txt
--rw-r--r--   0 kiran-raga   (501) staff       (20)       82 2024-05-08 11:34:03.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval.egg-info/entry_points.txt
--rw-r--r--   0 kiran-raga   (501) staff       (20)      956 2024-05-08 11:34:03.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval.egg-info/requires.txt
--rw-r--r--   0 kiran-raga   (501) staff       (20)       31 2024-05-08 11:34:03.000000 raga_llm_eval-2.1.1b1/src/raga_llm_eval.egg-info/top_level.txt
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.938018 raga_llm_eval-2.1.1b1/src/raga_rag_builder/
--rw-r--r--   0 kiran-raga   (501) staff       (20)      518 2024-04-18 11:24:07.000000 raga_llm_eval-2.1.1b1/src/raga_rag_builder/__init__.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.938805 raga_llm_eval-2.1.1b1/src/raga_rag_builder/data_loader/
--rw-r--r--   0 kiran-raga   (501) staff       (20)       98 2024-04-16 13:57:13.000000 raga_llm_eval-2.1.1b1/src/raga_rag_builder/data_loader/__init__.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2402 2024-04-18 11:24:25.000000 raga_llm_eval-2.1.1b1/src/raga_rag_builder/data_loader/content_loader.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1255 2024-04-17 02:37:05.000000 raga_llm_eval-2.1.1b1/src/raga_rag_builder/data_loader/document_preprocessor.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.939924 raga_llm_eval-2.1.1b1/src/raga_rag_builder/indexer/
--rw-r--r--   0 kiran-raga   (501) staff       (20)      120 2024-04-16 13:57:14.000000 raga_llm_eval-2.1.1b1/src/raga_rag_builder/indexer/__init__.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      774 2024-04-16 13:57:14.000000 raga_llm_eval-2.1.1b1/src/raga_rag_builder/indexer/embedder.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     3733 2024-05-08 09:47:04.000000 raga_llm_eval-2.1.1b1/src/raga_rag_builder/indexer/tokenizer.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     6658 2024-05-08 09:47:04.000000 raga_llm_eval-2.1.1b1/src/raga_rag_builder/indexer/vector_db.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.940487 raga_llm_eval-2.1.1b1/src/raga_rag_builder/language_model_service/
--rw-r--r--   0 kiran-raga   (501) staff       (20)       44 2024-04-16 13:57:13.000000 raga_llm_eval-2.1.1b1/src/raga_rag_builder/language_model_service/__init__.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2684 2024-04-18 11:24:25.000000 raga_llm_eval-2.1.1b1/src/raga_rag_builder/language_model_service/model_inference.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)    13047 2024-05-08 09:47:04.000000 raga_llm_eval-2.1.1b1/src/raga_rag_builder/rag_builder.py
--rw-rw-r--   0 kiran-raga   (501) staff       (20)     2025 2024-04-18 11:24:07.000000 raga_llm_eval-2.1.1b1/src/raga_rag_builder/raga_rag_builder_ui.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.940951 raga_llm_eval-2.1.1b1/src/raga_rag_builder/ranking_system/
--rw-r--r--   0 kiran-raga   (501) staff       (20)       29 2024-04-16 13:57:13.000000 raga_llm_eval-2.1.1b1/src/raga_rag_builder/ranking_system/__init__.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      710 2024-04-16 13:57:14.000000 raga_llm_eval-2.1.1b1/src/raga_rag_builder/ranking_system/ranker.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.941424 raga_llm_eval-2.1.1b1/src/raga_rag_builder/retrieval_engine/
--rw-r--r--   0 kiran-raga   (501) staff       (20)       42 2024-04-15 13:49:01.000000 raga_llm_eval-2.1.1b1/src/raga_rag_builder/retrieval_engine/__init__.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2136 2024-04-17 10:19:54.000000 raga_llm_eval-2.1.1b1/src/raga_rag_builder/retrieval_engine/prompt_manager.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.942046 raga_llm_eval-2.1.1b1/src/raga_rag_builder/templates/
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2840 2024-04-18 08:20:07.000000 raga_llm_eval-2.1.1b1/src/raga_rag_builder/templates/chat.html
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:34:03.942423 raga_llm_eval-2.1.1b1/src/raga_rag_builder/ui_files/
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4769 2024-04-16 10:42:15.000000 raga_llm_eval-2.1.1b1/src/raga_rag_builder/ui_files/RagaAI_logo.png
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:56.019898 raga_llm_eval-2.1.1b2/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)        0 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/LICENSE
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      777 2024-04-18 11:24:07.000000 raga_llm_eval-2.1.1b2/MANIFEST.in
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    13148 2024-05-08 11:54:56.019428 raga_llm_eval-2.1.1b2/PKG-INFO
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    10122 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/README.md
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     3665 2024-05-08 11:54:42.000000 raga_llm_eval-2.1.1b2/pyproject.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)       38 2024-05-08 11:54:56.019951 raga_llm_eval-2.1.1b2/setup.cfg
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:55.899639 raga_llm_eval-2.1.1b2/src/
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:55.902726 raga_llm_eval-2.1.1b2/src/raga_llm_eval/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      431 2024-04-16 16:29:47.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1599 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/api_client_manager.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4085 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/db_manager.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:55.911104 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1526 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    14106 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:55.915331 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      582 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4687 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/analyzer.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)       51 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/exception.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2277 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/faker.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     7851 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/ner_mapping.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:55.915792 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/predefined_recognizers/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      483 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/predefined_recognizers/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      233 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/predefined_recognizers/phone_recognizer.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:55.916519 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/predefined_recognizers/zh/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      380 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/predefined_recognizers/zh/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      288 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/predefined_recognizers/zh/crypto_recognizer.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      626 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/predefined_recognizers/zh/custom_pattern_recognizer.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      359 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/predefined_recognizers/zh/email_recognizer.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1282 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/predefined_recognizers/zh/ip_recognizer.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     9500 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/regex_patterns.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     7006 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/transformers_helpers.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    14149 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/transformers_recognizer.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     3670 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/ban_competitors.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4168 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/ban_substrings.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4402 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/ban_topics.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     5980 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/code.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     5040 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/deanonymize.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2668 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/factual_consistency.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1401 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/gibberish.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1817 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/invisible_text.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1178 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/ir_metrics_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     3085 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/json_verify.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     6611 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/language.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     3192 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/language_same.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2573 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/malicious_url.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      324 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/match_type.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     3324 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/no_refusal.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1397 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/nsfw.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1293 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/politeness.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2047 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/profanity.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1595 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/reading_time.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4141 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/regex.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:55.916651 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:55.933759 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)        0 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      477 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/adafruit.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      621 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/adobe.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      349 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/age_secret_key.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      486 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/airtable_api_key.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      353 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/algolia_api_key.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      652 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/alibaba.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      761 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/asana.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      549 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/atlassian_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      571 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/authress_access_key.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      521 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/beamer_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      812 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/bitbucket.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      786 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/bittrex.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      361 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/clojars_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      534 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/codecov_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      542 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/coinbase_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      827 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/confluent.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      525 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/contentful_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      370 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/databricks_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      502 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/datadog_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      558 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/defined_networking_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      631 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/digitalocean.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1009 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/discord.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      361 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/doppler_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      534 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/droneci_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1046 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/dropbox.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      371 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/duffel_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      385 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/dynatrace_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      437 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/easypost.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      516 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/etsy_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      540 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/facebook_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      507 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/fastly_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      802 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/finicity.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      534 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/finnhub_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      528 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/flickr_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      563 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/flutterwave.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      367 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/frameio_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      552 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/freshbooks_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      366 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/gcp_api_key.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      637 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/github_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      539 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/gitlab.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      530 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/gitter_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      570 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/gocardless_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      682 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/grafana.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      462 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/hashicorp_tf_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      526 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/heroku_api_key.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      567 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/hubspot_api_key.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      557 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/huggingface.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      500 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/intercom_api_key.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      827 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/jfrog.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1145 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/jwt.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      539 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/kraken_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      829 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/kucoin.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      531 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/launchdarkly_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      609 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/linear.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      804 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/linkedin.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      778 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/lob.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1099 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/mailgun.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      531 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/mapbox_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      552 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/mattermost_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      891 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/messagebird.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      608 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/microsoft_teams_webhook.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      541 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/netlify_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1115 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/new_relic.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      556 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/nytimes_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      491 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/okta_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      395 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/openai_api_key.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      689 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/planetscale.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      374 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/postman_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      346 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/prefect_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      342 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/pulumi_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      337 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/pypi_upload_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      509 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/rapidapi_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      343 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/readme_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      352 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/rubygems_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      325 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/scalingo_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      832 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/sendbird.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      356 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/sendgrid_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      389 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/sendinblue_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      497 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/sentry_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      371 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/shippo_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      766 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/shopify.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      804 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/sidekiq.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1217 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/slack.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      523 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/snyk_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      570 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/squarespace_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      652 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/sumologic.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      397 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/telegram_bot_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      508 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/travisci_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      485 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/twitch_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1512 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/twitter.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      505 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/typeform_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      470 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/vault.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1028 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/yandex.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      494 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/zendesk_secret_key.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     9444 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/sensitive_patterns.json
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    16818 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/secrets.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     6377 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/sensitive.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2772 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/sentiment.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2112 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/token_limit.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2441 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/url_reachability.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     6341 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/utils.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1754 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/valid_csv.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1384 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/valid_python.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      603 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/valid_sql.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1063 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/vault.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:55.933942 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      312 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/base_metrics.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:55.940681 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      677 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      749 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/accuracy.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      699 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/ap.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1073 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/bpm.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      574 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/bpref.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      652 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/compat.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1888 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/f1_at_k.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2291 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/f1_score.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      574 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/infAP.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      832 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/insq.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      832 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/inst.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      854 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/iprec.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      597 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/judged.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      998 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/ndcg.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      839 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/nerr10.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      839 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/nerr11.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      950 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/nerr8.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      950 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/nerr9.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      514 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/numq.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      661 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/numrel.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      576 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/numret.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      752 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/p.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1525 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/precision.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1580 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/precision_at_k.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      752 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/r.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      716 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/rbp.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1528 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/recall.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1580 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/recall_at_k.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1019 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/retrieval_metrics.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      688 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/rprec.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1085 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/sdcg.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      688 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/setap.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      750 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/setf.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      829 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/setp.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      572 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/setr.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      764 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/success.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:55.941237 raga_llm_eval-2.1.1b2/src/raga_llm_eval/observer/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      116 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/observer/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2405 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/observer/raga_observer.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4150 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/raga_llm_eval.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2848 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/raga_llm_observer.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4773 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/result_manager.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    10745 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/test_manager.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:55.972849 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2929 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2009 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/bias_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2087 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/chunk_impact_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     3398 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/coherence_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2741 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/complexity_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4200 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/conciseness_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     6496 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/consistency_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4096 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/context_retrieval_metrics_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     5505 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/contextual_precision_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     5313 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/contextual_recall_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     5211 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/contextual_relevancy_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4540 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/correctness_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1593 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/cosine_similarity_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      913 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/cost_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1856 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/cover_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     8479 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/dan_detectors.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    55600 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/dan_probes.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4493 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/dan_vulnerability_scanner.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     6258 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/faithfulness_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     5343 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/generic_evaluation_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1371 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/grade_score_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     5070 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/hallucination_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4122 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/harmless_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4978 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/ir_metrics_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      953 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/latency_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1293 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/length_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     8011 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/lmrc_detectors.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     8540 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/lmrc_probes.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4832 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/lmrc_vulnerability_scanner.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2748 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/maliciousness_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1731 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/matcher.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2777 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/overall_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1873 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/pos_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     6679 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/prompt_injection_modeleval.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1068 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/prompt_injection_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    34353 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/prompt_template.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     3342 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/readability_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1994 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/refusal_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     6157 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/relevancy_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     3056 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/response_toxicity_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1367 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/sentiment_analysis_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     5739 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/summarisation_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     5657 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/template.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:55.973985 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)       66 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/__init__.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:56.004549 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1387 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/anonymize_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      791 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/ban_competitors_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1032 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/ban_substrings_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1290 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/ban_topics_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1371 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/bias_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      997 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/chunk_impact_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2057 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/code.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2703 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/coherence_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      881 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/complexity_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2841 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/conciseness_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1236 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/consistency_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     6415 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/context_retrieval_metrics_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2829 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/contextual_precision_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1525 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/contextual_recall_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2629 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/contextual_relevancy_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      940 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/correctness_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1951 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/cosine_similarity_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)       75 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/cost_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1162 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/cover_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2263 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/factual_consistency_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2195 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/faithfulness_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2801 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/generic_evaluation_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1297 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/grade_score_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1695 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/hallucination_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1467 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/harmful_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1467 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/harmless_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      772 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/invisible_text_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      865 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/ir_metrics_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      526 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/json_verify_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      664 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/language_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1341 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/language_same_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)       92 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/latency_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      300 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/length_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)        0 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/lmrc_vulnerability_scanner.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      334 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/malicious_url_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2005 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/maliciousness_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2933 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/no_refusal_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1914 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/overall_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1343 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/pos_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)       23 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/prompt_injection_modeleval_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1322 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/prompt_injection_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)       23 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/promptinject_modelcompare_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1319 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/readability_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2732 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/reading_time_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1113 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/refusal_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      129 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/regex_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2296 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/relevancy_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1086 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/response_toxicity_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)       97 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/secrets_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1739 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/sensitive_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      843 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/sentiment_analysis_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      223 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/sentiment_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4780 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/summarisation_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1035 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/tokenlimit_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      299 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/toxicity_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      192 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/url_reachability_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1019 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/winner_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1494 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/test_data.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    28078 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_details.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    52555 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_executor.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     5266 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_utils.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2857 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/toxicity_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2378 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/winner_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     3719 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/track_manager.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:56.004885 raga_llm_eval-2.1.1b2/src/raga_llm_eval/utils/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)        0 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/utils/__init__.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:56.009630 raga_llm_eval-2.1.1b2/src/raga_llm_eval/utils/data_files/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)  1331765 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/utils/data_files/inthewild_jailbreak_llms.txt
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     3777 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/utils/data_files/ldnoobw-en.txt
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2839 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/utils/data_files/ofcom-potentially-offensive.txt
+-rw-r--r--   0 kiran-raga   (501) staff       (20)   104116 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/utils/data_files/profanity_en.csv
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1609 2024-03-06 19:09:51.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval/utils/utils.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:56.018341 raga_llm_eval-2.1.1b2/src/raga_llm_eval.egg-info/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    13148 2024-05-08 11:54:55.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval.egg-info/PKG-INFO
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    19187 2024-05-08 11:54:55.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 kiran-raga   (501) staff       (20)        1 2024-05-08 11:54:55.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 kiran-raga   (501) staff       (20)       82 2024-05-08 11:54:55.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval.egg-info/entry_points.txt
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      987 2024-05-08 11:54:55.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval.egg-info/requires.txt
+-rw-r--r--   0 kiran-raga   (501) staff       (20)       31 2024-05-08 11:54:55.000000 raga_llm_eval-2.1.1b2/src/raga_llm_eval.egg-info/top_level.txt
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:56.012813 raga_llm_eval-2.1.1b2/src/raga_rag_builder/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      518 2024-04-18 11:24:07.000000 raga_llm_eval-2.1.1b2/src/raga_rag_builder/__init__.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:56.013682 raga_llm_eval-2.1.1b2/src/raga_rag_builder/data_loader/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)       98 2024-04-16 13:57:13.000000 raga_llm_eval-2.1.1b2/src/raga_rag_builder/data_loader/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2402 2024-04-18 11:24:25.000000 raga_llm_eval-2.1.1b2/src/raga_rag_builder/data_loader/content_loader.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1255 2024-04-17 02:37:05.000000 raga_llm_eval-2.1.1b2/src/raga_rag_builder/data_loader/document_preprocessor.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:56.015006 raga_llm_eval-2.1.1b2/src/raga_rag_builder/indexer/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      120 2024-04-16 13:57:14.000000 raga_llm_eval-2.1.1b2/src/raga_rag_builder/indexer/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      774 2024-04-16 13:57:14.000000 raga_llm_eval-2.1.1b2/src/raga_rag_builder/indexer/embedder.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     3733 2024-05-08 09:47:04.000000 raga_llm_eval-2.1.1b2/src/raga_rag_builder/indexer/tokenizer.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     6658 2024-05-08 09:47:04.000000 raga_llm_eval-2.1.1b2/src/raga_rag_builder/indexer/vector_db.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:56.015784 raga_llm_eval-2.1.1b2/src/raga_rag_builder/language_model_service/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)       44 2024-04-16 13:57:13.000000 raga_llm_eval-2.1.1b2/src/raga_rag_builder/language_model_service/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2684 2024-04-18 11:24:25.000000 raga_llm_eval-2.1.1b2/src/raga_rag_builder/language_model_service/model_inference.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    13047 2024-05-08 09:47:04.000000 raga_llm_eval-2.1.1b2/src/raga_rag_builder/rag_builder.py
+-rw-rw-r--   0 kiran-raga   (501) staff       (20)     2025 2024-04-18 11:24:07.000000 raga_llm_eval-2.1.1b2/src/raga_rag_builder/raga_rag_builder_ui.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:56.016448 raga_llm_eval-2.1.1b2/src/raga_rag_builder/ranking_system/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)       29 2024-04-16 13:57:13.000000 raga_llm_eval-2.1.1b2/src/raga_rag_builder/ranking_system/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      710 2024-04-16 13:57:14.000000 raga_llm_eval-2.1.1b2/src/raga_rag_builder/ranking_system/ranker.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:56.017116 raga_llm_eval-2.1.1b2/src/raga_rag_builder/retrieval_engine/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)       42 2024-04-15 13:49:01.000000 raga_llm_eval-2.1.1b2/src/raga_rag_builder/retrieval_engine/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2136 2024-04-17 10:19:54.000000 raga_llm_eval-2.1.1b2/src/raga_rag_builder/retrieval_engine/prompt_manager.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:56.017429 raga_llm_eval-2.1.1b2/src/raga_rag_builder/templates/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2840 2024-04-18 08:20:07.000000 raga_llm_eval-2.1.1b2/src/raga_rag_builder/templates/chat.html
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-08 11:54:56.017938 raga_llm_eval-2.1.1b2/src/raga_rag_builder/ui_files/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4769 2024-04-16 10:42:15.000000 raga_llm_eval-2.1.1b2/src/raga_rag_builder/ui_files/RagaAI_logo.png
```

### Comparing `raga_llm_eval-2.1.1b1/MANIFEST.in` & `raga_llm_eval-2.1.1b2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/PKG-INFO` & `raga_llm_eval-2.1.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-llm-eval
-Version: 2.1.1b1
+Version: 2.1.1b2
 Summary: Package for LLM Evaluation
 Author-email: Raga AI <kiran.scaria@raga.ai>
 Project-URL: Homepage, https://raga.ai
 Project-URL: Documentation, https://github.com/aristotle-ai/raga-llm-eval/blob/main/doc
 Project-URL: Repository, https://github.com/aristotle-ai/raga-llm-eval
 Project-URL: Issues, https://github.com/aristotle-ai/raga-llm-eval/issues
 Keywords: ragaai,raga,llm,testing,llm-eval
@@ -55,14 +55,15 @@
 Requires-Dist: litellm~=1.35.8
 Requires-Dist: streamlit~=1.31.1
 Requires-Dist: unstructured~=0.12
 Requires-Dist: docx2txt~=0.8
 Requires-Dist: pypdf~=4.0
 Requires-Dist: ragatouille~=0.0.8
 Requires-Dist: flask-ngrok3~=0.3.1
+Requires-Dist: langchain-experimental~=0.0.58
 Provides-Extra: docs-dev
 Requires-Dist: mkdocs==1.5.3; extra == "docs-dev"
 Requires-Dist: mkdocs-autorefs==0.5.0; extra == "docs-dev"
 Requires-Dist: mkdocs-material==9.5.9; extra == "docs-dev"
 Requires-Dist: mkdocs-material-extensions==1.3.1; extra == "docs-dev"
 Requires-Dist: mkdocstrings==0.24.0; extra == "docs-dev"
 Requires-Dist: mkdocstrings-python==1.8.0; extra == "docs-dev"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: raga-llm-eval Version: 2.1.1b1 Summary: Package for
+Metadata-Version: 2.1 Name: raga-llm-eval Version: 2.1.1b2 Summary: Package for
 LLM Evaluation Author-email: Raga AI
 raga.ai> Project-URL: Homepage, https://raga.ai Project-URL: Documentation,
 https://github.com/aristotle-ai/raga-llm-eval/blob/main/doc Project-URL:
 Repository, https://github.com/aristotle-ai/raga-llm-eval Project-URL: Issues,
 https://github.com/aristotle-ai/raga-llm-eval/issues Keywords:
 ragaai,raga,llm,testing,llm-eval Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
@@ -25,24 +25,25 @@
 structlog~=24.1.0 Requires-Dist: json-repair~=0.9.0 Requires-Dist:
 fuzzysearch~=0.7.3 Requires-Dist: waitress~=3.0.0 Requires-Dist:
 sqlvalidator~=0.0.20 Requires-Dist: Flask~=3.0.2 Requires-Dist: langchain-
 community~=0.0.29 Requires-Dist: langchain-openai~=0.0.5 Requires-Dist:
 langchain-text-splitters~=0.0.1 Requires-Dist: langchain-chroma~=0.1.0
 Requires-Dist: litellm~=1.35.8 Requires-Dist: streamlit~=1.31.1 Requires-Dist:
 unstructured~=0.12 Requires-Dist: docx2txt~=0.8 Requires-Dist: pypdf~=4.0
-Requires-Dist: ragatouille~=0.0.8 Requires-Dist: flask-ngrok3~=0.3.1 Provides-
-Extra: docs-dev Requires-Dist: mkdocs==1.5.3; extra == "docs-dev" Requires-
-Dist: mkdocs-autorefs==0.5.0; extra == "docs-dev" Requires-Dist: mkdocs-
-material==9.5.9; extra == "docs-dev" Requires-Dist: mkdocs-material-
-extensions==1.3.1; extra == "docs-dev" Requires-Dist: mkdocstrings==0.24.0;
-extra == "docs-dev" Requires-Dist: mkdocstrings-python==1.8.0; extra == "docs-
-dev" Provides-Extra: dev Requires-Dist: black; extra == "dev" Requires-Dist:
-flake8; extra == "dev" Requires-Dist: isort; extra == "dev" Requires-Dist:
-mypy; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist:
-pytest-cov; extra == "dev" Requires-Dist: build; extra == "dev"
+Requires-Dist: ragatouille~=0.0.8 Requires-Dist: flask-ngrok3~=0.3.1 Requires-
+Dist: langchain-experimental~=0.0.58 Provides-Extra: docs-dev Requires-Dist:
+mkdocs==1.5.3; extra == "docs-dev" Requires-Dist: mkdocs-autorefs==0.5.0; extra
+== "docs-dev" Requires-Dist: mkdocs-material==9.5.9; extra == "docs-dev"
+Requires-Dist: mkdocs-material-extensions==1.3.1; extra == "docs-dev" Requires-
+Dist: mkdocstrings==0.24.0; extra == "docs-dev" Requires-Dist: mkdocstrings-
+python==1.8.0; extra == "docs-dev" Provides-Extra: dev Requires-Dist: black;
+extra == "dev" Requires-Dist: flake8; extra == "dev" Requires-Dist: isort;
+extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-Dist: pytest; extra
+== "dev" Requires-Dist: pytest-cov; extra == "dev" Requires-Dist: build; extra
+== "dev"
                                 [RagaAI - Logo]
                           ************ RRaaggaa LLLLMM HHuubb ************
               ******** _RR_aa_gg_aa_ _AA_II || _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn || _GG_ee_tt_tt_ii_nn_gg_ _SS_tt_aa_rr_tt_ee_dd ********
           [![PyPI - Version](https://img.shields.io/pypi/v/raga-llm-
 eval?label=PyPI%20Package)](https://badge.fury.io/py/raga-llm-eval) [![Open In
   Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1PQGqDGdcSUxhSvpSQYX8ZdHf5r90WSYf?usp=sharing)
```

### Comparing `raga_llm_eval-2.1.1b1/README.md` & `raga_llm_eval-2.1.1b2/README.md`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/pyproject.toml` & `raga_llm_eval-2.1.1b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "raga-llm-eval"
-version = "2.1.1.beta1"
+version = "2.1.1.beta2"
 authors = [{ name = "Raga AI", email = "kiran.scaria@raga.ai" }]
 description = "Package for LLM Evaluation"
 readme = "README.md"
 keywords = ["ragaai", "raga", "llm", "testing", "llm-eval"]
 license = { file = "LICENSE" }
 
 classifiers = [
@@ -57,14 +57,15 @@
     "litellm~=1.35.8",
     "streamlit~=1.31.1",
     "unstructured~=0.12",
     "docx2txt~=0.8",
     "pypdf~=4.0",
     "ragatouille~=0.0.8",
     "flask-ngrok3~=0.3.1",
+    "langchain-experimental~=0.0.58"
 ]
 
 
 [project.optional-dependencies]
 docs-dev = [
     "mkdocs==1.5.3",
     "mkdocs-autorefs==0.5.0",
```

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/api_client_manager.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/api_client_manager.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/db_manager.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/db_manager.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/__init__.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/__init__.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/__init__.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/analyzer.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/analyzer.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/faker.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/faker.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/ner_mapping.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/ner_mapping.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/predefined_recognizers/zh/custom_pattern_recognizer.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/predefined_recognizers/zh/custom_pattern_recognizer.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/predefined_recognizers/zh/ip_recognizer.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/predefined_recognizers/zh/ip_recognizer.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/regex_patterns.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/regex_patterns.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/transformers_helpers.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/transformers_helpers.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/anonymize_helpers/transformers_recognizer.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/anonymize_helpers/transformers_recognizer.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/ban_competitors.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/ban_competitors.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/ban_substrings.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/ban_substrings.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/ban_topics.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/ban_topics.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/code.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/code.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/deanonymize.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/deanonymize.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/factual_consistency.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/factual_consistency.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/gibberish.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/gibberish.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/invisible_text.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/invisible_text.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/ir_metrics_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/ir_metrics_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/json_verify.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/json_verify.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/language.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/language.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/language_same.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/language_same.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/malicious_url.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/malicious_url.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/no_refusal.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/no_refusal.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/nsfw.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/nsfw.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/politeness.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/politeness.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/profanity.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/profanity.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/reading_time.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/reading_time.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/regex.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/regex.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/adobe.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/adobe.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/alibaba.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/alibaba.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/asana.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/asana.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/atlassian_api_token.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/atlassian_api_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/authress_access_key.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/authress_access_key.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/beamer_api_token.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/beamer_api_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/bitbucket.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/bitbucket.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/bittrex.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/bittrex.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/codecov_access_token.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/codecov_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/coinbase_access_token.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/coinbase_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/confluent.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/confluent.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/contentful_api_token.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/contentful_api_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/defined_networking_api_token.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/defined_networking_api_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/digitalocean.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/digitalocean.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/discord.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/discord.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/droneci_access_token.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/droneci_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/dropbox.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/dropbox.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/etsy_access_token.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/etsy_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/facebook_access_token.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/facebook_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/finicity.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/finicity.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/finnhub_access_token.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/finnhub_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/flickr_access_token.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/flickr_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/flutterwave.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/flutterwave.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/freshbooks_access_token.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/freshbooks_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/github_token.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/github_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/gitlab.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/gitlab.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/gitter_access_token.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/gitter_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/gocardless_api_token.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/gocardless_api_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/grafana.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/grafana.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/heroku_api_key.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/heroku_api_key.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/hubspot_api_key.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/hubspot_api_key.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/huggingface.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/huggingface.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/jfrog.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/jfrog.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/jwt.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/jwt.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/kraken_access_token.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/kraken_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/kucoin.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/kucoin.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/launchdarkly_access_token.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/launchdarkly_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/linear.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/linear.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/linkedin.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/linkedin.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/lob.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/lob.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/mailgun.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/mailgun.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/mapbox_api_token.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/mapbox_api_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/mattermost_access_token.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/mattermost_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/messagebird.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/messagebird.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/microsoft_teams_webhook.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/microsoft_teams_webhook.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/netlify_access_token.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/netlify_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/new_relic.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/new_relic.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/nytimes_access_token.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/nytimes_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/planetscale.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/planetscale.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/sendbird.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/sendbird.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/shopify.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/shopify.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/sidekiq.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/sidekiq.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/slack.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/slack.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/snyk_api_token.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/snyk_api_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/squarespace_access_token.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/squarespace_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/sumologic.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/sumologic.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/twitter.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/twitter.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/secrets_plugins/yandex.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/secrets_plugins/yandex.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/resources/sensitive_patterns.json` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/resources/sensitive_patterns.json`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/secrets.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/secrets.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/sensitive.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/sensitive.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/sentiment.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/sentiment.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/token_limit.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/token_limit.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/url_reachability.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/url_reachability.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/utils.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/utils.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/valid_csv.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/valid_csv.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/valid_python.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/valid_python.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/valid_sql.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/valid_sql.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/guardrails/vault.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/guardrails/vault.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/__init__.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/accuracy.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/accuracy.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/ap.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/ap.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/bpm.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/bpm.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/bpref.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/bpref.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/compat.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/compat.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/f1_at_k.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/f1_at_k.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/f1_score.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/f1_score.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/infAP.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/infAP.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/insq.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/insq.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/inst.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/inst.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/iprec.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/iprec.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/judged.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/judged.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/ndcg.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/ndcg.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/nerr10.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/nerr10.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/nerr11.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/nerr11.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/nerr8.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/nerr8.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/nerr9.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/nerr9.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/numq.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/numq.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/numrel.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/numrel.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/numret.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/numret.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/p.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/p.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/precision.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/precision.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/precision_at_k.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/precision_at_k.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/r.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/r.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/rbp.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/rbp.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/recall.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/recall.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/recall_at_k.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/recall_at_k.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/retrieval_metrics.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/retrieval_metrics.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/rprec.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/rprec.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/sdcg.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/sdcg.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/setap.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/setap.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/setf.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/setf.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/setp.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/setp.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/setr.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/setr.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/metrics/retrieval/success.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/metrics/retrieval/success.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/observer/raga_observer.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/observer/raga_observer.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/raga_llm_eval.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/raga_llm_eval.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/raga_llm_observer.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/raga_llm_observer.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/result_manager.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/result_manager.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/test_manager.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/test_manager.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/__init__.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/bias_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/bias_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/chunk_impact_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/chunk_impact_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/coherence_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/coherence_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/complexity_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/complexity_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/conciseness_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/conciseness_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/consistency_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/consistency_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/context_retrieval_metrics_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/context_retrieval_metrics_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/contextual_precision_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/contextual_precision_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/contextual_recall_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/contextual_recall_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/contextual_relevancy_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/contextual_relevancy_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/correctness_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/correctness_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/cosine_similarity_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/cosine_similarity_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/cost_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/cost_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/cover_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/cover_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/dan_detectors.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/dan_detectors.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/dan_probes.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/dan_probes.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/dan_vulnerability_scanner.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/dan_vulnerability_scanner.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/faithfulness_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/faithfulness_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/generic_evaluation_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/generic_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/grade_score_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/grade_score_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/hallucination_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/hallucination_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/harmless_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/harmless_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/ir_metrics_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/ir_metrics_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/latency_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/latency_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/length_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/length_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/lmrc_detectors.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/lmrc_detectors.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/lmrc_probes.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/lmrc_probes.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/lmrc_vulnerability_scanner.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/lmrc_vulnerability_scanner.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/maliciousness_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/maliciousness_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/matcher.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/matcher.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/overall_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/overall_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/pos_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/pos_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/prompt_injection_modeleval.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/prompt_injection_modeleval.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/prompt_injection_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/prompt_injection_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/prompt_template.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/prompt_template.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/readability_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/readability_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/refusal_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/refusal_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/relevancy_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/relevancy_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/response_toxicity_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/response_toxicity_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/sentiment_analysis_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/sentiment_analysis_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/summarisation_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/summarisation_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/template.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/template.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/anonymize_guardrail.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/anonymize_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/ban_competitors_guardrail.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/ban_competitors_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/ban_substrings_guardrail.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/ban_substrings_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/ban_topics_guardrail.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/ban_topics_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/bias_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/bias_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/chunk_impact_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/chunk_impact_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/code.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/code.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/coherence_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/coherence_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/complexity_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/complexity_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/conciseness_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/conciseness_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/consistency_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/consistency_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/context_retrieval_metrics_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/context_retrieval_metrics_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/contextual_precision_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/contextual_precision_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/contextual_recall_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/contextual_recall_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/contextual_relevancy_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/contextual_relevancy_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/correctness_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/correctness_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/cosine_similarity_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/cosine_similarity_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/cover_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/cover_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/factual_consistency_guardrail.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/factual_consistency_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/faithfulness_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/faithfulness_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/generic_evaluation_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/generic_evaluation_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/grade_score_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/grade_score_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/hallucination_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/hallucination_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/harmful_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/harmful_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/harmless_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/harmless_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/invisible_text_guardrail.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/invisible_text_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/ir_metrics_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/ir_metrics_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/json_verify_guardrail.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/json_verify_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/language_guardrail.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/language_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/language_same_guardrail.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/language_same_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/maliciousness_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/maliciousness_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/no_refusal_guardrail.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/no_refusal_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/overall_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/overall_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/pos_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/pos_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/prompt_injection_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/prompt_injection_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/readability_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/readability_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/reading_time_guardrail.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/reading_time_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/refusal_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/refusal_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/relevancy_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/relevancy_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/response_toxicity_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/response_toxicity_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/sensitive_guardrail.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/sensitive_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/sentiment_analysis_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/sentiment_analysis_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/summarisation_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/summarisation_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/tokenlimit_guardrail.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/tokenlimit_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/data_files/winner_test.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/data_files/winner_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_data/test_data.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_data/test_data.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_details.toml` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_details.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_executor.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/test_utils.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/toxicity_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/toxicity_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/tests/winner_test.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/tests/winner_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/track_manager.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/track_manager.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/utils/data_files/inthewild_jailbreak_llms.txt` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/utils/data_files/inthewild_jailbreak_llms.txt`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/utils/data_files/ldnoobw-en.txt` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/utils/data_files/ldnoobw-en.txt`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/utils/data_files/ofcom-potentially-offensive.txt` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/utils/data_files/ofcom-potentially-offensive.txt`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/utils/data_files/profanity_en.csv` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/utils/data_files/profanity_en.csv`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval/utils/utils.py` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval/utils/utils.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval.egg-info/PKG-INFO` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-llm-eval
-Version: 2.1.1b1
+Version: 2.1.1b2
 Summary: Package for LLM Evaluation
 Author-email: Raga AI <kiran.scaria@raga.ai>
 Project-URL: Homepage, https://raga.ai
 Project-URL: Documentation, https://github.com/aristotle-ai/raga-llm-eval/blob/main/doc
 Project-URL: Repository, https://github.com/aristotle-ai/raga-llm-eval
 Project-URL: Issues, https://github.com/aristotle-ai/raga-llm-eval/issues
 Keywords: ragaai,raga,llm,testing,llm-eval
@@ -55,14 +55,15 @@
 Requires-Dist: litellm~=1.35.8
 Requires-Dist: streamlit~=1.31.1
 Requires-Dist: unstructured~=0.12
 Requires-Dist: docx2txt~=0.8
 Requires-Dist: pypdf~=4.0
 Requires-Dist: ragatouille~=0.0.8
 Requires-Dist: flask-ngrok3~=0.3.1
+Requires-Dist: langchain-experimental~=0.0.58
 Provides-Extra: docs-dev
 Requires-Dist: mkdocs==1.5.3; extra == "docs-dev"
 Requires-Dist: mkdocs-autorefs==0.5.0; extra == "docs-dev"
 Requires-Dist: mkdocs-material==9.5.9; extra == "docs-dev"
 Requires-Dist: mkdocs-material-extensions==1.3.1; extra == "docs-dev"
 Requires-Dist: mkdocstrings==0.24.0; extra == "docs-dev"
 Requires-Dist: mkdocstrings-python==1.8.0; extra == "docs-dev"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: raga-llm-eval Version: 2.1.1b1 Summary: Package for
+Metadata-Version: 2.1 Name: raga-llm-eval Version: 2.1.1b2 Summary: Package for
 LLM Evaluation Author-email: Raga AI
 raga.ai> Project-URL: Homepage, https://raga.ai Project-URL: Documentation,
 https://github.com/aristotle-ai/raga-llm-eval/blob/main/doc Project-URL:
 Repository, https://github.com/aristotle-ai/raga-llm-eval Project-URL: Issues,
 https://github.com/aristotle-ai/raga-llm-eval/issues Keywords:
 ragaai,raga,llm,testing,llm-eval Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
@@ -25,24 +25,25 @@
 structlog~=24.1.0 Requires-Dist: json-repair~=0.9.0 Requires-Dist:
 fuzzysearch~=0.7.3 Requires-Dist: waitress~=3.0.0 Requires-Dist:
 sqlvalidator~=0.0.20 Requires-Dist: Flask~=3.0.2 Requires-Dist: langchain-
 community~=0.0.29 Requires-Dist: langchain-openai~=0.0.5 Requires-Dist:
 langchain-text-splitters~=0.0.1 Requires-Dist: langchain-chroma~=0.1.0
 Requires-Dist: litellm~=1.35.8 Requires-Dist: streamlit~=1.31.1 Requires-Dist:
 unstructured~=0.12 Requires-Dist: docx2txt~=0.8 Requires-Dist: pypdf~=4.0
-Requires-Dist: ragatouille~=0.0.8 Requires-Dist: flask-ngrok3~=0.3.1 Provides-
-Extra: docs-dev Requires-Dist: mkdocs==1.5.3; extra == "docs-dev" Requires-
-Dist: mkdocs-autorefs==0.5.0; extra == "docs-dev" Requires-Dist: mkdocs-
-material==9.5.9; extra == "docs-dev" Requires-Dist: mkdocs-material-
-extensions==1.3.1; extra == "docs-dev" Requires-Dist: mkdocstrings==0.24.0;
-extra == "docs-dev" Requires-Dist: mkdocstrings-python==1.8.0; extra == "docs-
-dev" Provides-Extra: dev Requires-Dist: black; extra == "dev" Requires-Dist:
-flake8; extra == "dev" Requires-Dist: isort; extra == "dev" Requires-Dist:
-mypy; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist:
-pytest-cov; extra == "dev" Requires-Dist: build; extra == "dev"
+Requires-Dist: ragatouille~=0.0.8 Requires-Dist: flask-ngrok3~=0.3.1 Requires-
+Dist: langchain-experimental~=0.0.58 Provides-Extra: docs-dev Requires-Dist:
+mkdocs==1.5.3; extra == "docs-dev" Requires-Dist: mkdocs-autorefs==0.5.0; extra
+== "docs-dev" Requires-Dist: mkdocs-material==9.5.9; extra == "docs-dev"
+Requires-Dist: mkdocs-material-extensions==1.3.1; extra == "docs-dev" Requires-
+Dist: mkdocstrings==0.24.0; extra == "docs-dev" Requires-Dist: mkdocstrings-
+python==1.8.0; extra == "docs-dev" Provides-Extra: dev Requires-Dist: black;
+extra == "dev" Requires-Dist: flake8; extra == "dev" Requires-Dist: isort;
+extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-Dist: pytest; extra
+== "dev" Requires-Dist: pytest-cov; extra == "dev" Requires-Dist: build; extra
+== "dev"
                                 [RagaAI - Logo]
                           ************ RRaaggaa LLLLMM HHuubb ************
               ******** _RR_aa_gg_aa_ _AA_II || _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn || _GG_ee_tt_tt_ii_nn_gg_ _SS_tt_aa_rr_tt_ee_dd ********
           [![PyPI - Version](https://img.shields.io/pypi/v/raga-llm-
 eval?label=PyPI%20Package)](https://badge.fury.io/py/raga-llm-eval) [![Open In
   Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1PQGqDGdcSUxhSvpSQYX8ZdHf5r90WSYf?usp=sharing)
```

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval.egg-info/SOURCES.txt` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_llm_eval.egg-info/requires.txt` & `raga_llm_eval-2.1.1b2/src/raga_llm_eval.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 litellm~=1.35.8
 streamlit~=1.31.1
 unstructured~=0.12
 docx2txt~=0.8
 pypdf~=4.0
 ragatouille~=0.0.8
 flask-ngrok3~=0.3.1
+langchain-experimental~=0.0.58
 
 [dev]
 black
 flake8
 isort
 mypy
 pytest
```

### Comparing `raga_llm_eval-2.1.1b1/src/raga_rag_builder/__init__.py` & `raga_llm_eval-2.1.1b2/src/raga_rag_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_rag_builder/data_loader/content_loader.py` & `raga_llm_eval-2.1.1b2/src/raga_rag_builder/data_loader/content_loader.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_rag_builder/data_loader/document_preprocessor.py` & `raga_llm_eval-2.1.1b2/src/raga_rag_builder/data_loader/document_preprocessor.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_rag_builder/indexer/embedder.py` & `raga_llm_eval-2.1.1b2/src/raga_rag_builder/indexer/embedder.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_rag_builder/indexer/tokenizer.py` & `raga_llm_eval-2.1.1b2/src/raga_rag_builder/indexer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_rag_builder/indexer/vector_db.py` & `raga_llm_eval-2.1.1b2/src/raga_rag_builder/indexer/vector_db.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_rag_builder/language_model_service/model_inference.py` & `raga_llm_eval-2.1.1b2/src/raga_rag_builder/language_model_service/model_inference.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_rag_builder/rag_builder.py` & `raga_llm_eval-2.1.1b2/src/raga_rag_builder/rag_builder.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_rag_builder/raga_rag_builder_ui.py` & `raga_llm_eval-2.1.1b2/src/raga_rag_builder/raga_rag_builder_ui.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_rag_builder/ranking_system/ranker.py` & `raga_llm_eval-2.1.1b2/src/raga_rag_builder/ranking_system/ranker.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_rag_builder/retrieval_engine/prompt_manager.py` & `raga_llm_eval-2.1.1b2/src/raga_rag_builder/retrieval_engine/prompt_manager.py`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_rag_builder/templates/chat.html` & `raga_llm_eval-2.1.1b2/src/raga_rag_builder/templates/chat.html`

 * *Files identical despite different names*

### Comparing `raga_llm_eval-2.1.1b1/src/raga_rag_builder/ui_files/RagaAI_logo.png` & `raga_llm_eval-2.1.1b2/src/raga_rag_builder/ui_files/RagaAI_logo.png`

 * *Files identical despite different names*

