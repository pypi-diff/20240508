# Comparing `tmp/HelloPyOnly-0.1.23.tar.gz` & `tmp/HelloPyOnly-0.1.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HelloPyOnly-0.1.23.tar", last modified: Fri Apr 19 07:23:41 2024, max compression
+gzip compressed data, was "HelloPyOnly-0.1.24.tar", last modified: Wed May  8 07:56:42 2024, max compression
```

## Comparing `HelloPyOnly-0.1.23.tar` & `HelloPyOnly-0.1.24.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 07:23:41.931085 HelloPyOnly-0.1.23/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:23:41.717260 HelloPyOnly-0.1.23/HelloPyOnly.egg-info/
--rw-rw-rw-   0        0        0      553 2024-04-19 07:23:41.000000 HelloPyOnly-0.1.23/HelloPyOnly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      750 2024-04-19 07:23:41.000000 HelloPyOnly-0.1.23/HelloPyOnly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 07:23:41.000000 HelloPyOnly-0.1.23/HelloPyOnly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-19 07:23:41.000000 HelloPyOnly-0.1.23/HelloPyOnly.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-19 07:23:41.000000 HelloPyOnly-0.1.23/HelloPyOnly.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      553 2024-04-19 07:23:41.930078 HelloPyOnly-0.1.23/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-19 07:23:41.819614 HelloPyOnly-0.1.23/hellopy/
--rw-rw-rw-   0        0        0     2064 2023-12-02 03:15:10.000000 HelloPyOnly-0.1.23/hellopy/__init__.py
--rw-rw-rw-   0        0        0     4597 2023-10-20 05:46:44.000000 HelloPyOnly-0.1.23/hellopy/collision.py
--rw-rw-rw-   0        0        0      268 2023-12-02 03:24:54.000000 HelloPyOnly-0.1.23/hellopy/demo.py
--rw-rw-rw-   0        0        0     2773 2023-10-17 14:39:56.000000 HelloPyOnly-0.1.23/hellopy/events.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:23:41.925070 HelloPyOnly-0.1.23/hellopy/gameobject/
--rw-rw-rw-   0        0        0      389 2023-10-18 06:44:19.000000 HelloPyOnly-0.1.23/hellopy/gameobject/__init__.py
--rw-rw-rw-   0        0        0     2051 2023-10-17 08:13:10.000000 HelloPyOnly-0.1.23/hellopy/gameobject/circle.py
--rw-rw-rw-   0        0        0      220 2023-10-17 06:43:33.000000 HelloPyOnly-0.1.23/hellopy/gameobject/ellipse.py
--rw-rw-rw-   0        0        0      384 2023-10-16 07:28:41.000000 HelloPyOnly-0.1.23/hellopy/gameobject/gameobject.py
--rw-rw-rw-   0        0        0     2467 2023-10-17 06:43:38.000000 HelloPyOnly-0.1.23/hellopy/gameobject/line.py
--rw-rw-rw-   0        0        0     3676 2023-12-28 02:51:59.000000 HelloPyOnly-0.1.23/hellopy/gameobject/polygon.py
--rw-rw-rw-   0        0        0      545 2023-10-19 01:46:38.000000 HelloPyOnly-0.1.23/hellopy/gameobject/rectangle.py
--rw-rw-rw-   0        0        0    10478 2024-04-06 00:45:00.000000 HelloPyOnly-0.1.23/hellopy/gameobject/sprite.py
--rw-rw-rw-   0        0        0        0 2024-04-06 00:29:09.000000 HelloPyOnly-0.1.23/hellopy/gameobject/test.py
--rw-rw-rw-   0        0        0     2777 2024-01-06 08:20:48.000000 HelloPyOnly-0.1.23/hellopy/gameobject/text.py
--rw-rw-rw-   0        0        0      649 2023-12-27 01:58:30.000000 HelloPyOnly-0.1.23/hellopy/gameobject/triangle.py
--rw-rw-rw-   0        0        0      258 2023-10-17 06:30:34.000000 HelloPyOnly-0.1.23/hellopy/key.py
--rw-rw-rw-   0        0        0      136 2023-10-16 05:53:09.000000 HelloPyOnly-0.1.23/hellopy/mouse.py
--rw-rw-rw-   0        0        0     1882 2023-10-20 05:46:53.000000 HelloPyOnly-0.1.23/hellopy/resource.py
--rw-rw-rw-   0        0        0      388 2023-10-18 06:58:07.000000 HelloPyOnly-0.1.23/hellopy/sound.py
--rw-rw-rw-   0        0        0      341 2023-10-17 06:42:53.000000 HelloPyOnly-0.1.23/hellopy/util.py
--rw-rw-rw-   0        0        0     3164 2024-01-04 03:37:58.000000 HelloPyOnly-0.1.23/hellopy/window.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:23:41.929080 HelloPyOnly-0.1.23/onlydemos/
--rw-rw-rw-   0        0        0     5983 2024-04-19 07:19:44.000000 HelloPyOnly-0.1.23/onlydemos/LoongPy.py
--rw-rw-rw-   0        0        0     1797 2023-10-20 05:45:56.000000 HelloPyOnly-0.1.23/onlydemos/__init__.py
--rw-rw-rw-   0        0        0     4352 2023-10-20 07:23:57.000000 HelloPyOnly-0.1.23/onlydemos/pumpkin.py
--rw-rw-rw-   0        0        0       42 2024-04-19 07:23:41.931085 HelloPyOnly-0.1.23/setup.cfg
--rw-rw-rw-   0        0        0     1049 2024-04-19 07:23:14.000000 HelloPyOnly-0.1.23/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:56:42.916568 HelloPyOnly-0.1.24/
+drwxrwxrwx   0        0        0        0 2024-05-08 07:56:42.895241 HelloPyOnly-0.1.24/HelloPyOnly.egg-info/
+-rw-rw-rw-   0        0        0      553 2024-05-08 07:56:42.000000 HelloPyOnly-0.1.24/HelloPyOnly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      760 2024-05-08 07:56:42.000000 HelloPyOnly-0.1.24/HelloPyOnly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 07:56:42.000000 HelloPyOnly-0.1.24/HelloPyOnly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-08 07:56:42.000000 HelloPyOnly-0.1.24/HelloPyOnly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-08 07:56:42.000000 HelloPyOnly-0.1.24/HelloPyOnly.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      553 2024-05-08 07:56:42.915577 HelloPyOnly-0.1.24/PKG-INFO
+-rw-rw-rw-   0        0        0       89 2024-05-04 08:02:44.000000 HelloPyOnly-0.1.24/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 07:56:42.903891 HelloPyOnly-0.1.24/hellopy/
+-rw-rw-rw-   0        0        0     2064 2023-12-02 03:15:10.000000 HelloPyOnly-0.1.24/hellopy/__init__.py
+-rw-rw-rw-   0        0        0     4597 2023-10-20 05:46:44.000000 HelloPyOnly-0.1.24/hellopy/collision.py
+-rw-rw-rw-   0        0        0      268 2023-12-02 03:24:54.000000 HelloPyOnly-0.1.24/hellopy/demo.py
+-rw-rw-rw-   0        0        0     2773 2023-10-17 14:39:56.000000 HelloPyOnly-0.1.24/hellopy/events.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:56:42.912568 HelloPyOnly-0.1.24/hellopy/gameobject/
+-rw-rw-rw-   0        0        0      389 2023-10-18 06:44:19.000000 HelloPyOnly-0.1.24/hellopy/gameobject/__init__.py
+-rw-rw-rw-   0        0        0     2051 2023-10-17 08:13:10.000000 HelloPyOnly-0.1.24/hellopy/gameobject/circle.py
+-rw-rw-rw-   0        0        0      220 2023-10-17 06:43:33.000000 HelloPyOnly-0.1.24/hellopy/gameobject/ellipse.py
+-rw-rw-rw-   0        0        0      384 2023-10-16 07:28:41.000000 HelloPyOnly-0.1.24/hellopy/gameobject/gameobject.py
+-rw-rw-rw-   0        0        0     2467 2023-10-17 06:43:38.000000 HelloPyOnly-0.1.24/hellopy/gameobject/line.py
+-rw-rw-rw-   0        0        0     3676 2023-12-28 02:51:59.000000 HelloPyOnly-0.1.24/hellopy/gameobject/polygon.py
+-rw-rw-rw-   0        0        0      545 2023-10-19 01:46:38.000000 HelloPyOnly-0.1.24/hellopy/gameobject/rectangle.py
+-rw-rw-rw-   0        0        0    10478 2024-04-06 00:45:00.000000 HelloPyOnly-0.1.24/hellopy/gameobject/sprite.py
+-rw-rw-rw-   0        0        0        0 2024-04-06 00:29:09.000000 HelloPyOnly-0.1.24/hellopy/gameobject/test.py
+-rw-rw-rw-   0        0        0     2777 2024-01-06 08:20:48.000000 HelloPyOnly-0.1.24/hellopy/gameobject/text.py
+-rw-rw-rw-   0        0        0      649 2023-12-27 01:58:30.000000 HelloPyOnly-0.1.24/hellopy/gameobject/triangle.py
+-rw-rw-rw-   0        0        0      258 2023-10-17 06:30:34.000000 HelloPyOnly-0.1.24/hellopy/key.py
+-rw-rw-rw-   0        0        0      136 2023-10-16 05:53:09.000000 HelloPyOnly-0.1.24/hellopy/mouse.py
+-rw-rw-rw-   0        0        0     1882 2023-10-20 05:46:53.000000 HelloPyOnly-0.1.24/hellopy/resource.py
+-rw-rw-rw-   0        0        0      388 2023-10-18 06:58:07.000000 HelloPyOnly-0.1.24/hellopy/sound.py
+-rw-rw-rw-   0        0        0      341 2023-10-17 06:42:53.000000 HelloPyOnly-0.1.24/hellopy/util.py
+-rw-rw-rw-   0        0        0     3263 2024-05-08 07:49:07.000000 HelloPyOnly-0.1.24/hellopy/window.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:56:42.915577 HelloPyOnly-0.1.24/onlydemos/
+-rw-rw-rw-   0        0        0     5983 2024-04-19 07:19:44.000000 HelloPyOnly-0.1.24/onlydemos/LoongPy.py
+-rw-rw-rw-   0        0        0     1797 2023-10-20 05:45:56.000000 HelloPyOnly-0.1.24/onlydemos/__init__.py
+-rw-rw-rw-   0        0        0     4352 2023-10-20 07:23:57.000000 HelloPyOnly-0.1.24/onlydemos/pumpkin.py
+-rw-rw-rw-   0        0        0       42 2024-05-08 07:56:42.916568 HelloPyOnly-0.1.24/setup.cfg
+-rw-rw-rw-   0        0        0     1049 2024-05-08 07:52:21.000000 HelloPyOnly-0.1.24/setup.py
```

### Comparing `HelloPyOnly-0.1.23/HelloPyOnly.egg-info/PKG-INFO` & `HelloPyOnly-0.1.24/HelloPyOnly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HelloPyOnly
-Version: 0.1.23
+Version: 0.1.24
 Summary: This is the game engine of Only Hello Science project.
 Home-page: https://github.com/zfan0311/hellopy.git
 Author: funk.zhang
 Author-email: zhangfangid@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `HelloPyOnly-0.1.23/HelloPyOnly.egg-info/SOURCES.txt` & `HelloPyOnly-0.1.24/HelloPyOnly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+README.md
 setup.py
 HelloPyOnly.egg-info/PKG-INFO
 HelloPyOnly.egg-info/SOURCES.txt
 HelloPyOnly.egg-info/dependency_links.txt
 HelloPyOnly.egg-info/requires.txt
 HelloPyOnly.egg-info/top_level.txt
 hellopy/__init__.py
```

