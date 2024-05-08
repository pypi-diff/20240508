# Comparing `tmp/talklib-1.2.1.tar.gz` & `tmp/talklib-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talklib-1.2.1.tar", last modified: Thu Apr 18 19:27:28 2024, max compression
+gzip compressed data, was "talklib-1.2.2.tar", last modified: Wed May  8 18:50:31 2024, max compression
```

## Comparing `talklib-1.2.1.tar` & `talklib-1.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:27:28.707447 talklib-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-18 19:27:22.000000 talklib-1.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-04-18 19:27:28.707447 talklib-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11593 2024-04-18 19:27:22.000000 talklib-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-18 19:27:22.000000 talklib-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-18 19:27:22.000000 talklib-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:27:28.707447 talklib-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:27:28.703447 talklib-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:27:28.707447 talklib-1.2.1/src/talklib/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-18 19:27:22.000000 talklib-1.2.1/src/talklib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-18 19:27:22.000000 talklib-1.2.1/src/talklib/ev.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-18 19:27:22.000000 talklib-1.2.1/src/talklib/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-18 19:27:22.000000 talklib-1.2.1/src/talklib/notify.py
--rw-r--r--   0 runner    (1001) docker     (127)    21338 2024-04-18 19:27:22.000000 talklib-1.2.1/src/talklib/show.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-18 19:27:22.000000 talklib-1.2.1/src/talklib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:27:28.707447 talklib-1.2.1/src/talklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-04-18 19:27:28.000000 talklib-1.2.1/src/talklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-18 19:27:28.000000 talklib-1.2.1/src/talklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:27:28.000000 talklib-1.2.1/src/talklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-18 19:27:28.000000 talklib-1.2.1/src/talklib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 19:27:28.000000 talklib-1.2.1/src/talklib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:50:31.885595 talklib-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-08 18:50:26.000000 talklib-1.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-05-08 18:50:31.885595 talklib-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11593 2024-05-08 18:50:26.000000 talklib-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-08 18:50:26.000000 talklib-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-08 18:50:26.000000 talklib-1.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:50:31.885595 talklib-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:50:31.881595 talklib-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:50:31.885595 talklib-1.2.2/src/talklib/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-08 18:50:26.000000 talklib-1.2.2/src/talklib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-08 18:50:26.000000 talklib-1.2.2/src/talklib/ev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-08 18:50:26.000000 talklib-1.2.2/src/talklib/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-08 18:50:26.000000 talklib-1.2.2/src/talklib/notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22297 2024-05-08 18:50:26.000000 talklib-1.2.2/src/talklib/show.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-08 18:50:26.000000 talklib-1.2.2/src/talklib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:50:31.885595 talklib-1.2.2/src/talklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-05-08 18:50:31.000000 talklib-1.2.2/src/talklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-08 18:50:31.000000 talklib-1.2.2/src/talklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:50:31.000000 talklib-1.2.2/src/talklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-08 18:50:31.000000 talklib-1.2.2/src/talklib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 18:50:31.000000 talklib-1.2.2/src/talklib.egg-info/top_level.txt
```

### Comparing `talklib-1.2.1/LICENSE.txt` & `talklib-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `talklib-1.2.1/PKG-INFO` & `talklib-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talklib
-Version: 1.2.1
+Version: 1.2.2
 Summary: A package to automate processing of shows/segments airing on the TL
 Author-email: Ben Weddle <ben.weddle@gmail.com>
 Maintainer-email: Ben Weddle <ben.weddle@gmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `talklib-1.2.1/README.md` & `talklib-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `talklib-1.2.1/pyproject.toml` & `talklib-1.2.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "talklib"
-version = "1.2.1"
+version = "1.2.2"
 description = "A package to automate processing of shows/segments airing on the TL"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 authors = [{name = "Ben Weddle", email = "ben.weddle@gmail.com"}]
 maintainers = [{name = "Ben Weddle", email = "ben.weddle@gmail.com"}]
 requires-python = ">=3.10"
 dynamic = ["dependencies"]
```

### Comparing `talklib-1.2.1/requirements.txt` & `talklib-1.2.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `talklib-1.2.1/src/talklib/ev.py` & `talklib-1.2.2/src/talklib/ev.py`

 * *Files identical despite different names*

