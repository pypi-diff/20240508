# Comparing `tmp/vayu_client-1.0.2.tar.gz` & `tmp/vayu_client-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vayu_client-1.0.2.tar", last modified: Thu Jan 25 09:51:53 2024, max compression
+gzip compressed data, was "vayu_client-1.0.3.tar", last modified: Wed May  8 15:19:37 2024, max compression
```

## Comparing `vayu_client-1.0.2.tar` & `vayu_client-1.0.3.tar`

### file list

```diff
@@ -1,30 +1,101 @@
-drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-01-25 09:51:53.000000 vayu_client-1.0.2/
--rw-r--r--   0 shaigross   (501) staff       (20)     3162 2024-01-25 09:51:53.000000 vayu_client-1.0.2/PKG-INFO
--rw-r--r--   0 shaigross   (501) staff       (20)      517 2024-01-24 18:02:42.000000 vayu_client-1.0.2/README.md
-drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-01-25 09:51:53.000000 vayu_client-1.0.2/openapi_client/
--rw-r--r--   0 shaigross   (501) staff       (20)     1413 2024-01-25 09:49:50.000000 vayu_client-1.0.2/openapi_client/__init__.py
-drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-01-25 09:51:53.000000 vayu_client-1.0.2/openapi_client/api/
--rw-r--r--   0 shaigross   (501) staff       (20)      148 2024-01-25 09:49:50.000000 vayu_client-1.0.2/openapi_client/api/__init__.py
--rw-r--r--   0 shaigross   (501) staff       (20)    12788 2024-01-25 09:49:50.000000 vayu_client-1.0.2/openapi_client/api/auth_api.py
--rw-r--r--   0 shaigross   (501) staff       (20)    13161 2024-01-25 09:49:50.000000 vayu_client-1.0.2/openapi_client/api/events_api.py
--rw-r--r--   0 shaigross   (501) staff       (20)    24761 2024-01-25 09:49:50.000000 vayu_client-1.0.2/openapi_client/api_client.py
--rw-r--r--   0 shaigross   (501) staff       (20)      674 2024-01-25 09:49:50.000000 vayu_client-1.0.2/openapi_client/api_response.py
--rw-r--r--   0 shaigross   (501) staff       (20)    14972 2024-01-25 09:49:50.000000 vayu_client-1.0.2/openapi_client/configuration.py
--rw-r--r--   0 shaigross   (501) staff       (20)     6121 2024-01-25 09:49:50.000000 vayu_client-1.0.2/openapi_client/exceptions.py
-drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-01-25 09:51:53.000000 vayu_client-1.0.2/openapi_client/models/
--rw-r--r--   0 shaigross   (501) staff       (20)      769 2024-01-25 09:49:50.000000 vayu_client-1.0.2/openapi_client/models/__init__.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3637 2024-01-25 09:49:50.000000 vayu_client-1.0.2/openapi_client/models/event_input.py
--rw-r--r--   0 shaigross   (501) staff       (20)     2751 2024-01-25 09:49:50.000000 vayu_client-1.0.2/openapi_client/models/login_request.py
--rw-r--r--   0 shaigross   (501) staff       (20)     2609 2024-01-25 09:49:50.000000 vayu_client-1.0.2/openapi_client/models/login_response.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3114 2024-01-25 09:49:50.000000 vayu_client-1.0.2/openapi_client/models/send_events_request.py
--rw-r--r--   0 shaigross   (501) staff       (20)     9963 2024-01-25 09:49:50.000000 vayu_client-1.0.2/openapi_client/rest.py
--rw-r--r--   0 shaigross   (501) staff       (20)      420 2024-01-25 09:51:53.000000 vayu_client-1.0.2/setup.cfg
--rw-r--r--   0 shaigross   (501) staff       (20)      296 2024-01-24 16:49:22.000000 vayu_client-1.0.2/setup.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1547 2024-01-24 18:03:16.000000 vayu_client-1.0.2/vayu.py
-drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-01-25 09:51:53.000000 vayu_client-1.0.2/vayu_client.egg-info/
--rw-r--r--   0 shaigross   (501) staff       (20)     3162 2024-01-25 09:51:53.000000 vayu_client-1.0.2/vayu_client.egg-info/PKG-INFO
--rw-r--r--   0 shaigross   (501) staff       (20)      686 2024-01-25 09:51:53.000000 vayu_client-1.0.2/vayu_client.egg-info/SOURCES.txt
--rw-r--r--   0 shaigross   (501) staff       (20)        1 2024-01-25 09:51:53.000000 vayu_client-1.0.2/vayu_client.egg-info/dependency_links.txt
--rw-r--r--   0 shaigross   (501) staff       (20)      102 2024-01-25 09:51:53.000000 vayu_client-1.0.2/vayu_client.egg-info/requires.txt
--rw-r--r--   0 shaigross   (501) staff       (20)       32 2024-01-25 09:51:53.000000 vayu_client-1.0.2/vayu_client.egg-info/top_level.txt
--rw-r--r--   0 shaigross   (501) staff       (20)       38 2024-01-24 11:17:29.000000 vayu_client-1.0.2/vayu_consts.py
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-08 15:19:37.450335 vayu_client-1.0.3/
+-rw-r--r--   0 shaigross   (501) staff       (20)     2539 2024-05-08 15:19:37.450404 vayu_client-1.0.3/PKG-INFO
+-rw-r--r--   0 shaigross   (501) staff       (20)      481 2024-05-08 15:19:35.000000 vayu_client-1.0.3/README.md
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-08 15:19:37.430451 vayu_client-1.0.3/entity_clients/
+-rw-r--r--   0 shaigross   (501) staff       (20)       46 2024-05-08 13:47:16.000000 vayu_client-1.0.3/entity_clients/__init__.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1178 2024-05-08 14:04:33.000000 vayu_client-1.0.3/entity_clients/contracts_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1328 2024-05-08 13:49:15.000000 vayu_client-1.0.3/entity_clients/customers_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1413 2024-05-08 14:59:08.000000 vayu_client-1.0.3/entity_clients/events_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)      517 2024-05-08 14:06:03.000000 vayu_client-1.0.3/entity_clients/invoices_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1840 2024-05-08 14:06:04.000000 vayu_client-1.0.3/entity_clients/meters_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)      561 2024-05-08 13:49:18.000000 vayu_client-1.0.3/entity_clients/plans_client.py
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-08 15:19:37.432188 vayu_client-1.0.3/openapi_client/
+-rw-r--r--   0 shaigross   (501) staff       (20)     6948 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/__init__.py
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-08 15:19:37.436323 vayu_client-1.0.3/openapi_client/api/
+-rw-r--r--   0 shaigross   (501) staff       (20)      422 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/api/__init__.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    12591 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/api/auth_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    43742 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/api/contracts_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    55565 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/api/customers_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    61236 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/api/events_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    22281 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/api/invoices_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    43924 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/api/meters_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    32198 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/api/plans_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    26550 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/api_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)      652 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/api_response.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    15152 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/configuration.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     6180 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/exceptions.py
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-08 15:19:37.449683 vayu_client-1.0.3/openapi_client/models/
+-rw-r--r--   0 shaigross   (501) staff       (20)     6030 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/__init__.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3340 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/aggregation_method.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1161 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/aggregation_operator.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1052 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/billing_interval.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3214 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/condition.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4112 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/create_contract_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3126 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/create_contract_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3084 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/create_customer_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/create_customer_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3889 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/create_customer_response_schema_customer.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3034 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/criterion.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1202 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/criterion_operator.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3126 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/delete_contract_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/delete_customer_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3134 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/delete_event_by_ref_id_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4983 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/delete_event_by_ref_id_response_schema_event.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3063 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/delete_meter_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3042 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/delete_plan_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4127 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/event.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3243 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/events_dry_run_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4380 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/events_dry_run_response_schema_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3921 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/events_dry_run_response_schema_inner_event.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4556 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3461 2024-05-08 11:11:33.000000 vayu_client-1.0.3/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner_aggregation_method.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3477 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/filter.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3114 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_contract_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4858 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_contract_response_schema_contract.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3126 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_customer_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3110 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_event_by_ref_id_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4861 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_event_by_ref_id_response_schema_event.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3093 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_invoice_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     6159 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_invoice_response_schema_invoice.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3515 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_invoice_response_schema_invoice_line_items_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3051 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_meter_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4720 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_meter_response_schema_meter.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3030 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_plan_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4195 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_plan_response_schema_plan.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3737 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/list_contracts_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4766 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/list_contracts_response_schema_contracts_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3737 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/list_customers_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3785 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/list_customers_response_schema_customers_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3716 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/list_invoices_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     6067 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/list_invoices_response_schema_invoices_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3674 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/list_meters_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4628 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/list_meters_response_schema_meters_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3653 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/list_plans_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4103 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/list_plans_response_schema_plans_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     2883 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/login_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     2870 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/login_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     2883 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/period.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3483 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/plan_billing_data.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1023 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/plan_status.py
+-rw-r--r--   0 shaigross   (501) staff       (20)      947 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/plan_type.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3353 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/query_events_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4866 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/query_events_response_schema_events_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3235 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/send_events_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4230 2024-05-08 14:01:03.000000 vayu_client-1.0.3/openapi_client/models/send_events_request_schema_events_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4212 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/send_events_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3218 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/send_events_response_schema_invalid_events_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3108 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/update_customer_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/update_customer_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4011 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/update_meter_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3063 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/update_meter_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     9616 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/rest.py
+-rw-r--r--   0 shaigross   (501) staff       (20)      420 2024-05-08 15:19:37.450634 vayu_client-1.0.3/setup.cfg
+-rw-r--r--   0 shaigross   (501) staff       (20)      296 2024-01-24 16:49:22.000000 vayu_client-1.0.3/setup.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     2090 2024-05-08 15:03:11.000000 vayu_client-1.0.3/vayu.py
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-08 15:19:37.450246 vayu_client-1.0.3/vayu_client.egg-info/
+-rw-r--r--   0 shaigross   (501) staff       (20)     2539 2024-05-08 15:19:37.000000 vayu_client-1.0.3/vayu_client.egg-info/PKG-INFO
+-rw-r--r--   0 shaigross   (501) staff       (20)     4400 2024-05-08 15:19:37.000000 vayu_client-1.0.3/vayu_client.egg-info/SOURCES.txt
+-rw-r--r--   0 shaigross   (501) staff       (20)        1 2024-05-08 15:19:37.000000 vayu_client-1.0.3/vayu_client.egg-info/dependency_links.txt
+-rw-r--r--   0 shaigross   (501) staff       (20)      102 2024-05-08 15:19:37.000000 vayu_client-1.0.3/vayu_client.egg-info/requires.txt
+-rw-r--r--   0 shaigross   (501) staff       (20)       47 2024-05-08 15:19:37.000000 vayu_client-1.0.3/vayu_client.egg-info/top_level.txt
+-rw-r--r--   0 shaigross   (501) staff       (20)       38 2024-01-24 11:17:29.000000 vayu_client-1.0.3/vayu_consts.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vayu_client-1.0.2/PKG-INFO` & `vayu_client-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,85 +1,84 @@
 Metadata-Version: 2.1
 Name: vayu_client
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple and easy to use python package for utilizing vayu billing system
 Home-page: https://withvayu.com
 Author: Vayu, Inc.
 Author-email: team@withvayu.com
