# Comparing `tmp/xingu-1.6.9.tar.gz` & `tmp/xingu-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingu-1.6.9.tar", last modified: Wed Jan 31 21:51:04 2024, max compression
+gzip compressed data, was "xingu-1.7.tar", last modified: Wed May  8 21:51:48 2024, max compression
```

## Comparing `xingu-1.6.9.tar` & `xingu-1.7.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-01-31 21:51:04.851259 xingu-1.6.9/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7652 2024-01-03 19:20:34.000000 xingu-1.6.9/LICENSE
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    21763 2024-01-31 21:51:04.851259 xingu-1.6.9/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11571 2024-01-10 19:09:00.000000 xingu-1.6.9/README.md
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1281 2024-01-31 21:50:53.000000 xingu-1.6.9/pyproject.toml
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-01-31 21:51:04.851259 xingu-1.6.9/setup.cfg
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-01-31 21:51:04.847259 xingu-1.6.9/xingu/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      434 2024-01-24 19:13:14.000000 xingu-1.6.9/xingu/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    18877 2024-01-24 19:09:01.000000 xingu-1.6.9/xingu/__main__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    50342 2024-01-15 13:29:17.000000 xingu-1.6.9/xingu/coach.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7378 2024-01-03 19:20:34.000000 xingu-1.6.9/xingu/config_manager.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    22307 2024-01-24 22:47:35.000000 xingu-1.6.9/xingu/dataprovider.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5498 2024-01-03 19:20:34.000000 xingu-1.6.9/xingu/dataproviderfactory.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2506 2024-01-03 19:20:34.000000 xingu-1.6.9/xingu/estimator.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-01-31 21:51:04.851259 xingu-1.6.9/xingu/estimators/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12628 2024-01-03 19:20:34.000000 xingu-1.6.9/xingu/estimators/catboost.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    26251 2024-01-31 20:48:38.000000 xingu-1.6.9/xingu/estimators/xgboost_optuna.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    98710 2024-01-22 18:57:22.000000 xingu-1.6.9/xingu/model.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-01-31 21:51:04.851259 xingu-1.6.9/xingu.egg-info/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    21763 2024-01-31 21:51:04.000000 xingu-1.6.9/xingu.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      432 2024-01-31 21:51:04.000000 xingu-1.6.9/xingu.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-01-31 21:51:04.000000 xingu-1.6.9/xingu.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       46 2024-01-31 21:51:04.000000 xingu-1.6.9/xingu.egg-info/entry_points.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      117 2024-01-31 21:51:04.000000 xingu-1.6.9/xingu.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        6 2024-01-31 21:51:04.000000 xingu-1.6.9/xingu.egg-info/top_level.txt
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-08 21:51:48.616026 xingu-1.7/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7652 2024-01-03 19:20:34.000000 xingu-1.7/LICENSE
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    21759 2024-05-08 21:51:48.616026 xingu-1.7/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11571 2024-01-10 19:09:00.000000 xingu-1.7/README.md
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1275 2024-05-08 21:50:45.000000 xingu-1.7/pyproject.toml
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-05-08 21:51:48.616026 xingu-1.7/setup.cfg
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-08 21:51:48.616026 xingu-1.7/xingu/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      434 2024-01-24 19:13:14.000000 xingu-1.7/xingu/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    18963 2024-02-08 01:10:52.000000 xingu-1.7/xingu/__main__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    50476 2024-05-08 14:27:16.000000 xingu-1.7/xingu/coach.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7378 2024-01-03 19:20:34.000000 xingu-1.7/xingu/config_manager.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    22307 2024-01-24 22:47:35.000000 xingu-1.7/xingu/dataprovider.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5498 2024-01-03 19:20:34.000000 xingu-1.7/xingu/dataproviderfactory.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2506 2024-01-03 19:20:34.000000 xingu-1.7/xingu/estimator.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-08 21:51:48.616026 xingu-1.7/xingu/estimators/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12628 2024-01-03 19:20:34.000000 xingu-1.7/xingu/estimators/catboost.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)   101841 2024-05-08 21:46:31.000000 xingu-1.7/xingu/model.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-08 21:51:48.616026 xingu-1.7/xingu.egg-info/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    21759 2024-05-08 21:51:48.000000 xingu-1.7/xingu.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      397 2024-05-08 21:51:48.000000 xingu-1.7/xingu.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-05-08 21:51:48.000000 xingu-1.7/xingu.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       46 2024-05-08 21:51:48.000000 xingu-1.7/xingu.egg-info/entry_points.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      115 2024-05-08 21:51:48.000000 xingu-1.7/xingu.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        6 2024-05-08 21:51:48.000000 xingu-1.7/xingu.egg-info/top_level.txt
```

### Comparing `xingu-1.6.9/LICENSE` & `xingu-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xingu-1.6.9/PKG-INFO` & `xingu-1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingu
-Version: 1.6.9
+Version: 1.7
 Summary: Automated ML model training and packaging
 Author-email: Avi Alkalay <avi@unix.sh>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -182,15 +182,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: python-decouple
