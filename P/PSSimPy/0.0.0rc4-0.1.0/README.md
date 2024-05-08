# Comparing `tmp/PSSimPy-0.0.0rc4.tar.gz` & `tmp/PSSimPy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PSSimPy-0.0.0rc4.tar", last modified: Thu Mar 21 12:07:53 2024, max compression
+gzip compressed data, was "PSSimPy-0.1.0.tar", last modified: Wed May  8 12:21:54 2024, max compression
```

## Comparing `PSSimPy-0.0.0rc4.tar` & `PSSimPy-0.1.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:07:53.611608 PSSimPy-0.0.0rc4/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-21 12:07:53.611608 PSSimPy-0.0.0rc4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:07:53.607608 PSSimPy-0.0.0rc4/PSSimPy/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/account.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/bank.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:07:53.607608 PSSimPy-0.0.0rc4/PSSimPy/constraint_handler/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/constraint_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/constraint_handler/abstract_constraint_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/constraint_handler/max_size_constraint_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/constraint_handler/min_balance_constraint_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/constraint_handler/pass_through_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:07:53.607608 PSSimPy-0.0.0rc4/PSSimPy/credit_facilities/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/credit_facilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/credit_facilities/abstract_credit_facility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/credit_facilities/simple_collateralized.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/credit_facilities/simple_priced.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:07:53.607608 PSSimPy-0.0.0rc4/PSSimPy/queues/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/queues/abstract_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/queues/direct_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/queues/fifo_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/queues/priority_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:07:53.611608 PSSimPy-0.0.0rc4/PSSimPy/simulator/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17375 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/simulator/abm_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/simulator/basic_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:07:53.611608 PSSimPy-0.0.0rc4/PSSimPy/transaction_fee/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/transaction_fee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/transaction_fee/abstract_transaction_fee.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/transaction_fee/fixed_transaction_fee.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:07:53.611608 PSSimPy-0.0.0rc4/PSSimPy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/utils/account_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/utils/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/PSSimPy/utils/transaction_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:07:53.607608 PSSimPy-0.0.0rc4/PSSimPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-21 12:07:52.000000 PSSimPy-0.0.0rc4/PSSimPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-03-21 12:07:53.000000 PSSimPy-0.0.0rc4/PSSimPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 12:07:52.000000 PSSimPy-0.0.0rc4/PSSimPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-21 12:07:52.000000 PSSimPy-0.0.0rc4/PSSimPy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-21 12:07:52.000000 PSSimPy-0.0.0rc4/PSSimPy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 12:07:53.611608 PSSimPy-0.0.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-21 12:07:24.000000 PSSimPy-0.0.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:21:54.920112 PSSimPy-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22651 2024-05-08 12:21:54.920112 PSSimPy-0.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:21:54.916112 PSSimPy-0.1.0/PSSimPy/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/bank.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:21:54.916112 PSSimPy-0.1.0/PSSimPy/constraint_handler/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/constraint_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/constraint_handler/abstract_constraint_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/constraint_handler/max_size_constraint_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/constraint_handler/min_balance_constraint_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/constraint_handler/pass_through_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:21:54.916112 PSSimPy-0.1.0/PSSimPy/credit_facilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/credit_facilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/credit_facilities/abstract_credit_facility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/credit_facilities/simple_collateralized.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/credit_facilities/simple_priced.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:21:54.916112 PSSimPy-0.1.0/PSSimPy/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/queues/abstract_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/queues/direct_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/queues/fifo_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/queues/priority_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:21:54.920112 PSSimPy-0.1.0/PSSimPy/simulator/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17450 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/simulator/abm_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10557 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/simulator/basic_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:21:54.920112 PSSimPy-0.1.0/PSSimPy/transaction_fee/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/transaction_fee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/transaction_fee/abstract_transaction_fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/transaction_fee/fixed_transaction_fee.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:21:54.920112 PSSimPy-0.1.0/PSSimPy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/utils/account_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/utils/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/PSSimPy/utils/transaction_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:21:54.916112 PSSimPy-0.1.0/PSSimPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22651 2024-05-08 12:21:54.000000 PSSimPy-0.1.0/PSSimPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-08 12:21:54.000000 PSSimPy-0.1.0/PSSimPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:21:54.000000 PSSimPy-0.1.0/PSSimPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-08 12:21:54.000000 PSSimPy-0.1.0/PSSimPy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 12:21:54.000000 PSSimPy-0.1.0/PSSimPy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20628 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 12:21:54.920112 PSSimPy-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-08 12:21:39.000000 PSSimPy-0.1.0/setup.py
```

### Comparing `PSSimPy-0.0.0rc4/LICENSE` & `PSSimPy-0.1.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 Kenneth See
+Copyright (c) 2024 Kenneth See Dehui
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `PSSimPy-0.0.0rc4/PSSimPy/account.py` & `PSSimPy-0.1.0/PSSimPy/account.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,10 +8,10 @@
         self.txn_in = set()
         self.txn_out = set()
 
         # Use the kwargs to store additional user-defined attributes
         for key, value in kwargs.items():
             setattr(self, key, value)
 
-    def transfer_to(self, receipient: 'Account', amount: float) -> None:
+    def transfer_to(self, recipient: 'Account', amount: float) -> None:
         self.balance -= amount
-        receipient.balance += amount
+        recipient.balance += amount
```