-License: UNKNOWN
-Description: # Vayu python client
-        
-        ## Prerequisites
-        
-        - Python 3.7 and above
-        - Install the `vayu-client` package (`pip install vayu-client`)
-        
-        ## End-to-End Code Example
-        
-        To illustrate how to use the `Vayu` library for sending events to Vayu's API, here is a complete code snippet. This example combines all the steps detailed in previous sections:
-        
-        ```python
-        from datetime import datetime
-        from vayu import Vayu
-        
-        vayu = Vayu('YOUR_ACCESS_KEY')
-        
-        vayu.send_events([{
-            'name': 'api_call',
-            'timestamp': datetime.now(),
-            'customerAlias': 'customer_12345',
-            'data': {
-                'processing_duration': 124.83,
-                'api_endpoint': '/api/v1/users',
-            },
-            'ref': '4f6cf35x-2c4y-483z-a0a9-158621f77a21'
-        }])
-        ```
-        
-        That's it! This example demonstrates how to send an event using Python and the `Vayu` library.
-        
-        ## Step-by-step Guide
-        
-        ### Step 1: Import Vayu
-        
-        The first step is to import the `Vayu` class from the `Vayu` package.
-        
-        ```python
-        from vayu import Vayu
-        ```
-        
-        ### Step 2: Initialize the Client
-        
-        After importing, create a new `Vayu` instance and pass the api key
-        
-        ```python
-        vayu = Vayu('YOUR_API_KEY')
-        ```
-        
-        ### Step 3: Send Events
-        
-        Finally, you can send events to the Vayu API by using the `send_events` method. The method takes a list of dictionaries, where each dictionary represents a single event. Each event dictionary should contain the following fields:
-        
-        - `name` (string - required): A distinctive label assigned to an event. It serves as a critical identifier for categorizing and pricing events.
-        - `timestamp` (datetime): The exact moment when the event occurs.
-        - `customerAlias` (string): A unique identifier for each customer, which may be pseudonymous or obfuscated.
-        - `data` (object): A schema-less JSON object containing miscellaneous attributes and metrics associated with the event.
-        - `ref` (string, optional): A UUID or other high-entropy string serving as an immutable reference for each event entry.
-        
-        Example:
-        
-        ```python
-        vayu.send_events([{
-            'name': 'api_call',
-            'timestamp': datetime.now(),
-            'customerAlias': 'customer_12345',
-            'data': {
-                'processing_duration': 124.83,
-                'api_endpoint': '/api/v1/users',
-            },
-            'ref': '4f6cf35x-2c4y-483z-a0a9-158621f77a21'
-        }])
-        ```
 Keywords: vayu,billing,events,python,sdk
-Platform: UNKNOWN
 Requires-Python: ==3.7.*
 Description-Content-Type: text/markdown