-Requires-Dist: SQLAlchemy<2
+Requires-Dist: SQLAlchemy
 Requires-Dist: tabulate
 Requires-Dist: pygit2
 Requires-Dist: randomname
 Requires-Dist: pyyaml
 Requires-Dist: s3path
 Requires-Dist: smart_open
 Requires-Dist: scikit-learn
```

### Comparing `xingu-1.6.9/README.md` & `xingu-1.7/README.md`

 * *Files identical despite different names*

### Comparing `xingu-1.6.9/pyproject.toml` & `xingu-1.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xingu"
-version = '1.6.9'
+version = '1.7'
 description = "Automated ML model training and packaging"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 authors = [
     { name = "Avi Alkalay", email = "avi@unix.sh" },
 ]
@@ -13,15 +13,15 @@
     "mlengineering",
     "xingu",
 ]
 
 dependencies = [
     "pandas",
     "python-decouple",
-    "SQLAlchemy < 2",
+    "SQLAlchemy",
     "tabulate",
     "pygit2",
     "randomname",
     "pyyaml",
     "s3path",
     "smart_open",
     "scikit-learn",
```

### Comparing `xingu-1.6.9/xingu/__main__.py` & `xingu-1.7/xingu/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -500,20 +500,20 @@
         simpledp = DPSimple(**args)
 
 
     # Gather all DataProviders requested
     if 'DATAPROVIDER_LIST' in args:
         dpf = DataProviderFactory(
             providers_list=[x.strip() for x in args['DATAPROVIDER_LIST'].split(',')],
-            providers_folder=args['DATAPROVIDER_FOLDER'],
+            providers_folder=args['DATAPROVIDER_FOLDER'] if 'DATAPROVIDER_FOLDER' in args else None,
             providers_extra_objects=simpledp,
         )
     else:
         dpf = DataProviderFactory(
-            providers_folder=args['DATAPROVIDER_FOLDER'],
+            providers_folder=args['DATAPROVIDER_FOLDER'] if 'DATAPROVIDER_FOLDER' in args else None,
             providers_extra_objects=simpledp,
         )
 
     # Prepare list of databases to be parsed latter by Coach.get_db_connection()
     if isinstance(args['DATABASES'],list):
         args['DATABASES'] = '|'.join(args['DATABASES'])
```

### Comparing `xingu-1.6.9/xingu/coach.py` & `xingu-1.7/xingu/coach.py`

 * *Files 3% similar despite different names*

```diff
@@ -378,16 +378,14 @@
                 ) as executor:
             tasks=[]
             while True:
                 # Block until a Model object is trained and ready to be used for post processing
                 model=self.post_train_queue.get()
                 self.post_train_queue.task_done()
 
-                self.logger.debug('Post process queue size after queue.get(): ' + str(self.post_train_queue.qsize()))
-
                 if model is None:
                     # A sign that all was done. Exit the endless loop.
                     self.post_processing=False
                     self.logger.info('All post-process tasks done. Shutting down queue.')
                     break
 
                 self.logger.info(f'A fresh Model({model.dp.id}) is ready for post-processing')
