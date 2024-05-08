# Comparing `tmp/omero-dropbox-5.6.dev3.tar.gz` & `tmp/omero-dropbox-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/omero-dropbox-5.6.dev3.tar", last modified: Tue Nov 26 11:56:21 2019, max compression
+gzip compressed data, was "omero-dropbox-5.7.0.tar", last modified: Wed May  8 12:43:55 2024, max compression
```

## Comparing `omero-dropbox-5.6.dev3.tar` & `omero-dropbox-5.7.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-26 11:56:21.000000 omero-dropbox-5.6.dev3/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2463 2019-11-26 11:56:21.000000 omero-dropbox-5.6.dev3/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-26 11:56:21.000000 omero-dropbox-5.6.dev3/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-26 11:56:21.000000 omero-dropbox-5.6.dev3/src/omero_dropbox.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2463 2019-11-26 11:56:21.000000 omero-dropbox-5.6.dev3/src/omero_dropbox.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-26 11:56:21.000000 omero-dropbox-5.6.dev3/src/omero_dropbox.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      226 2019-11-26 11:56:21.000000 omero-dropbox-5.6.dev3/src/omero_dropbox.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      554 2019-11-26 11:56:21.000000 omero-dropbox-5.6.dev3/src/omero_dropbox.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2019-11-26 11:56:21.000000 omero-dropbox-5.6.dev3/src/omero_dropbox.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3998 2019-11-26 11:55:50.000000 omero-dropbox-5.6.dev3/src/fsUtil.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23066 2019-11-26 11:55:50.000000 omero-dropbox-5.6.dev3/src/fsDropBox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19729 2019-11-26 11:55:50.000000 omero-dropbox-5.6.dev3/src/fsFileServer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27275 2019-11-26 11:55:50.000000 omero-dropbox-5.6.dev3/src/fsDropBoxMonitorClient.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3963 2019-11-26 11:55:50.000000 omero-dropbox-5.6.dev3/src/fsLists.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8332 2019-11-26 11:55:50.000000 omero-dropbox-5.6.dev3/src/fsMonitorServer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2620 2019-11-26 11:55:50.000000 omero-dropbox-5.6.dev3/src/fsServerFS.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11654 2019-11-26 11:55:50.000000 omero-dropbox-5.6.dev3/src/fsMac-10-5-Monitor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8277 2019-11-26 11:55:50.000000 omero-dropbox-5.6.dev3/src/fsMonitor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19835 2019-11-26 11:55:50.000000 omero-dropbox-5.6.dev3/src/fsPyinotifyMonitor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23642 2019-11-26 11:55:50.000000 omero-dropbox-5.6.dev3/src/fsDirectory.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1752 2019-11-26 11:55:50.000000 omero-dropbox-5.6.dev3/src/fsNotificationScheduler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9498 2019-11-26 11:55:50.000000 omero-dropbox-5.6.dev3/src/fsWin-XP-Monitor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2795 2019-11-26 11:55:50.000000 omero-dropbox-5.6.dev3/src/fsServerMS.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1879 2019-11-26 11:55:50.000000 omero-dropbox-5.6.dev3/src/fsAbstractPlatformMonitor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-11-26 11:56:21.000000 omero-dropbox-5.6.dev3/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1168 2019-11-26 11:55:50.000000 omero-dropbox-5.6.dev3/README.rst
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1743 2019-11-26 11:55:50.000000 omero-dropbox-5.6.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:43:55.444412 omero-dropbox-5.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    17987 2024-05-08 12:43:49.000000 omero-dropbox-5.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-08 12:43:55.444412 omero-dropbox-5.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-08 12:43:49.000000 omero-dropbox-5.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 12:43:55.448412 omero-dropbox-5.7.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1774 2024-05-08 12:43:49.000000 omero-dropbox-5.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:43:55.444412 omero-dropbox-5.7.0/src/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1850 2024-05-08 12:43:49.000000 omero-dropbox-5.7.0/src/fsAbstractPlatformMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23500 2024-05-08 12:43:49.000000 omero-dropbox-5.7.0/src/fsDirectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22925 2024-05-08 12:43:49.000000 omero-dropbox-5.7.0/src/fsDropBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27249 2024-05-08 12:43:49.000000 omero-dropbox-5.7.0/src/fsDropBoxMonitorClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19574 2024-05-08 12:43:49.000000 omero-dropbox-5.7.0/src/fsFileServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-05-08 12:43:49.000000 omero-dropbox-5.7.0/src/fsLists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11485 2024-05-08 12:43:49.000000 omero-dropbox-5.7.0/src/fsMac-10-5-Monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-05-08 12:43:49.000000 omero-dropbox-5.7.0/src/fsMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-05-08 12:43:49.000000 omero-dropbox-5.7.0/src/fsMonitorServer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1654 2024-05-08 12:43:49.000000 omero-dropbox-5.7.0/src/fsNotificationScheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19621 2024-05-08 12:43:49.000000 omero-dropbox-5.7.0/src/fsPyinotifyMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-08 12:43:49.000000 omero-dropbox-5.7.0/src/fsServerFS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-08 12:43:49.000000 omero-dropbox-5.7.0/src/fsServerMS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-08 12:43:49.000000 omero-dropbox-5.7.0/src/fsUtil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9356 2024-05-08 12:43:49.000000 omero-dropbox-5.7.0/src/fsWin-XP-Monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:43:55.444412 omero-dropbox-5.7.0/src/omero_dropbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-08 12:43:55.000000 omero-dropbox-5.7.0/src/omero_dropbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-08 12:43:55.000000 omero-dropbox-5.7.0/src/omero_dropbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:43:55.000000 omero-dropbox-5.7.0/src/omero_dropbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 12:43:55.000000 omero-dropbox-5.7.0/src/omero_dropbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-08 12:43:55.000000 omero-dropbox-5.7.0/src/omero_dropbox.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `omero-dropbox-5.6.dev3/src/omero_dropbox.egg-info/SOURCES.txt` & `omero-dropbox-5.7.0/src/omero_dropbox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.rst
 setup.py
 src/fsAbstractPlatformMonitor.py
 src/fsDirectory.py
 src/fsDropBox.py
 src/fsDropBoxMonitorClient.py
 src/fsFileServer.py
```

