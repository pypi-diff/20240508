# Comparing `tmp/python_telegram_broadcast-0.9.3.tar.gz` & `tmp/python_telegram_broadcast-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_telegram_broadcast-0.9.3.tar", last modified: Tue May  7 07:02:19 2024, max compression
+gzip compressed data, was "python_telegram_broadcast-0.9.4.tar", last modified: Tue May  7 09:49:42 2024, max compression
```

## Comparing `python_telegram_broadcast-0.9.3.tar` & `python_telegram_broadcast-0.9.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 07:02:19.528690 python_telegram_broadcast-0.9.3/
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     1067 2024-05-06 01:52:00.000000 python_telegram_broadcast-0.9.3/LICENSE
--rw-r--r--   0 jonah     (1000) jonah     (1000)     3920 2024-05-07 07:02:19.528690 python_telegram_broadcast-0.9.3/PKG-INFO
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     3331 2024-05-07 02:48:22.000000 python_telegram_broadcast-0.9.3/README.md
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 07:02:19.528690 python_telegram_broadcast-0.9.3/python_telegram_broadcast/
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     4268 2024-05-07 07:01:41.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast/__init__.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     4039 2024-05-07 06:58:19.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast/custom_dataclass.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     1616 2024-05-06 08:35:01.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast/custom_exception.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     3338 2024-05-07 06:58:49.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast/custom_util.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     3859 2024-05-07 06:57:58.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast/main.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)    18085 2024-05-07 06:57:43.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast/send_method.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)    17860 2024-05-07 06:57:50.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast/strategy.py
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 07:02:19.528690 python_telegram_broadcast-0.9.3/python_telegram_broadcast.egg-info/
--rw-r--r--   0 jonah     (1000) jonah     (1000)     3920 2024-05-07 07:02:19.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast.egg-info/PKG-INFO
--rw-rw-r--   0 jonah     (1000) jonah     (1000)      554 2024-05-07 07:02:19.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast.egg-info/SOURCES.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)        1 2024-05-07 07:02:19.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast.egg-info/dependency_links.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       33 2024-05-07 07:02:19.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast.egg-info/requires.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       26 2024-05-07 07:02:19.000000 python_telegram_broadcast-0.9.3/python_telegram_broadcast.egg-info/top_level.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       38 2024-05-07 07:02:19.528690 python_telegram_broadcast-0.9.3/setup.cfg
--rw-rw-r--   0 jonah     (1000) jonah     (1000)      952 2024-05-07 07:01:58.000000 python_telegram_broadcast-0.9.3/setup.py
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 09:49:42.882277 python_telegram_broadcast-0.9.4/
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     1067 2024-05-06 01:52:00.000000 python_telegram_broadcast-0.9.4/LICENSE
+-rw-r--r--   0 jonah     (1000) jonah     (1000)     3920 2024-05-07 09:49:42.882277 python_telegram_broadcast-0.9.4/PKG-INFO
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     3331 2024-05-07 02:48:22.000000 python_telegram_broadcast-0.9.4/README.md
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 09:49:42.882277 python_telegram_broadcast-0.9.4/python_telegram_broadcast/
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     4268 2024-05-07 07:01:41.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast/__init__.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     4039 2024-05-07 06:58:19.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast/custom_dataclass.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     1616 2024-05-06 08:35:01.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast/custom_exception.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     3338 2024-05-07 06:58:49.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast/custom_util.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     3859 2024-05-07 06:57:58.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast/main.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)    17721 2024-05-07 09:46:20.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast/send_method.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)    17860 2024-05-07 06:57:50.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast/strategy.py
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-07 09:49:42.882277 python_telegram_broadcast-0.9.4/python_telegram_broadcast.egg-info/
+-rw-r--r--   0 jonah     (1000) jonah     (1000)     3920 2024-05-07 09:49:42.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast.egg-info/PKG-INFO
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)      554 2024-05-07 09:49:42.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)        1 2024-05-07 09:49:42.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)       33 2024-05-07 09:49:42.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast.egg-info/requires.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)       26 2024-05-07 09:49:42.000000 python_telegram_broadcast-0.9.4/python_telegram_broadcast.egg-info/top_level.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)       38 2024-05-07 09:49:42.882277 python_telegram_broadcast-0.9.4/setup.cfg
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)      952 2024-05-07 09:49:29.000000 python_telegram_broadcast-0.9.4/setup.py
```

### Comparing `python_telegram_broadcast-0.9.3/LICENSE` & `python_telegram_broadcast-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.3/PKG-INFO` & `python_telegram_broadcast-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_telegram_broadcast
-Version: 0.9.3
+Version: 0.9.4
 Summary: Package that wraps the python-telegram-bot library to make broadcasting easier.
 Author: jonah_whaler_2348
 Author-email: jk_saga@proton.me
 License: MIT
 Keywords: python,telegram,broadcast,bot
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `python_telegram_broadcast-0.9.3/README.md` & `python_telegram_broadcast-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.3/python_telegram_broadcast/__init__.py` & `python_telegram_broadcast-0.9.4/python_telegram_broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.3/python_telegram_broadcast/custom_dataclass.py` & `python_telegram_broadcast-0.9.4/python_telegram_broadcast/custom_dataclass.py`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.3/python_telegram_broadcast/custom_exception.py` & `python_telegram_broadcast-0.9.4/python_telegram_broadcast/custom_exception.py`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.3/python_telegram_broadcast/custom_util.py` & `python_telegram_broadcast-0.9.4/python_telegram_broadcast/custom_util.py`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.3/python_telegram_broadcast/main.py` & `python_telegram_broadcast-0.9.4/python_telegram_broadcast/main.py`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.3/python_telegram_broadcast/send_method.py` & `python_telegram_broadcast-0.9.4/python_telegram_broadcast/send_method.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,16 +113,16 @@
         t2 = time.time()
         sent_time = t2 - t1
         error_message = (f'telegram_id: "{target_id}", '
                          f'username: "NA", payload: '
                          f'payload: "{message}", '
                          f'elapsed_seconds: "{sent_time}"')
         raise TimedOut("{" + error_message + "}")
-    except BadRequest as bad_request_err:
-        raise TelegramSendError(target_id, "NA", message, str(bad_request_err))
+    except BadRequest:
+        raise
     except Forbidden as _:
         raise Forbidden(str(target_id))
     except TelegramError as tg_err:
         raise TelegramSendError(target_id, "NA", message, str(tg_err))
     except Exception as err:
         raise TelegramSendError(target_id, "NA", message, str(err))
 
@@ -190,16 +190,16 @@
     except TimedOut:
         sent_time = time.time() - t1
         error_message = (f'telegram_id: "{target_id}", '
                          f'username: "NA", payload: '
                          f'payload: "{filename_or_url}", '
                          f'elapsed_seconds: "{sent_time}"')
         raise TimedOut("{" + error_message + "}")
-    except BadRequest as bad_request_err:
-        raise TelegramSendError(target_id, "NA", filename_or_url, str(bad_request_err))
+    except BadRequest:
+        raise
     except Forbidden as _:
         raise Forbidden(str(target_id))
     except TelegramError as tg_err:
         raise TelegramSendError(target_id, "NA", filename_or_url, str(tg_err))
     except Exception as err:
         raise TelegramSendError(target_id, "NA", filename_or_url, str(err))
 
@@ -263,16 +263,16 @@
     except TimedOut:
         sent_time = time.time() - t1
         error_message = (f'telegram_id: "{target_id}", '
                          f'username: "NA", payload: '
                          f'payload: "{filename_or_url}", '
                          f'elapsed_seconds: "{sent_time}"')
         raise TimedOut("{" + error_message + "}")
-    except BadRequest as bad_request_err:
-        raise TelegramSendError(target_id, "NA", filename_or_url, str(bad_request_err))
+    except BadRequest:
+        raise
     except Forbidden as _:
         raise Forbidden(str(target_id))
     except TelegramError as tg_err:
         raise TelegramSendError(target_id, "NA", filename_or_url, str(tg_err))
     except Exception as err:
         raise TelegramSendError(target_id, "NA", filename_or_url, str(err))
 
@@ -341,16 +341,16 @@
     except TimedOut:
         sent_time = time.time() - t1
         error_message = (f'telegram_id: "{target_id}", '
                          f'username: "NA", payload: '
                          f'payload: "{filename_or_url}", '
                          f'elapsed_seconds: "{sent_time}"')
         raise TimedOut("{" + error_message + "}")
-    except BadRequest as bad_request_err:
-        raise TelegramSendError(target_id, "NA", filename_or_url, str(bad_request_err))
+    except BadRequest:
+        raise
     except Forbidden as _:
         raise Forbidden(str(target_id))
     except TelegramError as tg_err:
         raise TelegramSendError(target_id, "NA", filename_or_url, str(tg_err))
     except Exception as err:
         raise TelegramSendError(target_id, "NA", filename_or_url, str(err))
```