@@ -403,15 +401,15 @@
                         **dict(
                             path      = self.get_config(    'TRAINED_MODELS_PATH'),
                             dvc_path  = self.get_config('DVC_TRAINED_MODELS_PATH'),
                         )
                     )
                 )
 
-                if self.get_config('SAVE_SETS'):
+                if self.get_config('SAVE_SETS', 'true', cast=bool):
                     # Save trainsets to DB
                     tasks.append(executor.submit(model.trainsets_save))
 
                 # Predict and compute metrics over train data
                 tasks.append(executor.submit(model.trainsets_predict))
 
                 # Batch predict and metrics computation
@@ -948,27 +946,30 @@
 
             # DB Engine was just created; check if all tables are there
             if databases[i] == 'xingu':
                 self.init_db(self.databases[databases[i]])
 
             self.logger.debug(f"Data source «{databases[i]}» is {current['conn']}. Created with config: {engine_config}.")
 
-        return self.databases[nickname]['conn']
+        if nickname in self.databases.keys():
+            return self.databases[nickname]['conn']
+        else:
+            raise KeyError(f"No database with nickname «{nickname}». Only those ones are known: {list(self.databases.keys())}")
 
 
 
     def init_db(self, con):
         if self.get_config('XINGU_DB_URL'):
             # This is just to raise an exception if not set.
             # Can't do Coach business without a DB.
             pass
 
         import sqlalchemy
 
-        self.xingu_db_metadata = sqlalchemy.MetaData(bind=con['conn'])
+        self.xingu_db_metadata = sqlalchemy.MetaData()
 
         self.xingu_db_table_prefix=self.get_config('XINGU_DB_TABLE_PREFIX','')
 
         table_name='training'
         self.tables[table_name] = sqlalchemy.Table(
             self.xingu_db_table_prefix + table_name,
             self.xingu_db_metadata,
@@ -1073,19 +1074,19 @@
                     self.xingu_db_table_prefix + 'training.train_session_id',
                     self.xingu_db_table_prefix + 'training.train_id',
                 ]
             ),
         )
 
         if 'awsathena' not in con['url']:
-            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_time',             self.tables[table_name].time),
-            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_dataprovider_id',  self.tables[table_name].dataprovider_id),
-            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_train_session_id', self.tables[table_name].train_session_id),
-            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_train_id',         self.tables[table_name].train_id),
-            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_status',           self.tables[table_name].status),
+            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_time',             self.tables[table_name].c.time),
+            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_dataprovider_id',  self.tables[table_name].c.dataprovider_id),
+            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_train_session_id', self.tables[table_name].c.train_session_id),
+            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_train_id',         self.tables[table_name].c.train_id),
+            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_status',           self.tables[table_name].c.status),
 
 
         table_name='sets'
         self.tables[table_name] = sqlalchemy.Table(
             self.xingu_db_table_prefix + table_name,
             self.xingu_db_metadata,
             sqlalchemy.Column(
@@ -1121,17 +1122,17 @@
                     self.xingu_db_table_prefix + 'training.train_session_id',
                     self.xingu_db_table_prefix + 'training.train_id',
                 ]
             ),
         )
 
         if 'awsathena' not in con['url']:
-            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_dataprovider_id',  self.tables[table_name].dataprovider_id),
-            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_train_session_id', self.tables[table_name].train_session_id),
-            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_train_id',         self.tables[table_name].train_id),
+            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_dataprovider_id',  self.tables[table_name].c.dataprovider_id),
+            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_train_session_id', self.tables[table_name].c.train_session_id),
+            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_train_id',         self.tables[table_name].c.train_id),
 
 
         table_name='metrics_model'
         self.tables[table_name] = sqlalchemy.Table(
             self.xingu_db_table_prefix + table_name,
             self.xingu_db_metadata,
             sqlalchemy.Column(
@@ -1178,18 +1179,18 @@
                     self.xingu_db_table_prefix + 'training.train_session_id',
                     self.xingu_db_table_prefix + 'training.train_id',
                 ]
             ),
         )
 
         if 'awsathena' not in con['url']:
-            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_time',             self.tables[table_name].time),
-            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_dataprovider_id',  self.tables[table_name].dataprovider_id),
-            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_train_session_id', self.tables[table_name].train_session_id),
-            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_train_id',         self.tables[table_name].train_id),
+            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_time',             self.tables[table_name].c.time),
+            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_dataprovider_id',  self.tables[table_name].c.dataprovider_id),
+            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_train_session_id', self.tables[table_name].c.train_session_id),
+            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_train_id',         self.tables[table_name].c.train_id),
 
 
         table_name='metrics_estimation'
         self.tables[table_name] = sqlalchemy.Table(
             self.xingu_db_table_prefix + table_name,
             self.xingu_db_metadata,
             sqlalchemy.Column(
@@ -1236,18 +1237,18 @@
                     self.xingu_db_table_prefix + 'training.train_session_id',
                     self.xingu_db_table_prefix + 'training.train_id',
                 ]
             ),
         )
 
         if 'awsathena' not in con['url']:
-            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_time',             self.tables[table_name].time),
-            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_dataprovider_id',  self.tables[table_name].dataprovider_id),
-            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_train_session_id', self.tables[table_name].train_session_id),
-            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_train_id',         self.tables[table_name].train_id),
+            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_time',             self.tables[table_name].c.time),
+            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_dataprovider_id',  self.tables[table_name].c.dataprovider_id),
+            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_train_session_id', self.tables[table_name].c.train_session_id),
+            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_train_id',         self.tables[table_name].c.train_id),
 
 
         table_name='estimations'
         self.tables[table_name] = sqlalchemy.Table(
             self.xingu_db_table_prefix + table_name,
             self.xingu_db_metadata,
             sqlalchemy.Column(
@@ -1288,16 +1289,16 @@
                     self.xingu_db_table_prefix + 'training.train_session_id',
                     self.xingu_db_table_prefix + 'training.train_id',
                 ]
             ),
         )
 
         if 'awsathena' not in con['url']:
-            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_time',             self.tables[table_name].time),
-            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_dataprovider_id',  self.tables[table_name].dataprovider_id),
-            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_train_session_id', self.tables[table_name].train_session_id),
-            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_train_id',         self.tables[table_name].train_id),
+            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_time',             self.tables[table_name].c.time),
+            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_dataprovider_id',  self.tables[table_name].c.dataprovider_id),
+            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_train_session_id', self.tables[table_name].c.train_session_id),
+            sqlalchemy.Index(self.xingu_db_table_prefix + table_name + '_by_train_id',         self.tables[table_name].c.train_id),
 
 
         self.logger.info('Going to create tables on Xingu DB')
 
-        self.xingu_db_metadata.create_all()
+        self.xingu_db_metadata.create_all(bind=con['conn'])
```

### Comparing `xingu-1.6.9/xingu/config_manager.py` & `xingu-1.7/xingu/config_manager.py`

 * *Files identical despite different names*

### Comparing `xingu-1.6.9/xingu/dataprovider.py` & `xingu-1.7/xingu/dataprovider.py`

 * *Files identical despite different names*

### Comparing `xingu-1.6.9/xingu/dataproviderfactory.py` & `xingu-1.7/xingu/dataproviderfactory.py`

 * *Files identical despite different names*

### Comparing `xingu-1.6.9/xingu/estimator.py` & `xingu-1.7/xingu/estimator.py`

 * *Files identical despite different names*

### Comparing `xingu-1.6.9/xingu/estimators/catboost.py` & `xingu-1.7/xingu/estimators/catboost.py`

 * *Files identical despite different names*

### Comparing `xingu-1.6.9/xingu/model.py` & `xingu-1.7/xingu/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,23 +168,14 @@
             self.github_actor      = self.get_config('GITHUB_ACTOR', None)
             self.github_workflow   = self.get_config('GITHUB_WORKFLOW', None)
             self.github_run_id     = self.get_config('GITHUB_RUN_ID', None)
             self.github_run_number = self.get_config('GITHUB_RUN_NUMBER', None)
 
             self.log(message=str(self.dp.get_estimator_class()))
 
