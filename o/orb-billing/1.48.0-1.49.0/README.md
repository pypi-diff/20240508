# Comparing `tmp/orb_billing-1.48.0.tar.gz` & `tmp/orb_billing-1.49.0.tar.gz`

## Comparing `orb_billing-1.48.0.tar` & `orb_billing-1.49.0.tar`

### file list

```diff
@@ -1,178 +1,180 @@
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/__init__.py
--rw-r--r--   0        0        0    65289 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_base_client.py
--rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_constants.py
--rw-r--r--   0        0        0    15693 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_files.py
--rw-r--r--   0        0        0    15418 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_legacy_response.py
--rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_qs.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_resource.py
--rw-r--r--   0        0        0    28559 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_response.py
--rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_streaming.py
--rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_types.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_version.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/pagination.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_utils/__init__.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/lib/.keep
--rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/__init__.py
--rw-r--r--   0        0        0     9545 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/credit_notes.py
--rw-r--r--   0        0        0     7970 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/invoice_line_items.py
--rw-r--r--   0        0        0    39562 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/invoices.py
--rw-r--r--   0        0        0    12177 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/items.py
--rw-r--r--   0        0        0    16140 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/metrics.py
--rw-r--r--   0        0        0   163148 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/subscriptions.py
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/top_level.py
--rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/webhooks.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/coupons/__init__.py
--rw-r--r--   0        0        0    20895 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/coupons/coupons.py
--rw-r--r--   0        0        0     6995 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/coupons/subscriptions.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/customers/__init__.py
--rw-r--r--   0        0        0    16173 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/customers/balance_transactions.py
--rw-r--r--   0        0        0    44927 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/customers/costs.py
--rw-r--r--   0        0        0   139802 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/customers/customers.py
--rw-r--r--   0        0        0    31859 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/customers/usage.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/customers/credits/__init__.py
--rw-r--r--   0        0        0    14550 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/customers/credits/credits.py
--rw-r--r--   0        0        0   204046 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/customers/credits/ledger.py
--rw-r--r--   0        0        0    34978 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/customers/credits/top_ups.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/events/__init__.py
--rw-r--r--   0        0        0    27956 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/events/backfills.py
--rw-r--r--   0        0        0    52976 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/events/events.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/plans/__init__.py
--rw-r--r--   0        0        0    13319 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/plans/external_plan_id.py
--rw-r--r--   0        0        0    25451 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/plans/plans.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/prices/__init__.py
--rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/prices/external_price_id.py
--rw-r--r--   0        0        0   134801 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/resources/prices/prices.py
--rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/__init__.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/coupon.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/coupon_create_params.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/coupon_list_params.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/credit_note.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/credit_note_list_params.py
--rw-r--r--   0        0        0    17584 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customer.py
--rw-r--r--   0        0        0    18502 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customer_create_params.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customer_list_params.py
--rw-r--r--   0        0        0    18262 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customer_update_by_external_id_params.py
--rw-r--r--   0        0        0    18238 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customer_update_params.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/evaluate_price_group.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/event_deprecate_response.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/event_ingest_params.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/event_ingest_response.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/event_search_params.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/event_search_response.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/event_update_params.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/event_update_response.py
--rw-r--r--   0        0        0    34433 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/invoice.py
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/invoice_create_params.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/invoice_fetch_upcoming_params.py
--rw-r--r--   0        0        0    34474 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/invoice_fetch_upcoming_response.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/invoice_line_item_create_params.py
--rw-r--r--   0        0        0    11492 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/invoice_line_item_create_response.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/invoice_list_params.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/invoice_mark_paid_params.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/item.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/item_create_params.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/item_list_params.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/metric_create_params.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/metric_create_response.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/metric_fetch_response.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/metric_list_params.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/metric_list_response.py
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/plan.py
--rw-r--r--   0        0        0    24502 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/plan_create_params.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/plan_list_params.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/plan_update_params.py
--rw-r--r--   0        0        0    36435 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/price.py
--rw-r--r--   0        0        0    28352 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/price_create_params.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/price_evaluate_params.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/price_evaluate_response.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/price_list_params.py
--rw-r--r--   0        0        0    16838 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_cancel_params.py
--rw-r--r--   0        0        0    31028 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_create_params.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_fetch_costs_params.py
--rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_fetch_costs_response.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_fetch_schedule_params.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_fetch_schedule_response.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_fetch_usage_params.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_list_params.py
--rw-r--r--   0        0        0    33927 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_price_intervals_params.py
--rw-r--r--   0        0        0    31434 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_schedule_plan_change_params.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_trigger_phase_params.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_unschedule_fixed_fee_quantity_updates_params.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_update_fixed_fee_quantity_params.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_update_params.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscription_usage.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/subscriptions.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/top_level_ping_response.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/beta/evaluate_price_group.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/beta/price_evaluate_params.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/beta/price_evaluate_response.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/coupons/__init__.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/coupons/subscription_list_params.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/balance_transaction_create_params.py
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/balance_transaction_create_response.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/balance_transaction_list_params.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/balance_transaction_list_response.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/cost_list_by_external_id_params.py
--rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/cost_list_by_external_id_response.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/cost_list_params.py
--rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/cost_list_response.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credit_list_by_external_id_params.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credit_list_by_external_id_response.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credit_list_params.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credit_list_response.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/usage_update_by_external_id_params.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/usage_update_by_external_id_response.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/usage_update_params.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/usage_update_response.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/__init__.py
--rw-r--r--   0        0        0     8686 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_params.py
--rw-r--r--   0        0        0     8678 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_response.py
--rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/ledger_create_entry_params.py
--rw-r--r--   0        0        0     8654 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/ledger_create_entry_response.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/ledger_list_by_external_id_params.py
--rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/ledger_list_by_external_id_response.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/ledger_list_params.py
--rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/ledger_list_response.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/top_up_create_by_external_id_params.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/top_up_create_by_external_id_response.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/top_up_create_params.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/top_up_create_response.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/top_up_list_by_external_id_params.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/top_up_list_by_external_id_response.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/top_up_list_params.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/customers/credits/top_up_list_response.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/events/__init__.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/events/backfill_close_response.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/events/backfill_create_params.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/events/backfill_create_response.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/events/backfill_fetch_response.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/events/backfill_list_params.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/events/backfill_list_response.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/events/backfill_revert_response.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/plans/__init__.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/plans/external_plan_id_update_params.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/prices/__init__.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/shared/__init__.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/shared/billing_cycle_relative_date.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/shared/discount.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/shared/pagination_metadata.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/shared_params/__init__.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 orb_billing-1.48.0/src/orb/types/shared_params/billing_cycle_relative_date.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 orb_billing-1.48.0/.gitignore
--rw-r--r--   0        0        0    11333 2020-02-02 00:00:00.000000 orb_billing-1.48.0/LICENSE
--rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 orb_billing-1.48.0/pyproject.toml
--rw-r--r--   0        0        0    15252 2020-02-02 00:00:00.000000 orb_billing-1.48.0/PKG-INFO
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/__init__.py
+-rw-r--r--   0        0        0    65289 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/_base_client.py
+-rw-r--r--   0        0        0    27569 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/_constants.py
+-rw-r--r--   0        0        0    15693 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/_files.py
+-rw-r--r--   0        0        0    15418 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/_legacy_response.py
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/_qs.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/_resource.py
+-rw-r--r--   0        0        0    28559 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/_response.py
+-rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/_streaming.py
+-rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/_types.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/_version.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/pagination.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/_utils/__init__.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/lib/.keep
+-rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/__init__.py
+-rw-r--r--   0        0        0     5245 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/alerts.py
+-rw-r--r--   0        0        0     9545 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/credit_notes.py
+-rw-r--r--   0        0        0     7970 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/invoice_line_items.py
+-rw-r--r--   0        0        0    39562 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/invoices.py
+-rw-r--r--   0        0        0    12177 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/items.py
+-rw-r--r--   0        0        0    16140 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/metrics.py
+-rw-r--r--   0        0        0   163148 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/subscriptions.py
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/top_level.py
+-rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/webhooks.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/coupons/__init__.py
+-rw-r--r--   0        0        0    20895 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/coupons/coupons.py
+-rw-r--r--   0        0        0     6995 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/coupons/subscriptions.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/customers/__init__.py
+-rw-r--r--   0        0        0    16173 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/customers/balance_transactions.py
+-rw-r--r--   0        0        0    44927 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/customers/costs.py
+-rw-r--r--   0        0        0   159002 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/customers/customers.py
+-rw-r--r--   0        0        0    31859 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/customers/usage.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/customers/credits/__init__.py
+-rw-r--r--   0        0        0    14550 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/customers/credits/credits.py
+-rw-r--r--   0        0        0   204046 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/customers/credits/ledger.py
+-rw-r--r--   0        0        0    34978 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/customers/credits/top_ups.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/events/__init__.py
+-rw-r--r--   0        0        0    27956 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/events/backfills.py
+-rw-r--r--   0        0        0    52976 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/events/events.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/plans/__init__.py
+-rw-r--r--   0        0        0    13319 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/plans/external_plan_id.py
+-rw-r--r--   0        0        0    25451 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/plans/plans.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/prices/__init__.py
+-rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/prices/external_price_id.py
+-rw-r--r--   0        0        0   134801 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/resources/prices/prices.py
+-rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/__init__.py
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/alert.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/coupon.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/coupon_create_params.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/coupon_list_params.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/credit_note.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/credit_note_list_params.py
+-rw-r--r--   0        0        0    21166 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customer.py
+-rw-r--r--   0        0        0    22228 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customer_create_params.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customer_list_params.py
+-rw-r--r--   0        0        0    21988 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customer_update_by_external_id_params.py
+-rw-r--r--   0        0        0    21964 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customer_update_params.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/evaluate_price_group.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/event_deprecate_response.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/event_ingest_params.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/event_ingest_response.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/event_search_params.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/event_search_response.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/event_update_params.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/event_update_response.py
+-rw-r--r--   0        0        0    38015 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/invoice.py
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/invoice_create_params.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/invoice_fetch_upcoming_params.py
+-rw-r--r--   0        0        0    38056 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/invoice_fetch_upcoming_response.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/invoice_line_item_create_params.py
+-rw-r--r--   0        0        0    11492 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/invoice_line_item_create_response.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/invoice_list_params.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/invoice_mark_paid_params.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/item.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/item_create_params.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/item_list_params.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/metric_create_params.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/metric_create_response.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/metric_fetch_response.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/metric_list_params.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/metric_list_response.py
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/plan.py
+-rw-r--r--   0        0        0    24502 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/plan_create_params.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/plan_list_params.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/plan_update_params.py
+-rw-r--r--   0        0        0    36435 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/price.py
+-rw-r--r--   0        0        0    28352 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/price_create_params.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/price_evaluate_params.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/price_evaluate_response.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/price_list_params.py
+-rw-r--r--   0        0        0    16838 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/subscription.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/subscription_cancel_params.py
+-rw-r--r--   0        0        0    31028 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/subscription_create_params.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/subscription_fetch_costs_params.py
+-rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/subscription_fetch_costs_response.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/subscription_fetch_schedule_params.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/subscription_fetch_schedule_response.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/subscription_fetch_usage_params.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/subscription_list_params.py
+-rw-r--r--   0        0        0    33927 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/subscription_price_intervals_params.py
+-rw-r--r--   0        0        0    31434 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/subscription_schedule_plan_change_params.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/subscription_trigger_phase_params.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/subscription_unschedule_fixed_fee_quantity_updates_params.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/subscription_update_fixed_fee_quantity_params.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/subscription_update_params.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/subscription_usage.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/subscriptions.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/top_level_ping_response.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/beta/evaluate_price_group.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/beta/price_evaluate_params.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/beta/price_evaluate_response.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/coupons/__init__.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/coupons/subscription_list_params.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/balance_transaction_create_params.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/balance_transaction_create_response.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/balance_transaction_list_params.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/balance_transaction_list_response.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/cost_list_by_external_id_params.py
+-rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/cost_list_by_external_id_response.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/cost_list_params.py
+-rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/cost_list_response.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/credit_list_by_external_id_params.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/credit_list_by_external_id_response.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/credit_list_params.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/credit_list_response.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/usage_update_by_external_id_params.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/usage_update_by_external_id_response.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/usage_update_params.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/usage_update_response.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/credits/__init__.py
+-rw-r--r--   0        0        0     8686 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_params.py
+-rw-r--r--   0        0        0     8678 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_response.py
+-rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/credits/ledger_create_entry_params.py
+-rw-r--r--   0        0        0     8654 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/credits/ledger_create_entry_response.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/credits/ledger_list_by_external_id_params.py
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/credits/ledger_list_by_external_id_response.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/credits/ledger_list_params.py
+-rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/credits/ledger_list_response.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/credits/top_up_create_by_external_id_params.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/credits/top_up_create_by_external_id_response.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/credits/top_up_create_params.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/credits/top_up_create_response.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/credits/top_up_list_by_external_id_params.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/credits/top_up_list_by_external_id_response.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/credits/top_up_list_params.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/customers/credits/top_up_list_response.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/events/__init__.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/events/backfill_close_response.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/events/backfill_create_params.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/events/backfill_create_response.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/events/backfill_fetch_response.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/events/backfill_list_params.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/events/backfill_list_response.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/events/backfill_revert_response.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/plans/__init__.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/plans/external_plan_id_update_params.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/prices/__init__.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/shared/__init__.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/shared/billing_cycle_relative_date.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/shared/discount.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/shared/pagination_metadata.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/shared_params/__init__.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 orb_billing-1.49.0/src/orb/types/shared_params/billing_cycle_relative_date.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 orb_billing-1.49.0/.gitignore
+-rw-r--r--   0        0        0    11333 2020-02-02 00:00:00.000000 orb_billing-1.49.0/LICENSE
+-rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 orb_billing-1.49.0/pyproject.toml
+-rw-r--r--   0        0        0    15252 2020-02-02 00:00:00.000000 orb_billing-1.49.0/PKG-INFO
```

### Comparing `orb_billing-1.48.0/src/orb/__init__.py` & `orb_billing-1.49.0/src/orb/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/_base_client.py` & `orb_billing-1.49.0/src/orb/_base_client.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/_client.py` & `orb_billing-1.49.0/src/orb/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     invoices: resources.Invoices
     items: resources.Items
     metrics: resources.Metrics
     plans: resources.Plans
     prices: resources.Prices
     subscriptions: resources.Subscriptions
     webhooks: resources.Webhooks
+    alerts: resources.Alerts
     with_raw_response: OrbWithRawResponse
     with_streaming_response: OrbWithStreamedResponse
 
     # client options
     api_key: str
     webhook_secret: str | None
 
@@ -136,14 +137,16 @@
         self.invoices = resources.Invoices(self)
         self.items = resources.Items(self)
         self.metrics = resources.Metrics(self)
         self.plans = resources.Plans(self)
         self.prices = resources.Prices(self)
         self.subscriptions = resources.Subscriptions(self)
         self.webhooks = resources.Webhooks(self)
+        self.alerts = resources.Alerts(self)
+        self.with_raw_response = OrbWithRawResponse(self)
         self.with_streaming_response = OrbWithStreamedResponse(self)
 
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="brackets")
 
@@ -307,14 +310,15 @@
     invoices: resources.AsyncInvoices
     items: resources.AsyncItems
     metrics: resources.AsyncMetrics
     plans: resources.AsyncPlans
     prices: resources.AsyncPrices
     subscriptions: resources.AsyncSubscriptions
     webhooks: resources.AsyncWebhooks
+    alerts: resources.AsyncAlerts
     with_raw_response: AsyncOrbWithRawResponse
     with_streaming_response: AsyncOrbWithStreamedResponse
 
     # client options
     api_key: str
     webhook_secret: str | None
 
@@ -387,14 +391,15 @@
         self.invoices = resources.AsyncInvoices(self)
         self.items = resources.AsyncItems(self)
         self.metrics = resources.AsyncMetrics(self)
         self.plans = resources.AsyncPlans(self)
         self.prices = resources.AsyncPrices(self)
         self.subscriptions = resources.AsyncSubscriptions(self)
         self.webhooks = resources.AsyncWebhooks(self)
+        self.alerts = resources.AsyncAlerts(self)
         self.with_raw_response = AsyncOrbWithRawResponse(self)
         self.with_streaming_response = AsyncOrbWithStreamedResponse(self)
 
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="brackets")
@@ -559,14 +564,15 @@
         self.invoice_line_items = resources.InvoiceLineItemsWithRawResponse(client.invoice_line_items)
         self.invoices = resources.InvoicesWithRawResponse(client.invoices)
         self.items = resources.ItemsWithRawResponse(client.items)
         self.metrics = resources.MetricsWithRawResponse(client.metrics)
         self.plans = resources.PlansWithRawResponse(client.plans)
         self.prices = resources.PricesWithRawResponse(client.prices)
         self.subscriptions = resources.SubscriptionsWithRawResponse(client.subscriptions)
+        self.alerts = resources.AlertsWithRawResponse(client.alerts)
 
 
 class AsyncOrbWithRawResponse:
     def __init__(self, client: AsyncOrb) -> None:
         self.top_level = resources.AsyncTopLevelWithRawResponse(client.top_level)
         self.coupons = resources.AsyncCouponsWithRawResponse(client.coupons)
         self.credit_notes = resources.AsyncCreditNotesWithRawResponse(client.credit_notes)
@@ -575,14 +581,15 @@
         self.invoice_line_items = resources.AsyncInvoiceLineItemsWithRawResponse(client.invoice_line_items)
         self.invoices = resources.AsyncInvoicesWithRawResponse(client.invoices)
         self.items = resources.AsyncItemsWithRawResponse(client.items)
         self.metrics = resources.AsyncMetricsWithRawResponse(client.metrics)
         self.plans = resources.AsyncPlansWithRawResponse(client.plans)
         self.prices = resources.AsyncPricesWithRawResponse(client.prices)
         self.subscriptions = resources.AsyncSubscriptionsWithRawResponse(client.subscriptions)
+        self.alerts = resources.AsyncAlertsWithRawResponse(client.alerts)
 
 
 class OrbWithStreamedResponse:
     def __init__(self, client: Orb) -> None:
         self.top_level = resources.TopLevelWithStreamingResponse(client.top_level)
         self.coupons = resources.CouponsWithStreamingResponse(client.coupons)
         self.credit_notes = resources.CreditNotesWithStreamingResponse(client.credit_notes)
@@ -591,14 +598,15 @@
         self.invoice_line_items = resources.InvoiceLineItemsWithStreamingResponse(client.invoice_line_items)
         self.invoices = resources.InvoicesWithStreamingResponse(client.invoices)
         self.items = resources.ItemsWithStreamingResponse(client.items)
         self.metrics = resources.MetricsWithStreamingResponse(client.metrics)
         self.plans = resources.PlansWithStreamingResponse(client.plans)
         self.prices = resources.PricesWithStreamingResponse(client.prices)
         self.subscriptions = resources.SubscriptionsWithStreamingResponse(client.subscriptions)
+        self.alerts = resources.AlertsWithStreamingResponse(client.alerts)
 
 
 class AsyncOrbWithStreamedResponse:
     def __init__(self, client: AsyncOrb) -> None:
         self.top_level = resources.AsyncTopLevelWithStreamingResponse(client.top_level)
         self.coupons = resources.AsyncCouponsWithStreamingResponse(client.coupons)
         self.credit_notes = resources.AsyncCreditNotesWithStreamingResponse(client.credit_notes)
@@ -607,12 +615,13 @@
         self.invoice_line_items = resources.AsyncInvoiceLineItemsWithStreamingResponse(client.invoice_line_items)
         self.invoices = resources.AsyncInvoicesWithStreamingResponse(client.invoices)
         self.items = resources.AsyncItemsWithStreamingResponse(client.items)
         self.metrics = resources.AsyncMetricsWithStreamingResponse(client.metrics)
         self.plans = resources.AsyncPlansWithStreamingResponse(client.plans)
         self.prices = resources.AsyncPricesWithStreamingResponse(client.prices)
         self.subscriptions = resources.AsyncSubscriptionsWithStreamingResponse(client.subscriptions)
+        self.alerts = resources.AsyncAlertsWithStreamingResponse(client.alerts)
 
 
 Client = Orb
 
 AsyncClient = AsyncOrb
```

### Comparing `orb_billing-1.48.0/src/orb/_compat.py` & `orb_billing-1.49.0/src/orb/_compat.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/_exceptions.py` & `orb_billing-1.49.0/src/orb/_exceptions.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/_files.py` & `orb_billing-1.49.0/src/orb/_files.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/_legacy_response.py` & `orb_billing-1.49.0/src/orb/_legacy_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/_models.py` & `orb_billing-1.49.0/src/orb/_models.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/_qs.py` & `orb_billing-1.49.0/src/orb/_qs.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/_resource.py` & `orb_billing-1.49.0/src/orb/_resource.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/_response.py` & `orb_billing-1.49.0/src/orb/_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/_streaming.py` & `orb_billing-1.49.0/src/orb/_streaming.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/_types.py` & `orb_billing-1.49.0/src/orb/_types.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/pagination.py` & `orb_billing-1.49.0/src/orb/pagination.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/_utils/__init__.py` & `orb_billing-1.49.0/src/orb/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/_utils/_logs.py` & `orb_billing-1.49.0/src/orb/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/_utils/_proxy.py` & `orb_billing-1.49.0/src/orb/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/_utils/_sync.py` & `orb_billing-1.49.0/src/orb/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/_utils/_transform.py` & `orb_billing-1.49.0/src/orb/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/_utils/_typing.py` & `orb_billing-1.49.0/src/orb/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/_utils/_utils.py` & `orb_billing-1.49.0/src/orb/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/__init__.py` & `orb_billing-1.49.0/src/orb/resources/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,22 @@
     Plans,
     AsyncPlans,
     PlansWithRawResponse,
     AsyncPlansWithRawResponse,
     PlansWithStreamingResponse,
     AsyncPlansWithStreamingResponse,
 )
+from .alerts import (
+    Alerts,
+    AsyncAlerts,
+    AlertsWithRawResponse,
+    AsyncAlertsWithRawResponse,
+    AlertsWithStreamingResponse,
+    AsyncAlertsWithStreamingResponse,
+)
 from .events import (
     Events,
     AsyncEvents,
     EventsWithRawResponse,
     AsyncEventsWithRawResponse,
     EventsWithStreamingResponse,
     AsyncEventsWithStreamingResponse,
@@ -172,8 +180,14 @@
     "AsyncSubscriptions",
     "SubscriptionsWithRawResponse",
     "AsyncSubscriptionsWithRawResponse",
     "SubscriptionsWithStreamingResponse",
     "AsyncSubscriptionsWithStreamingResponse",
     "Webhooks",
     "AsyncWebhooks",
+    "Alerts",
+    "AsyncAlerts",
+    "AlertsWithRawResponse",
+    "AsyncAlertsWithRawResponse",
+    "AlertsWithStreamingResponse",
+    "AsyncAlertsWithStreamingResponse",
 ]
```

### Comparing `orb_billing-1.48.0/src/orb/resources/credit_notes.py` & `orb_billing-1.49.0/src/orb/resources/credit_notes.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/invoice_line_items.py` & `orb_billing-1.49.0/src/orb/resources/invoice_line_items.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/invoices.py` & `orb_billing-1.49.0/src/orb/resources/invoices.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/items.py` & `orb_billing-1.49.0/src/orb/resources/items.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/metrics.py` & `orb_billing-1.49.0/src/orb/resources/metrics.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/subscriptions.py` & `orb_billing-1.49.0/src/orb/resources/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/top_level.py` & `orb_billing-1.49.0/src/orb/resources/top_level.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/webhooks.py` & `orb_billing-1.49.0/src/orb/resources/webhooks.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/coupons/__init__.py` & `orb_billing-1.49.0/src/orb/resources/coupons/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/coupons/coupons.py` & `orb_billing-1.49.0/src/orb/resources/coupons/coupons.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/coupons/subscriptions.py` & `orb_billing-1.49.0/src/orb/resources/coupons/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/customers/__init__.py` & `orb_billing-1.49.0/src/orb/resources/customers/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/customers/balance_transactions.py` & `orb_billing-1.49.0/src/orb/resources/customers/balance_transactions.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/customers/costs.py` & `orb_billing-1.49.0/src/orb/resources/customers/costs.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/customers/customers.py` & `orb_billing-1.49.0/src/orb/resources/customers/customers.py`

 * *Files 15% similar despite different names*

```diff
@@ -169,92 +169,112 @@
           tax_id: Tax IDs are commonly required to be displayed on customer invoices, which are
               added to the headers of invoices.
 
               ### Supported Tax ID Countries and Types
 
               | Country              | Type         | Description                                                                                             |
               | -------------------- | ------------ | ------------------------------------------------------------------------------------------------------- |
-              | Andorra              | `ad_nrt`     | Andorran NRT number                                                                                     |
+              | Andorra              | `ad_nrt`     | Andorran NRT Number                                                                                     |
+              | Argentina            | `ar_cuit`    | Argentinian Tax ID Number                                                                               |
               | Australia            | `au_abn`     | Australian Business Number (AU ABN)                                                                     |
               | Australia            | `au_arn`     | Australian Taxation Office Reference Number                                                             |
-              | Austria              | `eu_vat`     | European VAT number                                                                                     |
-              | Belgium              | `eu_vat`     | European VAT number                                                                                     |
-              | Brazil               | `br_cnpj`    | Brazilian CNPJ number                                                                                   |
-              | Brazil               | `br_cpf`     | Brazilian CPF number                                                                                    |
+              | Austria              | `eu_vat`     | European VAT Number                                                                                     |
+              | Bahrain              | `bh_vat`     | Bahraini VAT Number                                                                                     |
+              | Belgium              | `eu_vat`     | European VAT Number                                                                                     |
+              | Bolivia              | `bo_tin`     | Bolivian Tax ID                                                                                         |
+              | Brazil               | `br_cnpj`    | Brazilian CNPJ Number                                                                                   |
+              | Brazil               | `br_cpf`     | Brazilian CPF Number                                                                                    |
               | Bulgaria             | `bg_uic`     | Bulgaria Unified Identification Code                                                                    |
-              | Bulgaria             | `eu_vat`     | European VAT number                                                                                     |
+              | Bulgaria             | `eu_vat`     | European VAT Number                                                                                     |
               | Canada               | `ca_bn`      | Canadian BN                                                                                             |
