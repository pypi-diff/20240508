# Comparing `tmp/vayu_client-1.0.3.tar.gz` & `tmp/vayu_client-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vayu_client-1.0.3.tar", last modified: Wed May  8 15:19:37 2024, max compression
+gzip compressed data, was "vayu_client-1.0.4.tar", last modified: Wed May  8 15:27:34 2024, max compression
```

## Comparing `vayu_client-1.0.3.tar` & `vayu_client-1.0.4.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-08 15:19:37.450335 vayu_client-1.0.3/
--rw-r--r--   0 shaigross   (501) staff       (20)     2539 2024-05-08 15:19:37.450404 vayu_client-1.0.3/PKG-INFO
--rw-r--r--   0 shaigross   (501) staff       (20)      481 2024-05-08 15:19:35.000000 vayu_client-1.0.3/README.md
-drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-08 15:19:37.430451 vayu_client-1.0.3/entity_clients/
--rw-r--r--   0 shaigross   (501) staff       (20)       46 2024-05-08 13:47:16.000000 vayu_client-1.0.3/entity_clients/__init__.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1178 2024-05-08 14:04:33.000000 vayu_client-1.0.3/entity_clients/contracts_client.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1328 2024-05-08 13:49:15.000000 vayu_client-1.0.3/entity_clients/customers_client.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1413 2024-05-08 14:59:08.000000 vayu_client-1.0.3/entity_clients/events_client.py
--rw-r--r--   0 shaigross   (501) staff       (20)      517 2024-05-08 14:06:03.000000 vayu_client-1.0.3/entity_clients/invoices_client.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1840 2024-05-08 14:06:04.000000 vayu_client-1.0.3/entity_clients/meters_client.py
--rw-r--r--   0 shaigross   (501) staff       (20)      561 2024-05-08 13:49:18.000000 vayu_client-1.0.3/entity_clients/plans_client.py
-drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-08 15:19:37.432188 vayu_client-1.0.3/openapi_client/
--rw-r--r--   0 shaigross   (501) staff       (20)     6948 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/__init__.py
-drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-08 15:19:37.436323 vayu_client-1.0.3/openapi_client/api/
--rw-r--r--   0 shaigross   (501) staff       (20)      422 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/api/__init__.py
--rw-r--r--   0 shaigross   (501) staff       (20)    12591 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/api/auth_api.py
--rw-r--r--   0 shaigross   (501) staff       (20)    43742 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/api/contracts_api.py
--rw-r--r--   0 shaigross   (501) staff       (20)    55565 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/api/customers_api.py
--rw-r--r--   0 shaigross   (501) staff       (20)    61236 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/api/events_api.py
--rw-r--r--   0 shaigross   (501) staff       (20)    22281 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/api/invoices_api.py
--rw-r--r--   0 shaigross   (501) staff       (20)    43924 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/api/meters_api.py
--rw-r--r--   0 shaigross   (501) staff       (20)    32198 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/api/plans_api.py
--rw-r--r--   0 shaigross   (501) staff       (20)    26550 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/api_client.py
--rw-r--r--   0 shaigross   (501) staff       (20)      652 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/api_response.py
--rw-r--r--   0 shaigross   (501) staff       (20)    15152 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/configuration.py
--rw-r--r--   0 shaigross   (501) staff       (20)     6180 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/exceptions.py
-drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-08 15:19:37.449683 vayu_client-1.0.3/openapi_client/models/
--rw-r--r--   0 shaigross   (501) staff       (20)     6030 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/__init__.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3340 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/aggregation_method.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1161 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/aggregation_operator.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1052 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/billing_interval.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3214 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/condition.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4112 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/create_contract_request_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3126 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/create_contract_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3084 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/create_customer_request_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/create_customer_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3889 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/create_customer_response_schema_customer.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3034 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/criterion.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1202 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/criterion_operator.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3126 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/delete_contract_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/delete_customer_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3134 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/delete_event_by_ref_id_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4983 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/delete_event_by_ref_id_response_schema_event.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3063 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/delete_meter_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3042 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/delete_plan_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4127 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/event.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3243 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/events_dry_run_request_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4380 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/events_dry_run_response_schema_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3921 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/events_dry_run_response_schema_inner_event.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4556 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3461 2024-05-08 11:11:33.000000 vayu_client-1.0.3/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner_aggregation_method.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3477 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/filter.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3114 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_contract_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4858 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_contract_response_schema_contract.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3126 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_customer_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3110 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_event_by_ref_id_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4861 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_event_by_ref_id_response_schema_event.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3093 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_invoice_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     6159 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_invoice_response_schema_invoice.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3515 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_invoice_response_schema_invoice_line_items_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3051 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_meter_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4720 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_meter_response_schema_meter.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3030 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_plan_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4195 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/get_plan_response_schema_plan.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3737 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/list_contracts_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4766 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/list_contracts_response_schema_contracts_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3737 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/list_customers_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3785 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/list_customers_response_schema_customers_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3716 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/list_invoices_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     6067 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/list_invoices_response_schema_invoices_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3674 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/list_meters_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4628 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/list_meters_response_schema_meters_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3653 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/list_plans_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4103 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/list_plans_response_schema_plans_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     2883 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/login_request_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     2870 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/login_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     2883 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/period.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3483 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/plan_billing_data.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1023 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/plan_status.py
--rw-r--r--   0 shaigross   (501) staff       (20)      947 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/plan_type.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3353 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/query_events_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4866 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/query_events_response_schema_events_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3235 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/send_events_request_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4230 2024-05-08 14:01:03.000000 vayu_client-1.0.3/openapi_client/models/send_events_request_schema_events_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4212 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/send_events_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3218 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/send_events_response_schema_invalid_events_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3108 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/update_customer_request_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/update_customer_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4011 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/update_meter_request_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3063 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/models/update_meter_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     9616 2024-05-08 15:05:35.000000 vayu_client-1.0.3/openapi_client/rest.py
--rw-r--r--   0 shaigross   (501) staff       (20)      420 2024-05-08 15:19:37.450634 vayu_client-1.0.3/setup.cfg
--rw-r--r--   0 shaigross   (501) staff       (20)      296 2024-01-24 16:49:22.000000 vayu_client-1.0.3/setup.py
--rw-r--r--   0 shaigross   (501) staff       (20)     2090 2024-05-08 15:03:11.000000 vayu_client-1.0.3/vayu.py
-drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-08 15:19:37.450246 vayu_client-1.0.3/vayu_client.egg-info/
--rw-r--r--   0 shaigross   (501) staff       (20)     2539 2024-05-08 15:19:37.000000 vayu_client-1.0.3/vayu_client.egg-info/PKG-INFO
--rw-r--r--   0 shaigross   (501) staff       (20)     4400 2024-05-08 15:19:37.000000 vayu_client-1.0.3/vayu_client.egg-info/SOURCES.txt
--rw-r--r--   0 shaigross   (501) staff       (20)        1 2024-05-08 15:19:37.000000 vayu_client-1.0.3/vayu_client.egg-info/dependency_links.txt
--rw-r--r--   0 shaigross   (501) staff       (20)      102 2024-05-08 15:19:37.000000 vayu_client-1.0.3/vayu_client.egg-info/requires.txt
--rw-r--r--   0 shaigross   (501) staff       (20)       47 2024-05-08 15:19:37.000000 vayu_client-1.0.3/vayu_client.egg-info/top_level.txt
--rw-r--r--   0 shaigross   (501) staff       (20)       38 2024-01-24 11:17:29.000000 vayu_client-1.0.3/vayu_consts.py
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-08 15:27:34.606670 vayu_client-1.0.4/
+-rw-r--r--   0 shaigross   (501) staff       (20)     2539 2024-05-08 15:27:34.606791 vayu_client-1.0.4/PKG-INFO
+-rw-r--r--   0 shaigross   (501) staff       (20)      481 2024-05-08 15:19:35.000000 vayu_client-1.0.4/README.md
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-08 15:27:34.585702 vayu_client-1.0.4/entity_clients/
+-rw-r--r--   0 shaigross   (501) staff       (20)       46 2024-05-08 13:47:16.000000 vayu_client-1.0.4/entity_clients/__init__.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1178 2024-05-08 14:04:33.000000 vayu_client-1.0.4/entity_clients/contracts_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1295 2024-05-08 15:27:22.000000 vayu_client-1.0.4/entity_clients/customers_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1413 2024-05-08 14:59:08.000000 vayu_client-1.0.4/entity_clients/events_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)      517 2024-05-08 14:06:03.000000 vayu_client-1.0.4/entity_clients/invoices_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1807 2024-05-08 15:25:09.000000 vayu_client-1.0.4/entity_clients/meters_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)      561 2024-05-08 13:49:18.000000 vayu_client-1.0.4/entity_clients/plans_client.py
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-08 15:27:34.587940 vayu_client-1.0.4/openapi_client/
+-rw-r--r--   0 shaigross   (501) staff       (20)     6948 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/__init__.py
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-08 15:27:34.593937 vayu_client-1.0.4/openapi_client/api/
+-rw-r--r--   0 shaigross   (501) staff       (20)      422 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/api/__init__.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    12591 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/api/auth_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    43742 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/api/contracts_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    55565 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/api/customers_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    61236 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/api/events_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    22281 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/api/invoices_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    43924 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/api/meters_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    32198 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/api/plans_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    26550 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/api_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)      652 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/api_response.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    15152 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/configuration.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     6180 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/exceptions.py
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-08 15:27:34.605829 vayu_client-1.0.4/openapi_client/models/
+-rw-r--r--   0 shaigross   (501) staff       (20)     6030 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/__init__.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3340 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/aggregation_method.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1161 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/aggregation_operator.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1052 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/billing_interval.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3214 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/condition.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4112 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/create_contract_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3126 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/create_contract_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3084 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/create_customer_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/create_customer_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3889 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/create_customer_response_schema_customer.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3034 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/criterion.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1202 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/criterion_operator.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3126 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/delete_contract_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/delete_customer_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3134 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/delete_event_by_ref_id_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4983 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/delete_event_by_ref_id_response_schema_event.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3063 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/delete_meter_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3042 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/delete_plan_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4127 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/event.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3243 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/events_dry_run_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4380 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/events_dry_run_response_schema_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3921 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/events_dry_run_response_schema_inner_event.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4556 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3461 2024-05-08 11:11:33.000000 vayu_client-1.0.4/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner_aggregation_method.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3477 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/filter.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3114 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/get_contract_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4858 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/get_contract_response_schema_contract.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3126 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/get_customer_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3110 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/get_event_by_ref_id_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4861 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/get_event_by_ref_id_response_schema_event.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3093 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/get_invoice_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     6159 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/get_invoice_response_schema_invoice.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3515 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/get_invoice_response_schema_invoice_line_items_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3051 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/get_meter_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4720 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/get_meter_response_schema_meter.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3030 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/get_plan_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4195 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/get_plan_response_schema_plan.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3737 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/list_contracts_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4766 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/list_contracts_response_schema_contracts_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3737 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/list_customers_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3785 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/list_customers_response_schema_customers_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3716 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/list_invoices_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     6067 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/list_invoices_response_schema_invoices_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3674 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/list_meters_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4628 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/list_meters_response_schema_meters_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3653 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/list_plans_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4103 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/list_plans_response_schema_plans_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     2883 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/login_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     2870 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/login_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     2883 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/period.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3483 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/plan_billing_data.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1023 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/plan_status.py
+-rw-r--r--   0 shaigross   (501) staff       (20)      947 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/plan_type.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3353 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/query_events_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4866 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/query_events_response_schema_events_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3235 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/send_events_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4230 2024-05-08 14:01:03.000000 vayu_client-1.0.4/openapi_client/models/send_events_request_schema_events_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4212 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/send_events_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3218 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/send_events_response_schema_invalid_events_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3108 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/update_customer_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/update_customer_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4011 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/update_meter_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3063 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/models/update_meter_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     9616 2024-05-08 15:05:35.000000 vayu_client-1.0.4/openapi_client/rest.py
+-rw-r--r--   0 shaigross   (501) staff       (20)      420 2024-05-08 15:27:34.607076 vayu_client-1.0.4/setup.cfg
+-rw-r--r--   0 shaigross   (501) staff       (20)      296 2024-01-24 16:49:22.000000 vayu_client-1.0.4/setup.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     2152 2024-05-08 15:27:09.000000 vayu_client-1.0.4/vayu.py
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-08 15:27:34.606558 vayu_client-1.0.4/vayu_client.egg-info/
+-rw-r--r--   0 shaigross   (501) staff       (20)     2539 2024-05-08 15:27:34.000000 vayu_client-1.0.4/vayu_client.egg-info/PKG-INFO
+-rw-r--r--   0 shaigross   (501) staff       (20)     4400 2024-05-08 15:27:34.000000 vayu_client-1.0.4/vayu_client.egg-info/SOURCES.txt
+-rw-r--r--   0 shaigross   (501) staff       (20)        1 2024-05-08 15:27:34.000000 vayu_client-1.0.4/vayu_client.egg-info/dependency_links.txt
+-rw-r--r--   0 shaigross   (501) staff       (20)      102 2024-05-08 15:27:34.000000 vayu_client-1.0.4/vayu_client.egg-info/requires.txt
+-rw-r--r--   0 shaigross   (501) staff       (20)       47 2024-05-08 15:27:34.000000 vayu_client-1.0.4/vayu_client.egg-info/top_level.txt
+-rw-r--r--   0 shaigross   (501) staff       (20)       33 2024-05-08 15:24:39.000000 vayu_client-1.0.4/vayu_consts.py
```

### Comparing `vayu_client-1.0.3/PKG-INFO` & `vayu_client-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vayu_client
-Version: 1.0.3
+Version: 1.0.4
 Summary: Simple and easy to use python package for utilizing vayu billing system
 Home-page: https://withvayu.com
 Author: Vayu, Inc.
 Author-email: team@withvayu.com
 Keywords: vayu,billing,events,python,sdk
 Requires-Python: ==3.7.*
 Description-Content-Type: text/markdown