-            if self.dp.hollow:
-                self.estimator     = None
-            else:
-                self.estimator     = self.dp.get_estimator_class()(
-                    **self.dp.get_estimator_class_params(),
-                    params      = self.dp.get_estimator_params(),
-                    hyperparams = self.dp.get_estimator_hyperparams(),
-                )
-
         if delayed_prereq_binding is False:
             self.load_pre_req_model()
 
 
 
     ######################################################################################
     ##
@@ -413,23 +404,38 @@
                 )
             report='; '.join(report)
 
             self.log(message=f'Sizes of train sets: {report}',level=logging.DEBUG)
 
         self.log_train_status('train_dataprep_end')
 
-        if not self.dp.hollow:
+        if self.dp.hollow:
+            self.estimator     = None
+        else:
+            self.estimator     = self.dp.get_estimator_class()(
+                **self.dp.get_estimator_class_params(),
+                params      = self.dp.get_estimator_params(),
+                hyperparams = self.dp.get_estimator_hyperparams(),
+            )
+
             self.hyperparam_optimize()
 
             self.dp.post_process_after_hyperparam_optimize(self)
 
-            self.log(
-                message=f"Hyperparameters from {self.algo_params['source_train_id']}:\n" + pandas.Series(self.algo_params['hyperparams']).to_markdown(),
-                level=logging.DEBUG
-            )
+            if self.algo_params['hyperparams']:
+                self.log(
+                    message=f"Hyperparameters from {self.algo_params['source_train_id']}:\n" + pandas.Series(self.algo_params['hyperparams']).to_markdown(),
+                    level=logging.DEBUG
+                )
+            else:
+                # Hyperparameters are empty. Warn user.
+                self.log(
+                    message="Training with no hyperparameters. This is probably undesired behavior.",
+                    level=logging.WARNING
+                )
 
             self.context='train_fit'
             self.log_train_status('train_fit_start')
 
             self.log(message='Training an Estimator')
 
             self.estimator.fit(
@@ -590,56 +596,67 @@
         if self.sets is not None:
             self.context='train_savesets'
             self.log_train_status('train_savesets_start')
 
             with self.coach.get_db_connection('xingu').connect() as db:
                 # Record sets in DB
                 for part in self.sets.keys():
-                    self.log(f'Saving {part} dataset to DB')
+                    self.log(f'Saving «{part}» dataset to DB')
 
                     target=self.dp.get_target()
                     if target in self.sets[part].columns:
-                        (
-                            # Start with just the index and target column
-                            self.sets[part][[target]]
-
-                            # Standardize target column name
-                            .rename(columns={target: 'target'})
-
-                            # Tag table with context
-                            .assign(
-                                set                = part,
-                                dataprovider_id    = self.dp.id,
-                                train_id           = self.train_id,
-                                train_session_id   = self.train_session_id,
-                            )
+                        import sqlalchemy
+                        try:
+                            (
+                                # Start with just the index and target column
+                                self.sets[part][[target]]
+
+                                # Standardize target column name
+                                .rename(columns={target: 'target'})
+
+                                # Tag table with context
+                                .assign(
+                                    set                = part,
+                                    dataprovider_id    = self.dp.id,
+                                    train_id           = self.train_id,
+                                    train_session_id   = self.train_session_id,
+                                )
 
-                            # Standardize index
-                            .reset_index(names='index')
+                                # Standardize index
+                                .reset_index(names='index')
 
-                            # Force data types, some DBs (cough Athena cough) will complain otherwise
-                            .assign(
-                                index=lambda table: table['index'].astype(str),
-                                target=lambda table: table.target.astype(float),
-                            )
+                                # Force data types, some DBs (cough Athena cough) will complain otherwise
+                                .assign(
+                                    index=lambda table: table['index'].astype(str),
+                                    target=lambda table: table.target.astype(float),
+                                )
 
-                            # Write debug message to console
-                            .pipe(lambda table: ddebug(
-                                table,
-                                f'{part}: {table.shape[0]}×{table.shape[1]}'
-                            ))
-
-                            # Commit to DB
-                            .to_sql(
-                                self.coach.tables['sets'].name,
-                                if_exists='append',
-                                index=False,
-                                con=db
+                                # Write debug message to console
+                                .pipe(lambda table: ddebug(
+                                    table,
+                                    f'{part}: {table.shape[0]}×{table.shape[1]}'
+                                ))
+
+                                # Commit to DB
+                                .to_sql(
+                                    self.coach.tables['sets'].name,
+                                    if_exists='append',
+                                    index=False,
+                                    method='multi',
+                                    con=db
+                                )
                             )
-                        )
+                        except sqlalchemy.exc.OperationalError as e:
+                            m=(
+                                "Failed to write sets to DB due to a bug "
+                                "between Pandas and SQLite. Set "
+                                "SAVE_SETS=false to ignore silently."
+                            )
+                            self.log(m,level=logging.WARNING)
+                            raise e
 
             self.log_train_status('train_savesets_end')
 
 
 
     def trainsets_predict(self):
         if not hasattr(self, 'sets'):
@@ -711,14 +728,15 @@
 
                     # Commit to DB
                     .to_sql(
                         con          = db,
                         name         = self.coach.tables['estimations'].name,
                         if_exists    = 'append',
                         index        = False,
+                        method       = 'multi',
                     )
                 )
 
 
 
     ######################################################################################
     ##
@@ -1030,15 +1048,15 @@
         model_signature = matplotlib.offsetbox.AnchoredText(
             prop=dict(size=size),
             frameon=True,
             loc=loc,
             s=template.format(
                 dp=self.dp.id,
                 complete_train_id=self.get_full_train_id(),
-                trained=self.trained.strftime("%Y-%m-%d %H:%M:%S %Z"),
+                trained=self.trained.strftime("%Y-%m-%d %H:%M:%S %Z") if type(self.trained)==datetime.datetime else '(untrained)',
             ),
         )
 
         model_signature.patch.set_alpha(alpha)
         model_signature.patch.set_boxstyle("round,pad=0.,rounding_size=0.2")
 
         ax.add_artist(model_signature)
@@ -1269,14 +1287,15 @@
                     )
 
                     # Save metrics to DB
                     .to_sql(
                         name           = self.coach.tables['metrics_model'].name,
                         if_exists      = 'append',
                         index          = False,
+                        method         = 'multi',
                         con            = db
                     )
                 )
 
         plots = self.render_model_plots(channel)
 
         if plots is not None and len(plots.keys())>0:
@@ -1322,16 +1341,19 @@
             return self.compute_estimation_metrics(self.batch_predict_data,self.batch_predict_estimations)
         else:
             self.log('No data to compute estimations metrics.', level=logging.WARNING)
 
 
 
     def compute_batch_model_metrics_classical(self, XY: pandas.DataFrame, Y_pred: pandas.DataFrame) -> dict:
-        mask = ~XY[self.dp.get_target()].isna()
-        return self.compute_trainsets_model_metrics_classical(XY[mask],Y_pred[mask])
+        if self.dp.get_target() in XY.columns:
+            mask = ~XY[self.dp.get_target()].isna()
+            return self.compute_trainsets_model_metrics_classical(XY[mask],Y_pred[mask])
+        else:
+            return dict()
 
 
 
     def compute_estimation_metrics(self, XY: pandas.DataFrame, Y_pred: pandas.DataFrame) -> pandas.DataFrame:
         """
         Calls all compute_estimation_metrics_{NAME}() from Model and DataProvider.
 
@@ -1410,14 +1432,15 @@
                 self.log(f'Save estimations metrics to DB')
 
                 with self.coach.get_db_connection('xingu').connect() as db:
                     metrics.reset_index(names='index').to_sql(
                         name         = self.coach.tables['metrics_estimation'].name,
                         if_exists    = 'append',
                         index        = False,
+                        method       = 'multi',
                         con          = db
                     )
 
 
 
     def compute_and_save_metrics(self, channel='trainsets'):
         """