+
+# Vayu python client
+
+## Prerequisites
+
+- Python 3.7 and above
+- Install the `vayu-client` package (`pip install vayu-client`)
+
+## End-to-End Code Example
+
+To illustrate how to use the `Vayu` library for sending events to Vayu's API, here is a complete code snippet. This example combines all the steps detailed in previous sections:
+
+```python
+from datetime import datetime
+from vayu import Vayu
+
+vayu = Vayu('YOUR_ACCESS_KEY')
+
+vayu.send_events([{
+    'name': 'api_call',
+    'timestamp': datetime.now(),
+    'customerAlias': 'customer_12345',
+    'data': {
+        'processing_duration': 124.83,
+        'api_endpoint': '/api/v1/users',
+    },
+    'ref': '4f6cf35x-2c4y-483z-a0a9-158621f77a21'
+}])
+```
+
+That's it! This example demonstrates how to send an event using Python and the `Vayu` library.
+
+## Step-by-step Guide
+
+### Step 1: Import Vayu
+
+The first step is to import the `Vayu` class from the `Vayu` package.
+
+```python
+from vayu import Vayu
+```
+
+### Step 2: Initialize the Client
+
+After importing, create a new `Vayu` instance and pass the api key
+
+```python
+vayu = Vayu('YOUR_API_KEY')
+```
+
+### Step 3: Send Events
+
+Finally, you can send events to the Vayu API by using the `send_events` method. The method takes a list of dictionaries, where each dictionary represents a single event. Each event dictionary should contain the following fields:
+
+- `name` (string - required): A distinctive label assigned to an event. It serves as a critical identifier for categorizing and pricing events.
+- `timestamp` (datetime): The exact moment when the event occurs.
+- `customerAlias` (string): A unique identifier for each customer, which may be pseudonymous or obfuscated.
+- `data` (object): A schema-less JSON object containing miscellaneous attributes and metrics associated with the event.
+- `ref` (string, optional): A UUID or other high-entropy string serving as an immutable reference for each event entry.
+
+Example:
+
+```python
+vayu.send_events([{
+    'name': 'api_call',
+    'timestamp': datetime.now(),
+    'customerAlias': 'customer_12345',
+    'data': {
+        'processing_duration': 124.83,
+        'api_endpoint': '/api/v1/users',
+    },
+    'ref': '4f6cf35x-2c4y-483z-a0a9-158621f77a21'
+}])
+```
```

### Comparing `vayu_client-1.0.2/openapi_client/api/auth_api.py` & `vayu_client-1.0.3/openapi_client/api/auth_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,30 @@
 # coding: utf-8
 
 """
-    Vayu Events Api
+    Vayu API
 
-    The Vayu Event Ingestion API is a RESTful API that allows you to submit events for processing and storage. The API is secured using the Bearer Authentication scheme with JWT tokens. To obtain a JWT token, please contact Vayu at team@withvayu.com 
+    The Vayu API is a RESTful API that allows you to submit events for processing and storage & manage billing related entities.           The API is secured using the Bearer Authentication scheme with JWT tokens.           To obtain a JWT token, please contact Vayu at team@withvayu.com
 
-    The version of the OpenAPI document: 2.3.1
+    The version of the OpenAPI document: 1.0.0
+    Contact: dev@withvayu.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
-
-import io
 import warnings
-
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
-from typing import Dict, List, Optional, Tuple, Union, Any
-
-try:
-    from typing import Annotated
-except ImportError:
-    from typing_extensions import Annotated
-
-from pydantic import Field
+from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
-from openapi_client.models.login_request import LoginRequest
-from openapi_client.models.login_response import LoginResponse
 
-from openapi_client.api_client import ApiClient
+from openapi_client.models.login_request_schema import LoginRequestSchema
+from openapi_client.models.login_response_schema import LoginResponseSchema
+
+from openapi_client.api_client import ApiClient, RequestSerialized
 from openapi_client.api_response import ApiResponse
 from openapi_client.rest import RESTResponseType
 
 
 class AuthApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
@@ -45,34 +37,34 @@
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
     def login(
         self,
-        login_request: Annotated[LoginRequest, Field(description="The body contains the refresh token required to obtain a new access token.")],
+        login_request_schema: LoginRequestSchema,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> LoginResponse:
+    ) -> LoginResponseSchema:
         """Login by obtaining a new access token
 
-        This endpoint is designed to acquire a temporary access token. Submit the auth token in the request body to obtain a new access token. Use this new token for subsequent API calls. Token is set to expire every hour. 
+        This endpoint is designed to acquire a temporary access token.     Submit the auth token in the request body to obtain a new access token.     Use this new token for subsequent API calls. Token is set to expire every hour.
 
-        :param login_request: The body contains the refresh token required to obtain a new access token. (required)
-        :type login_request: LoginRequest
+        :param login_request_schema: (required)
+        :type login_request_schema: LoginRequestSchema
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -88,24 +80,26 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._login_serialize(
-            login_request=login_request,
+            login_request_schema=login_request_schema,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "LoginResponse",
+            '200': "LoginResponseSchema",
             '400': None,
+            '401': None,
+            '429': None,
             '500': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -114,34 +108,34 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def login_with_http_info(
         self,
-        login_request: Annotated[LoginRequest, Field(description="The body contains the refresh token required to obtain a new access token.")],
+        login_request_schema: LoginRequestSchema,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[LoginResponse]:
+    ) -> ApiResponse[LoginResponseSchema]:
         """Login by obtaining a new access token
 
-        This endpoint is designed to acquire a temporary access token. Submit the auth token in the request body to obtain a new access token. Use this new token for subsequent API calls. Token is set to expire every hour. 
+        This endpoint is designed to acquire a temporary access token.     Submit the auth token in the request body to obtain a new access token.     Use this new token for subsequent API calls. Token is set to expire every hour.
 
-        :param login_request: The body contains the refresh token required to obtain a new access token. (required)
-        :type login_request: LoginRequest
+        :param login_request_schema: (required)
+        :type login_request_schema: LoginRequestSchema
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -157,24 +151,26 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._login_serialize(
-            login_request=login_request,
+            login_request_schema=login_request_schema,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "LoginResponse",
+            '200': "LoginResponseSchema",
             '400': None,
+            '401': None,
+            '429': None,
             '500': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -183,15 +179,15 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def login_without_preload_content(
         self,
-        login_request: Annotated[LoginRequest, Field(description="The body contains the refresh token required to obtain a new access token.")],
+        login_request_schema: LoginRequestSchema,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -199,18 +195,18 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Login by obtaining a new access token
 
-        This endpoint is designed to acquire a temporary access token. Submit the auth token in the request body to obtain a new access token. Use this new token for subsequent API calls. Token is set to expire every hour. 
+        This endpoint is designed to acquire a temporary access token.     Submit the auth token in the request body to obtain a new access token.     Use this new token for subsequent API calls. Token is set to expire every hour.
 
-        :param login_request: The body contains the refresh token required to obtain a new access token. (required)
-        :type login_request: LoginRequest
+        :param login_request_schema: (required)
+        :type login_request_schema: LoginRequestSchema
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -226,61 +222,63 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._login_serialize(
-            login_request=login_request,
+            login_request_schema=login_request_schema,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "LoginResponse",
+            '200': "LoginResponseSchema",
             '400': None,
+            '401': None,
+            '429': None,
             '500': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _login_serialize(
         self,
-        login_request,
+        login_request_schema,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
-    ) -> Tuple:
+    ) -> RequestSerialized:
 
         _host = None
 
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if login_request is not None:
-            _body_params = login_request
+        if login_request_schema is not None:
+            _body_params = login_request_schema
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
```

### Comparing `vayu_client-1.0.2/openapi_client/api_client.py` & `vayu_client-1.0.3/openapi_client/api_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 # coding: utf-8
 
 """
-    Vayu Events Api
+    Vayu API
 
-    The Vayu Event Ingestion API is a RESTful API that allows you to submit events for processing and storage. The API is secured using the Bearer Authentication scheme with JWT tokens. To obtain a JWT token, please contact Vayu at team@withvayu.com 
+    The Vayu API is a RESTful API that allows you to submit events for processing and storage & manage billing related entities.           The API is secured using the Bearer Authentication scheme with JWT tokens.           To obtain a JWT token, please contact Vayu at team@withvayu.com
 
-    The version of the OpenAPI document: 2.3.1
+    The version of the OpenAPI document: 1.0.0
+    Contact: dev@withvayu.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-import atexit
 import datetime
 from dateutil.parser import parse
+from enum import Enum
 import json
 import mimetypes
 import os
 import re
 import tempfile
 
 from urllib.parse import quote
-from typing import Tuple, Optional, List
+from typing import Tuple, Optional, List, Dict, Union
+from pydantic import SecretStr
 
 from openapi_client.configuration import Configuration
-from openapi_client.api_response import ApiResponse
+from openapi_client.api_response import ApiResponse, T as ApiResponseT
 import openapi_client.models
 from openapi_client import rest
 from openapi_client.exceptions import (
     ApiValueError,
     ApiException,
     BadRequestException,
     UnauthorizedException,
     ForbiddenException,
     NotFoundException,
     ServiceException
 )
 
+RequestSerialized = Tuple[str, str, Dict[str, str], Optional[str], List[str]]
 
 class ApiClient:
     """Generic API client for OpenAPI client library builds.
 
     OpenAPI generic API client. This client handles the client-
     server communication, and is invariant across implementations. Specifics of
     the methods and models for each application are generated from the OpenAPI
@@ -143,15 +146,15 @@
         header_params=None,
         body=None,
         post_params=None,
         files=None, auth_settings=None,
         collection_formats=None,
         _host=None,
         _request_auth=None
-    ) -> Tuple:
+    ) -> RequestSerialized:
 
         """Builds the HTTP request params needed by the request.
         :param method: Method to call.
         :param resource_path: Path to method endpoint.
         :param path_params: Path parameters in the url.
         :param query_params: Query parameters in the url.
         :param header_params: Header parameters to be
@@ -202,15 +205,16 @@
         if post_params or files:
             post_params = post_params if post_params else []
             post_params = self.sanitize_for_serialization(post_params)
             post_params = self.parameters_to_tuples(
                 post_params,
                 collection_formats
             )
-            post_params.extend(self.files_parameters(files))
+            if files:
+                post_params.extend(self.files_parameters(files))
 
         # auth setting
         self.update_params_for_auth(
             header_params,
             query_params,
             auth_settings,
             resource_path,
@@ -269,31 +273,31 @@
                 method, url,
                 headers=header_params,
                 body=body, post_params=post_params,
                 _request_timeout=_request_timeout
             )
 
         except ApiException as e:
-            if e.body:
-                e.body = e.body.decode('utf-8')
             raise e
 
         return response_data
 
     def response_deserialize(
         self,
-        response_data: rest.RESTResponse = None,
-        response_types_map=None
-    ) -> ApiResponse:
+        response_data: rest.RESTResponse,
+        response_types_map: Optional[Dict[str, ApiResponseT]]=None
+    ) -> ApiResponse[ApiResponseT]:
         """Deserializes response into an object.
         :param response_data: RESTResponse object to be deserialized.
         :param response_types_map: dict of response types.
         :return: ApiResponse
         """
 