-              | Canada               | `ca_gst_hst` | Canadian GST/HST number                                                                                 |
-              | Canada               | `ca_pst_bc`  | Canadian PST number (British Columbia)                                                                  |
-              | Canada               | `ca_pst_mb`  | Canadian PST number (Manitoba)                                                                          |
-              | Canada               | `ca_pst_sk`  | Canadian PST number (Saskatchewan)                                                                      |
-              | Canada               | `ca_qst`     | Canadian QST number (Québec)                                                                            |
+              | Canada               | `ca_gst_hst` | Canadian GST/HST Number                                                                                 |
+              | Canada               | `ca_pst_bc`  | Canadian PST Number (British Columbia)                                                                  |
+              | Canada               | `ca_pst_mb`  | Canadian PST Number (Manitoba)                                                                          |
+              | Canada               | `ca_pst_sk`  | Canadian PST Number (Saskatchewan)                                                                      |
+              | Canada               | `ca_qst`     | Canadian QST Number (Québec)                                                                            |
               | Chile                | `cl_tin`     | Chilean TIN                                                                                             |
-              | Croatia              | `eu_vat`     | European VAT number                                                                                     |
-              | Cyprus               | `eu_vat`     | European VAT number                                                                                     |
-              | Czech Republic       | `eu_vat`     | European VAT number                                                                                     |
-              | Denmark              | `eu_vat`     | European VAT number                                                                                     |
+              | China                | `cn_tin`     | Chinese Tax ID                                                                                          |
+              | Colombia             | `co_nit`     | Colombian NIT Number                                                                                    |
+              | Costa Rica           | `cr_tin`     | Costa Rican Tax ID                                                                                      |
+              | Croatia              | `eu_vat`     | European VAT Number                                                                                     |
+              | Cyprus               | `eu_vat`     | European VAT Number                                                                                     |
+              | Czech Republic       | `eu_vat`     | European VAT Number                                                                                     |
+              | Denmark              | `eu_vat`     | European VAT Number                                                                                     |
+              | Dominican Republic   | `do_rcn`     | Dominican RCN Number                                                                                    |
+              | Ecuador              | `ec_ruc`     | Ecuadorian RUC Number                                                                                   |
               | Egypt                | `eg_tin`     | Egyptian Tax Identification Number                                                                      |
-              | Estonia              | `eu_vat`     | European VAT number                                                                                     |
-              | EU                   | `eu_oss_vat` | European One Stop Shop VAT number for non-Union scheme                                                  |
-              | Finland              | `eu_vat`     | European VAT number                                                                                     |
-              | France               | `eu_vat`     | European VAT number                                                                                     |
+              | El Salvador          | `sv_nit`     | El Salvadorian NIT Number                                                                               |
+              | Estonia              | `eu_vat`     | European VAT Number                                                                                     |
+              | EU                   | `eu_oss_vat` | European One Stop Shop VAT Number for non-Union scheme                                                  |
+              | Finland              | `eu_vat`     | European VAT Number                                                                                     |
+              | France               | `eu_vat`     | European VAT Number                                                                                     |
               | Georgia              | `ge_vat`     | Georgian VAT                                                                                            |
-              | Germany              | `eu_vat`     | European VAT number                                                                                     |
-              | Greece               | `eu_vat`     | European VAT number                                                                                     |
-              | Hong Kong            | `hk_br`      | Hong Kong BR number                                                                                     |
-              | Hungary              | `eu_vat`     | European VAT number                                                                                     |
-              | Hungary              | `hu_tin`     | Hungary tax number (adószám)                                                                            |
+              | Germany              | `eu_vat`     | European VAT Number                                                                                     |
+              | Greece               | `eu_vat`     | European VAT Number                                                                                     |
+              | Hong Kong            | `hk_br`      | Hong Kong BR Number                                                                                     |
+              | Hungary              | `eu_vat`     | European VAT Number                                                                                     |
+              | Hungary              | `hu_tin`     | Hungary Tax Number (adószám)                                                                            |
               | Iceland              | `is_vat`     | Icelandic VAT                                                                                           |
-              | India                | `in_gst`     | Indian GST number                                                                                       |
-              | Indonesia            | `id_npwp`    | Indonesian NPWP number                                                                                  |
-              | Ireland              | `eu_vat`     | European VAT number                                                                                     |
+              | India                | `in_gst`     | Indian GST Number                                                                                       |
+              | Indonesia            | `id_npwp`    | Indonesian NPWP Number                                                                                  |
+              | Ireland              | `eu_vat`     | European VAT Number                                                                                     |
               | Israel               | `il_vat`     | Israel VAT                                                                                              |
-              | Italy                | `eu_vat`     | European VAT number                                                                                     |
+              | Italy                | `eu_vat`     | European VAT Number                                                                                     |
               | Japan                | `jp_cn`      | Japanese Corporate Number (_Hōjin Bangō_)                                                               |
               | Japan                | `jp_rn`      | Japanese Registered Foreign Businesses' Registration Number (_Tōroku Kokugai Jigyōsha no Tōroku Bangō_) |
               | Japan                | `jp_trn`     | Japanese Tax Registration Number (_Tōroku Bangō_)                                                       |
+              | Kazakhstan           | `kz_bin`     | Kazakhstani Business Identification Number                                                              |
               | Kenya                | `ke_pin`     | Kenya Revenue Authority Personal Identification Number                                                  |
-              | Latvia               | `eu_vat`     | European VAT number                                                                                     |
-              | Liechtenstein        | `li_uid`     | Liechtensteinian UID number                                                                             |
-              | Lithuania            | `eu_vat`     | European VAT number                                                                                     |
-              | Luxembourg           | `eu_vat`     | European VAT number                                                                                     |
-              | Malaysia             | `my_frp`     | Malaysian FRP number                                                                                    |
+              | Latvia               | `eu_vat`     | European VAT Number                                                                                     |
+              | Liechtenstein        | `li_uid`     | Liechtensteinian UID Number                                                                             |
+              | Lithuania            | `eu_vat`     | European VAT Number                                                                                     |
+              | Luxembourg           | `eu_vat`     | European VAT Number                                                                                     |
+              | Malaysia             | `my_frp`     | Malaysian FRP Number                                                                                    |
               | Malaysia             | `my_itn`     | Malaysian ITN                                                                                           |
-              | Malaysia             | `my_sst`     | Malaysian SST number                                                                                    |
-              | Malta                | `eu_vat `    | European VAT number                                                                                     |
-              | Mexico               | `mx_rfc`     | Mexican RFC number                                                                                      |
-              | Netherlands          | `eu_vat`     | European VAT number                                                                                     |
-              | New Zealand          | `nz_gst`     | New Zealand GST number                                                                                  |
-              | Norway               | `no_vat`     | Norwegian VAT number                                                                                    |
+              | Malaysia             | `my_sst`     | Malaysian SST Number                                                                                    |
+              | Malta                | `eu_vat `    | European VAT Number                                                                                     |
+              | Mexico               | `mx_rfc`     | Mexican RFC Number                                                                                      |
+              | Netherlands          | `eu_vat`     | European VAT Number                                                                                     |
+              | New Zealand          | `nz_gst`     | New Zealand GST Number                                                                                  |
+              | Nigeria              | `ng_tin`     | Nigerian Tax Identification Number                                                                      |
+              | Norway               | `no_vat`     | Norwegian VAT Number                                                                                    |
+              | Norway               | `no_voec`    | Norwegian VAT on e-commerce Number                                                                      |
+              | Oman                 | `om_vat`     | Omani VAT Number                                                                                        |
+              | Peru                 | `pe_ruc`     | Peruvian RUC Number                                                                                     |
               | Philippines          | `ph_tin `    | Philippines Tax Identification Number                                                                   |
-              | Poland               | `eu_vat`     | European VAT number                                                                                     |
-              | Portugal             | `eu_vat`     | European VAT number                                                                                     |
-              | Romania              | `eu_vat`     | European VAT number                                                                                     |
+              | Poland               | `eu_vat`     | European VAT Number                                                                                     |
+              | Portugal             | `eu_vat`     | European VAT Number                                                                                     |
+              | Romania              | `eu_vat`     | European VAT Number                                                                                     |
+              | Romania              | `ro_tin`     | Romanian Tax ID Number                                                                                  |
               | Russia               | `ru_inn`     | Russian INN                                                                                             |
               | Russia               | `ru_kpp`     | Russian KPP                                                                                             |
-              | Saudi Arabia         | `sg_gst`     | Singaporean GST                                                                                         |
+              | Saudi Arabia         | `sa_vat`     | Saudi Arabia VAT                                                                                        |
+              | Serbia               | `rs_pib`     | Serbian PIB Number                                                                                      |
+              | Singapore            | `sg_gst`     | Singaporean GST                                                                                         |
               | Singapore            | `sg_uen`     | Singaporean UEN                                                                                         |
-              | Slovakia             | `eu_vat`     | European VAT number                                                                                     |
-              | Slovenia             | `eu_vat`     | European VAT number                                                                                     |
-              | Slovenia             | `si_tin`     | Slovenia tax number (davčna številka)                                                                   |
-              | South Africa         | `za_vat`     | South African VAT number                                                                                |
+              | Slovakia             | `eu_vat`     | European VAT Number                                                                                     |
+              | Slovenia             | `eu_vat`     | European VAT Number                                                                                     |
+              | Slovenia             | `si_tin`     | Slovenia Tax Number (davčna številka)                                                                   |
+              | South Africa         | `za_vat`     | South African VAT Number                                                                                |
               | South Korea          | `kr_brn`     | Korean BRN                                                                                              |
-              | Spain                | `es_cif`     | Spanish NIF number (previously Spanish CIF number)                                                      |
-              | Spain                | `eu_vat`     | European VAT number                                                                                     |
-              | Sweden               | `eu_vat`     | European VAT number                                                                                     |
-              | Switzerland          | `ch_vat`     | Switzerland VAT number                                                                                  |
+              | Spain                | `es_cif`     | Spanish NIF Number (previously Spanish CIF Number)                                                      |
+              | Spain                | `eu_vat`     | European VAT Number                                                                                     |
+              | Sweden               | `eu_vat`     | European VAT Number                                                                                     |
+              | Switzerland          | `ch_vat`     | Switzerland VAT Number                                                                                  |
               | Taiwan               | `tw_vat`     | Taiwanese VAT                                                                                           |
               | Thailand             | `th_vat`     | Thai VAT                                                                                                |
               | Turkey               | `tr_tin`     | Turkish Tax Identification Number                                                                       |
               | Ukraine              | `ua_vat`     | Ukrainian VAT                                                                                           |
               | United Arab Emirates | `ae_trn`     | United Arab Emirates TRN                                                                                |
-              | United Kingdom       | `eu_vat`     | Northern Ireland VAT number                                                                             |
-              | United Kingdom       | `gb_vat`     | United Kingdom VAT number                                                                               |
+              | United Kingdom       | `eu_vat`     | Northern Ireland VAT Number                                                                             |
+              | United Kingdom       | `gb_vat`     | United Kingdom VAT Number                                                                               |
               | United States        | `us_ein`     | United States EIN                                                                                       |
+              | Uruguay              | `uy_ruc`     | Uruguayan RUC Number                                                                                    |
+              | Venezuela            | `ve_rif`     | Venezuelan RIF Number                                                                                   |
+              | Vietnam              | `vn_tin`     | Vietnamese Tax ID Number                                                                                |
 
           timezone: A timezone identifier from the IANA timezone database, such as
               `"America/Los_Angeles"`. This defaults to your account's timezone if not set.
               This cannot be changed after customer creation.
 
           extra_headers: Send extra headers
 
@@ -371,92 +391,112 @@
           tax_id: Tax IDs are commonly required to be displayed on customer invoices, which are
               added to the headers of invoices.
 
               ### Supported Tax ID Countries and Types
 
               | Country              | Type         | Description                                                                                             |
               | -------------------- | ------------ | ------------------------------------------------------------------------------------------------------- |
-              | Andorra              | `ad_nrt`     | Andorran NRT number                                                                                     |
+              | Andorra              | `ad_nrt`     | Andorran NRT Number                                                                                     |
+              | Argentina            | `ar_cuit`    | Argentinian Tax ID Number                                                                               |
               | Australia            | `au_abn`     | Australian Business Number (AU ABN)                                                                     |
               | Australia            | `au_arn`     | Australian Taxation Office Reference Number                                                             |
-              | Austria              | `eu_vat`     | European VAT number                                                                                     |
-              | Belgium              | `eu_vat`     | European VAT number                                                                                     |
-              | Brazil               | `br_cnpj`    | Brazilian CNPJ number                                                                                   |
-              | Brazil               | `br_cpf`     | Brazilian CPF number                                                                                    |
+              | Austria              | `eu_vat`     | European VAT Number                                                                                     |
+              | Bahrain              | `bh_vat`     | Bahraini VAT Number                                                                                     |
+              | Belgium              | `eu_vat`     | European VAT Number                                                                                     |
+              | Bolivia              | `bo_tin`     | Bolivian Tax ID                                                                                         |
+              | Brazil               | `br_cnpj`    | Brazilian CNPJ Number                                                                                   |
+              | Brazil               | `br_cpf`     | Brazilian CPF Number                                                                                    |
               | Bulgaria             | `bg_uic`     | Bulgaria Unified Identification Code                                                                    |
-              | Bulgaria             | `eu_vat`     | European VAT number                                                                                     |
+              | Bulgaria             | `eu_vat`     | European VAT Number                                                                                     |
               | Canada               | `ca_bn`      | Canadian BN                                                                                             |
-              | Canada               | `ca_gst_hst` | Canadian GST/HST number                                                                                 |
-              | Canada               | `ca_pst_bc`  | Canadian PST number (British Columbia)                                                                  |
-              | Canada               | `ca_pst_mb`  | Canadian PST number (Manitoba)                                                                          |
-              | Canada               | `ca_pst_sk`  | Canadian PST number (Saskatchewan)                                                                      |
-              | Canada               | `ca_qst`     | Canadian QST number (Québec)                                                                            |
+              | Canada               | `ca_gst_hst` | Canadian GST/HST Number                                                                                 |
+              | Canada               | `ca_pst_bc`  | Canadian PST Number (British Columbia)                                                                  |
+              | Canada               | `ca_pst_mb`  | Canadian PST Number (Manitoba)                                                                          |
+              | Canada               | `ca_pst_sk`  | Canadian PST Number (Saskatchewan)                                                                      |
+              | Canada               | `ca_qst`     | Canadian QST Number (Québec)                                                                            |
               | Chile                | `cl_tin`     | Chilean TIN                                                                                             |
-              | Croatia              | `eu_vat`     | European VAT number                                                                                     |
-              | Cyprus               | `eu_vat`     | European VAT number                                                                                     |
-              | Czech Republic       | `eu_vat`     | European VAT number                                                                                     |
-              | Denmark              | `eu_vat`     | European VAT number                                                                                     |
+              | China                | `cn_tin`     | Chinese Tax ID                                                                                          |
+              | Colombia             | `co_nit`     | Colombian NIT Number                                                                                    |
+              | Costa Rica           | `cr_tin`     | Costa Rican Tax ID                                                                                      |
+              | Croatia              | `eu_vat`     | European VAT Number                                                                                     |
+              | Cyprus               | `eu_vat`     | European VAT Number                                                                                     |
+              | Czech Republic       | `eu_vat`     | European VAT Number                                                                                     |
+              | Denmark              | `eu_vat`     | European VAT Number                                                                                     |
+              | Dominican Republic   | `do_rcn`     | Dominican RCN Number                                                                                    |
+              | Ecuador              | `ec_ruc`     | Ecuadorian RUC Number                                                                                   |
               | Egypt                | `eg_tin`     | Egyptian Tax Identification Number                                                                      |
-              | Estonia              | `eu_vat`     | European VAT number                                                                                     |
-              | EU                   | `eu_oss_vat` | European One Stop Shop VAT number for non-Union scheme                                                  |
-              | Finland              | `eu_vat`     | European VAT number                                                                                     |
-              | France               | `eu_vat`     | European VAT number                                                                                     |
+              | El Salvador          | `sv_nit`     | El Salvadorian NIT Number                                                                               |
+              | Estonia              | `eu_vat`     | European VAT Number                                                                                     |
+              | EU                   | `eu_oss_vat` | European One Stop Shop VAT Number for non-Union scheme                                                  |
+              | Finland              | `eu_vat`     | European VAT Number                                                                                     |
+              | France               | `eu_vat`     | European VAT Number                                                                                     |
               | Georgia              | `ge_vat`     | Georgian VAT                                                                                            |
-              | Germany              | `eu_vat`     | European VAT number                                                                                     |
-              | Greece               | `eu_vat`     | European VAT number                                                                                     |
-              | Hong Kong            | `hk_br`      | Hong Kong BR number                                                                                     |
-              | Hungary              | `eu_vat`     | European VAT number                                                                                     |
-              | Hungary              | `hu_tin`     | Hungary tax number (adószám)                                                                            |
+              | Germany              | `eu_vat`     | European VAT Number                                                                                     |
+              | Greece               | `eu_vat`     | European VAT Number                                                                                     |
+              | Hong Kong            | `hk_br`      | Hong Kong BR Number                                                                                     |
+              | Hungary              | `eu_vat`     | European VAT Number                                                                                     |
+              | Hungary              | `hu_tin`     | Hungary Tax Number (adószám)                                                                            |
               | Iceland              | `is_vat`     | Icelandic VAT                                                                                           |
-              | India                | `in_gst`     | Indian GST number                                                                                       |
-              | Indonesia            | `id_npwp`    | Indonesian NPWP number                                                                                  |
-              | Ireland              | `eu_vat`     | European VAT number                                                                                     |
+              | India                | `in_gst`     | Indian GST Number                                                                                       |
+              | Indonesia            | `id_npwp`    | Indonesian NPWP Number                                                                                  |
+              | Ireland              | `eu_vat`     | European VAT Number                                                                                     |
               | Israel               | `il_vat`     | Israel VAT                                                                                              |
-              | Italy                | `eu_vat`     | European VAT number                                                                                     |
+              | Italy                | `eu_vat`     | European VAT Number                                                                                     |
               | Japan                | `jp_cn`      | Japanese Corporate Number (_Hōjin Bangō_)                                                               |
               | Japan                | `jp_rn`      | Japanese Registered Foreign Businesses' Registration Number (_Tōroku Kokugai Jigyōsha no Tōroku Bangō_) |
               | Japan                | `jp_trn`     | Japanese Tax Registration Number (_Tōroku Bangō_)                                                       |
+              | Kazakhstan           | `kz_bin`     | Kazakhstani Business Identification Number                                                              |
               | Kenya                | `ke_pin`     | Kenya Revenue Authority Personal Identification Number                                                  |
-              | Latvia               | `eu_vat`     | European VAT number                                                                                     |
-              | Liechtenstein        | `li_uid`     | Liechtensteinian UID number                                                                             |
-              | Lithuania            | `eu_vat`     | European VAT number                                                                                     |
-              | Luxembourg           | `eu_vat`     | European VAT number                                                                                     |
-              | Malaysia             | `my_frp`     | Malaysian FRP number                                                                                    |
+              | Latvia               | `eu_vat`     | European VAT Number                                                                                     |
+              | Liechtenstein        | `li_uid`     | Liechtensteinian UID Number                                                                             |
+              | Lithuania            | `eu_vat`     | European VAT Number                                                                                     |
+              | Luxembourg           | `eu_vat`     | European VAT Number                                                                                     |
+              | Malaysia             | `my_frp`     | Malaysian FRP Number                                                                                    |
               | Malaysia             | `my_itn`     | Malaysian ITN                                                                                           |
-              | Malaysia             | `my_sst`     | Malaysian SST number                                                                                    |
-              | Malta                | `eu_vat `    | European VAT number                                                                                     |
-              | Mexico               | `mx_rfc`     | Mexican RFC number                                                                                      |
-              | Netherlands          | `eu_vat`     | European VAT number                                                                                     |
-              | New Zealand          | `nz_gst`     | New Zealand GST number                                                                                  |
-              | Norway               | `no_vat`     | Norwegian VAT number                                                                                    |
+              | Malaysia             | `my_sst`     | Malaysian SST Number                                                                                    |
+              | Malta                | `eu_vat `    | European VAT Number                                                                                     |
+              | Mexico               | `mx_rfc`     | Mexican RFC Number                                                                                      |
+              | Netherlands          | `eu_vat`     | European VAT Number                                                                                     |
+              | New Zealand          | `nz_gst`     | New Zealand GST Number                                                                                  |
+              | Nigeria              | `ng_tin`     | Nigerian Tax Identification Number                                                                      |
+              | Norway               | `no_vat`     | Norwegian VAT Number                                                                                    |
+              | Norway               | `no_voec`    | Norwegian VAT on e-commerce Number                                                                      |
+              | Oman                 | `om_vat`     | Omani VAT Number                                                                                        |
+              | Peru                 | `pe_ruc`     | Peruvian RUC Number                                                                                     |
               | Philippines          | `ph_tin `    | Philippines Tax Identification Number                                                                   |
-              | Poland               | `eu_vat`     | European VAT number                                                                                     |
-              | Portugal             | `eu_vat`     | European VAT number                                                                                     |
-              | Romania              | `eu_vat`     | European VAT number                                                                                     |
+              | Poland               | `eu_vat`     | European VAT Number                                                                                     |
+              | Portugal             | `eu_vat`     | European VAT Number                                                                                     |
+              | Romania              | `eu_vat`     | European VAT Number                                                                                     |
+              | Romania              | `ro_tin`     | Romanian Tax ID Number                                                                                  |
               | Russia               | `ru_inn`     | Russian INN                                                                                             |
               | Russia               | `ru_kpp`     | Russian KPP                                                                                             |
-              | Saudi Arabia         | `sg_gst`     | Singaporean GST                                                                                         |
+              | Saudi Arabia         | `sa_vat`     | Saudi Arabia VAT                                                                                        |
+              | Serbia               | `rs_pib`     | Serbian PIB Number                                                                                      |
+              | Singapore            | `sg_gst`     | Singaporean GST                                                                                         |
               | Singapore            | `sg_uen`     | Singaporean UEN                                                                                         |
-              | Slovakia             | `eu_vat`     | European VAT number                                                                                     |
-              | Slovenia             | `eu_vat`     | European VAT number                                                                                     |
-              | Slovenia             | `si_tin`     | Slovenia tax number (davčna številka)                                                                   |
-              | South Africa         | `za_vat`     | South African VAT number                                                                                |
+              | Slovakia             | `eu_vat`     | European VAT Number                                                                                     |
+              | Slovenia             | `eu_vat`     | European VAT Number                                                                                     |
+              | Slovenia             | `si_tin`     | Slovenia Tax Number (davčna številka)                                                                   |
+              | South Africa         | `za_vat`     | South African VAT Number                                                                                |
               | South Korea          | `kr_brn`     | Korean BRN                                                                                              |
-              | Spain                | `es_cif`     | Spanish NIF number (previously Spanish CIF number)                                                      |
-              | Spain                | `eu_vat`     | European VAT number                                                                                     |
-              | Sweden               | `eu_vat`     | European VAT number                                                                                     |
-              | Switzerland          | `ch_vat`     | Switzerland VAT number                                                                                  |
+              | Spain                | `es_cif`     | Spanish NIF Number (previously Spanish CIF Number)                                                      |
+              | Spain                | `eu_vat`     | European VAT Number                                                                                     |
+              | Sweden               | `eu_vat`     | European VAT Number                                                                                     |
+              | Switzerland          | `ch_vat`     | Switzerland VAT Number                                                                                  |
               | Taiwan               | `tw_vat`     | Taiwanese VAT                                                                                           |
               | Thailand             | `th_vat`     | Thai VAT                                                                                                |
               | Turkey               | `tr_tin`     | Turkish Tax Identification Number                                                                       |
               | Ukraine              | `ua_vat`     | Ukrainian VAT                                                                                           |
               | United Arab Emirates | `ae_trn`     | United Arab Emirates TRN                                                                                |
-              | United Kingdom       | `eu_vat`     | Northern Ireland VAT number                                                                             |
-              | United Kingdom       | `gb_vat`     | United Kingdom VAT number                                                                               |
+              | United Kingdom       | `eu_vat`     | Northern Ireland VAT Number                                                                             |
+              | United Kingdom       | `gb_vat`     | United Kingdom VAT Number                                                                               |
               | United States        | `us_ein`     | United States EIN                                                                                       |
+              | Uruguay              | `uy_ruc`     | Uruguayan RUC Number                                                                                    |
+              | Venezuela            | `ve_rif`     | Venezuelan RIF Number                                                                                   |
+              | Vietnam              | `vn_tin`     | Vietnamese Tax ID Number                                                                                |
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
@@ -763,92 +803,112 @@
           tax_id: Tax IDs are commonly required to be displayed on customer invoices, which are
               added to the headers of invoices.
 
               ### Supported Tax ID Countries and Types
 
               | Country              | Type         | Description                                                                                             |
               | -------------------- | ------------ | ------------------------------------------------------------------------------------------------------- |
-              | Andorra              | `ad_nrt`     | Andorran NRT number                                                                                     |
+              | Andorra              | `ad_nrt`     | Andorran NRT Number                                                                                     |
+              | Argentina            | `ar_cuit`    | Argentinian Tax ID Number                                                                               |
               | Australia            | `au_abn`     | Australian Business Number (AU ABN)                                                                     |
               | Australia            | `au_arn`     | Australian Taxation Office Reference Number                                                             |
-              | Austria              | `eu_vat`     | European VAT number                                                                                     |
-              | Belgium              | `eu_vat`     | European VAT number                                                                                     |
-              | Brazil               | `br_cnpj`    | Brazilian CNPJ number                                                                                   |
-              | Brazil               | `br_cpf`     | Brazilian CPF number                                                                                    |
+              | Austria              | `eu_vat`     | European VAT Number                                                                                     |
+              | Bahrain              | `bh_vat`     | Bahraini VAT Number                                                                                     |
+              | Belgium              | `eu_vat`     | European VAT Number                                                                                     |
+              | Bolivia              | `bo_tin`     | Bolivian Tax ID                                                                                         |
+              | Brazil               | `br_cnpj`    | Brazilian CNPJ Number                                                                                   |
+              | Brazil               | `br_cpf`     | Brazilian CPF Number                                                                                    |
               | Bulgaria             | `bg_uic`     | Bulgaria Unified Identification Code                                                                    |
-              | Bulgaria             | `eu_vat`     | European VAT number                                                                                     |
+              | Bulgaria             | `eu_vat`     | European VAT Number                                                                                     |
               | Canada               | `ca_bn`      | Canadian BN                                                                                             |
-              | Canada               | `ca_gst_hst` | Canadian GST/HST number                                                                                 |
-              | Canada               | `ca_pst_bc`  | Canadian PST number (British Columbia)                                                                  |
-              | Canada               | `ca_pst_mb`  | Canadian PST number (Manitoba)                                                                          |
-              | Canada               | `ca_pst_sk`  | Canadian PST number (Saskatchewan)                                                                      |
-              | Canada               | `ca_qst`     | Canadian QST number (Québec)                                                                            |
+              | Canada               | `ca_gst_hst` | Canadian GST/HST Number                                                                                 |
+              | Canada               | `ca_pst_bc`  | Canadian PST Number (British Columbia)                                                                  |
+              | Canada               | `ca_pst_mb`  | Canadian PST Number (Manitoba)                                                                          |
+              | Canada               | `ca_pst_sk`  | Canadian PST Number (Saskatchewan)                                                                      |
+              | Canada               | `ca_qst`     | Canadian QST Number (Québec)                                                                            |
               | Chile                | `cl_tin`     | Chilean TIN                                                                                             |