```

### Comparing `vayu_client-1.0.3/entity_clients/contracts_client.py` & `vayu_client-1.0.4/entity_clients/contracts_client.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/entity_clients/customers_client.py` & `vayu_client-1.0.4/entity_clients/customers_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from openapi_client.api.customers_api import CustomersApi
 from openapi_client.api_client import ApiClient
 from openapi_client.models.create_customer_request_schema import \
     CreateCustomerRequestSchema
 from openapi_client.models.update_customer_request_schema import \
     UpdateCustomerRequestSchema
-from vayu_consts import VAYU_URL
 
 
 class CustomersClient:
     __customers_client: CustomersApi = None
 
     def __init__(self, api_client: ApiClient):
         self.__customers_client = CustomersApi(api_client)
```

### Comparing `vayu_client-1.0.3/entity_clients/events_client.py` & `vayu_client-1.0.4/entity_clients/events_client.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/entity_clients/invoices_client.py` & `vayu_client-1.0.4/entity_clients/invoices_client.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/entity_clients/meters_client.py` & `vayu_client-1.0.4/entity_clients/meters_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from openapi_client.api.meters_api import MetersApi
 from openapi_client.api_client import ApiClient
 from openapi_client.models.aggregation_method import AggregationMethod
 from openapi_client.models.filter import Filter
 from openapi_client.models.update_meter_request_schema import \
     UpdateMeterRequestSchema
