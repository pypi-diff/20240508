# Comparing `tmp/sparkle_stock-1.0.0-py3-none-any.whl.zip` & `tmp/sparkle_stock-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2363 bytes, number of entries: 7
--rw-r--r--  2.0 unx     2034 b- defN 24-May-08 10:21 sparkle-stock/Stock.py
+Zip file size: 2366 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     2034 b- defN 24-May-08 12:44 sparkle-stock/Stock.py
 -rw-r--r--  2.0 unx       19 b- defN 24-May-08 12:29 sparkle-stock/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-08 12:30 sparkle_stock-1.0.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      301 b- defN 24-May-08 12:30 sparkle_stock-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-08 12:30 sparkle_stock-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 24-May-08 12:30 sparkle_stock-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      575 b- defN 24-May-08 12:30 sparkle_stock-1.0.0.dist-info/RECORD
-7 files, 3041 bytes uncompressed, 1329 bytes compressed:  56.3%
+-rw-r--r--  2.0 unx        0 b- defN 24-May-08 12:44 sparkle_stock-1.0.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      301 b- defN 24-May-08 12:44 sparkle_stock-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-08 12:44 sparkle_stock-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 24-May-08 12:44 sparkle_stock-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      575 b- defN 24-May-08 12:44 sparkle_stock-1.0.1.dist-info/RECORD
+7 files, 3041 bytes uncompressed, 1332 bytes compressed:  56.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: sparkle-stock/Stock.py
 Comment: 
 
 Filename: sparkle-stock/__init__.py
 Comment: 
 
-Filename: sparkle_stock-1.0.0.dist-info/LICENSE.txt
+Filename: sparkle_stock-1.0.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: sparkle_stock-1.0.0.dist-info/METADATA
+Filename: sparkle_stock-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: sparkle_stock-1.0.0.dist-info/WHEEL
+Filename: sparkle_stock-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: sparkle_stock-1.0.0.dist-info/top_level.txt
+Filename: sparkle_stock-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: sparkle_stock-1.0.0.dist-info/RECORD
+Filename: sparkle_stock-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sparkle-stock/Stock.py

```diff
@@ -51,15 +51,15 @@
 
 
     def sell_stock(self, amount:int):
         self.check_login()
 
         selling_status = post(self.address+'/api/sell', json={'id':self.id, 'pw':self.pw, 'amount':str(amount)}).text
         if selling_status == 'true':
-            print("매수에 성공했습니다.")
+            print("매도에 성공했습니다.")
         else:
             raise ConnectionError(selling_status)
 
 
     def check_my_asset(self):
         self.check_login()
```