-              | Croatia              | `eu_vat`     | European VAT number                                                                                     |
-              | Cyprus               | `eu_vat`     | European VAT number                                                                                     |
-              | Czech Republic       | `eu_vat`     | European VAT number                                                                                     |
-              | Denmark              | `eu_vat`     | European VAT number                                                                                     |
+              | China                | `cn_tin`     | Chinese Tax ID                                                                                          |
+              | Colombia             | `co_nit`     | Colombian NIT Number                                                                                    |
+              | Costa Rica           | `cr_tin`     | Costa Rican Tax ID                                                                                      |
+              | Croatia              | `eu_vat`     | European VAT Number                                                                                     |
+              | Cyprus               | `eu_vat`     | European VAT Number                                                                                     |
+              | Czech Republic       | `eu_vat`     | European VAT Number                                                                                     |
+              | Denmark              | `eu_vat`     | European VAT Number                                                                                     |
+              | Dominican Republic   | `do_rcn`     | Dominican RCN Number                                                                                    |
+              | Ecuador              | `ec_ruc`     | Ecuadorian RUC Number                                                                                   |
               | Egypt                | `eg_tin`     | Egyptian Tax Identification Number                                                                      |
-              | Estonia              | `eu_vat`     | European VAT number                                                                                     |
-              | EU                   | `eu_oss_vat` | European One Stop Shop VAT number for non-Union scheme                                                  |
-              | Finland              | `eu_vat`     | European VAT number                                                                                     |
-              | France               | `eu_vat`     | European VAT number                                                                                     |
+              | El Salvador          | `sv_nit`     | El Salvadorian NIT Number                                                                               |
+              | Estonia              | `eu_vat`     | European VAT Number                                                                                     |
+              | EU                   | `eu_oss_vat` | European One Stop Shop VAT Number for non-Union scheme                                                  |
+              | Finland              | `eu_vat`     | European VAT Number                                                                                     |
+              | France               | `eu_vat`     | European VAT Number                                                                                     |
               | Georgia              | `ge_vat`     | Georgian VAT                                                                                            |
-              | Germany              | `eu_vat`     | European VAT number                                                                                     |
-              | Greece               | `eu_vat`     | European VAT number                                                                                     |
-              | Hong Kong            | `hk_br`      | Hong Kong BR number                                                                                     |
-              | Hungary              | `eu_vat`     | European VAT number                                                                                     |
-              | Hungary              | `hu_tin`     | Hungary tax number (adószám)                                                                            |
+              | Germany              | `eu_vat`     | European VAT Number                                                                                     |
+              | Greece               | `eu_vat`     | European VAT Number                                                                                     |
+              | Hong Kong            | `hk_br`      | Hong Kong BR Number                                                                                     |
+              | Hungary              | `eu_vat`     | European VAT Number                                                                                     |
+              | Hungary              | `hu_tin`     | Hungary Tax Number (adószám)                                                                            |
               | Iceland              | `is_vat`     | Icelandic VAT                                                                                           |
-              | India                | `in_gst`     | Indian GST number                                                                                       |
-              | Indonesia            | `id_npwp`    | Indonesian NPWP number                                                                                  |
-              | Ireland              | `eu_vat`     | European VAT number                                                                                     |
+              | India                | `in_gst`     | Indian GST Number                                                                                       |
+              | Indonesia            | `id_npwp`    | Indonesian NPWP Number                                                                                  |
+              | Ireland              | `eu_vat`     | European VAT Number                                                                                     |
               | Israel               | `il_vat`     | Israel VAT                                                                                              |
-              | Italy                | `eu_vat`     | European VAT number                                                                                     |
+              | Italy                | `eu_vat`     | European VAT Number                                                                                     |
               | Japan                | `jp_cn`      | Japanese Corporate Number (_Hōjin Bangō_)                                                               |
               | Japan                | `jp_rn`      | Japanese Registered Foreign Businesses' Registration Number (_Tōroku Kokugai Jigyōsha no Tōroku Bangō_) |
               | Japan                | `jp_trn`     | Japanese Tax Registration Number (_Tōroku Bangō_)                                                       |
+              | Kazakhstan           | `kz_bin`     | Kazakhstani Business Identification Number                                                              |
               | Kenya                | `ke_pin`     | Kenya Revenue Authority Personal Identification Number                                                  |
-              | Latvia               | `eu_vat`     | European VAT number                                                                                     |
-              | Liechtenstein        | `li_uid`     | Liechtensteinian UID number                                                                             |
-              | Lithuania            | `eu_vat`     | European VAT number                                                                                     |
-              | Luxembourg           | `eu_vat`     | European VAT number                                                                                     |
-              | Malaysia             | `my_frp`     | Malaysian FRP number                                                                                    |
+              | Latvia               | `eu_vat`     | European VAT Number                                                                                     |
+              | Liechtenstein        | `li_uid`     | Liechtensteinian UID Number                                                                             |
+              | Lithuania            | `eu_vat`     | European VAT Number                                                                                     |
+              | Luxembourg           | `eu_vat`     | European VAT Number                                                                                     |
+              | Malaysia             | `my_frp`     | Malaysian FRP Number                                                                                    |
               | Malaysia             | `my_itn`     | Malaysian ITN                                                                                           |
-              | Malaysia             | `my_sst`     | Malaysian SST number                                                                                    |
-              | Malta                | `eu_vat `    | European VAT number                                                                                     |
-              | Mexico               | `mx_rfc`     | Mexican RFC number                                                                                      |
-              | Netherlands          | `eu_vat`     | European VAT number                                                                                     |
-              | New Zealand          | `nz_gst`     | New Zealand GST number                                                                                  |
-              | Norway               | `no_vat`     | Norwegian VAT number                                                                                    |
+              | Malaysia             | `my_sst`     | Malaysian SST Number                                                                                    |
+              | Malta                | `eu_vat `    | European VAT Number                                                                                     |
+              | Mexico               | `mx_rfc`     | Mexican RFC Number                                                                                      |
+              | Netherlands          | `eu_vat`     | European VAT Number                                                                                     |
+              | New Zealand          | `nz_gst`     | New Zealand GST Number                                                                                  |
+              | Nigeria              | `ng_tin`     | Nigerian Tax Identification Number                                                                      |
+              | Norway               | `no_vat`     | Norwegian VAT Number                                                                                    |
+              | Norway               | `no_voec`    | Norwegian VAT on e-commerce Number                                                                      |
+              | Oman                 | `om_vat`     | Omani VAT Number                                                                                        |
+              | Peru                 | `pe_ruc`     | Peruvian RUC Number                                                                                     |
               | Philippines          | `ph_tin `    | Philippines Tax Identification Number                                                                   |
-              | Poland               | `eu_vat`     | European VAT number                                                                                     |
-              | Portugal             | `eu_vat`     | European VAT number                                                                                     |
-              | Romania              | `eu_vat`     | European VAT number                                                                                     |
+              | Poland               | `eu_vat`     | European VAT Number                                                                                     |
+              | Portugal             | `eu_vat`     | European VAT Number                                                                                     |
+              | Romania              | `eu_vat`     | European VAT Number                                                                                     |
+              | Romania              | `ro_tin`     | Romanian Tax ID Number                                                                                  |
               | Russia               | `ru_inn`     | Russian INN                                                                                             |
               | Russia               | `ru_kpp`     | Russian KPP                                                                                             |
-              | Saudi Arabia         | `sg_gst`     | Singaporean GST                                                                                         |
+              | Saudi Arabia         | `sa_vat`     | Saudi Arabia VAT                                                                                        |
+              | Serbia               | `rs_pib`     | Serbian PIB Number                                                                                      |
+              | Singapore            | `sg_gst`     | Singaporean GST                                                                                         |
               | Singapore            | `sg_uen`     | Singaporean UEN                                                                                         |
-              | Slovakia             | `eu_vat`     | European VAT number                                                                                     |
-              | Slovenia             | `eu_vat`     | European VAT number                                                                                     |
-              | Slovenia             | `si_tin`     | Slovenia tax number (davčna številka)                                                                   |
-              | South Africa         | `za_vat`     | South African VAT number                                                                                |
+              | Slovakia             | `eu_vat`     | European VAT Number                                                                                     |
+              | Slovenia             | `eu_vat`     | European VAT Number                                                                                     |
+              | Slovenia             | `si_tin`     | Slovenia Tax Number (davčna številka)                                                                   |
+              | South Africa         | `za_vat`     | South African VAT Number                                                                                |
               | South Korea          | `kr_brn`     | Korean BRN                                                                                              |
-              | Spain                | `es_cif`     | Spanish NIF number (previously Spanish CIF number)                                                      |
-              | Spain                | `eu_vat`     | European VAT number                                                                                     |
-              | Sweden               | `eu_vat`     | European VAT number                                                                                     |
-              | Switzerland          | `ch_vat`     | Switzerland VAT number                                                                                  |
+              | Spain                | `es_cif`     | Spanish NIF Number (previously Spanish CIF Number)                                                      |
+              | Spain                | `eu_vat`     | European VAT Number                                                                                     |
+              | Sweden               | `eu_vat`     | European VAT Number                                                                                     |
+              | Switzerland          | `ch_vat`     | Switzerland VAT Number                                                                                  |
               | Taiwan               | `tw_vat`     | Taiwanese VAT                                                                                           |
               | Thailand             | `th_vat`     | Thai VAT                                                                                                |
               | Turkey               | `tr_tin`     | Turkish Tax Identification Number                                                                       |
               | Ukraine              | `ua_vat`     | Ukrainian VAT                                                                                           |
               | United Arab Emirates | `ae_trn`     | United Arab Emirates TRN                                                                                |
-              | United Kingdom       | `eu_vat`     | Northern Ireland VAT number                                                                             |
-              | United Kingdom       | `gb_vat`     | United Kingdom VAT number                                                                               |
+              | United Kingdom       | `eu_vat`     | Northern Ireland VAT Number                                                                             |
+              | United Kingdom       | `gb_vat`     | United Kingdom VAT Number                                                                               |
               | United States        | `us_ein`     | United States EIN                                                                                       |
+              | Uruguay              | `uy_ruc`     | Uruguayan RUC Number                                                                                    |
+              | Venezuela            | `ve_rif`     | Venezuelan RIF Number                                                                                   |
+              | Vietnam              | `vn_tin`     | Vietnamese Tax ID Number                                                                                |
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
@@ -994,92 +1054,112 @@
           tax_id: Tax IDs are commonly required to be displayed on customer invoices, which are
               added to the headers of invoices.
 
               ### Supported Tax ID Countries and Types
 
               | Country              | Type         | Description                                                                                             |
               | -------------------- | ------------ | ------------------------------------------------------------------------------------------------------- |
-              | Andorra              | `ad_nrt`     | Andorran NRT number                                                                                     |
+              | Andorra              | `ad_nrt`     | Andorran NRT Number                                                                                     |
+              | Argentina            | `ar_cuit`    | Argentinian Tax ID Number                                                                               |
               | Australia            | `au_abn`     | Australian Business Number (AU ABN)                                                                     |
               | Australia            | `au_arn`     | Australian Taxation Office Reference Number                                                             |
-              | Austria              | `eu_vat`     | European VAT number                                                                                     |
-              | Belgium              | `eu_vat`     | European VAT number                                                                                     |
-              | Brazil               | `br_cnpj`    | Brazilian CNPJ number                                                                                   |
-              | Brazil               | `br_cpf`     | Brazilian CPF number                                                                                    |
+              | Austria              | `eu_vat`     | European VAT Number                                                                                     |
+              | Bahrain              | `bh_vat`     | Bahraini VAT Number                                                                                     |
+              | Belgium              | `eu_vat`     | European VAT Number                                                                                     |
+              | Bolivia              | `bo_tin`     | Bolivian Tax ID                                                                                         |
+              | Brazil               | `br_cnpj`    | Brazilian CNPJ Number                                                                                   |
+              | Brazil               | `br_cpf`     | Brazilian CPF Number                                                                                    |
               | Bulgaria             | `bg_uic`     | Bulgaria Unified Identification Code                                                                    |
-              | Bulgaria             | `eu_vat`     | European VAT number                                                                                     |
+              | Bulgaria             | `eu_vat`     | European VAT Number                                                                                     |
               | Canada               | `ca_bn`      | Canadian BN                                                                                             |
-              | Canada               | `ca_gst_hst` | Canadian GST/HST number                                                                                 |
-              | Canada               | `ca_pst_bc`  | Canadian PST number (British Columbia)                                                                  |
-              | Canada               | `ca_pst_mb`  | Canadian PST number (Manitoba)                                                                          |
-              | Canada               | `ca_pst_sk`  | Canadian PST number (Saskatchewan)                                                                      |
-              | Canada               | `ca_qst`     | Canadian QST number (Québec)                                                                            |
+              | Canada               | `ca_gst_hst` | Canadian GST/HST Number                                                                                 |
+              | Canada               | `ca_pst_bc`  | Canadian PST Number (British Columbia)                                                                  |
+              | Canada               | `ca_pst_mb`  | Canadian PST Number (Manitoba)                                                                          |
+              | Canada               | `ca_pst_sk`  | Canadian PST Number (Saskatchewan)                                                                      |
+              | Canada               | `ca_qst`     | Canadian QST Number (Québec)                                                                            |
               | Chile                | `cl_tin`     | Chilean TIN                                                                                             |
-              | Croatia              | `eu_vat`     | European VAT number                                                                                     |
-              | Cyprus               | `eu_vat`     | European VAT number                                                                                     |
-              | Czech Republic       | `eu_vat`     | European VAT number                                                                                     |
-              | Denmark              | `eu_vat`     | European VAT number                                                                                     |
+              | China                | `cn_tin`     | Chinese Tax ID                                                                                          |
+              | Colombia             | `co_nit`     | Colombian NIT Number                                                                                    |
+              | Costa Rica           | `cr_tin`     | Costa Rican Tax ID                                                                                      |
+              | Croatia              | `eu_vat`     | European VAT Number                                                                                     |
+              | Cyprus               | `eu_vat`     | European VAT Number                                                                                     |
+              | Czech Republic       | `eu_vat`     | European VAT Number                                                                                     |
+              | Denmark              | `eu_vat`     | European VAT Number                                                                                     |
+              | Dominican Republic   | `do_rcn`     | Dominican RCN Number                                                                                    |
+              | Ecuador              | `ec_ruc`     | Ecuadorian RUC Number                                                                                   |
               | Egypt                | `eg_tin`     | Egyptian Tax Identification Number                                                                      |
-              | Estonia              | `eu_vat`     | European VAT number                                                                                     |
-              | EU                   | `eu_oss_vat` | European One Stop Shop VAT number for non-Union scheme                                                  |
-              | Finland              | `eu_vat`     | European VAT number                                                                                     |
-              | France               | `eu_vat`     | European VAT number                                                                                     |
+              | El Salvador          | `sv_nit`     | El Salvadorian NIT Number                                                                               |
+              | Estonia              | `eu_vat`     | European VAT Number                                                                                     |
+              | EU                   | `eu_oss_vat` | European One Stop Shop VAT Number for non-Union scheme                                                  |
+              | Finland              | `eu_vat`     | European VAT Number                                                                                     |
+              | France               | `eu_vat`     | European VAT Number                                                                                     |
               | Georgia              | `ge_vat`     | Georgian VAT                                                                                            |
-              | Germany              | `eu_vat`     | European VAT number                                                                                     |
-              | Greece               | `eu_vat`     | European VAT number                                                                                     |
-              | Hong Kong            | `hk_br`      | Hong Kong BR number                                                                                     |
-              | Hungary              | `eu_vat`     | European VAT number                                                                                     |
-              | Hungary              | `hu_tin`     | Hungary tax number (adószám)                                                                            |
+              | Germany              | `eu_vat`     | European VAT Number                                                                                     |
+              | Greece               | `eu_vat`     | European VAT Number                                                                                     |
+              | Hong Kong            | `hk_br`      | Hong Kong BR Number                                                                                     |
+              | Hungary              | `eu_vat`     | European VAT Number                                                                                     |
+              | Hungary              | `hu_tin`     | Hungary Tax Number (adószám)                                                                            |
               | Iceland              | `is_vat`     | Icelandic VAT                                                                                           |
-              | India                | `in_gst`     | Indian GST number                                                                                       |
-              | Indonesia            | `id_npwp`    | Indonesian NPWP number                                                                                  |
-              | Ireland              | `eu_vat`     | European VAT number                                                                                     |
+              | India                | `in_gst`     | Indian GST Number                                                                                       |
+              | Indonesia            | `id_npwp`    | Indonesian NPWP Number                                                                                  |
+              | Ireland              | `eu_vat`     | European VAT Number                                                                                     |
               | Israel               | `il_vat`     | Israel VAT                                                                                              |
-              | Italy                | `eu_vat`     | European VAT number                                                                                     |
+              | Italy                | `eu_vat`     | European VAT Number                                                                                     |
               | Japan                | `jp_cn`      | Japanese Corporate Number (_Hōjin Bangō_)                                                               |
               | Japan                | `jp_rn`      | Japanese Registered Foreign Businesses' Registration Number (_Tōroku Kokugai Jigyōsha no Tōroku Bangō_) |
               | Japan                | `jp_trn`     | Japanese Tax Registration Number (_Tōroku Bangō_)                                                       |
+              | Kazakhstan           | `kz_bin`     | Kazakhstani Business Identification Number                                                              |
               | Kenya                | `ke_pin`     | Kenya Revenue Authority Personal Identification Number                                                  |
-              | Latvia               | `eu_vat`     | European VAT number                                                                                     |
-              | Liechtenstein        | `li_uid`     | Liechtensteinian UID number                                                                             |
-              | Lithuania            | `eu_vat`     | European VAT number                                                                                     |
-              | Luxembourg           | `eu_vat`     | European VAT number                                                                                     |
-              | Malaysia             | `my_frp`     | Malaysian FRP number                                                                                    |
+              | Latvia               | `eu_vat`     | European VAT Number                                                                                     |
+              | Liechtenstein        | `li_uid`     | Liechtensteinian UID Number                                                                             |
+              | Lithuania            | `eu_vat`     | European VAT Number                                                                                     |
+              | Luxembourg           | `eu_vat`     | European VAT Number                                                                                     |
+              | Malaysia             | `my_frp`     | Malaysian FRP Number                                                                                    |
               | Malaysia             | `my_itn`     | Malaysian ITN                                                                                           |
-              | Malaysia             | `my_sst`     | Malaysian SST number                                                                                    |
-              | Malta                | `eu_vat `    | European VAT number                                                                                     |
-              | Mexico               | `mx_rfc`     | Mexican RFC number                                                                                      |
-              | Netherlands          | `eu_vat`     | European VAT number                                                                                     |
-              | New Zealand          | `nz_gst`     | New Zealand GST number                                                                                  |
-              | Norway               | `no_vat`     | Norwegian VAT number                                                                                    |
+              | Malaysia             | `my_sst`     | Malaysian SST Number                                                                                    |
+              | Malta                | `eu_vat `    | European VAT Number                                                                                     |
+              | Mexico               | `mx_rfc`     | Mexican RFC Number                                                                                      |
+              | Netherlands          | `eu_vat`     | European VAT Number                                                                                     |
+              | New Zealand          | `nz_gst`     | New Zealand GST Number                                                                                  |
+              | Nigeria              | `ng_tin`     | Nigerian Tax Identification Number                                                                      |
+              | Norway               | `no_vat`     | Norwegian VAT Number                                                                                    |
+              | Norway               | `no_voec`    | Norwegian VAT on e-commerce Number                                                                      |
+              | Oman                 | `om_vat`     | Omani VAT Number                                                                                        |
+              | Peru                 | `pe_ruc`     | Peruvian RUC Number                                                                                     |
               | Philippines          | `ph_tin `    | Philippines Tax Identification Number                                                                   |
-              | Poland               | `eu_vat`     | European VAT number                                                                                     |
-              | Portugal             | `eu_vat`     | European VAT number                                                                                     |
-              | Romania              | `eu_vat`     | European VAT number                                                                                     |
+              | Poland               | `eu_vat`     | European VAT Number                                                                                     |
+              | Portugal             | `eu_vat`     | European VAT Number                                                                                     |
+              | Romania              | `eu_vat`     | European VAT Number                                                                                     |
+              | Romania              | `ro_tin`     | Romanian Tax ID Number                                                                                  |
               | Russia               | `ru_inn`     | Russian INN                                                                                             |
               | Russia               | `ru_kpp`     | Russian KPP                                                                                             |
-              | Saudi Arabia         | `sg_gst`     | Singaporean GST                                                                                         |
+              | Saudi Arabia         | `sa_vat`     | Saudi Arabia VAT                                                                                        |
+              | Serbia               | `rs_pib`     | Serbian PIB Number                                                                                      |
+              | Singapore            | `sg_gst`     | Singaporean GST                                                                                         |
               | Singapore            | `sg_uen`     | Singaporean UEN                                                                                         |
-              | Slovakia             | `eu_vat`     | European VAT number                                                                                     |
-              | Slovenia             | `eu_vat`     | European VAT number                                                                                     |
-              | Slovenia             | `si_tin`     | Slovenia tax number (davčna številka)                                                                   |
-              | South Africa         | `za_vat`     | South African VAT number                                                                                |
+              | Slovakia             | `eu_vat`     | European VAT Number                                                                                     |
+              | Slovenia             | `eu_vat`     | European VAT Number                                                                                     |
+              | Slovenia             | `si_tin`     | Slovenia Tax Number (davčna številka)                                                                   |
+              | South Africa         | `za_vat`     | South African VAT Number                                                                                |
               | South Korea          | `kr_brn`     | Korean BRN                                                                                              |
-              | Spain                | `es_cif`     | Spanish NIF number (previously Spanish CIF number)                                                      |
-              | Spain                | `eu_vat`     | European VAT number                                                                                     |
-              | Sweden               | `eu_vat`     | European VAT number                                                                                     |
-              | Switzerland          | `ch_vat`     | Switzerland VAT number                                                                                  |
+              | Spain                | `es_cif`     | Spanish NIF Number (previously Spanish CIF Number)                                                      |
+              | Spain                | `eu_vat`     | European VAT Number                                                                                     |
+              | Sweden               | `eu_vat`     | European VAT Number                                                                                     |
+              | Switzerland          | `ch_vat`     | Switzerland VAT Number                                                                                  |
               | Taiwan               | `tw_vat`     | Taiwanese VAT                                                                                           |
               | Thailand             | `th_vat`     | Thai VAT                                                                                                |
               | Turkey               | `tr_tin`     | Turkish Tax Identification Number                                                                       |
               | Ukraine              | `ua_vat`     | Ukrainian VAT                                                                                           |
               | United Arab Emirates | `ae_trn`     | United Arab Emirates TRN                                                                                |
-              | United Kingdom       | `eu_vat`     | Northern Ireland VAT number                                                                             |
-              | United Kingdom       | `gb_vat`     | United Kingdom VAT number                                                                               |
+              | United Kingdom       | `eu_vat`     | Northern Ireland VAT Number                                                                             |
+              | United Kingdom       | `gb_vat`     | United Kingdom VAT Number                                                                               |
               | United States        | `us_ein`     | United States EIN                                                                                       |
+              | Uruguay              | `uy_ruc`     | Uruguayan RUC Number                                                                                    |
+              | Venezuela            | `ve_rif`     | Venezuelan RIF Number                                                                                   |
+              | Vietnam              | `vn_tin`     | Vietnamese Tax ID Number                                                                                |
 
           timezone: A timezone identifier from the IANA timezone database, such as
               `"America/Los_Angeles"`. This defaults to your account's timezone if not set.
               This cannot be changed after customer creation.
 
           extra_headers: Send extra headers
 
@@ -1196,92 +1276,112 @@
           tax_id: Tax IDs are commonly required to be displayed on customer invoices, which are
               added to the headers of invoices.
 
               ### Supported Tax ID Countries and Types
 
               | Country              | Type         | Description                                                                                             |
               | -------------------- | ------------ | ------------------------------------------------------------------------------------------------------- |
-              | Andorra              | `ad_nrt`     | Andorran NRT number                                                                                     |
+              | Andorra              | `ad_nrt`     | Andorran NRT Number                                                                                     |
+              | Argentina            | `ar_cuit`    | Argentinian Tax ID Number                                                                               |
               | Australia            | `au_abn`     | Australian Business Number (AU ABN)                                                                     |
               | Australia            | `au_arn`     | Australian Taxation Office Reference Number                                                             |
-              | Austria              | `eu_vat`     | European VAT number                                                                                     |
-              | Belgium              | `eu_vat`     | European VAT number                                                                                     |
-              | Brazil               | `br_cnpj`    | Brazilian CNPJ number                                                                                   |
-              | Brazil               | `br_cpf`     | Brazilian CPF number                                                                                    |
+              | Austria              | `eu_vat`     | European VAT Number                                                                                     |
+              | Bahrain              | `bh_vat`     | Bahraini VAT Number                                                                                     |
+              | Belgium              | `eu_vat`     | European VAT Number                                                                                     |
+              | Bolivia              | `bo_tin`     | Bolivian Tax ID                                                                                         |
+              | Brazil               | `br_cnpj`    | Brazilian CNPJ Number                                                                                   |
+              | Brazil               | `br_cpf`     | Brazilian CPF Number                                                                                    |
               | Bulgaria             | `bg_uic`     | Bulgaria Unified Identification Code                                                                    |
-              | Bulgaria             | `eu_vat`     | European VAT number                                                                                     |
+              | Bulgaria             | `eu_vat`     | European VAT Number                                                                                     |
               | Canada               | `ca_bn`      | Canadian BN                                                                                             |
-              | Canada               | `ca_gst_hst` | Canadian GST/HST number                                                                                 |
-              | Canada               | `ca_pst_bc`  | Canadian PST number (British Columbia)                                                                  |
-              | Canada               | `ca_pst_mb`  | Canadian PST number (Manitoba)                                                                          |
-              | Canada               | `ca_pst_sk`  | Canadian PST number (Saskatchewan)                                                                      |
-              | Canada               | `ca_qst`     | Canadian QST number (Québec)                                                                            |
+              | Canada               | `ca_gst_hst` | Canadian GST/HST Number                                                                                 |
+              | Canada               | `ca_pst_bc`  | Canadian PST Number (British Columbia)                                                                  |
+              | Canada               | `ca_pst_mb`  | Canadian PST Number (Manitoba)                                                                          |
+              | Canada               | `ca_pst_sk`  | Canadian PST Number (Saskatchewan)                                                                      |
+              | Canada               | `ca_qst`     | Canadian QST Number (Québec)                                                                            |
               | Chile                | `cl_tin`     | Chilean TIN                                                                                             |