### Comparing `PSSimPy-0.0.0rc4/PSSimPy/bank.py` & `PSSimPy-0.1.0/PSSimPy/bank.py`

 * *Files identical despite different names*

### Comparing `PSSimPy-0.0.0rc4/PSSimPy/constraint_handler/abstract_constraint_handler.py` & `PSSimPy-0.1.0/PSSimPy/constraint_handler/abstract_constraint_handler.py`

 * *Files identical despite different names*

### Comparing `PSSimPy-0.0.0rc4/PSSimPy/constraint_handler/max_size_constraint_handler.py` & `PSSimPy-0.1.0/PSSimPy/constraint_handler/max_size_constraint_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,22 +14,22 @@
         kwargs = (transaction.kwargs if hasattr(transaction, 'kwargs') else {})
 
         # Check if transaction size exceeds max size
         if transaction.amount > self.max_txn_size:
             # Split the transaction
             txn1 = Transaction(
                 sender_account=transaction.sender_account,
-                receipient_account=transaction.receipient_account,
+                recipient_account=transaction.recipient_account,
                 amount=self.max_txn_size,
                 priority=transaction.priority,
                 **kwargs
             )
             txn2 = Transaction(
                 sender_account=transaction.sender_account,
-                receipient_account=transaction.receipient_account,
+                recipient_account=transaction.recipient_account,
                 amount=transaction.amount - self.max_txn_size,
                 priority=transaction.priority,
                 **kwargs
             )
 
             # Update original transaction to update status
             transaction.update_transaction_status('Modified')
```

### Comparing `PSSimPy-0.0.0rc4/PSSimPy/constraint_handler/min_balance_constraint_handler.py` & `PSSimPy-0.1.0/PSSimPy/constraint_handler/min_balance_constraint_handler.py`

 * *Files identical despite different names*

### Comparing `PSSimPy-0.0.0rc4/PSSimPy/credit_facilities/abstract_credit_facility.py` & `PSSimPy-0.1.0/PSSimPy/credit_facilities/abstract_credit_facility.py`

 * *Files identical despite different names*

### Comparing `PSSimPy-0.0.0rc4/PSSimPy/credit_facilities/simple_collateralized.py` & `PSSimPy-0.1.0/PSSimPy/credit_facilities/simple_collateralized.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,17 +13,9 @@
     def lend_credit(self, account: Account, amount: float) -> float:
         if amount > account.posted_collateral: return
         self.used_credit[account.id].append(amount)
         account.balance += amount
         account.posted_collateral -= amount
     
     def collect_repayment(self, account: Account) -> None:
-        repaid_amount = 0
-        
-        for i, credit_amount in enumerate(self.used_credit[account.id]):
-            if credit_amount <= account.balance:
-                account.balance -= credit_amount
-                repaid_amount += credit_amount
-                self.used_credit[account.id][i] = 0
-        
-        self.used_credit[account.id] = [x for x in self.used_credit[account.id] if x != 0]
-        account.posted_collateral += repaid_amount
+        account.posted_collateral += self.get_total_credit(account)
+        self.used_credit[account.id] = []
```

### Comparing `PSSimPy-0.0.0rc4/PSSimPy/queues/abstract_queue.py` & `PSSimPy-0.1.0/PSSimPy/queues/abstract_queue.py`

 * *Files identical despite different names*

### Comparing `PSSimPy-0.0.0rc4/PSSimPy/queues/fifo_queue.py` & `PSSimPy-0.1.0/PSSimPy/queues/fifo_queue.py`

 * *Files identical despite different names*

### Comparing `PSSimPy-0.0.0rc4/PSSimPy/queues/priority_queue.py` & `PSSimPy-0.1.0/PSSimPy/queues/priority_queue.py`

 * *Files identical despite different names*

### Comparing `PSSimPy-0.0.0rc4/PSSimPy/simulator/abm_sim.py` & `PSSimPy-0.1.0/PSSimPy/simulator/abm_sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,31 +97,32 @@
         self.account_balance_logger = Logger(logger_file_name(name, 'account_balance'), ACCOUNT_BALANCE_HEADER)
         self.credit_facility_logger = Logger(logger_file_name(name, 'credit_facility'), CREDIT_FACILITY_LOGGER_HEADER)
 
     def load_transactions(self, transactions_dict: List[Dict]):
         """Overwrites existing transactions if they already exist"""
         transactions_revised_dict = transactions_dict.copy()
         transactions_revised_dict['sender_account'] = list(map(lambda x: self.accounts[x], transactions_dict['sender_account']))
-        transactions_revised_dict['receipient_account'] = list(map(lambda x: self.accounts[x], transactions_dict['receipient_account']))
+        transactions_revised_dict['recipient_account'] = list(map(lambda x: self.accounts[x], transactions_dict['recipient_account']))
         transactions_list = initialize_classes_from_dict(Transaction, transactions_revised_dict)
         transactions_list_with_time = [(transaction, transaction.day, transaction.time) for transaction in transactions_list]
         self.transactions = set(transactions_list_with_time)
 
     def run(self):
         """Main function that executes the simulation"""
         # repeate simulation for each day
         for i in range(self.num_days):
             self.env = simpy.Environment()
             self.env.process(self._simulate_day(i+1))
             self.env.run(until=minutes_between(self.open_time, self.close_time))
+            self.credit_facility.collect_all_repayment(self.accounts.values())
             # EOD handling - not implemented for now
         # logging
         # Transactions arrival - only if transactions are generated by the simulation
         if self.generate_txns_flag == 1:
-            arrived_transactions_to_log = [(day, time, transaction.sender_account.id, transaction.receipient_account.id, transaction.amount, transaction.priority) 
+            arrived_transactions_to_log = [(day, time, transaction.sender_account.id, transaction.recipient_account.id, transaction.amount, transaction.priority) 
                                            for transaction, day, time in self.transactions]
             self.transaction_arrival_logger.write(arrived_transactions_to_log)
 
     def _simulate_day(self, day: int=1):
         while True:
             current_time_str = add_minutes_to_time(self.open_time, self.env.now)
             period_end_time_str = add_minutes_to_time(current_time_str, self.processing_window - 1)
@@ -211,15 +212,15 @@
     @staticmethod
     def _extract_logging_details(transactions: Set[Transaction], day: int, time: str) -> List[Tuple]:
         return [
             (
                 day,
                 time,
                 transaction.sender_account.id,
-                transaction.receipient_account.id,
+                transaction.recipient_account.id,
                 transaction.amount,
                 'Success' if transaction.status_code == TRANSACTION_STATUS_CODES['Success'] else 'Failed'
             )
             for transaction in transactions
         ]
     
     def _load_initial_data(self, banks_dict: dict, accounts_dict: dict, transactions_dict: dict, strategy_mapping: dict=None):
```

### Comparing `PSSimPy-0.0.0rc4/PSSimPy/simulator/basic_sim.py` & `PSSimPy-0.1.0/PSSimPy/simulator/basic_sim.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,14 @@
         self.num_days = num_days
         self.constraint_handler = constraint_handler
         self.queue = queue
         self.credit_facility = credit_facility
         self.transaction_fee_handler = transaction_fee_handler
         self.transaction_fee_rate = transaction_fee_rate
         self.bank_failure = bank_failure
-        self.outstanding_transactions = set()
         
         # load data
         if isinstance(banks, pd.DataFrame):
             banks = banks.to_dict(orient='list')
         if isinstance(accounts, pd.DataFrame):
             accounts = accounts.to_dict(orient='list')
         if isinstance(transactions, pd.DataFrame):
@@ -83,36 +82,36 @@
         accounts_revised_dict['owner'] = list(map(lambda x: self.banks[x], accounts_dict['owner']))
         account_list = initialize_classes_from_dict(Account, accounts_revised_dict)
         self.accounts = {account.id: account for account in account_list}
         
         # load transactions
         transactions_revised_dict = transactions_dict.copy()
         transactions_revised_dict['sender_account'] = list(map(lambda x: self.accounts[x], transactions_dict['sender_account']))
-        transactions_revised_dict['receipient_account'] = list(map(lambda x: self.accounts[x], transactions_dict['receipient_account']))
+        transactions_revised_dict['recipient_account'] = list(map(lambda x: self.accounts[x], transactions_dict['recipient_account']))
         transactions_list = initialize_classes_from_dict(Transaction, transactions_revised_dict)
         transactions_list_with_time = [(transaction, transaction.day, transaction.time) for transaction in transactions_list]
         self.transactions = set(transactions_list_with_time)
     
     def _simulate_day(self, day: int = 1):
         while True:
             current_time_str = add_minutes_to_time(self.open_time, self.env.now)
             period_end_time_str = add_minutes_to_time(current_time_str, self.processing_window - 1) 
             self._update_failed_banks(day, current_time_str, period_end_time_str)
             
             # 1. get the transactions pertaining to this time window
             curr_period_transactions = self._gather_transactions_in_window(day, current_time_str, period_end_time_str, self.transactions)
             for account in self.accounts.values():
                 load_account_with_transactions(account, curr_period_transactions)
-            self.outstanding_transactions.update(curr_period_transactions)
+
             # -> remove transactions from failed banks
-            txns_failed_from_bank_failure = {transaction for transaction in self.outstanding_transactions if transaction.involves_failed_bank()}
+            txns_failed_from_bank_failure = {transaction for transaction in curr_period_transactions if transaction.involves_failed_bank()}
             for transaction in txns_failed_from_bank_failure:
                 transaction.status_code = TRANSACTION_STATUS_CODES['Failed']
-            self.outstanding_transactions -= txns_failed_from_bank_failure
             curr_period_transactions -= txns_failed_from_bank_failure
+            
             # 2. obtain necessary intraday credit
             liquidity_requirement = defaultdict(float)
             # -> calculate liquidity requirements for all outstanding transactions
             for txn in curr_period_transactions:
                 liquidity_requirement[txn.sender_account] += txn.amount
             # -> lend required credit                
             for acc, requirement in liquidity_requirement.items():
@@ -165,15 +164,15 @@
         
     @staticmethod
     def _extract_logging_details(transactions: Set[Transaction], day: int, time: str) -> List[Tuple]:
         return [(
             day,
             time,
             transaction.sender_account.id,
-            transaction.receipient_account.id,
+            transaction.recipient_account.id,
             transaction.amount,
             'Success' if transaction.status_code == TRANSACTION_STATUS_CODES['Success'] else 'Failed'
         ) for transaction in transactions]
     
     def _update_failed_banks(self, day, begin_time, end_time):
         if self.bank_failure is not None and day in self.bank_failure:
             failures_to_check = self.bank_failure[day]
```

### Comparing `PSSimPy-0.0.0rc4/PSSimPy/system.py` & `PSSimPy-0.1.0/PSSimPy/system.py`

 * *Files identical despite different names*

### Comparing `PSSimPy-0.0.0rc4/PSSimPy/transaction.py` & `PSSimPy-0.1.0/PSSimPy/transaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     def __new__(cls, *args, **kwargs):
         # Create a new instance
         instance = super().__new__(cls)
         # Add the new instance to the set of instances
         cls._instances.add(instance)
         return instance
 
-    def __init__(self, sender_account: Account, receipient_account: Account, amount: float, priority: int=1, **kwargs):
+    def __init__(self, sender_account: Account, recipient_account: Account, amount: float, priority: int=1, **kwargs):
         self.sender_account = sender_account
-        self.receipient_account = receipient_account
+        self.recipient_account = recipient_account
         self.amount = amount
         self.priority = priority
         self.status_code = TRANSACTION_STATUS_CODES['Open']
         
         # Use the kwargs to store additional user-defined attributes
         for key, value in kwargs.items():
             setattr(self, key, value)
@@ -32,16 +32,16 @@
     def update_transaction_status(self, status: str):
         try:
             self.status_code = TRANSACTION_STATUS_CODES[status]
         except KeyError:
             print(f"Invalid status: '{status}'. Please provide a valid transaction status.")
 
     def involves_failed_bank(self) -> bool:
-        """Checks if either the sender or receipient accounts belongs to a failed bank"""
-        return is_failed_account(self.sender_account) or is_failed_account(self.receipient_account)
+        """Checks if either the sender or recipient accounts belongs to a failed bank"""
+        return is_failed_account(self.sender_account) or is_failed_account(self.recipient_account)
 
     @classmethod
     def get_instances(cls):
         """Provides the set of all created transactions"""
         return cls._instances
 
     @classmethod
```

### Comparing `PSSimPy-0.0.0rc4/PSSimPy/utils/account_utils.py` & `PSSimPy-0.1.0/PSSimPy/utils/account_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 
 def load_account_with_transactions(account: Account, transactions: set):
     txn_in = set()
     txn_out = set()
     for transaction in transactions:
         if transaction.sender_account.id == account.id:
             txn_out.add(transaction)
-        elif transaction.receipient_account.id == account.id:
+        elif transaction.recipient_account.id == account.id:
             txn_in.add(transaction)
     account.txn_in.update(txn_in)
     account.txn_out.update(txn_out)
```

### Comparing `PSSimPy-0.0.0rc4/PSSimPy/utils/constants.py` & `PSSimPy-0.1.0/PSSimPy/utils/constants.py`

 * *Files identical despite different names*

### Comparing `PSSimPy-0.0.0rc4/PSSimPy/utils/data_utils.py` & `PSSimPy-0.1.0/PSSimPy/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `PSSimPy-0.0.0rc4/PSSimPy/utils/logger.py` & `PSSimPy-0.1.0/PSSimPy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `PSSimPy-0.0.0rc4/PSSimPy/utils/time_utils.py` & `PSSimPy-0.1.0/PSSimPy/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `PSSimPy-0.0.0rc4/PSSimPy.egg-info/SOURCES.txt` & `PSSimPy-0.1.0/PSSimPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PSSimPy-0.0.0rc4/setup.py` & `PSSimPy-0.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     requirements = f.read().splitlines()
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='PSSimPy',
-    version='0.0.0rc4',
+    version='0.1.0',
     author='Kenneth See, Hanzholah Shobri',
     author_email='see.k@u.nus.edu, hanzhshobri@gmail.com',
     packages=find_packages(),
     description='A simulator for Large Value Payment Systems',
     long_description=long_description,
     long_description_content_type='text/markdown',  # Specify the content type
     install_requires=requirements,
```