+        msg = "RESTResponse.read() must be called before passing it to response_deserialize()"
+        assert response_data.data is not None, msg
 
         response_type = response_types_map.get(str(response_data.status), None)
         if not response_type and isinstance(response_data.status, int) and 100 <= response_data.status <= 599:
             # if not found, look for '1XX', '2XX', etc.
             response_type = response_types_map.get(str(response_data.status)[0] + "XX", None)
 
         # deserialize response data
@@ -307,15 +311,18 @@
             elif response_type is not None:
                 match = None
                 content_type = response_data.getheader('content-type')
                 if content_type is not None:
                     match = re.search(r"charset=([a-zA-Z\-\d]+)[\s;]?", content_type)
                 encoding = match.group(1) if match else "utf-8"
                 response_text = response_data.data.decode(encoding)
-                return_data = self.deserialize(response_text, response_type)
+                if response_type in ["bytearray", "str"]:
+                    return_data = self.__deserialize_primitive(response_text, response_type)
+                else:
+                    return_data = self.deserialize(response_text, response_type)
         finally:
             if not 200 <= response_data.status <= 299:
                 raise ApiException.from_response(
                     http_resp=response_data,
                     body=response_text,
                     data=return_data,
                 )
@@ -327,26 +334,31 @@
             raw_data = response_data.data
         )
 
     def sanitize_for_serialization(self, obj):
         """Builds a JSON POST object.
 
         If obj is None, return None.
+        If obj is SecretStr, return obj.get_secret_value()
         If obj is str, int, long, float, bool, return directly.
         If obj is datetime.datetime, datetime.date
             convert to string in iso8601 format.
         If obj is list, sanitize each element in the list.
         If obj is dict, return the dict.
         If obj is OpenAPI model, return the properties dict.
 
         :param obj: The data to serialize.
         :return: The serialized form of data.
         """
         if obj is None:
             return None
+        elif isinstance(obj, Enum):
+            return obj.value
+        elif isinstance(obj, SecretStr):
+            return obj.get_secret_value()
         elif isinstance(obj, self.PRIMITIVE_TYPES):
             return obj
         elif isinstance(obj, list):
             return [
                 self.sanitize_for_serialization(sub_obj) for sub_obj in obj
             ]
         elif isinstance(obj, tuple):
@@ -360,15 +372,18 @@
             obj_dict = obj
         else:
             # Convert model obj to dict except
             # attributes `openapi_types`, `attribute_map`
             # and attributes which value is not None.
             # Convert attribute name to json key in
             # model definition for request.
-            obj_dict = obj.to_dict()
+            if hasattr(obj, 'to_dict') and callable(getattr(obj, 'to_dict')):
+                obj_dict = obj.to_dict()
+            else:
+                obj_dict = obj.__dict__
 
         return {
             key: self.sanitize_for_serialization(val)
             for key, val in obj_dict.items()
         }
 
     def deserialize(self, response_text, response_type):
@@ -398,20 +413,24 @@
         :return: object.
         """
         if data is None:
             return None
 
         if isinstance(klass, str):
             if klass.startswith('List['):
-                sub_kls = re.match(r'List\[(.*)]', klass).group(1)
+                m = re.match(r'List\[(.*)]', klass)
+                assert m is not None, "Malformed List type definition"
+                sub_kls = m.group(1)
                 return [self.__deserialize(sub_data, sub_kls)
                         for sub_data in data]
 
             if klass.startswith('Dict['):
-                sub_kls = re.match(r'Dict\[([^,]*), (.*)]', klass).group(2)
+                m = re.match(r'Dict\[([^,]*), (.*)]', klass)
+                assert m is not None, "Malformed Dict type definition"
+                sub_kls = m.group(2)
                 return {k: self.__deserialize(v, sub_kls)
                         for k, v in data.items()}
 
             # convert str to class
             if klass in self.NATIVE_TYPES_MAPPING:
                 klass = self.NATIVE_TYPES_MAPPING[klass]
             else:
@@ -421,25 +440,27 @@
             return self.__deserialize_primitive(data, klass)
         elif klass == object:
             return self.__deserialize_object(data)
         elif klass == datetime.date:
             return self.__deserialize_date(data)
         elif klass == datetime.datetime:
             return self.__deserialize_datetime(data)
+        elif issubclass(klass, Enum):
+            return self.__deserialize_enum(data, klass)
         else:
             return self.__deserialize_model(data, klass)
 
     def parameters_to_tuples(self, params, collection_formats):
         """Get parameters as list of tuples, formatting collections.
 
         :param params: Parameters as dict or list of two-tuples
         :param dict collection_formats: Parameter collection formats
         :return: Parameters as list of tuples, collections formatted
         """
-        new_params = []
+        new_params: List[Tuple[str, str]] = []
         if collection_formats is None:
             collection_formats = {}
         for k, v in params.items() if isinstance(params, dict) else params:
             if k in collection_formats:
                 collection_format = collection_formats[k]
                 if collection_format == 'multi':
                     new_params.extend((k, value) for value in v)
@@ -461,29 +482,29 @@
     def parameters_to_url_query(self, params, collection_formats):
         """Get parameters as list of tuples, formatting collections.
 
         :param params: Parameters as dict or list of two-tuples
         :param dict collection_formats: Parameter collection formats
         :return: URL query string (e.g. a=Hello%20World&b=123)
         """
-        new_params = []
+        new_params: List[Tuple[str, str]] = []
         if collection_formats is None:
             collection_formats = {}
         for k, v in params.items() if isinstance(params, dict) else params:
             if isinstance(v, bool):
                 v = str(v).lower()
             if isinstance(v, (int, float)):
                 v = str(v)
             if isinstance(v, dict):
                 v = json.dumps(v)
 
             if k in collection_formats:
                 collection_format = collection_formats[k]
                 if collection_format == 'multi':
-                    new_params.extend((k, value) for value in v)
+                    new_params.extend((k, str(value)) for value in v)
                 else:
                     if collection_format == 'ssv':
                         delimiter = ' '
                     elif collection_format == 'tsv':
                         delimiter = '\t'
                     elif collection_format == 'pipes':
                         delimiter = '|'
@@ -491,41 +512,40 @@
                         delimiter = ','
                     new_params.append(
                         (k, delimiter.join(quote(str(value)) for value in v))
                     )
             else:
                 new_params.append((k, quote(str(v))))
 
-        return "&".join(["=".join(item) for item in new_params])
+        return "&".join(["=".join(map(str, item)) for item in new_params])
 
-    def files_parameters(self, files=None):
+    def files_parameters(self, files: Dict[str, Union[str, bytes]]):
         """Builds form parameters.
 
         :param files: File parameters.
         :return: Form parameters with files.
         """
         params = []
-
-        if files:
-            for k, v in files.items():
-                if not v:
-                    continue
-                file_names = v if type(v) is list else [v]
-                for n in file_names:
-                    with open(n, 'rb') as f:
-                        filename = os.path.basename(f.name)
-                        filedata = f.read()
-                        mimetype = (
-                            mimetypes.guess_type(filename)[0]
-                            or 'application/octet-stream'
-                        )
-                        params.append(
-                            tuple([k, tuple([filename, filedata, mimetype])])
-                        )
-
+        for k, v in files.items():
+            if isinstance(v, str):
+                with open(v, 'rb') as f:
+                    filename = os.path.basename(f.name)
+                    filedata = f.read()
+            elif isinstance(v, bytes):
+                filename = k
+                filedata = v
+            else:
+                raise ValueError("Unsupported file value")
+            mimetype = (
+                mimetypes.guess_type(filename)[0]
+                or 'application/octet-stream'
+            )
+            params.append(
+                tuple([k, tuple([filename, filedata, mimetype])])
+            )
         return params
 
     def select_header_accept(self, accepts: List[str]) -> Optional[str]:
         """Returns `Accept` based on an array of accepts provided.
 
         :param accepts: List of headers.
         :return: Accept (e.g. application/json).