-              | Croatia              | `eu_vat`     | European VAT number                                                                                     |
-              | Cyprus               | `eu_vat`     | European VAT number                                                                                     |
-              | Czech Republic       | `eu_vat`     | European VAT number                                                                                     |
-              | Denmark              | `eu_vat`     | European VAT number                                                                                     |
+              | China                | `cn_tin`     | Chinese Tax ID                                                                                          |
+              | Colombia             | `co_nit`     | Colombian NIT Number                                                                                    |
+              | Costa Rica           | `cr_tin`     | Costa Rican Tax ID                                                                                      |
+              | Croatia              | `eu_vat`     | European VAT Number                                                                                     |
+              | Cyprus               | `eu_vat`     | European VAT Number                                                                                     |
+              | Czech Republic       | `eu_vat`     | European VAT Number                                                                                     |
+              | Denmark              | `eu_vat`     | European VAT Number                                                                                     |
+              | Dominican Republic   | `do_rcn`     | Dominican RCN Number                                                                                    |
+              | Ecuador              | `ec_ruc`     | Ecuadorian RUC Number                                                                                   |
               | Egypt                | `eg_tin`     | Egyptian Tax Identification Number                                                                      |
-              | Estonia              | `eu_vat`     | European VAT number                                                                                     |
-              | EU                   | `eu_oss_vat` | European One Stop Shop VAT number for non-Union scheme                                                  |
-              | Finland              | `eu_vat`     | European VAT number                                                                                     |
-              | France               | `eu_vat`     | European VAT number                                                                                     |
+              | El Salvador          | `sv_nit`     | El Salvadorian NIT Number                                                                               |
+              | Estonia              | `eu_vat`     | European VAT Number                                                                                     |
+              | EU                   | `eu_oss_vat` | European One Stop Shop VAT Number for non-Union scheme                                                  |
+              | Finland              | `eu_vat`     | European VAT Number                                                                                     |
+              | France               | `eu_vat`     | European VAT Number                                                                                     |
               | Georgia              | `ge_vat`     | Georgian VAT                                                                                            |
-              | Germany              | `eu_vat`     | European VAT number                                                                                     |
-              | Greece               | `eu_vat`     | European VAT number                                                                                     |
-              | Hong Kong            | `hk_br`      | Hong Kong BR number                                                                                     |
-              | Hungary              | `eu_vat`     | European VAT number                                                                                     |
-              | Hungary              | `hu_tin`     | Hungary tax number (adószám)                                                                            |
+              | Germany              | `eu_vat`     | European VAT Number                                                                                     |
+              | Greece               | `eu_vat`     | European VAT Number                                                                                     |
+              | Hong Kong            | `hk_br`      | Hong Kong BR Number                                                                                     |
+              | Hungary              | `eu_vat`     | European VAT Number                                                                                     |
+              | Hungary              | `hu_tin`     | Hungary Tax Number (adószám)                                                                            |
               | Iceland              | `is_vat`     | Icelandic VAT                                                                                           |
-              | India                | `in_gst`     | Indian GST number                                                                                       |
-              | Indonesia            | `id_npwp`    | Indonesian NPWP number                                                                                  |
-              | Ireland              | `eu_vat`     | European VAT number                                                                                     |
+              | India                | `in_gst`     | Indian GST Number                                                                                       |
+              | Indonesia            | `id_npwp`    | Indonesian NPWP Number                                                                                  |
+              | Ireland              | `eu_vat`     | European VAT Number                                                                                     |
               | Israel               | `il_vat`     | Israel VAT                                                                                              |
-              | Italy                | `eu_vat`     | European VAT number                                                                                     |
+              | Italy                | `eu_vat`     | European VAT Number                                                                                     |
               | Japan                | `jp_cn`      | Japanese Corporate Number (_Hōjin Bangō_)                                                               |
               | Japan                | `jp_rn`      | Japanese Registered Foreign Businesses' Registration Number (_Tōroku Kokugai Jigyōsha no Tōroku Bangō_) |
               | Japan                | `jp_trn`     | Japanese Tax Registration Number (_Tōroku Bangō_)                                                       |
+              | Kazakhstan           | `kz_bin`     | Kazakhstani Business Identification Number                                                              |
               | Kenya                | `ke_pin`     | Kenya Revenue Authority Personal Identification Number                                                  |
-              | Latvia               | `eu_vat`     | European VAT number                                                                                     |
-              | Liechtenstein        | `li_uid`     | Liechtensteinian UID number                                                                             |
-              | Lithuania            | `eu_vat`     | European VAT number                                                                                     |
-              | Luxembourg           | `eu_vat`     | European VAT number                                                                                     |
-              | Malaysia             | `my_frp`     | Malaysian FRP number                                                                                    |
+              | Latvia               | `eu_vat`     | European VAT Number                                                                                     |
+              | Liechtenstein        | `li_uid`     | Liechtensteinian UID Number                                                                             |
+              | Lithuania            | `eu_vat`     | European VAT Number                                                                                     |
+              | Luxembourg           | `eu_vat`     | European VAT Number                                                                                     |
+              | Malaysia             | `my_frp`     | Malaysian FRP Number                                                                                    |
               | Malaysia             | `my_itn`     | Malaysian ITN                                                                                           |
-              | Malaysia             | `my_sst`     | Malaysian SST number                                                                                    |
-              | Malta                | `eu_vat `    | European VAT number                                                                                     |
-              | Mexico               | `mx_rfc`     | Mexican RFC number                                                                                      |
-              | Netherlands          | `eu_vat`     | European VAT number                                                                                     |
-              | New Zealand          | `nz_gst`     | New Zealand GST number                                                                                  |
-              | Norway               | `no_vat`     | Norwegian VAT number                                                                                    |
+              | Malaysia             | `my_sst`     | Malaysian SST Number                                                                                    |
+              | Malta                | `eu_vat `    | European VAT Number                                                                                     |
+              | Mexico               | `mx_rfc`     | Mexican RFC Number                                                                                      |
+              | Netherlands          | `eu_vat`     | European VAT Number                                                                                     |
+              | New Zealand          | `nz_gst`     | New Zealand GST Number                                                                                  |
+              | Nigeria              | `ng_tin`     | Nigerian Tax Identification Number                                                                      |
+              | Norway               | `no_vat`     | Norwegian VAT Number                                                                                    |
+              | Norway               | `no_voec`    | Norwegian VAT on e-commerce Number                                                                      |
+              | Oman                 | `om_vat`     | Omani VAT Number                                                                                        |
+              | Peru                 | `pe_ruc`     | Peruvian RUC Number                                                                                     |
               | Philippines          | `ph_tin `    | Philippines Tax Identification Number                                                                   |
-              | Poland               | `eu_vat`     | European VAT number                                                                                     |
-              | Portugal             | `eu_vat`     | European VAT number                                                                                     |
-              | Romania              | `eu_vat`     | European VAT number                                                                                     |
+              | Poland               | `eu_vat`     | European VAT Number                                                                                     |
+              | Portugal             | `eu_vat`     | European VAT Number                                                                                     |
+              | Romania              | `eu_vat`     | European VAT Number                                                                                     |
+              | Romania              | `ro_tin`     | Romanian Tax ID Number                                                                                  |
               | Russia               | `ru_inn`     | Russian INN                                                                                             |
               | Russia               | `ru_kpp`     | Russian KPP                                                                                             |
-              | Saudi Arabia         | `sg_gst`     | Singaporean GST                                                                                         |
+              | Saudi Arabia         | `sa_vat`     | Saudi Arabia VAT                                                                                        |
+              | Serbia               | `rs_pib`     | Serbian PIB Number                                                                                      |
+              | Singapore            | `sg_gst`     | Singaporean GST                                                                                         |
               | Singapore            | `sg_uen`     | Singaporean UEN                                                                                         |
-              | Slovakia             | `eu_vat`     | European VAT number                                                                                     |
-              | Slovenia             | `eu_vat`     | European VAT number                                                                                     |
-              | Slovenia             | `si_tin`     | Slovenia tax number (davčna številka)                                                                   |
-              | South Africa         | `za_vat`     | South African VAT number                                                                                |
+              | Slovakia             | `eu_vat`     | European VAT Number                                                                                     |
+              | Slovenia             | `eu_vat`     | European VAT Number                                                                                     |
+              | Slovenia             | `si_tin`     | Slovenia Tax Number (davčna številka)                                                                   |
+              | South Africa         | `za_vat`     | South African VAT Number                                                                                |
               | South Korea          | `kr_brn`     | Korean BRN                                                                                              |
-              | Spain                | `es_cif`     | Spanish NIF number (previously Spanish CIF number)                                                      |
-              | Spain                | `eu_vat`     | European VAT number                                                                                     |
-              | Sweden               | `eu_vat`     | European VAT number                                                                                     |
-              | Switzerland          | `ch_vat`     | Switzerland VAT number                                                                                  |
+              | Spain                | `es_cif`     | Spanish NIF Number (previously Spanish CIF Number)                                                      |
+              | Spain                | `eu_vat`     | European VAT Number                                                                                     |
+              | Sweden               | `eu_vat`     | European VAT Number                                                                                     |
+              | Switzerland          | `ch_vat`     | Switzerland VAT Number                                                                                  |
               | Taiwan               | `tw_vat`     | Taiwanese VAT                                                                                           |
               | Thailand             | `th_vat`     | Thai VAT                                                                                                |
               | Turkey               | `tr_tin`     | Turkish Tax Identification Number                                                                       |
               | Ukraine              | `ua_vat`     | Ukrainian VAT                                                                                           |
               | United Arab Emirates | `ae_trn`     | United Arab Emirates TRN                                                                                |
-              | United Kingdom       | `eu_vat`     | Northern Ireland VAT number                                                                             |
-              | United Kingdom       | `gb_vat`     | United Kingdom VAT number                                                                               |
+              | United Kingdom       | `eu_vat`     | Northern Ireland VAT Number                                                                             |
+              | United Kingdom       | `gb_vat`     | United Kingdom VAT Number                                                                               |
               | United States        | `us_ein`     | United States EIN                                                                                       |
+              | Uruguay              | `uy_ruc`     | Uruguayan RUC Number                                                                                    |
+              | Venezuela            | `ve_rif`     | Venezuelan RIF Number                                                                                   |
+              | Vietnam              | `vn_tin`     | Vietnamese Tax ID Number                                                                                |
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
@@ -1588,92 +1688,112 @@
           tax_id: Tax IDs are commonly required to be displayed on customer invoices, which are
               added to the headers of invoices.
 
               ### Supported Tax ID Countries and Types
 
               | Country              | Type         | Description                                                                                             |
               | -------------------- | ------------ | ------------------------------------------------------------------------------------------------------- |
-              | Andorra              | `ad_nrt`     | Andorran NRT number                                                                                     |
+              | Andorra              | `ad_nrt`     | Andorran NRT Number                                                                                     |
+              | Argentina            | `ar_cuit`    | Argentinian Tax ID Number                                                                               |
               | Australia            | `au_abn`     | Australian Business Number (AU ABN)                                                                     |
               | Australia            | `au_arn`     | Australian Taxation Office Reference Number                                                             |
-              | Austria              | `eu_vat`     | European VAT number                                                                                     |
-              | Belgium              | `eu_vat`     | European VAT number                                                                                     |
-              | Brazil               | `br_cnpj`    | Brazilian CNPJ number                                                                                   |
-              | Brazil               | `br_cpf`     | Brazilian CPF number                                                                                    |
+              | Austria              | `eu_vat`     | European VAT Number                                                                                     |
+              | Bahrain              | `bh_vat`     | Bahraini VAT Number                                                                                     |
+              | Belgium              | `eu_vat`     | European VAT Number                                                                                     |
+              | Bolivia              | `bo_tin`     | Bolivian Tax ID                                                                                         |
+              | Brazil               | `br_cnpj`    | Brazilian CNPJ Number                                                                                   |
+              | Brazil               | `br_cpf`     | Brazilian CPF Number                                                                                    |
               | Bulgaria             | `bg_uic`     | Bulgaria Unified Identification Code                                                                    |
-              | Bulgaria             | `eu_vat`     | European VAT number                                                                                     |
+              | Bulgaria             | `eu_vat`     | European VAT Number                                                                                     |
               | Canada               | `ca_bn`      | Canadian BN                                                                                             |
-              | Canada               | `ca_gst_hst` | Canadian GST/HST number                                                                                 |
-              | Canada               | `ca_pst_bc`  | Canadian PST number (British Columbia)                                                                  |
-              | Canada               | `ca_pst_mb`  | Canadian PST number (Manitoba)                                                                          |
-              | Canada               | `ca_pst_sk`  | Canadian PST number (Saskatchewan)                                                                      |
-              | Canada               | `ca_qst`     | Canadian QST number (Québec)                                                                            |
+              | Canada               | `ca_gst_hst` | Canadian GST/HST Number                                                                                 |
+              | Canada               | `ca_pst_bc`  | Canadian PST Number (British Columbia)                                                                  |
+              | Canada               | `ca_pst_mb`  | Canadian PST Number (Manitoba)                                                                          |
+              | Canada               | `ca_pst_sk`  | Canadian PST Number (Saskatchewan)                                                                      |
+              | Canada               | `ca_qst`     | Canadian QST Number (Québec)                                                                            |
               | Chile                | `cl_tin`     | Chilean TIN                                                                                             |
-              | Croatia              | `eu_vat`     | European VAT number                                                                                     |
-              | Cyprus               | `eu_vat`     | European VAT number                                                                                     |
-              | Czech Republic       | `eu_vat`     | European VAT number                                                                                     |
-              | Denmark              | `eu_vat`     | European VAT number                                                                                     |
+              | China                | `cn_tin`     | Chinese Tax ID                                                                                          |
+              | Colombia             | `co_nit`     | Colombian NIT Number                                                                                    |
+              | Costa Rica           | `cr_tin`     | Costa Rican Tax ID                                                                                      |
+              | Croatia              | `eu_vat`     | European VAT Number                                                                                     |
+              | Cyprus               | `eu_vat`     | European VAT Number                                                                                     |
+              | Czech Republic       | `eu_vat`     | European VAT Number                                                                                     |
+              | Denmark              | `eu_vat`     | European VAT Number                                                                                     |
+              | Dominican Republic   | `do_rcn`     | Dominican RCN Number                                                                                    |
+              | Ecuador              | `ec_ruc`     | Ecuadorian RUC Number                                                                                   |
               | Egypt                | `eg_tin`     | Egyptian Tax Identification Number                                                                      |
-              | Estonia              | `eu_vat`     | European VAT number                                                                                     |
-              | EU                   | `eu_oss_vat` | European One Stop Shop VAT number for non-Union scheme                                                  |
-              | Finland              | `eu_vat`     | European VAT number                                                                                     |
-              | France               | `eu_vat`     | European VAT number                                                                                     |
+              | El Salvador          | `sv_nit`     | El Salvadorian NIT Number                                                                               |
+              | Estonia              | `eu_vat`     | European VAT Number                                                                                     |
+              | EU                   | `eu_oss_vat` | European One Stop Shop VAT Number for non-Union scheme                                                  |
+              | Finland              | `eu_vat`     | European VAT Number                                                                                     |
+              | France               | `eu_vat`     | European VAT Number                                                                                     |
               | Georgia              | `ge_vat`     | Georgian VAT                                                                                            |
-              | Germany              | `eu_vat`     | European VAT number                                                                                     |
-              | Greece               | `eu_vat`     | European VAT number                                                                                     |
-              | Hong Kong            | `hk_br`      | Hong Kong BR number                                                                                     |
-              | Hungary              | `eu_vat`     | European VAT number                                                                                     |
-              | Hungary              | `hu_tin`     | Hungary tax number (adószám)                                                                            |
+              | Germany              | `eu_vat`     | European VAT Number                                                                                     |
+              | Greece               | `eu_vat`     | European VAT Number                                                                                     |
+              | Hong Kong            | `hk_br`      | Hong Kong BR Number                                                                                     |
+              | Hungary              | `eu_vat`     | European VAT Number                                                                                     |
+              | Hungary              | `hu_tin`     | Hungary Tax Number (adószám)                                                                            |
               | Iceland              | `is_vat`     | Icelandic VAT                                                                                           |
-              | India                | `in_gst`     | Indian GST number                                                                                       |
-              | Indonesia            | `id_npwp`    | Indonesian NPWP number                                                                                  |
-              | Ireland              | `eu_vat`     | European VAT number                                                                                     |
+              | India                | `in_gst`     | Indian GST Number                                                                                       |
+              | Indonesia            | `id_npwp`    | Indonesian NPWP Number                                                                                  |
+              | Ireland              | `eu_vat`     | European VAT Number                                                                                     |
               | Israel               | `il_vat`     | Israel VAT                                                                                              |
-              | Italy                | `eu_vat`     | European VAT number                                                                                     |
+              | Italy                | `eu_vat`     | European VAT Number                                                                                     |
               | Japan                | `jp_cn`      | Japanese Corporate Number (_Hōjin Bangō_)                                                               |
               | Japan                | `jp_rn`      | Japanese Registered Foreign Businesses' Registration Number (_Tōroku Kokugai Jigyōsha no Tōroku Bangō_) |
               | Japan                | `jp_trn`     | Japanese Tax Registration Number (_Tōroku Bangō_)                                                       |
+              | Kazakhstan           | `kz_bin`     | Kazakhstani Business Identification Number                                                              |
               | Kenya                | `ke_pin`     | Kenya Revenue Authority Personal Identification Number                                                  |
-              | Latvia               | `eu_vat`     | European VAT number                                                                                     |
-              | Liechtenstein        | `li_uid`     | Liechtensteinian UID number                                                                             |
-              | Lithuania            | `eu_vat`     | European VAT number                                                                                     |
-              | Luxembourg           | `eu_vat`     | European VAT number                                                                                     |
-              | Malaysia             | `my_frp`     | Malaysian FRP number                                                                                    |
+              | Latvia               | `eu_vat`     | European VAT Number                                                                                     |
+              | Liechtenstein        | `li_uid`     | Liechtensteinian UID Number                                                                             |
+              | Lithuania            | `eu_vat`     | European VAT Number                                                                                     |
+              | Luxembourg           | `eu_vat`     | European VAT Number                                                                                     |
+              | Malaysia             | `my_frp`     | Malaysian FRP Number                                                                                    |
               | Malaysia             | `my_itn`     | Malaysian ITN                                                                                           |
-              | Malaysia             | `my_sst`     | Malaysian SST number                                                                                    |
-              | Malta                | `eu_vat `    | European VAT number                                                                                     |
-              | Mexico               | `mx_rfc`     | Mexican RFC number                                                                                      |
-              | Netherlands          | `eu_vat`     | European VAT number                                                                                     |
-              | New Zealand          | `nz_gst`     | New Zealand GST number                                                                                  |
-              | Norway               | `no_vat`     | Norwegian VAT number                                                                                    |
+              | Malaysia             | `my_sst`     | Malaysian SST Number                                                                                    |
+              | Malta                | `eu_vat `    | European VAT Number                                                                                     |
+              | Mexico               | `mx_rfc`     | Mexican RFC Number                                                                                      |
+              | Netherlands          | `eu_vat`     | European VAT Number                                                                                     |
+              | New Zealand          | `nz_gst`     | New Zealand GST Number                                                                                  |
+              | Nigeria              | `ng_tin`     | Nigerian Tax Identification Number                                                                      |
+              | Norway               | `no_vat`     | Norwegian VAT Number                                                                                    |
+              | Norway               | `no_voec`    | Norwegian VAT on e-commerce Number                                                                      |
+              | Oman                 | `om_vat`     | Omani VAT Number                                                                                        |
+              | Peru                 | `pe_ruc`     | Peruvian RUC Number                                                                                     |
               | Philippines          | `ph_tin `    | Philippines Tax Identification Number                                                                   |
-              | Poland               | `eu_vat`     | European VAT number                                                                                     |
-              | Portugal             | `eu_vat`     | European VAT number                                                                                     |
-              | Romania              | `eu_vat`     | European VAT number                                                                                     |
+              | Poland               | `eu_vat`     | European VAT Number                                                                                     |
+              | Portugal             | `eu_vat`     | European VAT Number                                                                                     |
+              | Romania              | `eu_vat`     | European VAT Number                                                                                     |
+              | Romania              | `ro_tin`     | Romanian Tax ID Number                                                                                  |
               | Russia               | `ru_inn`     | Russian INN                                                                                             |
               | Russia               | `ru_kpp`     | Russian KPP                                                                                             |
-              | Saudi Arabia         | `sg_gst`     | Singaporean GST                                                                                         |
+              | Saudi Arabia         | `sa_vat`     | Saudi Arabia VAT                                                                                        |
+              | Serbia               | `rs_pib`     | Serbian PIB Number                                                                                      |
+              | Singapore            | `sg_gst`     | Singaporean GST                                                                                         |
               | Singapore            | `sg_uen`     | Singaporean UEN                                                                                         |
-              | Slovakia             | `eu_vat`     | European VAT number                                                                                     |
-              | Slovenia             | `eu_vat`     | European VAT number                                                                                     |
-              | Slovenia             | `si_tin`     | Slovenia tax number (davčna številka)                                                                   |
-              | South Africa         | `za_vat`     | South African VAT number                                                                                |
+              | Slovakia             | `eu_vat`     | European VAT Number                                                                                     |
+              | Slovenia             | `eu_vat`     | European VAT Number                                                                                     |
+              | Slovenia             | `si_tin`     | Slovenia Tax Number (davčna številka)                                                                   |
+              | South Africa         | `za_vat`     | South African VAT Number                                                                                |
               | South Korea          | `kr_brn`     | Korean BRN                                                                                              |
-              | Spain                | `es_cif`     | Spanish NIF number (previously Spanish CIF number)                                                      |
-              | Spain                | `eu_vat`     | European VAT number                                                                                     |
-              | Sweden               | `eu_vat`     | European VAT number                                                                                     |
-              | Switzerland          | `ch_vat`     | Switzerland VAT number                                                                                  |
+              | Spain                | `es_cif`     | Spanish NIF Number (previously Spanish CIF Number)                                                      |
+              | Spain                | `eu_vat`     | European VAT Number                                                                                     |
+              | Sweden               | `eu_vat`     | European VAT Number                                                                                     |
+              | Switzerland          | `ch_vat`     | Switzerland VAT Number                                                                                  |
               | Taiwan               | `tw_vat`     | Taiwanese VAT                                                                                           |
               | Thailand             | `th_vat`     | Thai VAT                                                                                                |
               | Turkey               | `tr_tin`     | Turkish Tax Identification Number                                                                       |
               | Ukraine              | `ua_vat`     | Ukrainian VAT                                                                                           |
               | United Arab Emirates | `ae_trn`     | United Arab Emirates TRN                                                                                |
-              | United Kingdom       | `eu_vat`     | Northern Ireland VAT number                                                                             |
-              | United Kingdom       | `gb_vat`     | United Kingdom VAT number                                                                               |
+              | United Kingdom       | `eu_vat`     | Northern Ireland VAT Number                                                                             |
+              | United Kingdom       | `gb_vat`     | United Kingdom VAT Number                                                                               |
               | United States        | `us_ein`     | United States EIN                                                                                       |
+              | Uruguay              | `uy_ruc`     | Uruguayan RUC Number                                                                                    |
+              | Venezuela            | `ve_rif`     | Venezuelan RIF Number                                                                                   |
+              | Vietnam              | `vn_tin`     | Vietnamese Tax ID Number                                                                                |
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
```

### Comparing `orb_billing-1.48.0/src/orb/resources/customers/usage.py` & `orb_billing-1.49.0/src/orb/resources/customers/usage.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/customers/credits/__init__.py` & `orb_billing-1.49.0/src/orb/resources/customers/credits/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/customers/credits/credits.py` & `orb_billing-1.49.0/src/orb/resources/customers/credits/credits.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/customers/credits/ledger.py` & `orb_billing-1.49.0/src/orb/resources/customers/credits/ledger.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/customers/credits/top_ups.py` & `orb_billing-1.49.0/src/orb/resources/customers/credits/top_ups.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/events/__init__.py` & `orb_billing-1.49.0/src/orb/resources/events/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/events/backfills.py` & `orb_billing-1.49.0/src/orb/resources/events/backfills.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/events/events.py` & `orb_billing-1.49.0/src/orb/resources/events/events.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/plans/__init__.py` & `orb_billing-1.49.0/src/orb/resources/plans/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/plans/external_plan_id.py` & `orb_billing-1.49.0/src/orb/resources/plans/external_plan_id.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/plans/plans.py` & `orb_billing-1.49.0/src/orb/resources/plans/plans.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/prices/__init__.py` & `orb_billing-1.49.0/src/orb/resources/prices/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/prices/external_price_id.py` & `orb_billing-1.49.0/src/orb/resources/prices/external_price_id.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/resources/prices/prices.py` & `orb_billing-1.49.0/src/orb/resources/prices/prices.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/__init__.py` & `orb_billing-1.49.0/src/orb/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from .item import Item as Item
 from .plan import Plan as Plan
+from .alert import Alert as Alert
 from .price import Price as Price
 from .coupon import Coupon as Coupon
 from .shared import (
     Discount as Discount,
     PaginationMetadata as PaginationMetadata,
     BillingCycleRelativeDate as BillingCycleRelativeDate,
 )