### Comparing `omero-dropbox-5.6.dev3/src/fsUtil.py` & `omero-dropbox-5.7.0/src/fsUtil.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,28 @@
     Use is subject to license terms supplied in LICENSE.txt
 
 """
 
 import logging
 
 
+class NativeKeyDict(dict):
+
+    def __getitem__(self, key):
+        if isinstance(key, bytes):
+            key = key.decode("utf-8")
+        return dict.__getitem__(self, key)
+
+    def __setitem__(self, key, val):
+        if isinstance(key, bytes):
+            key = key.decode("utf-8")
+        return dict.__setitem__(self, key, val)
+
+
+
 def monitorPackage(platformCheck):
     """
         Helper function to determine correct package to load for platform.
 
     """
 
     log = logging.getLogger("fsclient." + __name__)
```

### Comparing `omero-dropbox-5.6.dev3/src/fsDropBox.py` & `omero-dropbox-5.7.0/src/fsDropBox.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,34 +4,28 @@
     OMERO.fs DropBox application
 
     Copyright 2009 University of Dundee. All rights reserved.
     Use is subject to license terms supplied in LICENSE.txt
 
 """
 
-from builtins import str
-from builtins import range
 import logging
 log = logging.getLogger("fsclient.DropBox")
 
 import os
 import sys
 import string
 import threading
 import shutil
 import uuid
 
 # Third party path package. It provides much of the
 # functionality of os.path but without the complexity.
 # Imported as pathModule to avoid clashes.
-try:
-    from omero_ext.path import path as pathModule
-except ImportError:
-    # Python 2
-    from path import path as pathModule
+from omero_ext import path as pathModule
 
 import omero.all
 import omero.grid.monitors as monitors
 
 import omero.rtypes
 import Ice
```

### Comparing `omero-dropbox-5.6.dev3/src/fsFileServer.py` & `omero-dropbox-5.7.0/src/fsFileServer.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,30 +3,22 @@
 """
     OMERO.fs FileServer module.
 
     Copyright 2009 University of Dundee. All rights reserved.
     Use is subject to license terms supplied in LICENSE.txt
 
 """
-from builtins import str
 import logging
 
-try:
-    from hashlib import sha1 as sha
-except:
-    from sha import sha
+from hashlib import sha1 as sha
 
 # Third party path package. It provides much of the
 # functionality of os.path but without the complexity.
 # Imported as pathModule to avoid potential clashes.
-try:
-    from omero_ext.path import path as pathModule
-except ImportError:
-    # Python 2
-    from path import path as pathModule
+from omero_ext import path as pathModule
 
 import omero.all
 import omero.grid.monitors as monitors
 
 
 class FileServerI(monitors.FileServer):