@@ -646,18 +666,20 @@
         """
         fd, path = tempfile.mkstemp(dir=self.configuration.temp_folder_path)
         os.close(fd)
         os.remove(path)
 
         content_disposition = response.getheader("Content-Disposition")
         if content_disposition:
-            filename = re.search(
+            m = re.search(
                 r'filename=[\'"]?([^\'"\s]+)[\'"]?',
                 content_disposition
-            ).group(1)
+            )
+            assert m is not None, "Unexpected 'content-disposition' header value"
+            filename = m.group(1)
             path = os.path.join(os.path.dirname(path), filename)
 
         with open(path, "wb") as f:
             f.write(response.data)
 
         return path
 
@@ -716,14 +738,32 @@
                 status=0,
                 reason=(
                     "Failed to parse `{0}` as datetime object"
                     .format(string)
                 )
             )
 
+    def __deserialize_enum(self, data, klass):
+        """Deserializes primitive type to enum.
+
+        :param data: primitive type.
+        :param klass: class literal.
+        :return: enum value.
+        """
+        try:
+            return klass(data)
+        except ValueError:
+            raise rest.ApiException(
+                status=0,
+                reason=(
+                    "Failed to parse `{0}` as `{1}`"
+                    .format(data, klass)
+                )
+            )
+
     def __deserialize_model(self, data, klass):
         """Deserializes list or dict to model.
 
         :param data: dict, list.
         :param klass: class literal.
         :return: model object.
         """
```

### Comparing `vayu_client-1.0.2/openapi_client/configuration.py` & `vayu_client-1.0.3/openapi_client/configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # coding: utf-8
 
 """
-    Vayu Events Api
+    Vayu API
 
-    The Vayu Event Ingestion API is a RESTful API that allows you to submit events for processing and storage. The API is secured using the Bearer Authentication scheme with JWT tokens. To obtain a JWT token, please contact Vayu at team@withvayu.com 
+    The Vayu API is a RESTful API that allows you to submit events for processing and storage & manage billing related entities.           The API is secured using the Bearer Authentication scheme with JWT tokens.           To obtain a JWT token, please contact Vayu at team@withvayu.com
 
-    The version of the OpenAPI document: 2.3.1
+    The version of the OpenAPI document: 1.0.0
+    Contact: dev@withvayu.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import copy
 import logging
+from logging import FileHandler
 import multiprocessing
 import sys
+from typing import Optional
 import urllib3
 
 import http.client as httplib
 
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
@@ -64,15 +67,15 @@
                  access_token=None,
                  server_index=None, server_variables=None,
                  server_operation_index=None, server_operation_variables=None,
                  ssl_ca_cert=None,
                  ) -> None:
         """Constructor
         """
-        self._base_path = "https://events.withvayu.com" if host is None else host
+        self._base_path = "https://connect.withvayu.com" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
         """Default server index
         """
         self.server_variables = server_variables or {}
@@ -112,15 +115,15 @@
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
         """
         self.logger_stream_handler = None
         """Log stream handler
         """
-        self.logger_file_handler = None
+        self.logger_file_handler: Optional[FileHandler] = None
         """Log file handler
         """
         self.logger_file = None
         """Debug file location
         """
         self.debug = False
         """Debug switch
@@ -152,15 +155,15 @@
         """urllib3 connection pool's maximum number of connections saved
            per pool. urllib3 uses 1 connection as default value, but this is
            not the best value when you are making a lot of possibly parallel
            requests to the same host, which is often the case here.
            cpu_count * 5 is used as default value to increase performance.
         """
 
-        self.proxy = None
+        self.proxy: Optional[str] = None
         """Proxy URL
         """
         self.proxy_headers = None
         """Proxy headers
         """
         self.safe_chars_for_path_param = ''
         """Safe chars for path_param
@@ -171,15 +174,15 @@
         # Enable client side validation
         self.client_side_validation = True
 
         self.socket_options = None
         """Options to pass down to the underlying urllib3 socket
         """
 
-        self.datetime_format = "%Y-%m-%dT%H:%M:%S%z"
+        self.datetime_format = "%Y-%m-%dT%H:%M:%S.%f%z"
         """datetime format
         """
 
         self.date_format = "%Y-%m-%d"
         """date format
         """
 
@@ -372,31 +375,31 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.3.1\n"\
+               "Version of the API: 1.0.0\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
         return [
             {
-                'url': "https://events.withvayu.com",
+                'url': "https://connect.withvayu.com",
                 'description': "Production server",
             },
             {
-                'url': "http://localhost:3000",
-                'description': "Local server",
+                'url': "https://staging-connect.withvayu.com",
+                'description': "Sandbox server",
             }
         ]
 
     def get_host_from_settings(self, index, variables=None, servers=None):
         """Gets host URL based on the index and variables
         :param index: array index of the host settings
         :param variables: hash of variable and the corresponding value
```

### Comparing `vayu_client-1.0.2/openapi_client/exceptions.py` & `vayu_client-1.0.3/openapi_client/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # coding: utf-8
 
 """
-    Vayu Events Api
+    Vayu API
 
-    The Vayu Event Ingestion API is a RESTful API that allows you to submit events for processing and storage. The API is secured using the Bearer Authentication scheme with JWT tokens. To obtain a JWT token, please contact Vayu at team@withvayu.com 
+    The Vayu API is a RESTful API that allows you to submit events for processing and storage & manage billing related entities.           The API is secured using the Bearer Authentication scheme with JWT tokens.           To obtain a JWT token, please contact Vayu at team@withvayu.com
 
-    The version of the OpenAPI document: 2.3.1
+    The version of the OpenAPI document: 1.0.0
+    Contact: dev@withvayu.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from typing import Any, Optional
-
 from typing_extensions import Self
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
 
 
 class ApiTypeError(OpenApiException, TypeError):
```

### Comparing `vayu_client-1.0.2/openapi_client/models/event_input.py` & `vayu_client-1.0.3/openapi_client/models/event.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,97 +1,103 @@
 # coding: utf-8
 
 """
-    Vayu Events Api
+    Vayu API
 