### Comparing `python_telegram_broadcast-0.9.3/python_telegram_broadcast/strategy.py` & `python_telegram_broadcast-0.9.4/python_telegram_broadcast/strategy.py`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.3/python_telegram_broadcast.egg-info/PKG-INFO` & `python_telegram_broadcast-0.9.4/python_telegram_broadcast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-telegram-broadcast
-Version: 0.9.3
+Version: 0.9.4
 Summary: Package that wraps the python-telegram-bot library to make broadcasting easier.
 Author: jonah_whaler_2348
 Author-email: jk_saga@proton.me
 License: MIT
 Keywords: python,telegram,broadcast,bot
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `python_telegram_broadcast-0.9.3/python_telegram_broadcast.egg-info/SOURCES.txt` & `python_telegram_broadcast-0.9.4/python_telegram_broadcast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_telegram_broadcast-0.9.3/setup.py` & `python_telegram_broadcast-0.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 DESCRIPTION = 'Package that wraps the python-telegram-bot library to make broadcasting easier.'
 
 # python3 setup.py sdist bdist_wheel
 # twine upload --skip-existing dist/*
 
-VERSION = '0.9.3'
+VERSION = '0.9.4'
 
 setup(
     name='python_telegram_broadcast',
     version=VERSION,
     packages=find_packages(),
     description=DESCRIPTION,
     long_description=open('README.md').read(),
```