```

### Comparing `omero-dropbox-5.6.dev3/src/fsDropBoxMonitorClient.py` & `omero-dropbox-5.7.0/src/fsDropBoxMonitorClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,20 @@
     OMERO.fs  DropBox implementation of a MonitorClient
 
     Copyright 2009 University of Dundee. All rights reserved.
     Use is subject to license terms supplied in LICENSE.txt
 
 """
 
-from future import standard_library
-standard_library.install_aliases()
-from builtins import str
-from builtins import range
-from builtins import object
 import shlex
 import logging
 import threading
 import queue
 import time
-try:
-    from omero_ext.path import path as pathModule
-except ImportError:
-    # Python 2
-    from path import path as pathModule
+from omero_ext import path as pathModule
 
 import omero
 import omero.cli
 import omero.rtypes
 
 import Ice
 import IceImport
@@ -620,14 +611,16 @@
         """
             Import file or directory using 'bin/omero importer'
             This method is solely responsible for logging the user in,
             attempting (possibly multiply) an import, logging and
             throwing an exception if necessary.
         """
 
+        t = None
+        to = None
         try:
             self.state.appropriateWait(self.throttleImport)  # See ticket:5739
 
             key = self.loginUser(exName)
             if not key:
                 self.log.info("File not imported: %s", fileName)
                 return
@@ -677,16 +670,20 @@
                     f.close()
                     for line in lines:
                         self.log.error(line.strip())
                 else:
                     self.log.error("%s not found !" % t)
                 self.log.error("***** end of output from importer-cli *****")
         finally:
-            remove_path(t)
-            remove_path(to)
+            for x in (t, to):
+                if x:
+                    try:
+                        remove_path(x)
+                    except Exception as e:
+                        self.log.error("failed to remove %s: %s" % (x, e))
 
         return imageId
 
     #
     # Setters
     #
```

### Comparing `omero-dropbox-5.6.dev3/src/fsLists.py` & `omero-dropbox-5.7.0/src/fsLists.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 
     Copyright 2009 University of Dundee. All rights reserved.
     Use is subject to license terms supplied in LICENSE.txt
 
 """
 
 
-from builtins import str
-from builtins import object
 class Greylist(object):
 
     """
         An abstract class representing a general list as a set.
 
         It's neither black nor white! It delegates behaviour to
         the Python set type using that data structure's feature
```

### Comparing `omero-dropbox-5.6.dev3/src/fsMonitorServer.py` & `omero-dropbox-5.7.0/src/fsMonitorServer.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,35 +3,25 @@
 """
     OMERO.fs MonitorServer module.
 
     Copyright 2009 University of Dundee. All rights reserved.
     Use is subject to license terms supplied in LICENSE.txt
 
 """
-from builtins import str
-from future.utils import native_str, bytes_to_native_str
 import logging
 
 import uuid
 
 from fsMonitor import MonitorFactory
+from fsUtil import NativeKeyDict
 
 import omero.all
 import omero.grid.monitors as monitors
 
 
-class NativeKeyDict(dict):
-
-    def __getitem__(self, key):
-        return dict.__getitem__(self, native_str(key))
-
-    def __setitem__(self, key, val):
-        return dict.__setitem__(self, native_str(key), val)mport omero.grid.monitors as monitors
-
-
 class MonitorServerI(monitors.MonitorServer):
 
     """
         Co-ordinates a number of Monitors
 
         :group Constructor: __init__
         :group Methods exposed in Slice: createMonitor, startMonitor,