```

### Comparing `orb_billing-1.48.0/src/orb/types/coupon.py` & `orb_billing-1.49.0/src/orb/types/coupon.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/coupon_create_params.py` & `orb_billing-1.49.0/src/orb/types/coupon_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/coupon_list_params.py` & `orb_billing-1.49.0/src/orb/types/coupon_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/credit_note.py` & `orb_billing-1.49.0/src/orb/types/credit_note.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customer.py` & `orb_billing-1.49.0/src/orb/types/customer.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,27 +45,35 @@
     state: Optional[str] = None
 
 
 class TaxID(BaseModel):
     country: Literal[
         "AD",
         "AE",
+        "AR",
         "AT",
         "AU",
         "BE",
         "BG",
+        "BH",
+        "BO",
         "BR",
         "CA",
         "CH",
         "CL",
+        "CN",
+        "CO",
+        "CR",
         "CY",
         "CZ",
         "DE",
         "DK",
         "EE",
+        "DO",
+        "EC",
         "EG",
         "ES",
         "EU",
         "FI",
         "FR",
         "GB",
         "GE",
@@ -78,59 +86,76 @@
         "IL",
         "IN",
         "IS",
         "IT",
         "JP",
         "KE",
         "KR",
+        "KZ",
         "LI",
         "LT",
         "LU",
         "LV",
         "MT",
         "MX",
         "MY",
+        "NG",
         "NL",
         "NO",
         "NZ",
+        "OM",
+        "PE",
         "PH",
         "PL",
         "PT",
         "RO",
+        "RS",
         "RU",
         "SA",
         "SE",
         "SG",
         "SI",
         "SK",
+        "SV",
         "TH",
         "TR",
         "TW",
         "UA",
         "US",
+        "UY",
+        "VE",
+        "VN",
         "ZA",
     ]
 
     type: Literal[
         "ad_nrt",
         "ae_trn",
+        "ar_cuit",
         "eu_vat",
         "au_abn",
         "au_arn",
         "bg_uic",
+        "bh_vat",
+        "bo_tin",
         "br_cnpj",
         "br_cpf",
         "ca_bn",
         "ca_gst_hst",
         "ca_pst_bc",
         "ca_pst_mb",
         "ca_pst_sk",
         "ca_qst",
         "ch_vat",
         "cl_tin",
+        "cn_tin",
+        "co_nit",
+        "cr_tin",
+        "do_rcn",
+        "ec_ruc",
         "eg_tin",
         "es_cif",
         "eu_oss_vat",
         "gb_vat",
         "ge_vat",
         "hk_br",
         "hu_tin",
@@ -139,33 +164,44 @@
         "in_gst",
         "is_vat",
         "jp_cn",
         "jp_rn",
         "jp_trn",
         "ke_pin",
         "kr_brn",
+        "kz_bin",
         "li_uid",
         "mx_rfc",
         "my_frp",
         "my_itn",
         "my_sst",
+        "ng_tin",
         "no_vat",
+        "no_voec",
         "nz_gst",
+        "om_vat",
+        "pe_ruc",
         "ph_tin",
+        "ro_tin",
+        "rs_pib",
         "ru_inn",
         "ru_kpp",
         "sa_vat",
         "sg_gst",
         "sg_uen",
         "si_tin",
+        "sv_nit",
         "th_vat",
         "tr_tin",
         "tw_vat",
         "ua_vat",
         "us_ein",
+        "uy_ruc",
+        "ve_rif",
+        "vn_tin",
         "za_vat",
     ]
 
     value: str
 
 
 class AccountingSyncConfigurationAccountingProvider(BaseModel):
@@ -249,92 +285,112 @@
     Tax IDs are commonly required to be displayed on customer invoices, which are
     added to the headers of invoices.
 
     ### Supported Tax ID Countries and Types
 
     | Country              | Type         | Description                                                                                             |
     | -------------------- | ------------ | ------------------------------------------------------------------------------------------------------- |
-    | Andorra              | `ad_nrt`     | Andorran NRT number                                                                                     |
+    | Andorra              | `ad_nrt`     | Andorran NRT Number                                                                                     |
+    | Argentina            | `ar_cuit`    | Argentinian Tax ID Number                                                                               |
     | Australia            | `au_abn`     | Australian Business Number (AU ABN)                                                                     |
     | Australia            | `au_arn`     | Australian Taxation Office Reference Number                                                             |
-    | Austria              | `eu_vat`     | European VAT number                                                                                     |
-    | Belgium              | `eu_vat`     | European VAT number                                                                                     |
-    | Brazil               | `br_cnpj`    | Brazilian CNPJ number                                                                                   |
-    | Brazil               | `br_cpf`     | Brazilian CPF number                                                                                    |
+    | Austria              | `eu_vat`     | European VAT Number                                                                                     |
+    | Bahrain              | `bh_vat`     | Bahraini VAT Number                                                                                     |
+    | Belgium              | `eu_vat`     | European VAT Number                                                                                     |
+    | Bolivia              | `bo_tin`     | Bolivian Tax ID                                                                                         |
+    | Brazil               | `br_cnpj`    | Brazilian CNPJ Number                                                                                   |
+    | Brazil               | `br_cpf`     | Brazilian CPF Number                                                                                    |
     | Bulgaria             | `bg_uic`     | Bulgaria Unified Identification Code                                                                    |
-    | Bulgaria             | `eu_vat`     | European VAT number                                                                                     |
+    | Bulgaria             | `eu_vat`     | European VAT Number                                                                                     |
     | Canada               | `ca_bn`      | Canadian BN                                                                                             |
-    | Canada               | `ca_gst_hst` | Canadian GST/HST number                                                                                 |
-    | Canada               | `ca_pst_bc`  | Canadian PST number (British Columbia)                                                                  |
-    | Canada               | `ca_pst_mb`  | Canadian PST number (Manitoba)                                                                          |
-    | Canada               | `ca_pst_sk`  | Canadian PST number (Saskatchewan)                                                                      |
-    | Canada               | `ca_qst`     | Canadian QST number (Québec)                                                                            |
+    | Canada               | `ca_gst_hst` | Canadian GST/HST Number                                                                                 |
+    | Canada               | `ca_pst_bc`  | Canadian PST Number (British Columbia)                                                                  |
+    | Canada               | `ca_pst_mb`  | Canadian PST Number (Manitoba)                                                                          |
+    | Canada               | `ca_pst_sk`  | Canadian PST Number (Saskatchewan)                                                                      |
+    | Canada               | `ca_qst`     | Canadian QST Number (Québec)                                                                            |
     | Chile                | `cl_tin`     | Chilean TIN                                                                                             |
-    | Croatia              | `eu_vat`     | European VAT number                                                                                     |
-    | Cyprus               | `eu_vat`     | European VAT number                                                                                     |
-    | Czech Republic       | `eu_vat`     | European VAT number                                                                                     |
-    | Denmark              | `eu_vat`     | European VAT number                                                                                     |
+    | China                | `cn_tin`     | Chinese Tax ID                                                                                          |
+    | Colombia             | `co_nit`     | Colombian NIT Number                                                                                    |
+    | Costa Rica           | `cr_tin`     | Costa Rican Tax ID                                                                                      |
+    | Croatia              | `eu_vat`     | European VAT Number                                                                                     |
+    | Cyprus               | `eu_vat`     | European VAT Number                                                                                     |
+    | Czech Republic       | `eu_vat`     | European VAT Number                                                                                     |
+    | Denmark              | `eu_vat`     | European VAT Number                                                                                     |
+    | Dominican Republic   | `do_rcn`     | Dominican RCN Number                                                                                    |
+    | Ecuador              | `ec_ruc`     | Ecuadorian RUC Number                                                                                   |
     | Egypt                | `eg_tin`     | Egyptian Tax Identification Number                                                                      |
-    | Estonia              | `eu_vat`     | European VAT number                                                                                     |
-    | EU                   | `eu_oss_vat` | European One Stop Shop VAT number for non-Union scheme                                                  |
-    | Finland              | `eu_vat`     | European VAT number                                                                                     |
-    | France               | `eu_vat`     | European VAT number                                                                                     |
+    | El Salvador          | `sv_nit`     | El Salvadorian NIT Number                                                                               |
+    | Estonia              | `eu_vat`     | European VAT Number                                                                                     |
+    | EU                   | `eu_oss_vat` | European One Stop Shop VAT Number for non-Union scheme                                                  |
+    | Finland              | `eu_vat`     | European VAT Number                                                                                     |
+    | France               | `eu_vat`     | European VAT Number                                                                                     |
     | Georgia              | `ge_vat`     | Georgian VAT                                                                                            |
-    | Germany              | `eu_vat`     | European VAT number                                                                                     |
-    | Greece               | `eu_vat`     | European VAT number                                                                                     |
-    | Hong Kong            | `hk_br`      | Hong Kong BR number                                                                                     |
-    | Hungary              | `eu_vat`     | European VAT number                                                                                     |
-    | Hungary              | `hu_tin`     | Hungary tax number (adószám)                                                                            |
+    | Germany              | `eu_vat`     | European VAT Number                                                                                     |
+    | Greece               | `eu_vat`     | European VAT Number                                                                                     |
+    | Hong Kong            | `hk_br`      | Hong Kong BR Number                                                                                     |
+    | Hungary              | `eu_vat`     | European VAT Number                                                                                     |
+    | Hungary              | `hu_tin`     | Hungary Tax Number (adószám)                                                                            |
     | Iceland              | `is_vat`     | Icelandic VAT                                                                                           |
-    | India                | `in_gst`     | Indian GST number                                                                                       |
-    | Indonesia            | `id_npwp`    | Indonesian NPWP number                                                                                  |
-    | Ireland              | `eu_vat`     | European VAT number                                                                                     |
+    | India                | `in_gst`     | Indian GST Number                                                                                       |
+    | Indonesia            | `id_npwp`    | Indonesian NPWP Number                                                                                  |
+    | Ireland              | `eu_vat`     | European VAT Number                                                                                     |
     | Israel               | `il_vat`     | Israel VAT                                                                                              |
-    | Italy                | `eu_vat`     | European VAT number                                                                                     |
+    | Italy                | `eu_vat`     | European VAT Number                                                                                     |
     | Japan                | `jp_cn`      | Japanese Corporate Number (_Hōjin Bangō_)                                                               |
     | Japan                | `jp_rn`      | Japanese Registered Foreign Businesses' Registration Number (_Tōroku Kokugai Jigyōsha no Tōroku Bangō_) |
     | Japan                | `jp_trn`     | Japanese Tax Registration Number (_Tōroku Bangō_)                                                       |
+    | Kazakhstan           | `kz_bin`     | Kazakhstani Business Identification Number                                                              |
     | Kenya                | `ke_pin`     | Kenya Revenue Authority Personal Identification Number                                                  |
-    | Latvia               | `eu_vat`     | European VAT number                                                                                     |
-    | Liechtenstein        | `li_uid`     | Liechtensteinian UID number                                                                             |
-    | Lithuania            | `eu_vat`     | European VAT number                                                                                     |
-    | Luxembourg           | `eu_vat`     | European VAT number                                                                                     |
-    | Malaysia             | `my_frp`     | Malaysian FRP number                                                                                    |
+    | Latvia               | `eu_vat`     | European VAT Number                                                                                     |
+    | Liechtenstein        | `li_uid`     | Liechtensteinian UID Number                                                                             |
+    | Lithuania            | `eu_vat`     | European VAT Number                                                                                     |
+    | Luxembourg           | `eu_vat`     | European VAT Number                                                                                     |
+    | Malaysia             | `my_frp`     | Malaysian FRP Number                                                                                    |
     | Malaysia             | `my_itn`     | Malaysian ITN                                                                                           |
-    | Malaysia             | `my_sst`     | Malaysian SST number                                                                                    |
-    | Malta                | `eu_vat `    | European VAT number                                                                                     |
-    | Mexico               | `mx_rfc`     | Mexican RFC number                                                                                      |
-    | Netherlands          | `eu_vat`     | European VAT number                                                                                     |
-    | New Zealand          | `nz_gst`     | New Zealand GST number                                                                                  |
-    | Norway               | `no_vat`     | Norwegian VAT number                                                                                    |
+    | Malaysia             | `my_sst`     | Malaysian SST Number                                                                                    |
+    | Malta                | `eu_vat `    | European VAT Number                                                                                     |
+    | Mexico               | `mx_rfc`     | Mexican RFC Number                                                                                      |
+    | Netherlands          | `eu_vat`     | European VAT Number                                                                                     |
+    | New Zealand          | `nz_gst`     | New Zealand GST Number                                                                                  |
+    | Nigeria              | `ng_tin`     | Nigerian Tax Identification Number                                                                      |
+    | Norway               | `no_vat`     | Norwegian VAT Number                                                                                    |
+    | Norway               | `no_voec`    | Norwegian VAT on e-commerce Number                                                                      |
+    | Oman                 | `om_vat`     | Omani VAT Number                                                                                        |
+    | Peru                 | `pe_ruc`     | Peruvian RUC Number                                                                                     |
     | Philippines          | `ph_tin `    | Philippines Tax Identification Number                                                                   |
-    | Poland               | `eu_vat`     | European VAT number                                                                                     |
-    | Portugal             | `eu_vat`     | European VAT number                                                                                     |
-    | Romania              | `eu_vat`     | European VAT number                                                                                     |
+    | Poland               | `eu_vat`     | European VAT Number                                                                                     |
+    | Portugal             | `eu_vat`     | European VAT Number                                                                                     |
+    | Romania              | `eu_vat`     | European VAT Number                                                                                     |
+    | Romania              | `ro_tin`     | Romanian Tax ID Number                                                                                  |
     | Russia               | `ru_inn`     | Russian INN                                                                                             |
     | Russia               | `ru_kpp`     | Russian KPP                                                                                             |
-    | Saudi Arabia         | `sg_gst`     | Singaporean GST                                                                                         |
+    | Saudi Arabia         | `sa_vat`     | Saudi Arabia VAT                                                                                        |
+    | Serbia               | `rs_pib`     | Serbian PIB Number                                                                                      |
+    | Singapore            | `sg_gst`     | Singaporean GST                                                                                         |
     | Singapore            | `sg_uen`     | Singaporean UEN                                                                                         |
-    | Slovakia             | `eu_vat`     | European VAT number                                                                                     |
-    | Slovenia             | `eu_vat`     | European VAT number                                                                                     |
-    | Slovenia             | `si_tin`     | Slovenia tax number (davčna številka)                                                                   |
-    | South Africa         | `za_vat`     | South African VAT number                                                                                |
+    | Slovakia             | `eu_vat`     | European VAT Number                                                                                     |
+    | Slovenia             | `eu_vat`     | European VAT Number                                                                                     |
+    | Slovenia             | `si_tin`     | Slovenia Tax Number (davčna številka)                                                                   |
+    | South Africa         | `za_vat`     | South African VAT Number                                                                                |
     | South Korea          | `kr_brn`     | Korean BRN                                                                                              |
-    | Spain                | `es_cif`     | Spanish NIF number (previously Spanish CIF number)                                                      |
-    | Spain                | `eu_vat`     | European VAT number                                                                                     |
-    | Sweden               | `eu_vat`     | European VAT number                                                                                     |
-    | Switzerland          | `ch_vat`     | Switzerland VAT number                                                                                  |
+    | Spain                | `es_cif`     | Spanish NIF Number (previously Spanish CIF Number)                                                      |
+    | Spain                | `eu_vat`     | European VAT Number                                                                                     |
+    | Sweden               | `eu_vat`     | European VAT Number                                                                                     |
+    | Switzerland          | `ch_vat`     | Switzerland VAT Number                                                                                  |
     | Taiwan               | `tw_vat`     | Taiwanese VAT                                                                                           |
     | Thailand             | `th_vat`     | Thai VAT                                                                                                |
     | Turkey               | `tr_tin`     | Turkish Tax Identification Number                                                                       |
     | Ukraine              | `ua_vat`     | Ukrainian VAT                                                                                           |
     | United Arab Emirates | `ae_trn`     | United Arab Emirates TRN                                                                                |
-    | United Kingdom       | `eu_vat`     | Northern Ireland VAT number                                                                             |
-    | United Kingdom       | `gb_vat`     | United Kingdom VAT number                                                                               |
+    | United Kingdom       | `eu_vat`     | Northern Ireland VAT Number                                                                             |
+    | United Kingdom       | `gb_vat`     | United Kingdom VAT Number                                                                               |
     | United States        | `us_ein`     | United States EIN                                                                                       |
+    | Uruguay              | `uy_ruc`     | Uruguayan RUC Number                                                                                    |
+    | Venezuela            | `ve_rif`     | Venezuelan RIF Number                                                                                   |
+    | Vietnam              | `vn_tin`     | Vietnamese Tax ID Number                                                                                |
     """
 
     timezone: str
     """
     A timezone identifier from the IANA timezone database, such as
     "America/Los_Angeles". This "defaults to your account's timezone if not set.
     This cannot be changed after customer creation.
```

### Comparing `orb_billing-1.48.0/src/orb/types/customer_create_params.py` & `orb_billing-1.49.0/src/orb/types/customer_create_params.py`

 * *Files 10% similar despite different names*

```diff
@@ -88,92 +88,112 @@
     Tax IDs are commonly required to be displayed on customer invoices, which are
     added to the headers of invoices.
 
     ### Supported Tax ID Countries and Types
 
     | Country              | Type         | Description                                                                                             |
     | -------------------- | ------------ | ------------------------------------------------------------------------------------------------------- |
-    | Andorra              | `ad_nrt`     | Andorran NRT number                                                                                     |
+    | Andorra              | `ad_nrt`     | Andorran NRT Number                                                                                     |
+    | Argentina            | `ar_cuit`    | Argentinian Tax ID Number                                                                               |
     | Australia            | `au_abn`     | Australian Business Number (AU ABN)                                                                     |
     | Australia            | `au_arn`     | Australian Taxation Office Reference Number                                                             |
-    | Austria              | `eu_vat`     | European VAT number                                                                                     |
-    | Belgium              | `eu_vat`     | European VAT number                                                                                     |
-    | Brazil               | `br_cnpj`    | Brazilian CNPJ number                                                                                   |
-    | Brazil               | `br_cpf`     | Brazilian CPF number                                                                                    |
+    | Austria              | `eu_vat`     | European VAT Number                                                                                     |
+    | Bahrain              | `bh_vat`     | Bahraini VAT Number                                                                                     |
+    | Belgium              | `eu_vat`     | European VAT Number                                                                                     |
+    | Bolivia              | `bo_tin`     | Bolivian Tax ID                                                                                         |
+    | Brazil               | `br_cnpj`    | Brazilian CNPJ Number                                                                                   |
+    | Brazil               | `br_cpf`     | Brazilian CPF Number                                                                                    |
     | Bulgaria             | `bg_uic`     | Bulgaria Unified Identification Code                                                                    |
-    | Bulgaria             | `eu_vat`     | European VAT number                                                                                     |
+    | Bulgaria             | `eu_vat`     | European VAT Number                                                                                     |
     | Canada               | `ca_bn`      | Canadian BN                                                                                             |
-    | Canada               | `ca_gst_hst` | Canadian GST/HST number                                                                                 |
-    | Canada               | `ca_pst_bc`  | Canadian PST number (British Columbia)                                                                  |
-    | Canada               | `ca_pst_mb`  | Canadian PST number (Manitoba)                                                                          |
-    | Canada               | `ca_pst_sk`  | Canadian PST number (Saskatchewan)                                                                      |
-    | Canada               | `ca_qst`     | Canadian QST number (Québec)                                                                            |
+    | Canada               | `ca_gst_hst` | Canadian GST/HST Number                                                                                 |
+    | Canada               | `ca_pst_bc`  | Canadian PST Number (British Columbia)                                                                  |
+    | Canada               | `ca_pst_mb`  | Canadian PST Number (Manitoba)                                                                          |
+    | Canada               | `ca_pst_sk`  | Canadian PST Number (Saskatchewan)                                                                      |
+    | Canada               | `ca_qst`     | Canadian QST Number (Québec)                                                                            |
     | Chile                | `cl_tin`     | Chilean TIN                                                                                             |
-    | Croatia              | `eu_vat`     | European VAT number                                                                                     |
-    | Cyprus               | `eu_vat`     | European VAT number                                                                                     |
-    | Czech Republic       | `eu_vat`     | European VAT number                                                                                     |
-    | Denmark              | `eu_vat`     | European VAT number                                                                                     |
+    | China                | `cn_tin`     | Chinese Tax ID                                                                                          |
+    | Colombia             | `co_nit`     | Colombian NIT Number                                                                                    |
+    | Costa Rica           | `cr_tin`     | Costa Rican Tax ID                                                                                      |
+    | Croatia              | `eu_vat`     | European VAT Number                                                                                     |
+    | Cyprus               | `eu_vat`     | European VAT Number                                                                                     |
+    | Czech Republic       | `eu_vat`     | European VAT Number                                                                                     |
+    | Denmark              | `eu_vat`     | European VAT Number                                                                                     |
+    | Dominican Republic   | `do_rcn`     | Dominican RCN Number                                                                                    |
+    | Ecuador              | `ec_ruc`     | Ecuadorian RUC Number                                                                                   |
     | Egypt                | `eg_tin`     | Egyptian Tax Identification Number                                                                      |
-    | Estonia              | `eu_vat`     | European VAT number                                                                                     |
-    | EU                   | `eu_oss_vat` | European One Stop Shop VAT number for non-Union scheme                                                  |
-    | Finland              | `eu_vat`     | European VAT number                                                                                     |
-    | France               | `eu_vat`     | European VAT number                                                                                     |
+    | El Salvador          | `sv_nit`     | El Salvadorian NIT Number                                                                               |
+    | Estonia              | `eu_vat`     | European VAT Number                                                                                     |
+    | EU                   | `eu_oss_vat` | European One Stop Shop VAT Number for non-Union scheme                                                  |
+    | Finland              | `eu_vat`     | European VAT Number                                                                                     |
+    | France               | `eu_vat`     | European VAT Number                                                                                     |
     | Georgia              | `ge_vat`     | Georgian VAT                                                                                            |
-    | Germany              | `eu_vat`     | European VAT number                                                                                     |
-    | Greece               | `eu_vat`     | European VAT number                                                                                     |
-    | Hong Kong            | `hk_br`      | Hong Kong BR number                                                                                     |
-    | Hungary              | `eu_vat`     | European VAT number                                                                                     |
-    | Hungary              | `hu_tin`     | Hungary tax number (adószám)                                                                            |
+    | Germany              | `eu_vat`     | European VAT Number                                                                                     |
+    | Greece               | `eu_vat`     | European VAT Number                                                                                     |
+    | Hong Kong            | `hk_br`      | Hong Kong BR Number                                                                                     |
+    | Hungary              | `eu_vat`     | European VAT Number                                                                                     |
+    | Hungary              | `hu_tin`     | Hungary Tax Number (adószám)                                                                            |
     | Iceland              | `is_vat`     | Icelandic VAT                                                                                           |
-    | India                | `in_gst`     | Indian GST number                                                                                       |
-    | Indonesia            | `id_npwp`    | Indonesian NPWP number                                                                                  |
-    | Ireland              | `eu_vat`     | European VAT number                                                                                     |
+    | India                | `in_gst`     | Indian GST Number                                                                                       |
+    | Indonesia            | `id_npwp`    | Indonesian NPWP Number                                                                                  |
+    | Ireland              | `eu_vat`     | European VAT Number                                                                                     |
     | Israel               | `il_vat`     | Israel VAT                                                                                              |
-    | Italy                | `eu_vat`     | European VAT number                                                                                     |
+    | Italy                | `eu_vat`     | European VAT Number                                                                                     |
     | Japan                | `jp_cn`      | Japanese Corporate Number (_Hōjin Bangō_)                                                               |
     | Japan                | `jp_rn`      | Japanese Registered Foreign Businesses' Registration Number (_Tōroku Kokugai Jigyōsha no Tōroku Bangō_) |
     | Japan                | `jp_trn`     | Japanese Tax Registration Number (_Tōroku Bangō_)                                                       |
+    | Kazakhstan           | `kz_bin`     | Kazakhstani Business Identification Number                                                              |
     | Kenya                | `ke_pin`     | Kenya Revenue Authority Personal Identification Number                                                  |
-    | Latvia               | `eu_vat`     | European VAT number                                                                                     |
-    | Liechtenstein        | `li_uid`     | Liechtensteinian UID number                                                                             |
-    | Lithuania            | `eu_vat`     | European VAT number                                                                                     |
-    | Luxembourg           | `eu_vat`     | European VAT number                                                                                     |
-    | Malaysia             | `my_frp`     | Malaysian FRP number                                                                                    |
+    | Latvia               | `eu_vat`     | European VAT Number                                                                                     |
+    | Liechtenstein        | `li_uid`     | Liechtensteinian UID Number                                                                             |
+    | Lithuania            | `eu_vat`     | European VAT Number                                                                                     |
+    | Luxembourg           | `eu_vat`     | European VAT Number                                                                                     |
+    | Malaysia             | `my_frp`     | Malaysian FRP Number                                                                                    |
     | Malaysia             | `my_itn`     | Malaysian ITN                                                                                           |
-    | Malaysia             | `my_sst`     | Malaysian SST number                                                                                    |
-    | Malta                | `eu_vat `    | European VAT number                                                                                     |
-    | Mexico               | `mx_rfc`     | Mexican RFC number                                                                                      |
-    | Netherlands          | `eu_vat`     | European VAT number                                                                                     |
-    | New Zealand          | `nz_gst`     | New Zealand GST number                                                                                  |
-    | Norway               | `no_vat`     | Norwegian VAT number                                                                                    |
+    | Malaysia             | `my_sst`     | Malaysian SST Number                                                                                    |
+    | Malta                | `eu_vat `    | European VAT Number                                                                                     |
+    | Mexico               | `mx_rfc`     | Mexican RFC Number                                                                                      |
+    | Netherlands          | `eu_vat`     | European VAT Number                                                                                     |
+    | New Zealand          | `nz_gst`     | New Zealand GST Number                                                                                  |
+    | Nigeria              | `ng_tin`     | Nigerian Tax Identification Number                                                                      |
+    | Norway               | `no_vat`     | Norwegian VAT Number                                                                                    |
+    | Norway               | `no_voec`    | Norwegian VAT on e-commerce Number                                                                      |
+    | Oman                 | `om_vat`     | Omani VAT Number                                                                                        |
+    | Peru                 | `pe_ruc`     | Peruvian RUC Number                                                                                     |
     | Philippines          | `ph_tin `    | Philippines Tax Identification Number                                                                   |
-    | Poland               | `eu_vat`     | European VAT number                                                                                     |
-    | Portugal             | `eu_vat`     | European VAT number                                                                                     |
-    | Romania              | `eu_vat`     | European VAT number                                                                                     |
+    | Poland               | `eu_vat`     | European VAT Number                                                                                     |
+    | Portugal             | `eu_vat`     | European VAT Number                                                                                     |
+    | Romania              | `eu_vat`     | European VAT Number                                                                                     |
+    | Romania              | `ro_tin`     | Romanian Tax ID Number                                                                                  |
     | Russia               | `ru_inn`     | Russian INN                                                                                             |
     | Russia               | `ru_kpp`     | Russian KPP                                                                                             |
-    | Saudi Arabia         | `sg_gst`     | Singaporean GST                                                                                         |
+    | Saudi Arabia         | `sa_vat`     | Saudi Arabia VAT                                                                                        |
+    | Serbia               | `rs_pib`     | Serbian PIB Number                                                                                      |
+    | Singapore            | `sg_gst`     | Singaporean GST                                                                                         |
     | Singapore            | `sg_uen`     | Singaporean UEN                                                                                         |
-    | Slovakia             | `eu_vat`     | European VAT number                                                                                     |
-    | Slovenia             | `eu_vat`     | European VAT number                                                                                     |
-    | Slovenia             | `si_tin`     | Slovenia tax number (davčna številka)                                                                   |
-    | South Africa         | `za_vat`     | South African VAT number                                                                                |
+    | Slovakia             | `eu_vat`     | European VAT Number                                                                                     |
+    | Slovenia             | `eu_vat`     | European VAT Number                                                                                     |
+    | Slovenia             | `si_tin`     | Slovenia Tax Number (davčna številka)                                                                   |
+    | South Africa         | `za_vat`     | South African VAT Number                                                                                |
     | South Korea          | `kr_brn`     | Korean BRN                                                                                              |