@@ -2155,29 +2178,63 @@
         """
         The url parameters points to a local file, http://... or s3://...
         resource.
 
         This method will use pandas.read_csv(), pandas.read_parquet() or
         pandas.read_json() depending on text found in the URL.
 
+        Or, pass format='parquet|json|csv|txt' to the params dict to force a
+        specific format.
+
         The params dict will be passed to the pandas method and might have any
         parameters accepted by these methods.
+
+        Example of `DataProvider.train_dataset_sources` entries that will be
+        processed by this method:
+
+        train_dataset_sources = dict(
+            df1 = dict(
+                url = 's3://bucket/folder1/object',
+                params = dict(format='parquet')
+            ),
+            df2 = dict(
+                url = 'some/local/file.txt',
+                # format is infered from URL. no need to pass it here
+                params = dict(sep='|')
+            ),
+            df3 = dict(
+                url = 's3://bucket/folder1/object2',
+                params = dict(
+                    format='json',
+
+                    # Arguments for pandas.read_json():
+                    orient='records',
+                    convert_axes=True,
+                )
+            ),
+        )
         """
         token_map=dict(
             json     = pandas.read_json,
             parquet  = pandas.read_parquet,
+            csv      = pandas.read_csv,
+            txt      = pandas.read_csv,
         )
 
         # Find correct Pandas method we´ll use.
         # Start with a default to pandas.read_csv()
         pandas_method = pandas.read_csv
-        for token in token_map.keys():
-            if token in url:
-                pandas_method = token_map[token]
-                break
+        if params is not None and 'format' in params:
+            pandas_method = token_map[params['format']]
+            del params['format']
+        else:
+            for token in token_map.keys():
+                if token in url:
+                    pandas_method = token_map[token]
+                    break
 
         self.log(
             level=logging.DEBUG,
             message='Using {method} to retrieve dataset from {url}'.format(
                 url = url,
                 method = pandas_method
             )
@@ -2221,15 +2278,18 @@
                 source='db_nickname' | 'xingu',
                 query="SELECT ..."
             )
 
         OR
 
             dict(
-                url="file:/..." | "http://..." | "s3://..."
+                url="file:/..." | "http://..." | "s3://...",
+                params=dict(
+                    # parameters to pandas.read_{csv|parquet|json}()
+                )
             )
 
         sourceid is the name of this source, as it appears in the DP's dict.
 
         This method is called in parallel by data_sources_to_data().
         """
 
@@ -2345,15 +2405,19 @@
                 df = self.data_source_to_data_from_query(
                     query_text,
                     data_source['source']
                 )
             elif key_type == 'url':
                 df = self.data_source_to_data_from_url(
                     query_text,
-                    params=data_source['params'] if 'params' in data_source else dict()
+                    params=(
+                        data_source['params']
+                        if 'params' in data_source and pandas.notna(data_source['params'])
+                        else dict()
+                    )
                 )
 
             self.log(
                 'Data for «{source}» on {context} has shape {rows}×{cols}.'.format(
                     source      = sourceid,
                     context     = self.context,
                     rows        = df.shape[0],
@@ -2576,15 +2640,25 @@
             )
         )
 
         self.log(
             level=logging.DEBUG,
             message=(
                 "Data extraction plan:\n" + (
-                    data_extraction_plan[['name','source','url']]
+                    data_extraction_plan
+                    .assign(
+                        **{
+                            'query or url': lambda table: (
+                                table.url.combine_first(table['query'])
+                                .replace(r'\n+|\s+',' ',regex=True)
+                                .replace(r'^(.{30}).*(.{15})$', r'\g<1> … \g<2>',regex=True)
+                            )
+                        }
+                    )
+                    [['name','source','query or url']]
                     .reset_index()
                     .to_markdown()
                 )
             )
         )
 
         # Iterate over all data sources groups and fire
```

### Comparing `xingu-1.6.9/xingu.egg-info/PKG-INFO` & `xingu-1.7/xingu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingu
-Version: 1.6.9
+Version: 1.7
 Summary: Automated ML model training and packaging
 Author-email: Avi Alkalay <avi@unix.sh>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -182,15 +182,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: python-decouple
-Requires-Dist: SQLAlchemy<2
+Requires-Dist: SQLAlchemy
 Requires-Dist: tabulate
 Requires-Dist: pygit2
 Requires-Dist: randomname
 Requires-Dist: pyyaml
 Requires-Dist: s3path
 Requires-Dist: smart_open
 Requires-Dist: scikit-learn
```