@@ -249,21 +239,23 @@
 
             :return: No explicit return value.
 
         """
 
         eventList = []
         for fileEvent in fileList:
-            fileId = bytes_to_native_str(fileEvent[0])
+            fileId = fileEvent[0]
+            if isinstance(fileId, bytes):
+                fileId = fileId.decode("utf-8")
             info = monitors.EventInfo(fileId, fileEvent[1])
             eventList.append(info)
 
         proxy = self.proxies[monitorId]
 
         try:
             self.log.info('Event notification on monitor id= %s', monitorId)
             self.log.debug(' ...notifications are: %s', str(eventList))
-            proxy.fsEventHappened(native_str(monitorId), eventList)
+            proxy.fsEventHappened(str(monitorId), eventList)
         except Exception as e:
             self.log.info(
                 'Callback to monitor id=' + monitorId
                 + ' failed. Reason: ' + str(e))
```

### Comparing `omero-dropbox-5.6.dev3/src/fsServerFS.py` & `omero-dropbox-5.7.0/src/fsServerFS.py`

 * *Files identical despite different names*

### Comparing `omero-dropbox-5.6.dev3/src/fsMac-10-5-Monitor.py` & `omero-dropbox-5.7.0/src/fsMac-10-5-Monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,31 +3,24 @@
 """
     OMERO.fs Monitor module for Mac Os.
 
     Copyright 2009 University of Dundee. All rights reserved.
     Use is subject to license terms supplied in LICENSE.txt
 
 """
-from builtins import str
-from builtins import range
-from builtins import object
 import logging
 import time
 from Foundation import NSAutoreleasePool, NSMutableArray, NSString
 import FSEvents
 
 
 # Third party path package. It provides much of the
 # functionality of os.path but without the complexity.
 # Imported as pathModule to avoid potential clashes.
-try:
-    from omero_ext.path import path as pathModule
-except ImportError:
-    # Python 2
-    from path import path as pathModule
+from omero_ext import path as pathModule
 
 __import__("omero.all")
 import omero.grid.monitors as monitors
 import uuid
 
 from fsAbstractPlatformMonitor import AbstractPlatformMonitor
 import fsDirectory
```

### Comparing `omero-dropbox-5.6.dev3/src/fsMonitor.py` & `omero-dropbox-5.7.0/src/fsMonitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 """
     OMERO.fs Monitor module .
 
     Copyright 2009 University of Dundee. All rights reserved.
     Use is subject to license terms supplied in LICENSE.txt
 
 """
-from builtins import str
-from builtins import object
 import logging
 import threading
 
 __import__("omero.all")
 import omero.grid.monitors as monitors
```

### Comparing `omero-dropbox-5.6.dev3/src/fsPyinotifyMonitor.py` & `omero-dropbox-5.7.0/src/fsPyinotifyMonitor.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,38 +3,33 @@
 """
     OMERO.fs Monitor module for Linux.
 
     Copyright 2009 University of Dundee. All rights reserved.
     Use is subject to license terms supplied in LICENSE.txt
 
 """
-from __future__ import division
-from builtins import str
-from past.utils import old_div
-from builtins import object
 import logging
 import copy
 import time
 
-# Third party path package. It provides much of the
-# functionality of os.path but without the complexity.
-# Imported as pathModule to avoid potential clashes.
-try:
-    from omero_ext.path import path as pathModule
-except ImportError:
-    # Python 2
-    from path import path as pathModule
-
-__import__("omero.all")
+__import__("omero.all")  # noqa
 import omero.grid.monitors as monitors
 from fsAbstractPlatformMonitor import AbstractPlatformMonitor
+from fsUtil import NativeKeyDict
 
-importlog = logging.getLogger("fsserver." + __name__)
 from omero_ext import pyinotify
-importlog.info("Imported pyinotify version %s", str(pyinotify.__version__))
+
+
+importlog = logging.getLogger("fsserver." + __name__)
+importlog.info("Imported pyinotify version %s" % pyinotify.__version__)
+
+# Third party path package. It provides much of the
+# functionality of os.path but without the complexity.
+# Imported as pathModule to avoid potential clashes.
+from omero_ext import path as pathModule
 
 
 class PlatformMonitor(AbstractPlatformMonitor):
 
     """
         A Thread to monitor a path.
 
@@ -96,18 +91,18 @@
             self.wm, ProcessEvent(
                 wm=self.wm, cb=self.propagateEvents, et=self.eTypes,
                 ignoreDirEvents=self.ignoreDirEvents))
         try:
             self.wm.addBaseWatch(
                 self.pathsToMonitor, (pyinotify.ALL_EVENTS), rec=recurse,
                 auto_add=follow)