-    | Spain                | `es_cif`     | Spanish NIF number (previously Spanish CIF number)                                                      |
-    | Spain                | `eu_vat`     | European VAT number                                                                                     |
-    | Sweden               | `eu_vat`     | European VAT number                                                                                     |
-    | Switzerland          | `ch_vat`     | Switzerland VAT number                                                                                  |
+    | Spain                | `es_cif`     | Spanish NIF Number (previously Spanish CIF Number)                                                      |
+    | Spain                | `eu_vat`     | European VAT Number                                                                                     |
+    | Sweden               | `eu_vat`     | European VAT Number                                                                                     |
+    | Switzerland          | `ch_vat`     | Switzerland VAT Number                                                                                  |
     | Taiwan               | `tw_vat`     | Taiwanese VAT                                                                                           |
     | Thailand             | `th_vat`     | Thai VAT                                                                                                |
     | Turkey               | `tr_tin`     | Turkish Tax Identification Number                                                                       |
     | Ukraine              | `ua_vat`     | Ukrainian VAT                                                                                           |
     | United Arab Emirates | `ae_trn`     | United Arab Emirates TRN                                                                                |
-    | United Kingdom       | `eu_vat`     | Northern Ireland VAT number                                                                             |
-    | United Kingdom       | `gb_vat`     | United Kingdom VAT number                                                                               |
+    | United Kingdom       | `eu_vat`     | Northern Ireland VAT Number                                                                             |
+    | United Kingdom       | `gb_vat`     | United Kingdom VAT Number                                                                               |
     | United States        | `us_ein`     | United States EIN                                                                                       |
+    | Uruguay              | `uy_ruc`     | Uruguayan RUC Number                                                                                    |
+    | Venezuela            | `ve_rif`     | Venezuelan RIF Number                                                                                   |
+    | Vietnam              | `vn_tin`     | Vietnamese Tax ID Number                                                                                |
     """
 
     timezone: Optional[str]
     """
     A timezone identifier from the IANA timezone database, such as
     `"America/Los_Angeles"`. This defaults to your account's timezone if not set.
     This cannot be changed after customer creation.
@@ -225,27 +245,35 @@
 
 
 class TaxID(TypedDict, total=False):
     country: Required[
         Literal[
             "AD",
             "AE",
+            "AR",
             "AT",
             "AU",
             "BE",
             "BG",
+            "BH",
+            "BO",
             "BR",
             "CA",
             "CH",
             "CL",
+            "CN",
+            "CO",
+            "CR",
             "CY",
             "CZ",
             "DE",
             "DK",
             "EE",
+            "DO",
+            "EC",
             "EG",
             "ES",
             "EU",
             "FI",
             "FR",
             "GB",
             "GE",
@@ -258,61 +286,78 @@
             "IL",
             "IN",
             "IS",
             "IT",
             "JP",
             "KE",
             "KR",
+            "KZ",
             "LI",
             "LT",
             "LU",
             "LV",
             "MT",
             "MX",
             "MY",
+            "NG",
             "NL",
             "NO",
             "NZ",
+            "OM",
+            "PE",
             "PH",
             "PL",
             "PT",
             "RO",
+            "RS",
             "RU",
             "SA",
             "SE",
             "SG",
             "SI",
             "SK",
+            "SV",
             "TH",
             "TR",
             "TW",
             "UA",
             "US",
+            "UY",
+            "VE",
+            "VN",
             "ZA",
         ]
     ]
 
     type: Required[
         Literal[
             "ad_nrt",
             "ae_trn",
+            "ar_cuit",
             "eu_vat",
             "au_abn",
             "au_arn",
             "bg_uic",
+            "bh_vat",
+            "bo_tin",
             "br_cnpj",
             "br_cpf",
             "ca_bn",
             "ca_gst_hst",
             "ca_pst_bc",
             "ca_pst_mb",
             "ca_pst_sk",
             "ca_qst",
             "ch_vat",
             "cl_tin",
+            "cn_tin",
+            "co_nit",
+            "cr_tin",
+            "do_rcn",
+            "ec_ruc",
             "eg_tin",
             "es_cif",
             "eu_oss_vat",
             "gb_vat",
             "ge_vat",
             "hk_br",
             "hu_tin",
@@ -321,31 +366,42 @@
             "in_gst",
             "is_vat",
             "jp_cn",
             "jp_rn",
             "jp_trn",
             "ke_pin",
             "kr_brn",
+            "kz_bin",
             "li_uid",
             "mx_rfc",
             "my_frp",
             "my_itn",
             "my_sst",
+            "ng_tin",
             "no_vat",
+            "no_voec",
             "nz_gst",
+            "om_vat",
+            "pe_ruc",
             "ph_tin",
+            "ro_tin",
+            "rs_pib",
             "ru_inn",
             "ru_kpp",
             "sa_vat",
             "sg_gst",
             "sg_uen",
             "si_tin",
+            "sv_nit",
             "th_vat",
             "tr_tin",
             "tw_vat",
             "ua_vat",
             "us_ein",
+            "uy_ruc",
+            "ve_rif",
+            "vn_tin",
             "za_vat",
         ]
     ]
 
     value: Required[str]
```

### Comparing `orb_billing-1.48.0/src/orb/types/customer_list_params.py` & `orb_billing-1.49.0/src/orb/types/customer_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customer_update_by_external_id_params.py` & `orb_billing-1.49.0/src/orb/types/customer_update_by_external_id_params.py`

 * *Files 20% similar despite different names*

```diff
@@ -88,92 +88,112 @@
     Tax IDs are commonly required to be displayed on customer invoices, which are
     added to the headers of invoices.
 
     ### Supported Tax ID Countries and Types
 
     | Country              | Type         | Description                                                                                             |
     | -------------------- | ------------ | ------------------------------------------------------------------------------------------------------- |
-    | Andorra              | `ad_nrt`     | Andorran NRT number                                                                                     |
+    | Andorra              | `ad_nrt`     | Andorran NRT Number                                                                                     |
+    | Argentina            | `ar_cuit`    | Argentinian Tax ID Number                                                                               |
     | Australia            | `au_abn`     | Australian Business Number (AU ABN)                                                                     |
     | Australia            | `au_arn`     | Australian Taxation Office Reference Number                                                             |
-    | Austria              | `eu_vat`     | European VAT number                                                                                     |
-    | Belgium              | `eu_vat`     | European VAT number                                                                                     |
-    | Brazil               | `br_cnpj`    | Brazilian CNPJ number                                                                                   |
-    | Brazil               | `br_cpf`     | Brazilian CPF number                                                                                    |
+    | Austria              | `eu_vat`     | European VAT Number                                                                                     |
+    | Bahrain              | `bh_vat`     | Bahraini VAT Number                                                                                     |
+    | Belgium              | `eu_vat`     | European VAT Number                                                                                     |
+    | Bolivia              | `bo_tin`     | Bolivian Tax ID                                                                                         |
+    | Brazil               | `br_cnpj`    | Brazilian CNPJ Number                                                                                   |
+    | Brazil               | `br_cpf`     | Brazilian CPF Number                                                                                    |
     | Bulgaria             | `bg_uic`     | Bulgaria Unified Identification Code                                                                    |
-    | Bulgaria             | `eu_vat`     | European VAT number                                                                                     |
+    | Bulgaria             | `eu_vat`     | European VAT Number                                                                                     |
     | Canada               | `ca_bn`      | Canadian BN                                                                                             |
-    | Canada               | `ca_gst_hst` | Canadian GST/HST number                                                                                 |
-    | Canada               | `ca_pst_bc`  | Canadian PST number (British Columbia)                                                                  |
-    | Canada               | `ca_pst_mb`  | Canadian PST number (Manitoba)                                                                          |
-    | Canada               | `ca_pst_sk`  | Canadian PST number (Saskatchewan)                                                                      |
-    | Canada               | `ca_qst`     | Canadian QST number (Québec)                                                                            |
+    | Canada               | `ca_gst_hst` | Canadian GST/HST Number                                                                                 |
+    | Canada               | `ca_pst_bc`  | Canadian PST Number (British Columbia)                                                                  |
+    | Canada               | `ca_pst_mb`  | Canadian PST Number (Manitoba)                                                                          |
+    | Canada               | `ca_pst_sk`  | Canadian PST Number (Saskatchewan)                                                                      |
+    | Canada               | `ca_qst`     | Canadian QST Number (Québec)                                                                            |
     | Chile                | `cl_tin`     | Chilean TIN                                                                                             |
-    | Croatia              | `eu_vat`     | European VAT number                                                                                     |
-    | Cyprus               | `eu_vat`     | European VAT number                                                                                     |
-    | Czech Republic       | `eu_vat`     | European VAT number                                                                                     |
-    | Denmark              | `eu_vat`     | European VAT number                                                                                     |
+    | China                | `cn_tin`     | Chinese Tax ID                                                                                          |
+    | Colombia             | `co_nit`     | Colombian NIT Number                                                                                    |
+    | Costa Rica           | `cr_tin`     | Costa Rican Tax ID                                                                                      |
+    | Croatia              | `eu_vat`     | European VAT Number                                                                                     |
+    | Cyprus               | `eu_vat`     | European VAT Number                                                                                     |
+    | Czech Republic       | `eu_vat`     | European VAT Number                                                                                     |
+    | Denmark              | `eu_vat`     | European VAT Number                                                                                     |
+    | Dominican Republic   | `do_rcn`     | Dominican RCN Number                                                                                    |
+    | Ecuador              | `ec_ruc`     | Ecuadorian RUC Number                                                                                   |
     | Egypt                | `eg_tin`     | Egyptian Tax Identification Number                                                                      |
-    | Estonia              | `eu_vat`     | European VAT number                                                                                     |
-    | EU                   | `eu_oss_vat` | European One Stop Shop VAT number for non-Union scheme                                                  |
-    | Finland              | `eu_vat`     | European VAT number                                                                                     |
-    | France               | `eu_vat`     | European VAT number                                                                                     |
+    | El Salvador          | `sv_nit`     | El Salvadorian NIT Number                                                                               |
+    | Estonia              | `eu_vat`     | European VAT Number                                                                                     |
+    | EU                   | `eu_oss_vat` | European One Stop Shop VAT Number for non-Union scheme                                                  |
+    | Finland              | `eu_vat`     | European VAT Number                                                                                     |
+    | France               | `eu_vat`     | European VAT Number                                                                                     |
     | Georgia              | `ge_vat`     | Georgian VAT                                                                                            |
-    | Germany              | `eu_vat`     | European VAT number                                                                                     |
-    | Greece               | `eu_vat`     | European VAT number                                                                                     |
-    | Hong Kong            | `hk_br`      | Hong Kong BR number                                                                                     |
-    | Hungary              | `eu_vat`     | European VAT number                                                                                     |
-    | Hungary              | `hu_tin`     | Hungary tax number (adószám)                                                                            |
+    | Germany              | `eu_vat`     | European VAT Number                                                                                     |
+    | Greece               | `eu_vat`     | European VAT Number                                                                                     |
+    | Hong Kong            | `hk_br`      | Hong Kong BR Number                                                                                     |
+    | Hungary              | `eu_vat`     | European VAT Number                                                                                     |
+    | Hungary              | `hu_tin`     | Hungary Tax Number (adószám)                                                                            |
     | Iceland              | `is_vat`     | Icelandic VAT                                                                                           |
-    | India                | `in_gst`     | Indian GST number                                                                                       |
-    | Indonesia            | `id_npwp`    | Indonesian NPWP number                                                                                  |
-    | Ireland              | `eu_vat`     | European VAT number                                                                                     |
+    | India                | `in_gst`     | Indian GST Number                                                                                       |
+    | Indonesia            | `id_npwp`    | Indonesian NPWP Number                                                                                  |
+    | Ireland              | `eu_vat`     | European VAT Number                                                                                     |
     | Israel               | `il_vat`     | Israel VAT                                                                                              |
-    | Italy                | `eu_vat`     | European VAT number                                                                                     |
+    | Italy                | `eu_vat`     | European VAT Number                                                                                     |
     | Japan                | `jp_cn`      | Japanese Corporate Number (_Hōjin Bangō_)                                                               |
     | Japan                | `jp_rn`      | Japanese Registered Foreign Businesses' Registration Number (_Tōroku Kokugai Jigyōsha no Tōroku Bangō_) |
     | Japan                | `jp_trn`     | Japanese Tax Registration Number (_Tōroku Bangō_)                                                       |
+    | Kazakhstan           | `kz_bin`     | Kazakhstani Business Identification Number                                                              |
     | Kenya                | `ke_pin`     | Kenya Revenue Authority Personal Identification Number                                                  |
-    | Latvia               | `eu_vat`     | European VAT number                                                                                     |
-    | Liechtenstein        | `li_uid`     | Liechtensteinian UID number                                                                             |
-    | Lithuania            | `eu_vat`     | European VAT number                                                                                     |
-    | Luxembourg           | `eu_vat`     | European VAT number                                                                                     |
-    | Malaysia             | `my_frp`     | Malaysian FRP number                                                                                    |
+    | Latvia               | `eu_vat`     | European VAT Number                                                                                     |
+    | Liechtenstein        | `li_uid`     | Liechtensteinian UID Number                                                                             |
+    | Lithuania            | `eu_vat`     | European VAT Number                                                                                     |
+    | Luxembourg           | `eu_vat`     | European VAT Number                                                                                     |
+    | Malaysia             | `my_frp`     | Malaysian FRP Number                                                                                    |
     | Malaysia             | `my_itn`     | Malaysian ITN                                                                                           |
-    | Malaysia             | `my_sst`     | Malaysian SST number                                                                                    |
-    | Malta                | `eu_vat `    | European VAT number                                                                                     |
-    | Mexico               | `mx_rfc`     | Mexican RFC number                                                                                      |
-    | Netherlands          | `eu_vat`     | European VAT number                                                                                     |
-    | New Zealand          | `nz_gst`     | New Zealand GST number                                                                                  |
-    | Norway               | `no_vat`     | Norwegian VAT number                                                                                    |
+    | Malaysia             | `my_sst`     | Malaysian SST Number                                                                                    |
+    | Malta                | `eu_vat `    | European VAT Number                                                                                     |
+    | Mexico               | `mx_rfc`     | Mexican RFC Number                                                                                      |
+    | Netherlands          | `eu_vat`     | European VAT Number                                                                                     |
+    | New Zealand          | `nz_gst`     | New Zealand GST Number                                                                                  |
+    | Nigeria              | `ng_tin`     | Nigerian Tax Identification Number                                                                      |
+    | Norway               | `no_vat`     | Norwegian VAT Number                                                                                    |
+    | Norway               | `no_voec`    | Norwegian VAT on e-commerce Number                                                                      |
+    | Oman                 | `om_vat`     | Omani VAT Number                                                                                        |
+    | Peru                 | `pe_ruc`     | Peruvian RUC Number                                                                                     |
     | Philippines          | `ph_tin `    | Philippines Tax Identification Number                                                                   |
-    | Poland               | `eu_vat`     | European VAT number                                                                                     |
-    | Portugal             | `eu_vat`     | European VAT number                                                                                     |
-    | Romania              | `eu_vat`     | European VAT number                                                                                     |
+    | Poland               | `eu_vat`     | European VAT Number                                                                                     |
+    | Portugal             | `eu_vat`     | European VAT Number                                                                                     |
+    | Romania              | `eu_vat`     | European VAT Number                                                                                     |
+    | Romania              | `ro_tin`     | Romanian Tax ID Number                                                                                  |
     | Russia               | `ru_inn`     | Russian INN                                                                                             |
     | Russia               | `ru_kpp`     | Russian KPP                                                                                             |
-    | Saudi Arabia         | `sg_gst`     | Singaporean GST                                                                                         |
+    | Saudi Arabia         | `sa_vat`     | Saudi Arabia VAT                                                                                        |
+    | Serbia               | `rs_pib`     | Serbian PIB Number                                                                                      |
+    | Singapore            | `sg_gst`     | Singaporean GST                                                                                         |
     | Singapore            | `sg_uen`     | Singaporean UEN                                                                                         |
-    | Slovakia             | `eu_vat`     | European VAT number                                                                                     |
-    | Slovenia             | `eu_vat`     | European VAT number                                                                                     |
-    | Slovenia             | `si_tin`     | Slovenia tax number (davčna številka)                                                                   |
-    | South Africa         | `za_vat`     | South African VAT number                                                                                |
+    | Slovakia             | `eu_vat`     | European VAT Number                                                                                     |
+    | Slovenia             | `eu_vat`     | European VAT Number                                                                                     |
+    | Slovenia             | `si_tin`     | Slovenia Tax Number (davčna številka)                                                                   |
+    | South Africa         | `za_vat`     | South African VAT Number                                                                                |
     | South Korea          | `kr_brn`     | Korean BRN                                                                                              |
-    | Spain                | `es_cif`     | Spanish NIF number (previously Spanish CIF number)                                                      |
-    | Spain                | `eu_vat`     | European VAT number                                                                                     |
-    | Sweden               | `eu_vat`     | European VAT number                                                                                     |
-    | Switzerland          | `ch_vat`     | Switzerland VAT number                                                                                  |
+    | Spain                | `es_cif`     | Spanish NIF Number (previously Spanish CIF Number)                                                      |
+    | Spain                | `eu_vat`     | European VAT Number                                                                                     |
+    | Sweden               | `eu_vat`     | European VAT Number                                                                                     |
+    | Switzerland          | `ch_vat`     | Switzerland VAT Number                                                                                  |
     | Taiwan               | `tw_vat`     | Taiwanese VAT                                                                                           |
     | Thailand             | `th_vat`     | Thai VAT                                                                                                |
     | Turkey               | `tr_tin`     | Turkish Tax Identification Number                                                                       |
     | Ukraine              | `ua_vat`     | Ukrainian VAT                                                                                           |
     | United Arab Emirates | `ae_trn`     | United Arab Emirates TRN                                                                                |
-    | United Kingdom       | `eu_vat`     | Northern Ireland VAT number                                                                             |
-    | United Kingdom       | `gb_vat`     | United Kingdom VAT number                                                                               |
+    | United Kingdom       | `eu_vat`     | Northern Ireland VAT Number                                                                             |
+    | United Kingdom       | `gb_vat`     | United Kingdom VAT Number                                                                               |
     | United States        | `us_ein`     | United States EIN                                                                                       |