-    The Vayu Event Ingestion API is a RESTful API that allows you to submit events for processing and storage. The API is secured using the Bearer Authentication scheme with JWT tokens. To obtain a JWT token, please contact Vayu at team@withvayu.com 
+    The Vayu API is a RESTful API that allows you to submit events for processing and storage & manage billing related entities.           The API is secured using the Bearer Authentication scheme with JWT tokens.           To obtain a JWT token, please contact Vayu at team@withvayu.com
 
-    The version of the OpenAPI document: 2.3.1
+    The version of the OpenAPI document: 1.0.0
+    Contact: dev@withvayu.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictStr
-from pydantic import Field
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
+from typing_extensions import Annotated
+from typing import Optional, Set
+from typing_extensions import Self
 
-class EventInput(BaseModel):
+class Event(BaseModel):
     """
-    EventInput
+    Event
     """ # noqa: E501
     name: StrictStr = Field(description="The distinctive label assigned to an event, serving as a critical identifier for categorizing and pricing events within the system's backend infrastructure.")
-    timestamp: datetime = Field(description="The temporal marker denoting the exact moment of event occurrence.")
-    customer_alias: StrictStr = Field(description="A pseudonymous or otherwise obfuscated identifier uniquely assigned to each customer.", alias="customerAlias")
+    timestamp: datetime = Field(description="The temporal marker denoting the exact moment of event occurrence. The timestamp is formatted as an ISO 8601 string and is expressed in Coordinated Universal Time (UTC). i.e. YYYY-MM-DDTHH:MM:SS.SSSZ")
+    customer_alias: Annotated[str, Field(min_length=1, strict=True)] = Field(description="A pseudonymous or otherwise obfuscated identifier uniquely assigned to each customer.", alias="customerAlias")
+    ref: StrictStr = Field(description="A universally unique identifier (UUID) or other form of high-entropy string serving as an immutable reference for each event entry.")
     data: Optional[Dict[str, Any]] = Field(default=None, description="A schema-less JSON object encapsulating miscellaneous attributes and metrics associated with the event.")
-    ref: Optional[StrictStr] = Field(default=None, description="A universally unique identifier (UUID) or other form of high-entropy string serving as an immutable reference for each event entry.")
-    __properties: ClassVar[List[str]] = ["name", "timestamp", "customerAlias", "data", "ref"]
+    __properties: ClassVar[List[str]] = ["name", "timestamp", "customerAlias", "ref", "data"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of EventInput from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of Event from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
+        excluded_fields: Set[str] = set([
+        ])
+
         _dict = self.model_dump(
             by_alias=True,
-            exclude={
-            },
+            exclude=excluded_fields,
             exclude_none=True,
         )
+        # set to None if data (nullable) is None
+        # and model_fields_set contains the field
+        if self.data is None and "data" in self.model_fields_set:
+            _dict['data'] = None
+
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of EventInput from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of Event from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "name": obj.get("name"),
             "timestamp": obj.get("timestamp"),
             "customerAlias": obj.get("customerAlias"),
-            "data": obj.get("data"),
-            "ref": obj.get("ref")
+            "ref": obj.get("ref"),
+            "data": obj.get("data")
         })
         return _obj
```

### Comparing `vayu_client-1.0.2/openapi_client/models/login_request.py` & `vayu_client-1.0.3/openapi_client/models/login_response_schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,89 +1,88 @@
 # coding: utf-8
 
 """
-    Vayu Events Api
+    Vayu API
 
-    The Vayu Event Ingestion API is a RESTful API that allows you to submit events for processing and storage. The API is secured using the Bearer Authentication scheme with JWT tokens. To obtain a JWT token, please contact Vayu at team@withvayu.com 
+    The Vayu API is a RESTful API that allows you to submit events for processing and storage & manage billing related entities.           The API is secured using the Bearer Authentication scheme with JWT tokens.           To obtain a JWT token, please contact Vayu at team@withvayu.com
 
-    The version of the OpenAPI document: 2.3.1
+    The version of the OpenAPI document: 1.0.0
+    Contact: dev@withvayu.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List
-from pydantic import BaseModel, StrictStr
-from pydantic import Field
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
+from typing import Optional, Set
+from typing_extensions import Self
 
-class LoginRequest(BaseModel):
+class LoginResponseSchema(BaseModel):
     """
-    LoginRequest
+    LoginResponseSchema
     """ # noqa: E501
-    refresh_token: StrictStr = Field(description="The refresh token issued previously during the authentication process. It is required to obtain a new access token.", alias="refreshToken")
-    __properties: ClassVar[List[str]] = ["refreshToken"]
+    access_token: StrictStr = Field(description="The new access token to be used for subsequent API calls. It is set to expire every hour.", alias="accessToken")
+    __properties: ClassVar[List[str]] = ["accessToken"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of LoginRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of LoginResponseSchema from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
+        excluded_fields: Set[str] = set([
+        ])
+
         _dict = self.model_dump(
             by_alias=True,
-            exclude={
-            },
+            exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of LoginRequest from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of LoginResponseSchema from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "refreshToken": obj.get("refreshToken")
+            "accessToken": obj.get("accessToken")
         })
         return _obj
```

### Comparing `vayu_client-1.0.2/openapi_client/models/login_response.py` & `vayu_client-1.0.3/openapi_client/models/delete_plan_response_schema.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,89 +1,92 @@
 # coding: utf-8
 
 """
-    Vayu Events Api
+    Vayu API
 
-    The Vayu Event Ingestion API is a RESTful API that allows you to submit events for processing and storage. The API is secured using the Bearer Authentication scheme with JWT tokens. To obtain a JWT token, please contact Vayu at team@withvayu.com 
+    The Vayu API is a RESTful API that allows you to submit events for processing and storage & manage billing related entities.           The API is secured using the Bearer Authentication scheme with JWT tokens.           To obtain a JWT token, please contact Vayu at team@withvayu.com
 
-    The version of the OpenAPI document: 2.3.1
+    The version of the OpenAPI document: 1.0.0
+    Contact: dev@withvayu.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
+from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
-from pydantic import BaseModel, StrictStr
-from pydantic import Field
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
+from openapi_client.models.get_plan_response_schema_plan import GetPlanResponseSchemaPlan
+from typing import Optional, Set
+from typing_extensions import Self
 
-class LoginResponse(BaseModel):
+class DeletePlanResponseSchema(BaseModel):
     """
-    LoginResponse
+    DeletePlanResponseSchema
     """ # noqa: E501
-    token: StrictStr = Field(description="The new access token")
-    __properties: ClassVar[List[str]] = ["token"]
+    plan: GetPlanResponseSchemaPlan
+    __properties: ClassVar[List[str]] = ["plan"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of LoginResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of DeletePlanResponseSchema from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
+        excluded_fields: Set[str] = set([
+        ])
+
         _dict = self.model_dump(
             by_alias=True,
-            exclude={
-            },
+            exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of plan
+        if self.plan:
+            _dict['plan'] = self.plan.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of LoginResponse from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of DeletePlanResponseSchema from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "token": obj.get("token")
+            "plan": GetPlanResponseSchemaPlan.from_dict(obj["plan"]) if obj.get("plan") is not None else None
         })
         return _obj
```

### Comparing `vayu_client-1.0.2/openapi_client/models/send_events_request.py` & `vayu_client-1.0.3/openapi_client/models/send_events_request_schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,98 +1,97 @@
 # coding: utf-8
 
 """
-    Vayu Events Api
+    Vayu API
 
-    The Vayu Event Ingestion API is a RESTful API that allows you to submit events for processing and storage. The API is secured using the Bearer Authentication scheme with JWT tokens. To obtain a JWT token, please contact Vayu at team@withvayu.com 
+    The Vayu API is a RESTful API that allows you to submit events for processing and storage & manage billing related entities.           The API is secured using the Bearer Authentication scheme with JWT tokens.           To obtain a JWT token, please contact Vayu at team@withvayu.com
 
-    The version of the OpenAPI document: 2.3.1
+    The version of the OpenAPI document: 1.0.0
+    Contact: dev@withvayu.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
+from pydantic import BaseModel, ConfigDict, Field
 from typing import Any, ClassVar, Dict, List
-from pydantic import BaseModel
-from pydantic import Field
 from typing_extensions import Annotated
-from openapi_client.models.event_input import EventInput
-try:
-    from typing import Self
-except ImportError:
-    from typing_extensions import Self
+from openapi_client.models.event import Event
+from typing import Optional, Set
+from typing_extensions import Self
 
-class SendEventsRequest(BaseModel):
+class SendEventsRequestSchema(BaseModel):
     """