### Comparing `talklib-1.2.1/src/talklib/ffmpeg.py` & `talklib-1.2.2/src/talklib/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `talklib-1.2.1/src/talklib/notify.py` & `talklib-1.2.2/src/talklib/notify.py`

 * *Files identical despite different names*

### Comparing `talklib-1.2.1/src/talklib/show.py` & `talklib-1.2.2/src/talklib/show.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import time
 import xml.etree.ElementTree as ET
 
 import requests
 
 from talklib.ev import EV
 from talklib.notify import Notify
-from talklib.utils import get_timestamp, clear_screen, print_to_screen_and_wait, today_is_weekday
+from talklib.utils import get_timestamp, clear_screen, raise_exception_and_wait, today_is_weekday
 from talklib.ffmpeg import FFMPEG
 
 
 class TLShow():
     '''TODO write something here'''
     def __init__(self):
 
@@ -207,15 +207,15 @@
                 success = True
             else:
                 toSend = (f"There was a problem with {self.show}.\n\n\
 It looks like the file either wasn't converted or didn't transfer correctly. \
 Please check manually!\n\n\
 {get_timestamp()}")
                 self.__send_notifications(message=toSend, subject='Error')
-                print_to_screen_and_wait(message=toSend)
+                raise_exception_and_wait(message=toSend)
                 break
         if success:
             self.__countdown()
 
     def __check_length(self, fileToCheck):
         '''
         Check length of converted file with ffprobe. if too long or short, send notification.
@@ -335,49 +335,63 @@
         we are checking whether an attribute is either type str or bool, depending on what is passed in.
         
         'attrib_return' is solely for printing the message back out to the screen/log,
         it is not needed for the actual type check.
         (I can't figure out how else to get the name of the attribute)
         '''
         if  type(attrib_to_check) != type_to_check:
-            raise Exception (f"Sorry, '{attrib_return}' attribute must be type: {type_to_check}, but you used {type(attrib_to_check)}.")
+            message = f"Sorry, '{attrib_return}' attribute must be type: {type_to_check}, but you used {type(attrib_to_check)}."
+            self.__send_notifications(message=message, subject="Error")
+            raise_exception_and_wait(message=message)
 
     def __check_int_and_float_type(self, attrib_to_check, attrib_return: str):
         '''
         Attributes passed here can be either int or float.
         '''
         if not (type(attrib_to_check) == int or type(attrib_to_check) == float):
-            raise Exception (f'Sorry, the {attrib_return} attribute must be a valid number (without quotes).')
+            message = f'Sorry, the {attrib_return} attribute must be a valid number (without quotes).'
+            self.__send_notifications(message=message, subject="Error")
+            raise_exception_and_wait(message=message)
 
     def __check_attributes_are_valid(self):
         '''
         Run some checks on the attributes the user has set. I.E. the required
         attributes have been set, they are the right type, etc.
         '''
         self.__prep_syslog(message='checking user defined attributes')
 
         if not self.show:
-            raise Exception ('Sorry, you need to specify a name for the show.')
+            message = 'Sorry, you need to specify a name for the show.'
+            self.__send_notifications(message=message, subject="Error")
+            raise_exception_and_wait(message=message)
         else:
             self.__check_str_and_bool_type(attrib_to_check=self.show, type_to_check=str, attrib_return='show')
 
         if not self.show_filename:
-            raise Exception ('Sorry, you need to specify a filename for the show.')
+            message = 'Sorry, you need to specify a filename for the show.'
+            self.__send_notifications(message=message, subject="Error")
+            raise_exception_and_wait(message=message)
         else:
             self.__check_str_and_bool_type(attrib_to_check=self.show_filename, type_to_check=str, attrib_return='show_filename')
 
         if not self.url:
             if not self.is_local:
-                raise Exception('Sorry, you need to specify either a URL or a local file')
+                message = 'Sorry, you need to specify either a URL or a local file'
+                self.__send_notifications(message=message, subject="Error")
+                raise_exception_and_wait('Sorry, you need to specify either a URL or a local file')
 
         if self.url and self.is_local:
-            raise Exception ('Sorry, you cannot specify both a URL and a local audio file. You must choose only one.')
+            message = 'Sorry, you cannot specify both a URL and a local audio file. You must choose only one.'
+            self.__send_notifications(message=message, subject="Error")
+            raise_exception_and_wait(message=message)
         
         if self.url and self.local_file:
-            raise Exception ('Sorry, you cannot specify both a URL and a local audio file. You must choose only one.')
+            message = 'Sorry, you cannot specify both a URL and a local audio file. You must choose only one.'
+            self.__send_notifications(message=message, subject="Error")
+            raise_exception_and_wait(message=message)
 
         if self.url:
             self.__check_str_and_bool_type(attrib_to_check=self.url, type_to_check=str, attrib_return='url')
         
         if self.is_local:
             self.__check_str_and_bool_type(attrib_to_check=self.is_local, type_to_check=bool, attrib_return='is_local')
 
@@ -429,15 +443,17 @@
             self.__run_URL_RSS()
 
         elif self.is_local:
             self.__prep_syslog(message='local show detected')
             self.__run_local()
                    
         else:
-            raise Exception ('Sorry, something bad happened')
+            message = "Sorry, something bad happened..."
+            self.__send_notifications(message=message, subject="Error")
+            raise_exception_and_wait(message=message)
 
     def __run_URL_permalink(self):
         # if url is declared, it's either an RSS or permalink show
         if self.url and self.is_permalink:
             self.__remove_yesterday_files()
             downloaded_file = self.__download_file()
             if self.check_downloaded_file(fileToCheck=downloaded_file, how_many_attempts=0):
@@ -460,16 +476,15 @@
         else:
             toSend = (
 f"There was a problem with {self.show}.\n\n\
 It looks like today's file hasn't yet been posted. Please check and download manually! Yesterday's file will remain.\n\n\
 {get_timestamp()}"
                 )
             self.__send_notifications(message=toSend, subject='Error')
-            print_to_screen_and_wait(message=toSend)
-            raise Exception
+            raise_exception_and_wait(message=toSend)
     
     def __run_local(self):
         if self.local_file:
             if self.check_downloaded_file(fileToCheck=self.local_file, how_many_attempts=0):
                 output_file = self.__convert(input=self.local_file)
             self.__check_length(fileToCheck=output_file)
             self.__remove(fileToDelete=self.local_file)
@@ -478,9 +493,8 @@
         else:
             to_send = (
 f"There was a problem with {self.show}.\n\n\
 It looks like the source file doesn't exist. Please check manually! Yesterday's file will remain.\n\n\
 {get_timestamp()}"
                 )
             self.__send_notifications(message=to_send, subject='Error')
-            print_to_screen_and_wait(message=to_send)
-            raise FileNotFoundError
+            raise_exception_and_wait(message=to_send, error=FileNotFoundError)
```

### Comparing `talklib-1.2.1/src/talklib/utils.py` & `talklib-1.2.2/src/talklib/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 def clear_screen() -> None:
     '''clears the terminal'''
     if os.name == 'nt':
         os.system('cls')
     else:
         os.system('clear')
 
-def print_to_screen_and_wait(message: str) -> None:
+def raise_exception_and_wait(message: str, error = Exception) -> None:
     '''clear terminal and print message to screen.'''
     clear_screen()
     print(f'{message}\n')  # get user's attention!
     input('(press enter to close this window)') # force user to acknowledge by closing window
+    raise error (message)
 
 def today_is_weekday() -> bool:
     '''crude mechanism for determining if today is a weekday.'''
     today = datetime.now().strftime('%a')
     weekend = ['Sat', 'Sun']
     if today not in weekend:
         return True
```

### Comparing `talklib-1.2.1/src/talklib.egg-info/PKG-INFO` & `talklib-1.2.2/src/talklib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talklib
-Version: 1.2.1
+Version: 1.2.2
 Summary: A package to automate processing of shows/segments airing on the TL
 Author-email: Ben Weddle <ben.weddle@gmail.com>
 Maintainer-email: Ben Weddle <ben.weddle@gmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `talklib-1.2.1/src/talklib.egg-info/requires.txt` & `talklib-1.2.2/src/talklib.egg-info/requires.txt`

 * *Files identical despite different names*