-            self.log.info('Monitor set-up on %s', str(self.pathsToMonitor))
-            self.log.info('Monitoring %s events', str(self.eTypes))
-        except:
-            self.log.error('Monitor failed on: %s', str(self.pathsToMonitor))
+            self.log.info('Monitor set-up on %s' % self.pathsToMonitor)
+            self.log.info('Monitoring %s events' % self.eTypes)
+        except Exception:
+            self.log.error('Monitor failed on: %s' % self.pathsToMonitor)
 
     def start(self):
         """
             Start monitoring an FSEventStream.
 
             This method, overridden from Thread, is run by
             calling the inherited method start(). The method attempts
@@ -142,80 +137,83 @@
     """
        Essentially a limited-function wrapper to WatchManager
 
        At present only one watch is allowed on each path. This
        may need to be fixed for applications outside of DropBox.
 
     """
-    watchPaths = {}
-    watchParams = {}
+    watchPaths = NativeKeyDict()
+    watchParams = NativeKeyDict()
     log = logging.getLogger("fsserver." + __name__)
 
     def isPathWatched(self, pathString):
         return pathString in list(self.watchPaths.keys())
 
     def addBaseWatch(self, path, mask, rec=False, auto_add=False):
         try:
             res = pyinotify.WatchManager.add_watch(
                 self, path, mask, rec=False, auto_add=False, quiet=False)
             self.watchPaths.update(res)
             self.watchParams[path] = WatchParameters(
                 mask, rec=rec, auto_add=auto_add)
-            self.log.info('Base watch created on: %s', path)
+            self.log.info('Base watch created on: %s' % path)
             if rec:
                 for d in pathModule.path(path).dirs():
                     self.addWatch(str(d), mask)
         except Exception as e:
             self.log.error(
-                'Unable to create base watch on: %s : %s', path, str(e))
+                'Unable to create base watch on: %s : %s' % (path, e))
             raise e
 
     def addWatch(self, path, mask):
         if not self.isPathWatched(path):
             try:
+                if isinstance(path, bytes):
+                    path_obj = pathModule.path(path.decode("utf-8"))
+                else:
+                    path_obj = pathModule.path(path)
                 res = pyinotify.WatchManager.add_watch(
                     self, path, mask, rec=False, auto_add=False, quiet=False)
                 self.watchPaths.update(res)
                 self.watchParams[path] = copy.copy(
-                    self.watchParams[pathModule.path(path).parent])
+                    self.watchParams[path_obj.parent])
                 if self.watchParams[path].getRec():
-                    for d in pathModule.path(path).dirs():
-                        self.addWatch(str(d), mask)
+                    for d in path_obj.dirs():
+                        self.addWatch(d, mask)
                 if self.isPathWatched(path):
-                    self.log.info('Watch added on: %s', path)
+                    self.log.info('Watch added on: %s' % path)
                 else:
-                    self.log.info('Unable to add watch on: %s', path)
+                    self.log.info('Unable to add watch on: %s' % path)
             except Exception as e:
                 self.log.error(
-                    'Unable to add watch on: %s : %s', path, str(e))
+                    'Unable to add watch on: %s : %s' % (path, e))
 
     def removeWatch(self, path):
         if self.isPathWatched(path):
             try:
                 removeDict = {}
-                self.log.info('Trying to remove : %s', path)
+                self.log.info('Trying to remove : %s' % path)
                 removeDict[self.watchPaths[path]] = path
                 for d in list(self.watchPaths.keys()):
                     if d.find(path + '/') == 0:
-                        self.log.info('    ... and : %s', d)
+                        self.log.info('    ... and : %s' % d)
                         removeDict[self.watchPaths[d]] = d
                 res = pyinotify.WatchManager.rm_watch(
                     self, list(removeDict.keys()), quiet=False)
                 for wd in list(res.keys()):
                     if res[wd]:
                         self.watchPaths.pop(removeDict[wd], True)
                         self.watchParams.pop(removeDict[wd], True)
-                        self.log.info('Watch removed on: %s', removeDict[wd])
+                        self.log.info('Watch removed on: %s' % removeDict[wd])
                     else:
                         self.log.info(
-                            'Watch remove failed, wd=%s, on: %s',
-                            wd, removeDict[wd])
+                            'Watch remove failed, wd=%s, on: %s' % (wd, removeDict[wd]))
             except Exception as e:
                 self.log.error(
-                    'Unable to remove watch on: %s : %s', path, str(e))
+                    'Unable to remove watch on: %s : %s' % (path, e))
 
     def getWatchPaths(self):
         for (path, wd) in list(self.watchPaths.items()):
             yield (path, wd)
 
 
 class WatchParameters(object):
@@ -248,141 +246,137 @@
 
     def process_default(self, event):
 
         try:
             # pyinotify 0.8
             name = event.pathname
             maskname = event.maskname
-        except:
+        except Exception:
             # pyinotify 0.7 or below
-            name = old_div(pathModule.path(event.path), pathModule.path(event.name))
+            name = (pathModule.path(event.path) /
+                pathModule.path(event.name))
             maskname = event.event_name
 
         el = []
 
         # This is a tricky one. I'm not sure why these events arise exactly.
         # It seems to happen when inotify isn't sure of the path. Yet all the
         # events seem to have otherwise good paths. So, remove the suffix and
         # allow the event to be dealt with as normal.
         if name.find(b'-unknown-path') > 0:
             self.log.debug(
-                'Event with "-unknown-path" of type %s : %s', maskname, name)
+                'Event with "-unknown-path" of type %s : %s' % (maskname, name))
             name = name.replace(b'-unknown-path', b'')
 
         # New directory within watch area,
         # either created, moved in or modfied attributes, ie now readable.
+        path_name = pathModule.path(name.decode("utf-8"))
         if (event.mask == (pyinotify.IN_CREATE | pyinotify.IN_ISDIR)
                 or event.mask == (pyinotify.IN_MOVED_TO | pyinotify.IN_ISDIR)
                 or event.mask == (pyinotify.IN_ATTRIB | pyinotify.IN_ISDIR)):
             self.log.info(
-                'New directory event of type %s at: %s', maskname, name)
+                'New directory event of type %s at: %s' % (maskname, name))
             if "Creation" in self.et:
                 if name.find(b'untitled folder') == -1:
                     if not self.ignoreDirEvents:
                         el.append((name, monitors.EventType.Create))
                     else:
                         self.log.info('Not propagated.')
                     # Handle the recursion plus create any potentially missed
                     # Create events
-                    if self.wm.watchParams[
-                            pathModule.path(name).parent].getAutoAdd():
+                    if self.wm.watchParams[path_name.parent].getAutoAdd():
                         self.wm.addWatch(
                             name, self.wm.watchParams[
-                                pathModule.path(name).parent].getMask())
+                                path_name.parent].getMask())
                         if self.wm.isPathWatched(name):
                             if self.wm.watchParams[
-                                    pathModule.path(name).parent].getRec():
-                                for d in pathModule.path(name).walkdirs(
+                                    path_name.parent].getRec():
+                                for d in path_name.walkdirs(
                                         errors='warn'):
                                     self.log.info(
                                         ('NON-INOTIFY event: '
-                                         'New directory at: %s'),
-                                        str(d))
+                                         'New directory at: %s') % d)
                                     if not self.ignoreDirEvents:
                                         el.append((
                                             str(d),
                                             monitors.EventType.Create))
                                     else:
                                         self.log.info('Not propagated.')
                                     self.wm.addWatch(
                                         str(d), self.wm.watchParams[
-                                            pathModule.path(
-                                                name).parent].getMask())
-                                for f in pathModule.path(name).walkfiles(
+                                            path_name.parent].getMask())
+                                for f in path_name.walkfiles(
                                         errors='warn'):
                                     self.log.info(
-                                        'NON-INOTIFY event: New file at: %s',
-                                        str(f))
+                                        'NON-INOTIFY event: New file at: %s' % f)
                                     el.append(
                                         (str(f), monitors.EventType.Create))
                             else:
-                                for d in pathModule.path(name).dirs():
+                                for d in path_name.dirs():
                                     self.log.info(
                                         ('NON-INOTIFY event: '
-                                         'New directory at: %s'),
-                                        str(d))
+                                         'New directory at: %s') % d)
                                     if not self.ignoreDirEvents:
                                         el.append((
                                             str(d),
                                             monitors.EventType.Create))
                                     else:
                                         self.log.info('Not propagated.')
-                                for f in pathModule.path(name).files():
+                                for f in path_name.files():
                                     self.log.info(
-                                        'NON-INOTIFY event: New file at: %s',
-                                        str(f))
+                                        'NON-INOTIFY event: New file at: %s' % f)
                                     el.append(
                                         (str(f), monitors.EventType.Create))
                 else:
                     self.log.info('Created "untitled folder" ignored.')
             else:
                 self.log.info('Not propagated.')
 
         # Deleted directory or one moved out of the watch area.
         elif (event.mask == (pyinotify.IN_MOVED_FROM | pyinotify.IN_ISDIR)
                 or event.mask == (pyinotify.IN_DELETE | pyinotify.IN_ISDIR)):
             self.log.info(
-                'Deleted directory event of type %s at: %s', maskname, name)
+                'Deleted directory event of type %s at: %s' % (maskname, name))
             if "Deletion" in self.et:
                 if name.find(b'untitled folder') == -1:
                     if not self.ignoreDirEvents:
                         el.append((name, monitors.EventType.Delete))
                     else:
                         self.log.info('Not propagated.')
                     self.log.info(
-                        'Files and subfolders within %s may have been deleted '
-                        'without notice', name)
+                        ('Files and subfolders within %s may have been deleted '
+                        'without notice') % name)
                     self.wm.removeWatch(name)
                 else:
                     self.log.info('Deleted "untitled folder" ignored.')
             else:
                 self.log.info('Not propagated.')
 
         # New file within watch area, either created or moved into.
         # The file may have been created but it may not be complete and closed.
         # Modifications should be watched
         elif event.mask == pyinotify.IN_CREATE:
-            self.log.info('New file event of type %s at: %s', maskname, name)
+            self.log.info('New file event of type %s at: %s' % (maskname, name))
             if "Creation" in self.et:
                 self.waitingCreates.add(name)
             else:
                 self.log.info('Not propagated.')
 
         # New file within watch area.
         elif event.mask == pyinotify.IN_MOVED_TO:
-            self.log.info('New file event of type %s at: %s', maskname, name)
+            self.log.info('New file event of type %s at: %s' % (maskname, name))
             if "Creation" in self.et:
                 el.append((name, monitors.EventType.Create))
             else:
                 self.log.info('Not propagated.')
 
         # Modified file within watch area.
         elif event.mask == pyinotify.IN_CLOSE_WRITE:
             self.log.info(
-                'Modified file event of type %s at: %s', maskname, name)
+                'Modified file event of type %s at: %s' % (maskname, name))
             if name in self.waitingCreates:
                 if "Creation" in self.et:
                     el.append((name, monitors.EventType.Create))
                     self.waitingCreates.remove(name)
                 else:
                     self.log.info('Not propagated.')
             else:
@@ -391,71 +385,71 @@
                 else:
                     self.log.info('Not propagated.')
 
         # Modified file within watch area, only notify if file is not
         # waitingCreate.
         elif event.mask == pyinotify.IN_MODIFY:
             self.log.info(
-                'Modified file event of type %s at: %s', maskname, name)
+                'Modified file event of type %s at: %s' % (maskname, name))
             if name not in self.waitingCreates:
                 if "Modification" in self.et:
                     el.append((name, monitors.EventType.Modify))
                 else:
                     self.log.info('Not propagated.')
 
         # Deleted file  or one moved out of the watch area.
         elif (event.mask == pyinotify.IN_MOVED_FROM
                 or event.mask == pyinotify.IN_DELETE):
             self.log.info(
-                'Deleted file event of type %s at: %s', maskname, name)
+                'Deleted file event of type %s at: %s' % (maskname, name))
             if "Deletion" in self.et:
                 el.append((name, monitors.EventType.Delete))
             else:
                 self.log.info('Not propagated.')
 
         # These are all the currently ignored events.
         elif event.mask == pyinotify.IN_ATTRIB:
             # File attributes have changed? Useful?
-            self.log.debug('Ignored event of type %s at: %s', maskname, name)
+            self.log.debug('Ignored event of type %s at: %s' % (maskname, name))
         elif (event.mask == pyinotify.IN_DELETE_SELF
                 or event.mask == pyinotify.IN_IGNORED):
             # This is when a directory being watched is removed, handled above.
-            self.log.debug('Ignored event of type %s at: %s', maskname, name)
+            self.log.debug('Ignored event of type %s at: %s' % (maskname, name))
         elif event.mask == pyinotify.IN_MOVE_SELF:
             # This is when a directory being watched is moved out of the watch
             # area (itself!), handled above.
-            self.log.debug('Ignored event of type %s at: %s', maskname, name)
+            self.log.debug('Ignored event of type %s at: %s' % (maskname, name))
         elif event.mask == pyinotify.IN_OPEN | pyinotify.IN_ISDIR:
             # Event, dir open, we can ignore for now to reduce the log volume
             # at any rate.
-            self.log.debug('Ignored event of type %s at: %s', maskname, name)
+            self.log.debug('Ignored event of type %s at: %s' % (maskname, name))
         elif event.mask == pyinotify.IN_CLOSE_NOWRITE | pyinotify.IN_ISDIR:
             # Event, dir close, we can ignore for now to reduce the log volume
             # at any rate.
-            self.log.debug('Ignored event of type %s at: %s', maskname, name)
+            self.log.debug('Ignored event of type %s at: %s' % (maskname, name))
         elif event.mask == pyinotify.IN_ACCESS | pyinotify.IN_ISDIR:
             # Event, dir access, we can ignore for now to reduce the log volume
             # at any rate.
-            self.log.debug('Ignored event of type %s at: %s', maskname, name)
+            self.log.debug('Ignored event of type %s at: %s' % (maskname, name))
         elif event.mask == pyinotify.IN_OPEN:
             # Event, file open, we can ignore for now to reduce the log volume
             # at any rate.
-            self.log.debug('Ignored event of type %s at: %s', maskname, name)
+            self.log.debug('Ignored event of type %s at: %s' % (maskname, name))
         elif event.mask == pyinotify.IN_CLOSE_NOWRITE:
             # Event, file close, we can ignore for now to reduce the log volume
             # at any rate.
-            self.log.debug('Ignored event of type %s at: %s', maskname, name)
+            self.log.debug('Ignored event of type %s at: %s' % (maskname, name))
         elif event.mask == pyinotify.IN_ACCESS:
             # Event, file access, we can ignore for now to reduce the log
             # volume at any rate.
-            self.log.debug('Ignored event of type %s at: %s', maskname, name)
+            self.log.debug('Ignored event of type %s at: %s' % (maskname, name))
 
         # Other events, log them since they really should be caught above
         else:
-            self.log.info('Uncaught event of type %s at: %s', maskname, name)
+            self.log.info('Uncaught event of type %s at: %s' % (maskname, name))
             self.log.info('Not propagated.')
 
         if len(el) > 0:
             self.cb(el)
 
 
 if __name__ == "__main__":
@@ -474,12 +468,12 @@
     log.setLevel(logging.INFO)
     log = logging.getLogger("fstestserver." + __name__)
 
     p = Proxy()
     m = PlatformMonitor(
         [monitors.WatchEventType.Creation,
          monitors.WatchEventType.Modification],
-        monitors.PathMode.Follow, "\OMERO\DropBox", [], [], True, True, p)
+        monitors.PathMode.Follow, r"\OMERO\DropBox", [], [], True, True, p)
     try:
         m.start()
-    except:
+    except Exception:
         m.stop()
```

### Comparing `omero-dropbox-5.6.dev3/src/fsDirectory.py` & `omero-dropbox-5.7.0/src/fsDirectory.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,27 +7,21 @@
     a snaphot of a directory tree.
 
     Copyright 2009 University of Dundee. All rights reserved.
     Use is subject to license terms supplied in LICENSE.txt
 
 """
 