-from vayu_consts import VAYU_URL
 
 
 class MetersClient:
     __meters_client: MetersApi = None
 
     def __init__(self, api_client: ApiClient):
         self.__meters_client = MetersApi(api_client)
```

### Comparing `vayu_client-1.0.3/entity_clients/plans_client.py` & `vayu_client-1.0.4/entity_clients/plans_client.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/__init__.py` & `vayu_client-1.0.4/openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/api/auth_api.py` & `vayu_client-1.0.4/openapi_client/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/api/contracts_api.py` & `vayu_client-1.0.4/openapi_client/api/contracts_api.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/api/customers_api.py` & `vayu_client-1.0.4/openapi_client/api/customers_api.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/api/events_api.py` & `vayu_client-1.0.4/openapi_client/api/events_api.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/api/invoices_api.py` & `vayu_client-1.0.4/openapi_client/api/invoices_api.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/api/meters_api.py` & `vayu_client-1.0.4/openapi_client/api/meters_api.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/api/plans_api.py` & `vayu_client-1.0.4/openapi_client/api/plans_api.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/api_client.py` & `vayu_client-1.0.4/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/api_response.py` & `vayu_client-1.0.4/openapi_client/api_response.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/configuration.py` & `vayu_client-1.0.4/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/exceptions.py` & `vayu_client-1.0.4/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/__init__.py` & `vayu_client-1.0.4/openapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/aggregation_method.py` & `vayu_client-1.0.4/openapi_client/models/aggregation_method.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/aggregation_operator.py` & `vayu_client-1.0.4/openapi_client/models/aggregation_operator.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/billing_interval.py` & `vayu_client-1.0.4/openapi_client/models/billing_interval.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/condition.py` & `vayu_client-1.0.4/openapi_client/models/condition.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/create_contract_request_schema.py` & `vayu_client-1.0.4/openapi_client/models/create_contract_request_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/create_contract_response_schema.py` & `vayu_client-1.0.4/openapi_client/models/create_contract_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/create_customer_request_schema.py` & `vayu_client-1.0.4/openapi_client/models/create_customer_request_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/create_customer_response_schema.py` & `vayu_client-1.0.4/openapi_client/models/create_customer_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/create_customer_response_schema_customer.py` & `vayu_client-1.0.4/openapi_client/models/create_customer_response_schema_customer.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/criterion.py` & `vayu_client-1.0.4/openapi_client/models/criterion.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/criterion_operator.py` & `vayu_client-1.0.4/openapi_client/models/criterion_operator.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/delete_contract_response_schema.py` & `vayu_client-1.0.4/openapi_client/models/delete_contract_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/delete_customer_response_schema.py` & `vayu_client-1.0.4/openapi_client/models/delete_customer_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/delete_event_by_ref_id_response_schema.py` & `vayu_client-1.0.4/openapi_client/models/delete_event_by_ref_id_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/delete_event_by_ref_id_response_schema_event.py` & `vayu_client-1.0.4/openapi_client/models/delete_event_by_ref_id_response_schema_event.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/delete_meter_response_schema.py` & `vayu_client-1.0.4/openapi_client/models/delete_meter_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/delete_plan_response_schema.py` & `vayu_client-1.0.4/openapi_client/models/delete_plan_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/event.py` & `vayu_client-1.0.4/openapi_client/models/event.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/events_dry_run_request_schema.py` & `vayu_client-1.0.4/openapi_client/models/events_dry_run_request_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/events_dry_run_response_schema_inner.py` & `vayu_client-1.0.4/openapi_client/models/events_dry_run_response_schema_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/events_dry_run_response_schema_inner_event.py` & `vayu_client-1.0.4/openapi_client/models/events_dry_run_response_schema_inner_event.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner.py` & `vayu_client-1.0.4/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner_aggregation_method.py` & `vayu_client-1.0.4/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner_aggregation_method.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/filter.py` & `vayu_client-1.0.4/openapi_client/models/filter.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/get_contract_response_schema.py` & `vayu_client-1.0.4/openapi_client/models/get_contract_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/get_contract_response_schema_contract.py` & `vayu_client-1.0.4/openapi_client/models/get_contract_response_schema_contract.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/get_customer_response_schema.py` & `vayu_client-1.0.4/openapi_client/models/get_customer_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/get_event_by_ref_id_response_schema.py` & `vayu_client-1.0.4/openapi_client/models/get_event_by_ref_id_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/get_event_by_ref_id_response_schema_event.py` & `vayu_client-1.0.4/openapi_client/models/get_event_by_ref_id_response_schema_event.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/get_invoice_response_schema.py` & `vayu_client-1.0.4/openapi_client/models/get_invoice_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/get_invoice_response_schema_invoice.py` & `vayu_client-1.0.4/openapi_client/models/get_invoice_response_schema_invoice.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/get_invoice_response_schema_invoice_line_items_inner.py` & `vayu_client-1.0.4/openapi_client/models/get_invoice_response_schema_invoice_line_items_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/get_meter_response_schema.py` & `vayu_client-1.0.4/openapi_client/models/get_meter_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/get_meter_response_schema_meter.py` & `vayu_client-1.0.4/openapi_client/models/get_meter_response_schema_meter.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/get_plan_response_schema.py` & `vayu_client-1.0.4/openapi_client/models/get_plan_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/get_plan_response_schema_plan.py` & `vayu_client-1.0.4/openapi_client/models/get_plan_response_schema_plan.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/list_contracts_response_schema.py` & `vayu_client-1.0.4/openapi_client/models/list_contracts_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/list_contracts_response_schema_contracts_inner.py` & `vayu_client-1.0.4/openapi_client/models/list_contracts_response_schema_contracts_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/list_customers_response_schema.py` & `vayu_client-1.0.4/openapi_client/models/list_customers_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/list_customers_response_schema_customers_inner.py` & `vayu_client-1.0.4/openapi_client/models/list_customers_response_schema_customers_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/list_invoices_response_schema.py` & `vayu_client-1.0.4/openapi_client/models/list_invoices_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/list_invoices_response_schema_invoices_inner.py` & `vayu_client-1.0.4/openapi_client/models/list_invoices_response_schema_invoices_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/list_meters_response_schema.py` & `vayu_client-1.0.4/openapi_client/models/list_meters_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/list_meters_response_schema_meters_inner.py` & `vayu_client-1.0.4/openapi_client/models/list_meters_response_schema_meters_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/list_plans_response_schema.py` & `vayu_client-1.0.4/openapi_client/models/list_plans_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/list_plans_response_schema_plans_inner.py` & `vayu_client-1.0.4/openapi_client/models/list_plans_response_schema_plans_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/login_request_schema.py` & `vayu_client-1.0.4/openapi_client/models/login_request_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/login_response_schema.py` & `vayu_client-1.0.4/openapi_client/models/login_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/period.py` & `vayu_client-1.0.4/openapi_client/models/period.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/plan_billing_data.py` & `vayu_client-1.0.4/openapi_client/models/plan_billing_data.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/plan_status.py` & `vayu_client-1.0.4/openapi_client/models/plan_status.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/plan_type.py` & `vayu_client-1.0.4/openapi_client/models/plan_type.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/query_events_response_schema.py` & `vayu_client-1.0.4/openapi_client/models/query_events_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/query_events_response_schema_events_inner.py` & `vayu_client-1.0.4/openapi_client/models/query_events_response_schema_events_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/send_events_request_schema.py` & `vayu_client-1.0.4/openapi_client/models/send_events_request_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/send_events_request_schema_events_inner.py` & `vayu_client-1.0.4/openapi_client/models/send_events_request_schema_events_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/send_events_response_schema.py` & `vayu_client-1.0.4/openapi_client/models/send_events_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/send_events_response_schema_invalid_events_inner.py` & `vayu_client-1.0.4/openapi_client/models/send_events_response_schema_invalid_events_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/update_customer_request_schema.py` & `vayu_client-1.0.4/openapi_client/models/update_customer_request_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/update_customer_response_schema.py` & `vayu_client-1.0.4/openapi_client/models/update_customer_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/update_meter_request_schema.py` & `vayu_client-1.0.4/openapi_client/models/update_meter_request_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/models/update_meter_response_schema.py` & `vayu_client-1.0.4/openapi_client/models/update_meter_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/openapi_client/rest.py` & `vayu_client-1.0.4/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.3/vayu.py` & `vayu_client-1.0.4/vayu.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,25 +11,30 @@
 from .entity_clients.customers_client import CustomersClient
 from .entity_clients.invoices_client import InvoicesClient
 from .entity_clients.meters_client import MetersClient
 from .entity_clients.plans_client import PlansClient
 
 
 class Vayu:
-    __api_key: str = None
+    __access_token: str = None
+    __host: str = VAYU_URL
+
+    def __init__(self, api_key: str):
+        self.__login(api_key)
+    
 
     @property
-    def __private_api_client(self):
-        configuration = Configuration(host=VAYU_URL, api_key=self.__api_key)
+    def __private_api_client(self, api_key: str):
+        configuration = Configuration(host=self.__host, api_key=self.__access_token)
         
         return ApiClient(configuration)
 
     @property
     def __public_api_client(self):
-        configuration = Configuration(host=VAYU_URL)
+        configuration = Configuration(host=self.__host)
         
         return ApiClient(configuration)
 
     @property
     def customers(self)->CustomersClient:
         return CustomersClient(self.__private_api_client)
 
@@ -52,17 +57,13 @@
     def invoices(self)->InvoicesClient:
         return InvoicesClient(self.__private_api_client)
 
     @property
     def events(self)->EventsClient:
         return EventsClient(self.__private_api_client)
 
-    def __init__(self, api_key: str):
-        self.__login(api_key)
-    
-
     def __login(self, refresh_token: str):
         auth_api = AuthApi(self.__public_api_client)
         login_request = LoginRequestSchema(refresh_token)
         refresh_response = auth_api.login(login_request)
 
-        self.__api_key = refresh_response.access_token
+        self.__access_token = refresh_response.access_token
```

### Comparing `vayu_client-1.0.3/vayu_client.egg-info/PKG-INFO` & `vayu_client-1.0.4/vayu_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vayu-client
-Version: 1.0.3
+Version: 1.0.4
 Summary: Simple and easy to use python package for utilizing vayu billing system
 Home-page: https://withvayu.com
 Author: Vayu, Inc.
 Author-email: team@withvayu.com
 Keywords: vayu,billing,events,python,sdk
 Requires-Python: ==3.7.*
 Description-Content-Type: text/markdown
```

### Comparing `vayu_client-1.0.3/vayu_client.egg-info/SOURCES.txt` & `vayu_client-1.0.4/vayu_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