+    | Uruguay              | `uy_ruc`     | Uruguayan RUC Number                                                                                    |
+    | Venezuela            | `ve_rif`     | Venezuelan RIF Number                                                                                   |
+    | Vietnam              | `vn_tin`     | Vietnamese Tax ID Number                                                                                |
     """
 
 
 class AccountingSyncConfigurationAccountingProvider(TypedDict, total=False):
     external_provider_id: Required[str]
 
     provider_type: Required[str]
@@ -218,27 +238,35 @@
 
 
 class TaxID(TypedDict, total=False):
     country: Required[
         Literal[
             "AD",
             "AE",
+            "AR",
             "AT",
             "AU",
             "BE",
             "BG",
+            "BH",
+            "BO",
             "BR",
             "CA",
             "CH",
             "CL",
+            "CN",
+            "CO",
+            "CR",
             "CY",
             "CZ",
             "DE",
             "DK",
             "EE",
+            "DO",
+            "EC",
             "EG",
             "ES",
             "EU",
             "FI",
             "FR",
             "GB",
             "GE",
@@ -251,61 +279,78 @@
             "IL",
             "IN",
             "IS",
             "IT",
             "JP",
             "KE",
             "KR",
+            "KZ",
             "LI",
             "LT",
             "LU",
             "LV",
             "MT",
             "MX",
             "MY",
+            "NG",
             "NL",
             "NO",
             "NZ",
+            "OM",
+            "PE",
             "PH",
             "PL",
             "PT",
             "RO",
+            "RS",
             "RU",
             "SA",
             "SE",
             "SG",
             "SI",
             "SK",
+            "SV",
             "TH",
             "TR",
             "TW",
             "UA",
             "US",
+            "UY",
+            "VE",
+            "VN",
             "ZA",
         ]
     ]
 
     type: Required[
         Literal[
             "ad_nrt",
             "ae_trn",
+            "ar_cuit",
             "eu_vat",
             "au_abn",
             "au_arn",
             "bg_uic",
+            "bh_vat",
+            "bo_tin",
             "br_cnpj",
             "br_cpf",
             "ca_bn",
             "ca_gst_hst",
             "ca_pst_bc",
             "ca_pst_mb",
             "ca_pst_sk",
             "ca_qst",
             "ch_vat",
             "cl_tin",
+            "cn_tin",
+            "co_nit",
+            "cr_tin",
+            "do_rcn",
+            "ec_ruc",
             "eg_tin",
             "es_cif",
             "eu_oss_vat",
             "gb_vat",
             "ge_vat",
             "hk_br",
             "hu_tin",
@@ -314,31 +359,42 @@
             "in_gst",
             "is_vat",
             "jp_cn",
             "jp_rn",
             "jp_trn",
             "ke_pin",
             "kr_brn",
+            "kz_bin",
             "li_uid",
             "mx_rfc",
             "my_frp",
             "my_itn",
             "my_sst",
+            "ng_tin",
             "no_vat",
+            "no_voec",
             "nz_gst",
+            "om_vat",
+            "pe_ruc",
             "ph_tin",
+            "ro_tin",
+            "rs_pib",
             "ru_inn",
             "ru_kpp",
             "sa_vat",
             "sg_gst",
             "sg_uen",
             "si_tin",
+            "sv_nit",
             "th_vat",
             "tr_tin",
             "tw_vat",
             "ua_vat",
             "us_ein",
+            "uy_ruc",
+            "ve_rif",
+            "vn_tin",
             "za_vat",
         ]
     ]
 
     value: Required[str]
```

### Comparing `orb_billing-1.48.0/src/orb/types/customer_update_params.py` & `orb_billing-1.49.0/src/orb/types/customer_update_params.py`

 * *Files 16% similar despite different names*

```diff
@@ -88,92 +88,112 @@
     Tax IDs are commonly required to be displayed on customer invoices, which are
     added to the headers of invoices.
 
     ### Supported Tax ID Countries and Types
 
     | Country              | Type         | Description                                                                                             |
     | -------------------- | ------------ | ------------------------------------------------------------------------------------------------------- |
-    | Andorra              | `ad_nrt`     | Andorran NRT number                                                                                     |
+    | Andorra              | `ad_nrt`     | Andorran NRT Number                                                                                     |
+    | Argentina            | `ar_cuit`    | Argentinian Tax ID Number                                                                               |
     | Australia            | `au_abn`     | Australian Business Number (AU ABN)                                                                     |
     | Australia            | `au_arn`     | Australian Taxation Office Reference Number                                                             |
-    | Austria              | `eu_vat`     | European VAT number                                                                                     |
-    | Belgium              | `eu_vat`     | European VAT number                                                                                     |
-    | Brazil               | `br_cnpj`    | Brazilian CNPJ number                                                                                   |
-    | Brazil               | `br_cpf`     | Brazilian CPF number                                                                                    |
+    | Austria              | `eu_vat`     | European VAT Number                                                                                     |
+    | Bahrain              | `bh_vat`     | Bahraini VAT Number                                                                                     |
+    | Belgium              | `eu_vat`     | European VAT Number                                                                                     |
+    | Bolivia              | `bo_tin`     | Bolivian Tax ID                                                                                         |
+    | Brazil               | `br_cnpj`    | Brazilian CNPJ Number                                                                                   |
+    | Brazil               | `br_cpf`     | Brazilian CPF Number                                                                                    |
     | Bulgaria             | `bg_uic`     | Bulgaria Unified Identification Code                                                                    |
-    | Bulgaria             | `eu_vat`     | European VAT number                                                                                     |
+    | Bulgaria             | `eu_vat`     | European VAT Number                                                                                     |
     | Canada               | `ca_bn`      | Canadian BN                                                                                             |
-    | Canada               | `ca_gst_hst` | Canadian GST/HST number                                                                                 |
-    | Canada               | `ca_pst_bc`  | Canadian PST number (British Columbia)                                                                  |
-    | Canada               | `ca_pst_mb`  | Canadian PST number (Manitoba)                                                                          |
-    | Canada               | `ca_pst_sk`  | Canadian PST number (Saskatchewan)                                                                      |
-    | Canada               | `ca_qst`     | Canadian QST number (Québec)                                                                            |
+    | Canada               | `ca_gst_hst` | Canadian GST/HST Number                                                                                 |
+    | Canada               | `ca_pst_bc`  | Canadian PST Number (British Columbia)                                                                  |
+    | Canada               | `ca_pst_mb`  | Canadian PST Number (Manitoba)                                                                          |
+    | Canada               | `ca_pst_sk`  | Canadian PST Number (Saskatchewan)                                                                      |
+    | Canada               | `ca_qst`     | Canadian QST Number (Québec)                                                                            |
     | Chile                | `cl_tin`     | Chilean TIN                                                                                             |
-    | Croatia              | `eu_vat`     | European VAT number                                                                                     |
-    | Cyprus               | `eu_vat`     | European VAT number                                                                                     |
-    | Czech Republic       | `eu_vat`     | European VAT number                                                                                     |
-    | Denmark              | `eu_vat`     | European VAT number                                                                                     |
+    | China                | `cn_tin`     | Chinese Tax ID                                                                                          |
+    | Colombia             | `co_nit`     | Colombian NIT Number                                                                                    |
+    | Costa Rica           | `cr_tin`     | Costa Rican Tax ID                                                                                      |
+    | Croatia              | `eu_vat`     | European VAT Number                                                                                     |
+    | Cyprus               | `eu_vat`     | European VAT Number                                                                                     |
+    | Czech Republic       | `eu_vat`     | European VAT Number                                                                                     |
+    | Denmark              | `eu_vat`     | European VAT Number                                                                                     |
+    | Dominican Republic   | `do_rcn`     | Dominican RCN Number                                                                                    |
+    | Ecuador              | `ec_ruc`     | Ecuadorian RUC Number                                                                                   |
     | Egypt                | `eg_tin`     | Egyptian Tax Identification Number                                                                      |
-    | Estonia              | `eu_vat`     | European VAT number                                                                                     |
-    | EU                   | `eu_oss_vat` | European One Stop Shop VAT number for non-Union scheme                                                  |
-    | Finland              | `eu_vat`     | European VAT number                                                                                     |
-    | France               | `eu_vat`     | European VAT number                                                                                     |
+    | El Salvador          | `sv_nit`     | El Salvadorian NIT Number                                                                               |
+    | Estonia              | `eu_vat`     | European VAT Number                                                                                     |
+    | EU                   | `eu_oss_vat` | European One Stop Shop VAT Number for non-Union scheme                                                  |
+    | Finland              | `eu_vat`     | European VAT Number                                                                                     |
+    | France               | `eu_vat`     | European VAT Number                                                                                     |
     | Georgia              | `ge_vat`     | Georgian VAT                                                                                            |
-    | Germany              | `eu_vat`     | European VAT number                                                                                     |
-    | Greece               | `eu_vat`     | European VAT number                                                                                     |
-    | Hong Kong            | `hk_br`      | Hong Kong BR number                                                                                     |
-    | Hungary              | `eu_vat`     | European VAT number                                                                                     |
-    | Hungary              | `hu_tin`     | Hungary tax number (adószám)                                                                            |
+    | Germany              | `eu_vat`     | European VAT Number                                                                                     |
+    | Greece               | `eu_vat`     | European VAT Number                                                                                     |
+    | Hong Kong            | `hk_br`      | Hong Kong BR Number                                                                                     |
+    | Hungary              | `eu_vat`     | European VAT Number                                                                                     |
+    | Hungary              | `hu_tin`     | Hungary Tax Number (adószám)                                                                            |
     | Iceland              | `is_vat`     | Icelandic VAT                                                                                           |
-    | India                | `in_gst`     | Indian GST number                                                                                       |
-    | Indonesia            | `id_npwp`    | Indonesian NPWP number                                                                                  |
-    | Ireland              | `eu_vat`     | European VAT number                                                                                     |
+    | India                | `in_gst`     | Indian GST Number                                                                                       |
+    | Indonesia            | `id_npwp`    | Indonesian NPWP Number                                                                                  |
+    | Ireland              | `eu_vat`     | European VAT Number                                                                                     |
     | Israel               | `il_vat`     | Israel VAT                                                                                              |
-    | Italy                | `eu_vat`     | European VAT number                                                                                     |
+    | Italy                | `eu_vat`     | European VAT Number                                                                                     |
     | Japan                | `jp_cn`      | Japanese Corporate Number (_Hōjin Bangō_)                                                               |
     | Japan                | `jp_rn`      | Japanese Registered Foreign Businesses' Registration Number (_Tōroku Kokugai Jigyōsha no Tōroku Bangō_) |
     | Japan                | `jp_trn`     | Japanese Tax Registration Number (_Tōroku Bangō_)                                                       |
+    | Kazakhstan           | `kz_bin`     | Kazakhstani Business Identification Number                                                              |
     | Kenya                | `ke_pin`     | Kenya Revenue Authority Personal Identification Number                                                  |
-    | Latvia               | `eu_vat`     | European VAT number                                                                                     |
-    | Liechtenstein        | `li_uid`     | Liechtensteinian UID number                                                                             |
-    | Lithuania            | `eu_vat`     | European VAT number                                                                                     |
-    | Luxembourg           | `eu_vat`     | European VAT number                                                                                     |
-    | Malaysia             | `my_frp`     | Malaysian FRP number                                                                                    |
+    | Latvia               | `eu_vat`     | European VAT Number                                                                                     |
+    | Liechtenstein        | `li_uid`     | Liechtensteinian UID Number                                                                             |
+    | Lithuania            | `eu_vat`     | European VAT Number                                                                                     |
+    | Luxembourg           | `eu_vat`     | European VAT Number                                                                                     |
+    | Malaysia             | `my_frp`     | Malaysian FRP Number                                                                                    |
     | Malaysia             | `my_itn`     | Malaysian ITN                                                                                           |
-    | Malaysia             | `my_sst`     | Malaysian SST number                                                                                    |
-    | Malta                | `eu_vat `    | European VAT number                                                                                     |
-    | Mexico               | `mx_rfc`     | Mexican RFC number                                                                                      |
-    | Netherlands          | `eu_vat`     | European VAT number                                                                                     |
-    | New Zealand          | `nz_gst`     | New Zealand GST number                                                                                  |
-    | Norway               | `no_vat`     | Norwegian VAT number                                                                                    |
+    | Malaysia             | `my_sst`     | Malaysian SST Number                                                                                    |
+    | Malta                | `eu_vat `    | European VAT Number                                                                                     |
+    | Mexico               | `mx_rfc`     | Mexican RFC Number                                                                                      |
+    | Netherlands          | `eu_vat`     | European VAT Number                                                                                     |
+    | New Zealand          | `nz_gst`     | New Zealand GST Number                                                                                  |
+    | Nigeria              | `ng_tin`     | Nigerian Tax Identification Number                                                                      |
+    | Norway               | `no_vat`     | Norwegian VAT Number                                                                                    |
+    | Norway               | `no_voec`    | Norwegian VAT on e-commerce Number                                                                      |
+    | Oman                 | `om_vat`     | Omani VAT Number                                                                                        |
+    | Peru                 | `pe_ruc`     | Peruvian RUC Number                                                                                     |
     | Philippines          | `ph_tin `    | Philippines Tax Identification Number                                                                   |
-    | Poland               | `eu_vat`     | European VAT number                                                                                     |
-    | Portugal             | `eu_vat`     | European VAT number                                                                                     |
-    | Romania              | `eu_vat`     | European VAT number                                                                                     |
+    | Poland               | `eu_vat`     | European VAT Number                                                                                     |
+    | Portugal             | `eu_vat`     | European VAT Number                                                                                     |
+    | Romania              | `eu_vat`     | European VAT Number                                                                                     |
+    | Romania              | `ro_tin`     | Romanian Tax ID Number                                                                                  |
     | Russia               | `ru_inn`     | Russian INN                                                                                             |
     | Russia               | `ru_kpp`     | Russian KPP                                                                                             |
-    | Saudi Arabia         | `sg_gst`     | Singaporean GST                                                                                         |
+    | Saudi Arabia         | `sa_vat`     | Saudi Arabia VAT                                                                                        |
+    | Serbia               | `rs_pib`     | Serbian PIB Number                                                                                      |
+    | Singapore            | `sg_gst`     | Singaporean GST                                                                                         |
     | Singapore            | `sg_uen`     | Singaporean UEN                                                                                         |
-    | Slovakia             | `eu_vat`     | European VAT number                                                                                     |
-    | Slovenia             | `eu_vat`     | European VAT number                                                                                     |
-    | Slovenia             | `si_tin`     | Slovenia tax number (davčna številka)                                                                   |
-    | South Africa         | `za_vat`     | South African VAT number                                                                                |
+    | Slovakia             | `eu_vat`     | European VAT Number                                                                                     |
+    | Slovenia             | `eu_vat`     | European VAT Number                                                                                     |
+    | Slovenia             | `si_tin`     | Slovenia Tax Number (davčna številka)                                                                   |
+    | South Africa         | `za_vat`     | South African VAT Number                                                                                |
     | South Korea          | `kr_brn`     | Korean BRN                                                                                              |
-    | Spain                | `es_cif`     | Spanish NIF number (previously Spanish CIF number)                                                      |
-    | Spain                | `eu_vat`     | European VAT number                                                                                     |
-    | Sweden               | `eu_vat`     | European VAT number                                                                                     |
-    | Switzerland          | `ch_vat`     | Switzerland VAT number                                                                                  |
+    | Spain                | `es_cif`     | Spanish NIF Number (previously Spanish CIF Number)                                                      |
+    | Spain                | `eu_vat`     | European VAT Number                                                                                     |
+    | Sweden               | `eu_vat`     | European VAT Number                                                                                     |
+    | Switzerland          | `ch_vat`     | Switzerland VAT Number                                                                                  |
     | Taiwan               | `tw_vat`     | Taiwanese VAT                                                                                           |
     | Thailand             | `th_vat`     | Thai VAT                                                                                                |
     | Turkey               | `tr_tin`     | Turkish Tax Identification Number                                                                       |
     | Ukraine              | `ua_vat`     | Ukrainian VAT                                                                                           |
     | United Arab Emirates | `ae_trn`     | United Arab Emirates TRN                                                                                |
-    | United Kingdom       | `eu_vat`     | Northern Ireland VAT number                                                                             |
-    | United Kingdom       | `gb_vat`     | United Kingdom VAT number                                                                               |
+    | United Kingdom       | `eu_vat`     | Northern Ireland VAT Number                                                                             |
+    | United Kingdom       | `gb_vat`     | United Kingdom VAT Number                                                                               |
     | United States        | `us_ein`     | United States EIN                                                                                       |
+    | Uruguay              | `uy_ruc`     | Uruguayan RUC Number                                                                                    |
+    | Venezuela            | `ve_rif`     | Venezuelan RIF Number                                                                                   |
+    | Vietnam              | `vn_tin`     | Vietnamese Tax ID Number                                                                                |
     """
 
 
 class AccountingSyncConfigurationAccountingProvider(TypedDict, total=False):
     external_provider_id: Required[str]
 
     provider_type: Required[str]
@@ -218,27 +238,35 @@
 
 
 class TaxID(TypedDict, total=False):
     country: Required[
         Literal[
             "AD",
             "AE",
+            "AR",
             "AT",
             "AU",
             "BE",
             "BG",
+            "BH",
+            "BO",
             "BR",
             "CA",
             "CH",
             "CL",
+            "CN",
+            "CO",
+            "CR",
             "CY",
             "CZ",
             "DE",
             "DK",
             "EE",
+            "DO",
+            "EC",
             "EG",
             "ES",
             "EU",
             "FI",
             "FR",
             "GB",
             "GE",
@@ -251,61 +279,78 @@
             "IL",
             "IN",
             "IS",
             "IT",
             "JP",
             "KE",
             "KR",
+            "KZ",
             "LI",
             "LT",
             "LU",
             "LV",
             "MT",
             "MX",
             "MY",
+            "NG",
             "NL",
             "NO",
             "NZ",
+            "OM",
+            "PE",
             "PH",
             "PL",
             "PT",
             "RO",
+            "RS",
             "RU",
             "SA",
             "SE",
             "SG",
             "SI",
             "SK",
+            "SV",
             "TH",
             "TR",
             "TW",
             "UA",
             "US",
+            "UY",
+            "VE",
+            "VN",
             "ZA",
         ]
     ]
 
     type: Required[
         Literal[
             "ad_nrt",
             "ae_trn",
+            "ar_cuit",
             "eu_vat",
             "au_abn",
             "au_arn",
             "bg_uic",
+            "bh_vat",
+            "bo_tin",
             "br_cnpj",
             "br_cpf",
             "ca_bn",
             "ca_gst_hst",
             "ca_pst_bc",
             "ca_pst_mb",
             "ca_pst_sk",
             "ca_qst",
             "ch_vat",
             "cl_tin",
+            "cn_tin",
+            "co_nit",
+            "cr_tin",
+            "do_rcn",
+            "ec_ruc",
             "eg_tin",
             "es_cif",
             "eu_oss_vat",
             "gb_vat",
             "ge_vat",
             "hk_br",
             "hu_tin",
@@ -314,31 +359,42 @@
             "in_gst",
             "is_vat",
             "jp_cn",
             "jp_rn",
             "jp_trn",
             "ke_pin",
             "kr_brn",
+            "kz_bin",
             "li_uid",
             "mx_rfc",
             "my_frp",
             "my_itn",
             "my_sst",
+            "ng_tin",
             "no_vat",
+            "no_voec",
             "nz_gst",
+            "om_vat",
+            "pe_ruc",
             "ph_tin",
+            "ro_tin",
+            "rs_pib",
             "ru_inn",
             "ru_kpp",
             "sa_vat",
             "sg_gst",
             "sg_uen",
             "si_tin",
+            "sv_nit",
             "th_vat",
             "tr_tin",
             "tw_vat",
             "ua_vat",
             "us_ein",
+            "uy_ruc",
+            "ve_rif",
+            "vn_tin",
             "za_vat",
         ]
     ]
 
     value: Required[str]
```

### Comparing `orb_billing-1.48.0/src/orb/types/event_ingest_params.py` & `orb_billing-1.49.0/src/orb/types/event_ingest_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/event_ingest_response.py` & `orb_billing-1.49.0/src/orb/types/event_ingest_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/event_search_params.py` & `orb_billing-1.49.0/src/orb/types/event_search_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/event_search_response.py` & `orb_billing-1.49.0/src/orb/types/event_search_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/event_update_params.py` & `orb_billing-1.49.0/src/orb/types/event_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/invoice.py` & `orb_billing-1.49.0/src/orb/types/invoice.py`

 * *Files 12% similar despite different names*

```diff
@@ -154,27 +154,35 @@
     type: Literal["increment", "decrement"]
 
 
 class CustomerTaxID(BaseModel):
     country: Literal[
         "AD",
         "AE",
+        "AR",
         "AT",
         "AU",
         "BE",
         "BG",
+        "BH",
+        "BO",
         "BR",
         "CA",
         "CH",
         "CL",
+        "CN",
+        "CO",
+        "CR",
         "CY",
         "CZ",
         "DE",
         "DK",
         "EE",
+        "DO",
+        "EC",
         "EG",
         "ES",
         "EU",
         "FI",
         "FR",
         "GB",
         "GE",
@@ -187,59 +195,76 @@
         "IL",
         "IN",
         "IS",
         "IT",
         "JP",
         "KE",
         "KR",
+        "KZ",
         "LI",
         "LT",
         "LU",
         "LV",
         "MT",
         "MX",
         "MY",
+        "NG",
         "NL",
         "NO",
         "NZ",
+        "OM",
+        "PE",
         "PH",
         "PL",
         "PT",
         "RO",
+        "RS",
         "RU",
         "SA",
         "SE",
         "SG",
         "SI",
         "SK",
+        "SV",
         "TH",
         "TR",
         "TW",
         "UA",
         "US",
+        "UY",
+        "VE",
+        "VN",
         "ZA",
     ]
 
     type: Literal[
         "ad_nrt",
         "ae_trn",
+        "ar_cuit",
         "eu_vat",
         "au_abn",
         "au_arn",
         "bg_uic",
+        "bh_vat",
+        "bo_tin",
         "br_cnpj",
         "br_cpf",
         "ca_bn",
         "ca_gst_hst",
         "ca_pst_bc",
         "ca_pst_mb",
         "ca_pst_sk",
         "ca_qst",
         "ch_vat",
         "cl_tin",
+        "cn_tin",
+        "co_nit",
+        "cr_tin",
+        "do_rcn",
+        "ec_ruc",
         "eg_tin",
         "es_cif",
         "eu_oss_vat",
         "gb_vat",
         "ge_vat",
         "hk_br",
         "hu_tin",
@@ -248,33 +273,44 @@
         "in_gst",
         "is_vat",
         "jp_cn",
         "jp_rn",
         "jp_trn",
         "ke_pin",
         "kr_brn",
+        "kz_bin",
         "li_uid",
         "mx_rfc",
         "my_frp",
         "my_itn",
         "my_sst",
+        "ng_tin",
         "no_vat",
+        "no_voec",
         "nz_gst",
+        "om_vat",
+        "pe_ruc",
         "ph_tin",
+        "ro_tin",
+        "rs_pib",
         "ru_inn",
         "ru_kpp",
         "sa_vat",
         "sg_gst",
         "sg_uen",
         "si_tin",
+        "sv_nit",
         "th_vat",
         "tr_tin",
         "tw_vat",
         "ua_vat",
         "us_ein",
+        "uy_ruc",
+        "ve_rif",
+        "vn_tin",
         "za_vat",
     ]
 
     value: str
 
 
 class LineItemMaximum(BaseModel):
@@ -749,92 +785,112 @@
     Tax IDs are commonly required to be displayed on customer invoices, which are
     added to the headers of invoices.
 
     ### Supported Tax ID Countries and Types
 
     | Country              | Type         | Description                                                                                             |
     | -------------------- | ------------ | ------------------------------------------------------------------------------------------------------- |
-    | Andorra              | `ad_nrt`     | Andorran NRT number                                                                                     |
+    | Andorra              | `ad_nrt`     | Andorran NRT Number                                                                                     |
+    | Argentina            | `ar_cuit`    | Argentinian Tax ID Number                                                                               |
     | Australia            | `au_abn`     | Australian Business Number (AU ABN)                                                                     |
     | Australia            | `au_arn`     | Australian Taxation Office Reference Number                                                             |
-    | Austria              | `eu_vat`     | European VAT number                                                                                     |
-    | Belgium              | `eu_vat`     | European VAT number                                                                                     |
-    | Brazil               | `br_cnpj`    | Brazilian CNPJ number                                                                                   |
-    | Brazil               | `br_cpf`     | Brazilian CPF number                                                                                    |
+    | Austria              | `eu_vat`     | European VAT Number                                                                                     |
+    | Bahrain              | `bh_vat`     | Bahraini VAT Number                                                                                     |
+    | Belgium              | `eu_vat`     | European VAT Number                                                                                     |
+    | Bolivia              | `bo_tin`     | Bolivian Tax ID                                                                                         |
+    | Brazil               | `br_cnpj`    | Brazilian CNPJ Number                                                                                   |
+    | Brazil               | `br_cpf`     | Brazilian CPF Number                                                                                    |
     | Bulgaria             | `bg_uic`     | Bulgaria Unified Identification Code                                                                    |
-    | Bulgaria             | `eu_vat`     | European VAT number                                                                                     |
+    | Bulgaria             | `eu_vat`     | European VAT Number                                                                                     |
     | Canada               | `ca_bn`      | Canadian BN                                                                                             |
-    | Canada               | `ca_gst_hst` | Canadian GST/HST number                                                                                 |
-    | Canada               | `ca_pst_bc`  | Canadian PST number (British Columbia)                                                                  |
-    | Canada               | `ca_pst_mb`  | Canadian PST number (Manitoba)                                                                          |
-    | Canada               | `ca_pst_sk`  | Canadian PST number (Saskatchewan)                                                                      |
-    | Canada               | `ca_qst`     | Canadian QST number (Québec)                                                                            |
+    | Canada               | `ca_gst_hst` | Canadian GST/HST Number                                                                                 |
+    | Canada               | `ca_pst_bc`  | Canadian PST Number (British Columbia)                                                                  |
+    | Canada               | `ca_pst_mb`  | Canadian PST Number (Manitoba)                                                                          |
+    | Canada               | `ca_pst_sk`  | Canadian PST Number (Saskatchewan)                                                                      |
+    | Canada               | `ca_qst`     | Canadian QST Number (Québec)                                                                            |
     | Chile                | `cl_tin`     | Chilean TIN                                                                                             |
-    | Croatia              | `eu_vat`     | European VAT number                                                                                     |
-    | Cyprus               | `eu_vat`     | European VAT number                                                                                     |
-    | Czech Republic       | `eu_vat`     | European VAT number                                                                                     |
-    | Denmark              | `eu_vat`     | European VAT number                                                                                     |
+    | China                | `cn_tin`     | Chinese Tax ID                                                                                          |
+    | Colombia             | `co_nit`     | Colombian NIT Number                                                                                    |
+    | Costa Rica           | `cr_tin`     | Costa Rican Tax ID                                                                                      |
+    | Croatia              | `eu_vat`     | European VAT Number                                                                                     |
+    | Cyprus               | `eu_vat`     | European VAT Number                                                                                     |
+    | Czech Republic       | `eu_vat`     | European VAT Number                                                                                     |
+    | Denmark              | `eu_vat`     | European VAT Number                                                                                     |
+    | Dominican Republic   | `do_rcn`     | Dominican RCN Number                                                                                    |
+    | Ecuador              | `ec_ruc`     | Ecuadorian RUC Number                                                                                   |
     | Egypt                | `eg_tin`     | Egyptian Tax Identification Number                                                                      |
-    | Estonia              | `eu_vat`     | European VAT number                                                                                     |
-    | EU                   | `eu_oss_vat` | European One Stop Shop VAT number for non-Union scheme                                                  |
-    | Finland              | `eu_vat`     | European VAT number                                                                                     |
-    | France               | `eu_vat`     | European VAT number                                                                                     |
+    | El Salvador          | `sv_nit`     | El Salvadorian NIT Number                                                                               |
+    | Estonia              | `eu_vat`     | European VAT Number                                                                                     |
+    | EU                   | `eu_oss_vat` | European One Stop Shop VAT Number for non-Union scheme                                                  |
+    | Finland              | `eu_vat`     | European VAT Number                                                                                     |
+    | France               | `eu_vat`     | European VAT Number                                                                                     |
     | Georgia              | `ge_vat`     | Georgian VAT                                                                                            |
-    | Germany              | `eu_vat`     | European VAT number                                                                                     |
-    | Greece               | `eu_vat`     | European VAT number                                                                                     |
-    | Hong Kong            | `hk_br`      | Hong Kong BR number                                                                                     |
-    | Hungary              | `eu_vat`     | European VAT number                                                                                     |
-    | Hungary              | `hu_tin`     | Hungary tax number (adószám)                                                                            |
+    | Germany              | `eu_vat`     | European VAT Number                                                                                     |
+    | Greece               | `eu_vat`     | European VAT Number                                                                                     |
+    | Hong Kong            | `hk_br`      | Hong Kong BR Number                                                                                     |
+    | Hungary              | `eu_vat`     | European VAT Number                                                                                     |
+    | Hungary              | `hu_tin`     | Hungary Tax Number (adószám)                                                                            |
     | Iceland              | `is_vat`     | Icelandic VAT                                                                                           |
-    | India                | `in_gst`     | Indian GST number                                                                                       |
-    | Indonesia            | `id_npwp`    | Indonesian NPWP number                                                                                  |
-    | Ireland              | `eu_vat`     | European VAT number                                                                                     |
+    | India                | `in_gst`     | Indian GST Number                                                                                       |
+    | Indonesia            | `id_npwp`    | Indonesian NPWP Number                                                                                  |
+    | Ireland              | `eu_vat`     | European VAT Number                                                                                     |
     | Israel               | `il_vat`     | Israel VAT                                                                                              |
-    | Italy                | `eu_vat`     | European VAT number                                                                                     |
+    | Italy                | `eu_vat`     | European VAT Number                                                                                     |
     | Japan                | `jp_cn`      | Japanese Corporate Number (_Hōjin Bangō_)                                                               |
     | Japan                | `jp_rn`      | Japanese Registered Foreign Businesses' Registration Number (_Tōroku Kokugai Jigyōsha no Tōroku Bangō_) |
     | Japan                | `jp_trn`     | Japanese Tax Registration Number (_Tōroku Bangō_)                                                       |
+    | Kazakhstan           | `kz_bin`     | Kazakhstani Business Identification Number                                                              |
     | Kenya                | `ke_pin`     | Kenya Revenue Authority Personal Identification Number                                                  |
-    | Latvia               | `eu_vat`     | European VAT number                                                                                     |
-    | Liechtenstein        | `li_uid`     | Liechtensteinian UID number                                                                             |
-    | Lithuania            | `eu_vat`     | European VAT number                                                                                     |
-    | Luxembourg           | `eu_vat`     | European VAT number                                                                                     |
-    | Malaysia             | `my_frp`     | Malaysian FRP number                                                                                    |
+    | Latvia               | `eu_vat`     | European VAT Number                                                                                     |
+    | Liechtenstein        | `li_uid`     | Liechtensteinian UID Number                                                                             |
+    | Lithuania            | `eu_vat`     | European VAT Number                                                                                     |
+    | Luxembourg           | `eu_vat`     | European VAT Number                                                                                     |
+    | Malaysia             | `my_frp`     | Malaysian FRP Number                                                                                    |
     | Malaysia             | `my_itn`     | Malaysian ITN                                                                                           |
-    | Malaysia             | `my_sst`     | Malaysian SST number                                                                                    |
-    | Malta                | `eu_vat `    | European VAT number                                                                                     |
-    | Mexico               | `mx_rfc`     | Mexican RFC number                                                                                      |
-    | Netherlands          | `eu_vat`     | European VAT number                                                                                     |
-    | New Zealand          | `nz_gst`     | New Zealand GST number                                                                                  |
-    | Norway               | `no_vat`     | Norwegian VAT number                                                                                    |
+    | Malaysia             | `my_sst`     | Malaysian SST Number                                                                                    |
+    | Malta                | `eu_vat `    | European VAT Number                                                                                     |
+    | Mexico               | `mx_rfc`     | Mexican RFC Number                                                                                      |
+    | Netherlands          | `eu_vat`     | European VAT Number                                                                                     |
+    | New Zealand          | `nz_gst`     | New Zealand GST Number                                                                                  |
+    | Nigeria              | `ng_tin`     | Nigerian Tax Identification Number                                                                      |
+    | Norway               | `no_vat`     | Norwegian VAT Number                                                                                    |
+    | Norway               | `no_voec`    | Norwegian VAT on e-commerce Number                                                                      |
+    | Oman                 | `om_vat`     | Omani VAT Number                                                                                        |
+    | Peru                 | `pe_ruc`     | Peruvian RUC Number                                                                                     |
     | Philippines          | `ph_tin `    | Philippines Tax Identification Number                                                                   |
-    | Poland               | `eu_vat`     | European VAT number                                                                                     |
-    | Portugal             | `eu_vat`     | European VAT number                                                                                     |
-    | Romania              | `eu_vat`     | European VAT number                                                                                     |
+    | Poland               | `eu_vat`     | European VAT Number                                                                                     |
+    | Portugal             | `eu_vat`     | European VAT Number                                                                                     |
+    | Romania              | `eu_vat`     | European VAT Number                                                                                     |
+    | Romania              | `ro_tin`     | Romanian Tax ID Number                                                                                  |
     | Russia               | `ru_inn`     | Russian INN                                                                                             |
     | Russia               | `ru_kpp`     | Russian KPP                                                                                             |
-    | Saudi Arabia         | `sg_gst`     | Singaporean GST                                                                                         |
+    | Saudi Arabia         | `sa_vat`     | Saudi Arabia VAT                                                                                        |
+    | Serbia               | `rs_pib`     | Serbian PIB Number                                                                                      |
+    | Singapore            | `sg_gst`     | Singaporean GST                                                                                         |
     | Singapore            | `sg_uen`     | Singaporean UEN                                                                                         |
-    | Slovakia             | `eu_vat`     | European VAT number                                                                                     |
-    | Slovenia             | `eu_vat`     | European VAT number                                                                                     |
-    | Slovenia             | `si_tin`     | Slovenia tax number (davčna številka)                                                                   |
-    | South Africa         | `za_vat`     | South African VAT number                                                                                |
+    | Slovakia             | `eu_vat`     | European VAT Number                                                                                     |
+    | Slovenia             | `eu_vat`     | European VAT Number                                                                                     |
+    | Slovenia             | `si_tin`     | Slovenia Tax Number (davčna številka)                                                                   |
+    | South Africa         | `za_vat`     | South African VAT Number                                                                                |
     | South Korea          | `kr_brn`     | Korean BRN                                                                                              |