-    SendEventsRequest
+    SendEventsRequestSchema
     """ # noqa: E501
-    events: Annotated[List[EventInput], Field(min_length=1, max_length=1000)]
+    events: Annotated[List[Event], Field(min_length=1, max_length=1000)]
     __properties: ClassVar[List[str]] = ["events"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Self:
-        """Create an instance of SendEventsRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of SendEventsRequestSchema from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         """
+        excluded_fields: Set[str] = set([
+        ])
+
         _dict = self.model_dump(
             by_alias=True,
-            exclude={
-            },
+            exclude=excluded_fields,
             exclude_none=True,
         )
         # override the default output from pydantic by calling `to_dict()` of each item in events (list)
         _items = []
         if self.events:
             for _item in self.events:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['events'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of SendEventsRequest from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of SendEventsRequestSchema from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "events": [EventInput.from_dict(_item) for _item in obj.get("events")] if obj.get("events") is not None else None
+            "events": [Event.from_dict(_item) for _item in obj["events"]] if obj.get("events") is not None else None
         })
         return _obj
```

### Comparing `vayu_client-1.0.2/openapi_client/rest.py` & `vayu_client-1.0.3/openapi_client/rest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # coding: utf-8
 
 """
-    Vayu Events Api
+    Vayu API
 
-    The Vayu Event Ingestion API is a RESTful API that allows you to submit events for processing and storage. The API is secured using the Bearer Authentication scheme with JWT tokens. To obtain a JWT token, please contact Vayu at team@withvayu.com 
+    The Vayu API is a RESTful API that allows you to submit events for processing and storage & manage billing related entities.           The API is secured using the Bearer Authentication scheme with JWT tokens.           To obtain a JWT token, please contact Vayu at team@withvayu.com
 
-    The version of the OpenAPI document: 2.3.1
+    The version of the OpenAPI document: 1.0.0
+    Contact: dev@withvayu.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
@@ -67,64 +68,53 @@
 
         # cert_reqs
         if configuration.verify_ssl:
             cert_reqs = ssl.CERT_REQUIRED
         else:
             cert_reqs = ssl.CERT_NONE
 
-        addition_pool_args = {}
+        pool_args = {
+            "cert_reqs": cert_reqs,
+            "ca_certs": configuration.ssl_ca_cert,
+            "cert_file": configuration.cert_file,
+            "key_file": configuration.key_file,
+        }
         if configuration.assert_hostname is not None:
-            addition_pool_args['assert_hostname'] = (
+            pool_args['assert_hostname'] = (
                 configuration.assert_hostname
             )
 
         if configuration.retries is not None:
-            addition_pool_args['retries'] = configuration.retries
+            pool_args['retries'] = configuration.retries
 
         if configuration.tls_server_name:
-            addition_pool_args['server_hostname'] = configuration.tls_server_name
+            pool_args['server_hostname'] = configuration.tls_server_name
 
 
         if configuration.socket_options is not None:
-            addition_pool_args['socket_options'] = configuration.socket_options
+            pool_args['socket_options'] = configuration.socket_options
 
         if configuration.connection_pool_maxsize is not None:
-            addition_pool_args['maxsize'] = configuration.connection_pool_maxsize
+            pool_args['maxsize'] = configuration.connection_pool_maxsize
 
         # https pool manager
+        self.pool_manager: urllib3.PoolManager
+
         if configuration.proxy:
             if is_socks_proxy_url(configuration.proxy):
                 from urllib3.contrib.socks import SOCKSProxyManager
-                self.pool_manager = SOCKSProxyManager(
-                        cert_reqs=cert_reqs,
-                        ca_certs=configuration.ssl_ca_cert,
-                        cert_file=configuration.cert_file,
-                        key_file=configuration.key_file,
-                        proxy_url=configuration.proxy,
-                        headers=configuration.proxy_headers,
-                        **addition_pool_args
-                    )
+                pool_args["proxy_url"] = configuration.proxy
+                pool_args["headers"] = configuration.proxy_headers
+                self.pool_manager = SOCKSProxyManager(**pool_args)
             else:
-                self.pool_manager = urllib3.ProxyManager(
-                    cert_reqs=cert_reqs,
-                    ca_certs=configuration.ssl_ca_cert,
-                    cert_file=configuration.cert_file,
-                    key_file=configuration.key_file,
-                    proxy_url=configuration.proxy,
-                    proxy_headers=configuration.proxy_headers,
-                    **addition_pool_args
-                )
+                pool_args["proxy_url"] = configuration.proxy
+                pool_args["proxy_headers"] = configuration.proxy_headers
+                self.pool_manager = urllib3.ProxyManager(**pool_args)
         else:
-            self.pool_manager = urllib3.PoolManager(
-                cert_reqs=cert_reqs,
-                ca_certs=configuration.ssl_ca_cert,
-                cert_file=configuration.cert_file,
-                key_file=configuration.key_file,
-                **addition_pool_args
-            )
+            self.pool_manager = urllib3.PoolManager(**pool_args)
 
     def request(
         self,
         method,
         url,
         headers=None,
         body=None,
@@ -209,32 +199,33 @@
                         preload_content=False
                     )
                 elif content_type == 'multipart/form-data':
                     # must del headers['Content-Type'], or the correct
                     # Content-Type which generated by urllib3 will be
                     # overwritten.
                     del headers['Content-Type']
+                    # Ensures that dict objects are serialized
+                    post_params = [(a, json.dumps(b)) if isinstance(b, dict) else (a,b) for a, b in post_params]
                     r = self.pool_manager.request(
                         method,
                         url,
                         fields=post_params,
                         encode_multipart=True,
                         timeout=timeout,
                         headers=headers,
                         preload_content=False
                     )
                 # Pass a `string` parameter directly in the body to support
-                # other content types than Json when `body` argument is
-                # provided in serialized form
+                # other content types than JSON when `body` argument is
+                # provided in serialized form.
                 elif isinstance(body, str) or isinstance(body, bytes):
-                    request_body = body
                     r = self.pool_manager.request(
                         method,
                         url,
-                        body=request_body,
+                        body=body,
                         timeout=timeout,
                         headers=headers,
                         preload_content=False
                     )
                 elif headers['Content-Type'] == 'text/plain' and isinstance(body, bool):
                     request_body = "true" if body else "false"
                     r = self.pool_manager.request(
```

### Comparing `vayu_client-1.0.2/vayu.py` & `vayu_client-1.0.3/vayu.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,68 @@
-from typing import List
-
-from openapi_client.api import auth_api, events_api
+from entity_clients.events_client import EventsClient
+from openapi_client.api.auth_api import AuthApi
 from openapi_client.api_client import ApiClient
 from openapi_client.configuration import Configuration
-from openapi_client.models import EventInput
-from openapi_client.models.login_request import LoginRequest
-from openapi_client.models.send_events_request import SendEventsRequest
+from openapi_client.models.aggregation_method import AggregationMethod
+from openapi_client.models.event import Event
+from openapi_client.models.login_request_schema import LoginRequestSchema
 from vayu_consts import VAYU_URL
 
+from .entity_clients.contracts_client import ContractsClient
+from .entity_clients.customers_client import CustomersClient
+from .entity_clients.invoices_client import InvoicesClient
+from .entity_clients.meters_client import MetersClient
+from .entity_clients.plans_client import PlansClient
+
 
 class Vayu:
-    def __init__(self, api_key: str):
-        self.__login(api_key)
-    
-    def send_events(self, events: List[EventInput]):
-        """
-        Send events to Weft
+    __api_key: str = None
+
+    @property
+    def __private_api_client(self):
+        configuration = Configuration(host=VAYU_URL, api_key=self.__api_key)
+        
+        return ApiClient(configuration)
+
+    @property
+    def __public_api_client(self):
+        configuration = Configuration(host=VAYU_URL)
+        
+        return ApiClient(configuration)
 
-        Args:
-            events ([EventInput]): events to send
-        """
+    @property
+    def customers(self)->CustomersClient:
+        return CustomersClient(self.__private_api_client)
 
-        events_api = self.__build_events_api(VAYU_URL)
-        send_events_request = SendEventsRequest(events=events)
+    @property
+    def plans(self)->PlansClient:
+        return PlansClient(self.__private_api_client)
 
-        return events_api.send_events(send_events_request)
 
-    def __login(self, api_key: str):
-        auth_api = self.__build_auth_api(VAYU_URL)
-        refresh_token_input = LoginRequest(refreshToken=api_key)
+    @property
+    def contracts(self)->ContractsClient:
+        return ContractsClient(self.__private_api_client)
 
-        refresh_response = auth_api.login(refresh_token_input)
 
-        self.__access_token = refresh_response.token
+    @property
+    def meters(self)->MetersClient:
+        return MetersClient(self.__private_api_client)
+
+
+    @property
+    def invoices(self)->InvoicesClient:
+        return InvoicesClient(self.__private_api_client)
+
+    @property
+    def events(self)->EventsClient:
+        return EventsClient(self.__private_api_client)
+
+    def __init__(self, api_key: str):
+        self.__login(api_key)
     
-    def __build_auth_api(self, host: str):
-        configuration = Configuration(host)
-        client = ApiClient(configuration)
-        
-        return auth_api.AuthApi(client)
 
-    def __build_events_api(self, host: str):
-        configuration = Configuration(host=host)
-        client = ApiClient(configuration, header_name='Authorization', header_value=f'Bearer {self.__access_token}')
-        
-        return events_api.EventsApi(client)
+    def __login(self, refresh_token: str):
+        auth_api = AuthApi(self.__public_api_client)
+        login_request = LoginRequestSchema(refresh_token)
+        refresh_response = auth_api.login(login_request)
+
+        self.__api_key = refresh_response.access_token
```

### Comparing `vayu_client-1.0.2/vayu_client.egg-info/PKG-INFO` & `vayu_client-1.0.3/vayu_client.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,85 +1,84 @@
 Metadata-Version: 2.1
 Name: vayu-client
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple and easy to use python package for utilizing vayu billing system
 Home-page: https://withvayu.com
 Author: Vayu, Inc.
 Author-email: team@withvayu.com
-License: UNKNOWN
-Description: # Vayu python client
-        
-        ## Prerequisites
-        
-        - Python 3.7 and above
-        - Install the `vayu-client` package (`pip install vayu-client`)
-        
-        ## End-to-End Code Example
-        
-        To illustrate how to use the `Vayu` library for sending events to Vayu's API, here is a complete code snippet. This example combines all the steps detailed in previous sections:
-        
-        ```python
-        from datetime import datetime
-        from vayu import Vayu
-        
-        vayu = Vayu('YOUR_ACCESS_KEY')
-        
-        vayu.send_events([{
-            'name': 'api_call',
-            'timestamp': datetime.now(),
-            'customerAlias': 'customer_12345',
-            'data': {
-                'processing_duration': 124.83,
-                'api_endpoint': '/api/v1/users',
-            },
-            'ref': '4f6cf35x-2c4y-483z-a0a9-158621f77a21'
-        }])
-        ```
-        
-        That's it! This example demonstrates how to send an event using Python and the `Vayu` library.
-        
-        ## Step-by-step Guide
-        
-        ### Step 1: Import Vayu
-        
-        The first step is to import the `Vayu` class from the `Vayu` package.
-        
-        ```python
-        from vayu import Vayu
-        ```
-        
-        ### Step 2: Initialize the Client
-        
-        After importing, create a new `Vayu` instance and pass the api key
-        
-        ```python
-        vayu = Vayu('YOUR_API_KEY')
-        ```
-        
-        ### Step 3: Send Events
-        
-        Finally, you can send events to the Vayu API by using the `send_events` method. The method takes a list of dictionaries, where each dictionary represents a single event. Each event dictionary should contain the following fields:
-        
-        - `name` (string - required): A distinctive label assigned to an event. It serves as a critical identifier for categorizing and pricing events.
-        - `timestamp` (datetime): The exact moment when the event occurs.
-        - `customerAlias` (string): A unique identifier for each customer, which may be pseudonymous or obfuscated.
-        - `data` (object): A schema-less JSON object containing miscellaneous attributes and metrics associated with the event.
-        - `ref` (string, optional): A UUID or other high-entropy string serving as an immutable reference for each event entry.
-        
-        Example:
-        
-        ```python
-        vayu.send_events([{
-            'name': 'api_call',
-            'timestamp': datetime.now(),
-            'customerAlias': 'customer_12345',
-            'data': {
-                'processing_duration': 124.83,
-                'api_endpoint': '/api/v1/users',
-            },
-            'ref': '4f6cf35x-2c4y-483z-a0a9-158621f77a21'
-        }])
-        ```
 Keywords: vayu,billing,events,python,sdk
-Platform: UNKNOWN
 Requires-Python: ==3.7.*
 Description-Content-Type: text/markdown
+
+# Vayu python client
+
+## Prerequisites
+
+- Python 3.7 and above
+- Install the `vayu-client` package (`pip install vayu-client`)
+
+## End-to-End Code Example
+
+To illustrate how to use the `Vayu` library for sending events to Vayu's API, here is a complete code snippet. This example combines all the steps detailed in previous sections:
+
+```python
+from datetime import datetime
+from vayu import Vayu
+
+vayu = Vayu('YOUR_ACCESS_KEY')
+
+vayu.send_events([{
+    'name': 'api_call',
+    'timestamp': datetime.now(),
+    'customerAlias': 'customer_12345',
+    'data': {
+        'processing_duration': 124.83,
+        'api_endpoint': '/api/v1/users',
+    },
+    'ref': '4f6cf35x-2c4y-483z-a0a9-158621f77a21'
+}])
+```
+
+That's it! This example demonstrates how to send an event using Python and the `Vayu` library.
+
+## Step-by-step Guide
+
+### Step 1: Import Vayu
+
+The first step is to import the `Vayu` class from the `Vayu` package.
+
+```python
+from vayu import Vayu
+```
+
+### Step 2: Initialize the Client
+
+After importing, create a new `Vayu` instance and pass the api key
+
+```python
+vayu = Vayu('YOUR_API_KEY')
+```
+
+### Step 3: Send Events
+
+Finally, you can send events to the Vayu API by using the `send_events` method. The method takes a list of dictionaries, where each dictionary represents a single event. Each event dictionary should contain the following fields:
+
+- `name` (string - required): A distinctive label assigned to an event. It serves as a critical identifier for categorizing and pricing events.
+- `timestamp` (datetime): The exact moment when the event occurs.
+- `customerAlias` (string): A unique identifier for each customer, which may be pseudonymous or obfuscated.
+- `data` (object): A schema-less JSON object containing miscellaneous attributes and metrics associated with the event.
+- `ref` (string, optional): A UUID or other high-entropy string serving as an immutable reference for each event entry.
+
+Example:
+
+```python
+vayu.send_events([{
+    'name': 'api_call',
+    'timestamp': datetime.now(),
+    'customerAlias': 'customer_12345',
+    'data': {
+        'processing_duration': 124.83,
+        'api_endpoint': '/api/v1/users',
+    },
+    'ref': '4f6cf35x-2c4y-483z-a0a9-158621f77a21'
+}])
+```
```