### Comparing `HelloPyOnly-0.1.23/PKG-INFO` & `HelloPyOnly-0.1.24/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HelloPyOnly
-Version: 0.1.23
+Version: 0.1.24
 Summary: This is the game engine of Only Hello Science project.
 Home-page: https://github.com/zfan0311/hellopy.git
 Author: funk.zhang
 Author-email: zhangfangid@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `HelloPyOnly-0.1.23/hellopy/__init__.py` & `HelloPyOnly-0.1.24/hellopy/__init__.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.23/hellopy/collision.py` & `HelloPyOnly-0.1.24/hellopy/collision.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.23/hellopy/events.py` & `HelloPyOnly-0.1.24/hellopy/events.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.23/hellopy/gameobject/circle.py` & `HelloPyOnly-0.1.24/hellopy/gameobject/circle.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.23/hellopy/gameobject/line.py` & `HelloPyOnly-0.1.24/hellopy/gameobject/line.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.23/hellopy/gameobject/polygon.py` & `HelloPyOnly-0.1.24/hellopy/gameobject/polygon.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.23/hellopy/gameobject/rectangle.py` & `HelloPyOnly-0.1.24/hellopy/gameobject/rectangle.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.23/hellopy/gameobject/sprite.py` & `HelloPyOnly-0.1.24/hellopy/gameobject/sprite.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.23/hellopy/gameobject/text.py` & `HelloPyOnly-0.1.24/hellopy/gameobject/text.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.23/hellopy/gameobject/triangle.py` & `HelloPyOnly-0.1.24/hellopy/gameobject/triangle.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.23/hellopy/resource.py` & `HelloPyOnly-0.1.24/hellopy/resource.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.23/hellopy/window.py` & `HelloPyOnly-0.1.24/hellopy/window.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,18 @@
     # 设置窗口刷新帧率
     def set_fps(self, fps):
         self.fps =fps
 
     # 清空屏幕
     def clear(self):
         self.screen.fill("black")
+
+    # 设置窗口背景颜色
+    def bg_color(self, color):
+        self.screen.fill(color)
     
     # 显示静态窗口
     def show(self,delay_time=0):
         if delay_time>0:
             CLOCK.tick(self.fps)
             for event in pygame.event.get():
                 if event.type == pygame.QUIT:
```

### Comparing `HelloPyOnly-0.1.23/onlydemos/LoongPy.py` & `HelloPyOnly-0.1.24/onlydemos/LoongPy.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.23/onlydemos/__init__.py` & `HelloPyOnly-0.1.24/onlydemos/__init__.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.23/onlydemos/pumpkin.py` & `HelloPyOnly-0.1.24/onlydemos/pumpkin.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.23/setup.py` & `HelloPyOnly-0.1.24/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='HelloPyOnly',  # 您的库的名称
-    version='0.1.23',  # 版本号
+    version='0.1.24',  # 版本号
     author='funk.zhang',  # 您的名字
     author_email='zhangfangid@126.com',  # 您的电子邮件地址
     description='This is the game engine of Only Hello Science project.',  # 您库的简短描述
     long_description='This is the game engine of Only Hello Science project. Based on pygame.',  # 更详细的描述
     # long_description_content_type='text/markdown',  # 描述类型（通常为Markdown）
     url='https://github.com/zfan0311/hellopy.git',  # 您库的代码托管URL
     packages=find_packages(),  # 包含的Python包
```