-    | Spain                | `es_cif`     | Spanish NIF number (previously Spanish CIF number)                                                      |
-    | Spain                | `eu_vat`     | European VAT number                                                                                     |
-    | Sweden               | `eu_vat`     | European VAT number                                                                                     |
-    | Switzerland          | `ch_vat`     | Switzerland VAT number                                                                                  |
+    | Spain                | `es_cif`     | Spanish NIF Number (previously Spanish CIF Number)                                                      |
+    | Spain                | `eu_vat`     | European VAT Number                                                                                     |
+    | Sweden               | `eu_vat`     | European VAT Number                                                                                     |
+    | Switzerland          | `ch_vat`     | Switzerland VAT Number                                                                                  |
     | Taiwan               | `tw_vat`     | Taiwanese VAT                                                                                           |
     | Thailand             | `th_vat`     | Thai VAT                                                                                                |
     | Turkey               | `tr_tin`     | Turkish Tax Identification Number                                                                       |
     | Ukraine              | `ua_vat`     | Ukrainian VAT                                                                                           |
     | United Arab Emirates | `ae_trn`     | United Arab Emirates TRN                                                                                |
-    | United Kingdom       | `eu_vat`     | Northern Ireland VAT number                                                                             |
-    | United Kingdom       | `gb_vat`     | United Kingdom VAT number                                                                               |
+    | United Kingdom       | `eu_vat`     | Northern Ireland VAT Number                                                                             |
+    | United Kingdom       | `gb_vat`     | United Kingdom VAT Number                                                                               |
     | United States        | `us_ein`     | United States EIN                                                                                       |
+    | Uruguay              | `uy_ruc`     | Uruguayan RUC Number                                                                                    |
+    | Venezuela            | `ve_rif`     | Venezuelan RIF Number                                                                                   |
+    | Vietnam              | `vn_tin`     | Vietnamese Tax ID Number                                                                                |
     """
 
     discount: Optional[Discount] = None
 
     discounts: List[Discount]
 
     due_date: datetime
```

### Comparing `orb_billing-1.48.0/src/orb/types/invoice_create_params.py` & `orb_billing-1.49.0/src/orb/types/invoice_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/invoice_fetch_upcoming_response.py` & `orb_billing-1.49.0/src/orb/types/invoice_fetch_upcoming_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -154,27 +154,35 @@
     type: Literal["increment", "decrement"]
 
 
 class CustomerTaxID(BaseModel):
     country: Literal[
         "AD",
         "AE",
+        "AR",
         "AT",
         "AU",
         "BE",
         "BG",
+        "BH",
+        "BO",
         "BR",
         "CA",
         "CH",
         "CL",
+        "CN",
+        "CO",
+        "CR",
         "CY",
         "CZ",
         "DE",
         "DK",
         "EE",
+        "DO",
+        "EC",
         "EG",
         "ES",
         "EU",
         "FI",
         "FR",
         "GB",
         "GE",
@@ -187,59 +195,76 @@
         "IL",
         "IN",
         "IS",
         "IT",
         "JP",
         "KE",
         "KR",
+        "KZ",
         "LI",
         "LT",
         "LU",
         "LV",
         "MT",
         "MX",
         "MY",
+        "NG",
         "NL",
         "NO",
         "NZ",
+        "OM",
+        "PE",
         "PH",
         "PL",
         "PT",
         "RO",
+        "RS",
         "RU",
         "SA",
         "SE",
         "SG",
         "SI",
         "SK",
+        "SV",
         "TH",
         "TR",
         "TW",
         "UA",
         "US",
+        "UY",
+        "VE",
+        "VN",
         "ZA",
     ]
 
     type: Literal[
         "ad_nrt",
         "ae_trn",
+        "ar_cuit",
         "eu_vat",
         "au_abn",
         "au_arn",
         "bg_uic",
+        "bh_vat",
+        "bo_tin",
         "br_cnpj",
         "br_cpf",
         "ca_bn",
         "ca_gst_hst",
         "ca_pst_bc",
         "ca_pst_mb",
         "ca_pst_sk",
         "ca_qst",
         "ch_vat",
         "cl_tin",
+        "cn_tin",
+        "co_nit",
+        "cr_tin",
+        "do_rcn",
+        "ec_ruc",
         "eg_tin",
         "es_cif",
         "eu_oss_vat",
         "gb_vat",
         "ge_vat",
         "hk_br",
         "hu_tin",
@@ -248,33 +273,44 @@
         "in_gst",
         "is_vat",
         "jp_cn",
         "jp_rn",
         "jp_trn",
         "ke_pin",
         "kr_brn",
+        "kz_bin",
         "li_uid",
         "mx_rfc",
         "my_frp",
         "my_itn",
         "my_sst",
+        "ng_tin",
         "no_vat",
+        "no_voec",
         "nz_gst",
+        "om_vat",
+        "pe_ruc",
         "ph_tin",
+        "ro_tin",
+        "rs_pib",
         "ru_inn",
         "ru_kpp",
         "sa_vat",
         "sg_gst",
         "sg_uen",
         "si_tin",
+        "sv_nit",
         "th_vat",
         "tr_tin",
         "tw_vat",
         "ua_vat",
         "us_ein",
+        "uy_ruc",
+        "ve_rif",
+        "vn_tin",
         "za_vat",
     ]
 
     value: str
 
 
 class LineItemMaximum(BaseModel):
@@ -749,92 +785,112 @@
     Tax IDs are commonly required to be displayed on customer invoices, which are
     added to the headers of invoices.
 
     ### Supported Tax ID Countries and Types
 
     | Country              | Type         | Description                                                                                             |
     | -------------------- | ------------ | ------------------------------------------------------------------------------------------------------- |
-    | Andorra              | `ad_nrt`     | Andorran NRT number                                                                                     |
+    | Andorra              | `ad_nrt`     | Andorran NRT Number                                                                                     |
+    | Argentina            | `ar_cuit`    | Argentinian Tax ID Number                                                                               |
     | Australia            | `au_abn`     | Australian Business Number (AU ABN)                                                                     |
     | Australia            | `au_arn`     | Australian Taxation Office Reference Number                                                             |
-    | Austria              | `eu_vat`     | European VAT number                                                                                     |
-    | Belgium              | `eu_vat`     | European VAT number                                                                                     |
-    | Brazil               | `br_cnpj`    | Brazilian CNPJ number                                                                                   |
-    | Brazil               | `br_cpf`     | Brazilian CPF number                                                                                    |
+    | Austria              | `eu_vat`     | European VAT Number                                                                                     |
+    | Bahrain              | `bh_vat`     | Bahraini VAT Number                                                                                     |
+    | Belgium              | `eu_vat`     | European VAT Number                                                                                     |
+    | Bolivia              | `bo_tin`     | Bolivian Tax ID                                                                                         |
+    | Brazil               | `br_cnpj`    | Brazilian CNPJ Number                                                                                   |
+    | Brazil               | `br_cpf`     | Brazilian CPF Number                                                                                    |
     | Bulgaria             | `bg_uic`     | Bulgaria Unified Identification Code                                                                    |
-    | Bulgaria             | `eu_vat`     | European VAT number                                                                                     |
+    | Bulgaria             | `eu_vat`     | European VAT Number                                                                                     |
     | Canada               | `ca_bn`      | Canadian BN                                                                                             |
-    | Canada               | `ca_gst_hst` | Canadian GST/HST number                                                                                 |
-    | Canada               | `ca_pst_bc`  | Canadian PST number (British Columbia)                                                                  |
-    | Canada               | `ca_pst_mb`  | Canadian PST number (Manitoba)                                                                          |
-    | Canada               | `ca_pst_sk`  | Canadian PST number (Saskatchewan)                                                                      |
-    | Canada               | `ca_qst`     | Canadian QST number (Québec)                                                                            |
+    | Canada               | `ca_gst_hst` | Canadian GST/HST Number                                                                                 |
+    | Canada               | `ca_pst_bc`  | Canadian PST Number (British Columbia)                                                                  |
+    | Canada               | `ca_pst_mb`  | Canadian PST Number (Manitoba)                                                                          |
+    | Canada               | `ca_pst_sk`  | Canadian PST Number (Saskatchewan)                                                                      |
+    | Canada               | `ca_qst`     | Canadian QST Number (Québec)                                                                            |
     | Chile                | `cl_tin`     | Chilean TIN                                                                                             |
-    | Croatia              | `eu_vat`     | European VAT number                                                                                     |
-    | Cyprus               | `eu_vat`     | European VAT number                                                                                     |
-    | Czech Republic       | `eu_vat`     | European VAT number                                                                                     |
-    | Denmark              | `eu_vat`     | European VAT number                                                                                     |
+    | China                | `cn_tin`     | Chinese Tax ID                                                                                          |
+    | Colombia             | `co_nit`     | Colombian NIT Number                                                                                    |
+    | Costa Rica           | `cr_tin`     | Costa Rican Tax ID                                                                                      |
+    | Croatia              | `eu_vat`     | European VAT Number                                                                                     |
+    | Cyprus               | `eu_vat`     | European VAT Number                                                                                     |
+    | Czech Republic       | `eu_vat`     | European VAT Number                                                                                     |
+    | Denmark              | `eu_vat`     | European VAT Number                                                                                     |
+    | Dominican Republic   | `do_rcn`     | Dominican RCN Number                                                                                    |
+    | Ecuador              | `ec_ruc`     | Ecuadorian RUC Number                                                                                   |
     | Egypt                | `eg_tin`     | Egyptian Tax Identification Number                                                                      |
-    | Estonia              | `eu_vat`     | European VAT number                                                                                     |
-    | EU                   | `eu_oss_vat` | European One Stop Shop VAT number for non-Union scheme                                                  |
-    | Finland              | `eu_vat`     | European VAT number                                                                                     |
-    | France               | `eu_vat`     | European VAT number                                                                                     |
+    | El Salvador          | `sv_nit`     | El Salvadorian NIT Number                                                                               |
+    | Estonia              | `eu_vat`     | European VAT Number                                                                                     |
+    | EU                   | `eu_oss_vat` | European One Stop Shop VAT Number for non-Union scheme                                                  |
+    | Finland              | `eu_vat`     | European VAT Number                                                                                     |
+    | France               | `eu_vat`     | European VAT Number                                                                                     |
     | Georgia              | `ge_vat`     | Georgian VAT                                                                                            |
-    | Germany              | `eu_vat`     | European VAT number                                                                                     |
-    | Greece               | `eu_vat`     | European VAT number                                                                                     |
-    | Hong Kong            | `hk_br`      | Hong Kong BR number                                                                                     |
-    | Hungary              | `eu_vat`     | European VAT number                                                                                     |
-    | Hungary              | `hu_tin`     | Hungary tax number (adószám)                                                                            |
+    | Germany              | `eu_vat`     | European VAT Number                                                                                     |
+    | Greece               | `eu_vat`     | European VAT Number                                                                                     |
+    | Hong Kong            | `hk_br`      | Hong Kong BR Number                                                                                     |
+    | Hungary              | `eu_vat`     | European VAT Number                                                                                     |
+    | Hungary              | `hu_tin`     | Hungary Tax Number (adószám)                                                                            |
     | Iceland              | `is_vat`     | Icelandic VAT                                                                                           |
-    | India                | `in_gst`     | Indian GST number                                                                                       |
-    | Indonesia            | `id_npwp`    | Indonesian NPWP number                                                                                  |
-    | Ireland              | `eu_vat`     | European VAT number                                                                                     |
+    | India                | `in_gst`     | Indian GST Number                                                                                       |
+    | Indonesia            | `id_npwp`    | Indonesian NPWP Number                                                                                  |
+    | Ireland              | `eu_vat`     | European VAT Number                                                                                     |
     | Israel               | `il_vat`     | Israel VAT                                                                                              |
-    | Italy                | `eu_vat`     | European VAT number                                                                                     |
+    | Italy                | `eu_vat`     | European VAT Number                                                                                     |
     | Japan                | `jp_cn`      | Japanese Corporate Number (_Hōjin Bangō_)                                                               |
     | Japan                | `jp_rn`      | Japanese Registered Foreign Businesses' Registration Number (_Tōroku Kokugai Jigyōsha no Tōroku Bangō_) |
     | Japan                | `jp_trn`     | Japanese Tax Registration Number (_Tōroku Bangō_)                                                       |
+    | Kazakhstan           | `kz_bin`     | Kazakhstani Business Identification Number                                                              |
     | Kenya                | `ke_pin`     | Kenya Revenue Authority Personal Identification Number                                                  |
-    | Latvia               | `eu_vat`     | European VAT number                                                                                     |
-    | Liechtenstein        | `li_uid`     | Liechtensteinian UID number                                                                             |
-    | Lithuania            | `eu_vat`     | European VAT number                                                                                     |
-    | Luxembourg           | `eu_vat`     | European VAT number                                                                                     |
-    | Malaysia             | `my_frp`     | Malaysian FRP number                                                                                    |
+    | Latvia               | `eu_vat`     | European VAT Number                                                                                     |
+    | Liechtenstein        | `li_uid`     | Liechtensteinian UID Number                                                                             |
+    | Lithuania            | `eu_vat`     | European VAT Number                                                                                     |
+    | Luxembourg           | `eu_vat`     | European VAT Number                                                                                     |
+    | Malaysia             | `my_frp`     | Malaysian FRP Number                                                                                    |
     | Malaysia             | `my_itn`     | Malaysian ITN                                                                                           |
-    | Malaysia             | `my_sst`     | Malaysian SST number                                                                                    |
-    | Malta                | `eu_vat `    | European VAT number                                                                                     |
-    | Mexico               | `mx_rfc`     | Mexican RFC number                                                                                      |
-    | Netherlands          | `eu_vat`     | European VAT number                                                                                     |
-    | New Zealand          | `nz_gst`     | New Zealand GST number                                                                                  |
-    | Norway               | `no_vat`     | Norwegian VAT number                                                                                    |
+    | Malaysia             | `my_sst`     | Malaysian SST Number                                                                                    |
+    | Malta                | `eu_vat `    | European VAT Number                                                                                     |
+    | Mexico               | `mx_rfc`     | Mexican RFC Number                                                                                      |
+    | Netherlands          | `eu_vat`     | European VAT Number                                                                                     |
+    | New Zealand          | `nz_gst`     | New Zealand GST Number                                                                                  |
+    | Nigeria              | `ng_tin`     | Nigerian Tax Identification Number                                                                      |
+    | Norway               | `no_vat`     | Norwegian VAT Number                                                                                    |
+    | Norway               | `no_voec`    | Norwegian VAT on e-commerce Number                                                                      |
+    | Oman                 | `om_vat`     | Omani VAT Number                                                                                        |
+    | Peru                 | `pe_ruc`     | Peruvian RUC Number                                                                                     |
     | Philippines          | `ph_tin `    | Philippines Tax Identification Number                                                                   |
-    | Poland               | `eu_vat`     | European VAT number                                                                                     |
-    | Portugal             | `eu_vat`     | European VAT number                                                                                     |
-    | Romania              | `eu_vat`     | European VAT number                                                                                     |
+    | Poland               | `eu_vat`     | European VAT Number                                                                                     |
+    | Portugal             | `eu_vat`     | European VAT Number                                                                                     |
+    | Romania              | `eu_vat`     | European VAT Number                                                                                     |
+    | Romania              | `ro_tin`     | Romanian Tax ID Number                                                                                  |
     | Russia               | `ru_inn`     | Russian INN                                                                                             |
     | Russia               | `ru_kpp`     | Russian KPP                                                                                             |
-    | Saudi Arabia         | `sg_gst`     | Singaporean GST                                                                                         |
+    | Saudi Arabia         | `sa_vat`     | Saudi Arabia VAT                                                                                        |
+    | Serbia               | `rs_pib`     | Serbian PIB Number                                                                                      |
+    | Singapore            | `sg_gst`     | Singaporean GST                                                                                         |
     | Singapore            | `sg_uen`     | Singaporean UEN                                                                                         |
-    | Slovakia             | `eu_vat`     | European VAT number                                                                                     |
-    | Slovenia             | `eu_vat`     | European VAT number                                                                                     |
-    | Slovenia             | `si_tin`     | Slovenia tax number (davčna številka)                                                                   |
-    | South Africa         | `za_vat`     | South African VAT number                                                                                |
+    | Slovakia             | `eu_vat`     | European VAT Number                                                                                     |
+    | Slovenia             | `eu_vat`     | European VAT Number                                                                                     |
+    | Slovenia             | `si_tin`     | Slovenia Tax Number (davčna številka)                                                                   |
+    | South Africa         | `za_vat`     | South African VAT Number                                                                                |
     | South Korea          | `kr_brn`     | Korean BRN                                                                                              |
-    | Spain                | `es_cif`     | Spanish NIF number (previously Spanish CIF number)                                                      |
-    | Spain                | `eu_vat`     | European VAT number                                                                                     |
-    | Sweden               | `eu_vat`     | European VAT number                                                                                     |
-    | Switzerland          | `ch_vat`     | Switzerland VAT number                                                                                  |
+    | Spain                | `es_cif`     | Spanish NIF Number (previously Spanish CIF Number)                                                      |
+    | Spain                | `eu_vat`     | European VAT Number                                                                                     |
+    | Sweden               | `eu_vat`     | European VAT Number                                                                                     |
+    | Switzerland          | `ch_vat`     | Switzerland VAT Number                                                                                  |
     | Taiwan               | `tw_vat`     | Taiwanese VAT                                                                                           |
     | Thailand             | `th_vat`     | Thai VAT                                                                                                |
     | Turkey               | `tr_tin`     | Turkish Tax Identification Number                                                                       |
     | Ukraine              | `ua_vat`     | Ukrainian VAT                                                                                           |
     | United Arab Emirates | `ae_trn`     | United Arab Emirates TRN                                                                                |
-    | United Kingdom       | `eu_vat`     | Northern Ireland VAT number                                                                             |
-    | United Kingdom       | `gb_vat`     | United Kingdom VAT number                                                                               |
+    | United Kingdom       | `eu_vat`     | Northern Ireland VAT Number                                                                             |
+    | United Kingdom       | `gb_vat`     | United Kingdom VAT Number                                                                               |
     | United States        | `us_ein`     | United States EIN                                                                                       |
+    | Uruguay              | `uy_ruc`     | Uruguayan RUC Number                                                                                    |
+    | Venezuela            | `ve_rif`     | Venezuelan RIF Number                                                                                   |
+    | Vietnam              | `vn_tin`     | Vietnamese Tax ID Number                                                                                |
     """
 
     discount: Optional[Discount] = None
 
     discounts: List[Discount]
 
     due_date: datetime
```

### Comparing `orb_billing-1.48.0/src/orb/types/invoice_line_item_create_params.py` & `orb_billing-1.49.0/src/orb/types/invoice_line_item_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/invoice_line_item_create_response.py` & `orb_billing-1.49.0/src/orb/types/invoice_line_item_create_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/invoice_list_params.py` & `orb_billing-1.49.0/src/orb/types/invoice_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/invoice_mark_paid_params.py` & `orb_billing-1.49.0/src/orb/types/invoice_mark_paid_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/item.py` & `orb_billing-1.49.0/src/orb/types/item.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/metric_create_params.py` & `orb_billing-1.49.0/src/orb/types/metric_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/metric_create_response.py` & `orb_billing-1.49.0/src/orb/types/metric_create_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/metric_fetch_response.py` & `orb_billing-1.49.0/src/orb/types/metric_fetch_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/metric_list_params.py` & `orb_billing-1.49.0/src/orb/types/metric_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/metric_list_response.py` & `orb_billing-1.49.0/src/orb/types/metric_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/plan.py` & `orb_billing-1.49.0/src/orb/types/plan.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/plan_create_params.py` & `orb_billing-1.49.0/src/orb/types/plan_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/plan_list_params.py` & `orb_billing-1.49.0/src/orb/types/plan_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/plan_update_params.py` & `orb_billing-1.49.0/src/orb/types/plan_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/price.py` & `orb_billing-1.49.0/src/orb/types/price.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/price_create_params.py` & `orb_billing-1.49.0/src/orb/types/price_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/price_evaluate_params.py` & `orb_billing-1.49.0/src/orb/types/price_evaluate_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/subscription.py` & `orb_billing-1.49.0/src/orb/types/subscription.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/subscription_cancel_params.py` & `orb_billing-1.49.0/src/orb/types/subscription_cancel_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/subscription_create_params.py` & `orb_billing-1.49.0/src/orb/types/subscription_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/subscription_fetch_costs_params.py` & `orb_billing-1.49.0/src/orb/types/subscription_fetch_costs_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/subscription_fetch_costs_response.py` & `orb_billing-1.49.0/src/orb/types/subscription_fetch_costs_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/subscription_fetch_schedule_params.py` & `orb_billing-1.49.0/src/orb/types/subscription_fetch_schedule_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/subscription_fetch_schedule_response.py` & `orb_billing-1.49.0/src/orb/types/subscription_fetch_schedule_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/subscription_fetch_usage_params.py` & `orb_billing-1.49.0/src/orb/types/subscription_fetch_usage_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/subscription_list_params.py` & `orb_billing-1.49.0/src/orb/types/subscription_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/subscription_price_intervals_params.py` & `orb_billing-1.49.0/src/orb/types/subscription_price_intervals_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/subscription_schedule_plan_change_params.py` & `orb_billing-1.49.0/src/orb/types/subscription_schedule_plan_change_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/subscription_trigger_phase_params.py` & `orb_billing-1.49.0/src/orb/types/subscription_trigger_phase_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/subscription_update_fixed_fee_quantity_params.py` & `orb_billing-1.49.0/src/orb/types/subscription_update_fixed_fee_quantity_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/subscription_update_params.py` & `orb_billing-1.49.0/src/orb/types/subscription_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/subscription_usage.py` & `orb_billing-1.49.0/src/orb/types/subscription_usage.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/beta/price_evaluate_params.py` & `orb_billing-1.49.0/src/orb/types/beta/price_evaluate_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/coupons/subscription_list_params.py` & `orb_billing-1.49.0/src/orb/types/coupons/subscription_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/__init__.py` & `orb_billing-1.49.0/src/orb/types/customers/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/balance_transaction_create_response.py` & `orb_billing-1.49.0/src/orb/types/customers/balance_transaction_create_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/balance_transaction_list_params.py` & `orb_billing-1.49.0/src/orb/types/customers/balance_transaction_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/balance_transaction_list_response.py` & `orb_billing-1.49.0/src/orb/types/customers/balance_transaction_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/cost_list_by_external_id_params.py` & `orb_billing-1.49.0/src/orb/types/customers/cost_list_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/cost_list_by_external_id_response.py` & `orb_billing-1.49.0/src/orb/types/customers/cost_list_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/cost_list_params.py` & `orb_billing-1.49.0/src/orb/types/customers/cost_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/cost_list_response.py` & `orb_billing-1.49.0/src/orb/types/customers/cost_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/credit_list_by_external_id_params.py` & `orb_billing-1.49.0/src/orb/types/customers/credit_list_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/credit_list_by_external_id_response.py` & `orb_billing-1.49.0/src/orb/types/customers/credit_list_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/credit_list_params.py` & `orb_billing-1.49.0/src/orb/types/customers/credit_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/usage_update_by_external_id_params.py` & `orb_billing-1.49.0/src/orb/types/customers/usage_update_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/usage_update_by_external_id_response.py` & `orb_billing-1.49.0/src/orb/types/customers/usage_update_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/usage_update_params.py` & `orb_billing-1.49.0/src/orb/types/customers/usage_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/credits/__init__.py` & `orb_billing-1.49.0/src/orb/types/customers/credits/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_params.py` & `orb_billing-1.49.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_response.py` & `orb_billing-1.49.0/src/orb/types/customers/credits/ledger_create_entry_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/credits/ledger_create_entry_params.py` & `orb_billing-1.49.0/src/orb/types/customers/credits/ledger_create_entry_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/credits/ledger_create_entry_response.py` & `orb_billing-1.49.0/src/orb/types/customers/credits/ledger_create_entry_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/credits/ledger_list_by_external_id_params.py` & `orb_billing-1.49.0/src/orb/types/customers/credits/ledger_list_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/credits/ledger_list_by_external_id_response.py` & `orb_billing-1.49.0/src/orb/types/customers/credits/ledger_list_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/credits/ledger_list_params.py` & `orb_billing-1.49.0/src/orb/types/customers/credits/ledger_list_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/credits/ledger_list_response.py` & `orb_billing-1.49.0/src/orb/types/customers/credits/ledger_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/credits/top_up_create_by_external_id_params.py` & `orb_billing-1.49.0/src/orb/types/customers/credits/top_up_create_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/credits/top_up_create_by_external_id_response.py` & `orb_billing-1.49.0/src/orb/types/customers/credits/top_up_create_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/credits/top_up_create_params.py` & `orb_billing-1.49.0/src/orb/types/customers/credits/top_up_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/credits/top_up_create_response.py` & `orb_billing-1.49.0/src/orb/types/customers/credits/top_up_create_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/credits/top_up_list_by_external_id_params.py` & `orb_billing-1.49.0/src/orb/types/customers/credits/top_up_list_by_external_id_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/credits/top_up_list_by_external_id_response.py` & `orb_billing-1.49.0/src/orb/types/customers/credits/top_up_list_by_external_id_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/customers/credits/top_up_list_response.py` & `orb_billing-1.49.0/src/orb/types/customers/credits/top_up_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/events/__init__.py` & `orb_billing-1.49.0/src/orb/types/events/__init__.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/events/backfill_close_response.py` & `orb_billing-1.49.0/src/orb/types/events/backfill_close_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/events/backfill_create_params.py` & `orb_billing-1.49.0/src/orb/types/events/backfill_create_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/events/backfill_create_response.py` & `orb_billing-1.49.0/src/orb/types/events/backfill_create_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/events/backfill_fetch_response.py` & `orb_billing-1.49.0/src/orb/types/events/backfill_fetch_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/events/backfill_list_response.py` & `orb_billing-1.49.0/src/orb/types/events/backfill_list_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/events/backfill_revert_response.py` & `orb_billing-1.49.0/src/orb/types/events/backfill_revert_response.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/plans/external_plan_id_update_params.py` & `orb_billing-1.49.0/src/orb/types/plans/external_plan_id_update_params.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/src/orb/types/shared/discount.py` & `orb_billing-1.49.0/src/orb/types/shared/discount.py`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/LICENSE` & `orb_billing-1.49.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orb_billing-1.48.0/pyproject.toml` & `orb_billing-1.49.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "orb-billing"
-version = "1.48.0"
+version = "1.49.0"
 description = "The official Python library for the orb API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Orb", email = "team@withorb.com" },
 ]
 dependencies = [
```

### Comparing `orb_billing-1.48.0/PKG-INFO` & `orb_billing-1.49.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: orb-billing
-Version: 1.48.0
+Version: 1.49.0
 Summary: The official Python library for the orb API
 Project-URL: Homepage, https://github.com/orbcorp/orb-python
 Project-URL: Repository, https://github.com/orbcorp/orb-python
 Author-email: Orb <team@withorb.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
```