-from builtins import str
-from builtins import object
 import logging
 from time import localtime, strftime
 
 # Third party path package. It provides much of the
 # functionality of os.path but without the complexity.
 # Imported as pathModule to avoid potential clashes.
-try:
-    from omero_ext.path import path as pathModule
-except ImportError:
-    # Python 2
-    from path import path as pathModule
+from omero_ext import path as pathModule
 
 import fsLists
 
 
 class Directory(object):
 
     """
```

### Comparing `omero-dropbox-5.6.dev3/src/fsNotificationScheduler.py` & `omero-dropbox-5.7.0/src/fsNotificationScheduler.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 """
     OMERO.fs Notification Scheduler.
 
     Copyright 2009 University of Dundee. All rights reserved.
     Use is subject to license terms supplied in LICENSE.txt
 
 """
-from future import standard_library
-standard_library.install_aliases()
-from builtins import range
 import logging
 import threading
 import queue
 import time
 
 
 class NotificationScheduler(threading.Thread):
```

### Comparing `omero-dropbox-5.6.dev3/src/fsWin-XP-Monitor.py` & `omero-dropbox-5.7.0/src/fsWin-XP-Monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,23 @@
 """
     OMERO.fs Monitor module for Window XP.
 
     Copyright 2009 University of Dundee. All rights reserved.
     Use is subject to license terms supplied in LICENSE.txt
 
 """
-from builtins import str
-from builtins import object
 import logging
 import threading
 import os
 import time
 
 # Third party path package. It provides much of the
 # functionality of os.path but without the complexity.
 # Imported as pathModule to avoid clashes.
-try:
-    from omero_ext.path import path as pathModule
-except ImportError:
-    # Python 2
-    from path import path as pathModule
+from omero_ext import path as pathModule
 
 __import__("omero.all")
 import omero.grid.monitors as monitors
 from fsAbstractPlatformMonitor import AbstractPlatformMonitor
 
 import win32file
 import win32con
```

### Comparing `omero-dropbox-5.6.dev3/src/fsServerMS.py` & `omero-dropbox-5.7.0/src/fsServerMS.py`

 * *Files identical despite different names*

### Comparing `omero-dropbox-5.6.dev3/src/fsAbstractPlatformMonitor.py` & `omero-dropbox-5.7.0/src/fsAbstractPlatformMonitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
     OMERO.fs Abstract Monitor module.
 
     Copyright 2009 University of Dundee. All rights reserved.
     Use is subject to license terms supplied in LICENSE.txt
 
 """
-from builtins import str
 import threading
 
 
 class AbstractPlatformMonitor(threading.Thread):
 
     """
         A Thread to monitor a path.
@@ -66,13 +65,13 @@
                     events.
 
             :return: No explicit return value.
 
         """
         if len(eventList) > 0:
             try:
-                self.log.info('Event notification : %s', str(eventList))
+                self.log.info('Event notification : %s' % eventList)
                 self.proxy.callback(eventList)
             except:
                 self.log.exception("Notification failed : ")
         else:
             self.log.info('No notifications propagated')
```

### Comparing `omero-dropbox-5.6.dev3/setup.py` & `omero-dropbox-5.7.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
-   Copyright 2008-2019 The Open Microscopy Environment, Glencoe Software, Inc.
+   Copyright 2008-2020 The Open Microscopy Environment, Glencoe Software, Inc.
    All rights reserved.
 
    Use is subject to license terms supplied in LICENSE.txt
 
 """
 
 import glob
 import sys
 import os
 
 from setuptools import setup
 
-VERSION = "5.6.dev3"
+VERSION = "5.7.0"
 
 url = 'https://docs.openmicroscopy.org/latest/omero/developers/Server/FS.html'
 
 packageless = glob.glob("src/*.py")
 packageless = [x[4:-3] for x in packageless]
 
 def read(fname):
@@ -38,20 +38,21 @@
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'Intended Audience :: System Administrators',
         'License :: OSI Approved :: GNU General Public License v2 '
         'or later (GPLv2+)',
         'Natural Language :: English',
         'Operating System :: OS Independent',
-        'Programming Language :: Python :: 2',
+        'Programming Language :: Python :: 3',
         'Topic :: Software Development :: Libraries :: Python Modules',
       ],  # Get strings from
           # http://pypi.python.org/pypi?%3Aaction=list_classifiers
       author="The Open Microscopy Team",
       author_email="ome-devel@lists.openmicroscopy.org.uk",
       url=url,
       package_dir={"": "src"},
       py_modules=packageless,
       install_requires=[
-          "omero-py>=5.6.dev6",  # requires Ice (use wheel for faster installs)
+          "omero-py",  # requires Ice (use wheel for faster installs)
       ],
-      tests_require=['pytest<3'])
+      python_requires='>=3.8',
+      tests_require=['pytest', 'pytest-mock'])
```

