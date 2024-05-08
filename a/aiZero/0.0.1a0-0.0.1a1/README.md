# Comparing `tmp/aiZero-0.0.1a0.tar.gz` & `tmp/aiZero-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiZero-0.0.1a0.tar", last modified: Tue May  7 07:25:13 2024, max compression
+gzip compressed data, was "aiZero-0.0.1a1.tar", last modified: Tue May  7 07:27:53 2024, max compression
```

## Comparing `aiZero-0.0.1a0.tar` & `aiZero-0.0.1a1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-07 07:25:13.249837 aiZero-0.0.1a0/
--rw-r--r--   0 emhang     (501) staff       (20)       71 2024-05-07 05:21:12.000000 aiZero-0.0.1a0/MANIFEST.in
--rw-r--r--   0 emhang     (501) staff       (20)     9593 2024-05-07 07:25:13.249691 aiZero-0.0.1a0/PKG-INFO
--rw-r--r--   0 emhang     (501) staff       (20)     9046 2024-05-07 07:23:23.000000 aiZero-0.0.1a0/README.md
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-07 07:25:13.246055 aiZero-0.0.1a0/aiZero/
--rw-r--r--   0 emhang     (501) staff       (20)    18346 2024-05-07 07:22:32.000000 aiZero-0.0.1a0/aiZero/__init__.py
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-07 07:25:13.245461 aiZero-0.0.1a0/aiZero/static/
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-07 07:25:13.247211 aiZero-0.0.1a0/aiZero/static/audios/
--rw-r--r--   0 emhang     (501) staff       (20)   276040 2024-05-07 07:22:42.000000 aiZero-0.0.1a0/aiZero/static/audios/1a32d899-90f3-46e7-a26c-7a744b1516a7.wav
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-07 07:25:13.248530 aiZero-0.0.1a0/aiZero/static/js/
--rw-r--r--   0 emhang     (501) staff       (20)    35418 2024-04-10 09:16:03.000000 aiZero-0.0.1a0/aiZero/static/js/marked.min.js
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-07 07:25:13.249174 aiZero-0.0.1a0/aiZero/templates/
--rw-r--r--   0 emhang     (501) staff       (20)    28097 2024-04-17 06:07:29.000000 aiZero-0.0.1a0/aiZero/templates/index.html
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-07 07:25:13.247073 aiZero-0.0.1a0/aiZero.egg-info/
--rw-r--r--   0 emhang     (501) staff       (20)     9593 2024-05-07 07:25:13.000000 aiZero-0.0.1a0/aiZero.egg-info/PKG-INFO
--rw-r--r--   0 emhang     (501) staff       (20)      319 2024-05-07 07:25:13.000000 aiZero-0.0.1a0/aiZero.egg-info/SOURCES.txt
--rw-r--r--   0 emhang     (501) staff       (20)        1 2024-05-07 07:25:13.000000 aiZero-0.0.1a0/aiZero.egg-info/dependency_links.txt
--rw-r--r--   0 emhang     (501) staff       (20)       48 2024-05-07 07:25:13.000000 aiZero-0.0.1a0/aiZero.egg-info/requires.txt
--rw-r--r--   0 emhang     (501) staff       (20)        7 2024-05-07 07:25:13.000000 aiZero-0.0.1a0/aiZero.egg-info/top_level.txt
--rw-r--r--   0 emhang     (501) staff       (20)       38 2024-05-07 07:25:13.249884 aiZero-0.0.1a0/setup.cfg
--rw-r--r--   0 emhang     (501) staff       (20)      827 2024-05-07 05:20:32.000000 aiZero-0.0.1a0/setup.py
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-07 07:27:53.611857 aiZero-0.0.1a1/
+-rw-r--r--   0 emhang     (501) staff       (20)       71 2024-05-07 05:21:12.000000 aiZero-0.0.1a1/MANIFEST.in
+-rw-r--r--   0 emhang     (501) staff       (20)     9594 2024-05-07 07:27:53.611724 aiZero-0.0.1a1/PKG-INFO
+-rw-r--r--   0 emhang     (501) staff       (20)     9047 2024-05-07 07:27:48.000000 aiZero-0.0.1a1/README.md
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-07 07:27:53.607744 aiZero-0.0.1a1/aiZero/
+-rw-r--r--   0 emhang     (501) staff       (20)    18346 2024-05-07 07:22:32.000000 aiZero-0.0.1a1/aiZero/__init__.py
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-07 07:27:53.607065 aiZero-0.0.1a1/aiZero/static/
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-07 07:27:53.608868 aiZero-0.0.1a1/aiZero/static/audios/
+-rw-r--r--   0 emhang     (501) staff       (20)   276040 2024-05-07 07:22:42.000000 aiZero-0.0.1a1/aiZero/static/audios/1a32d899-90f3-46e7-a26c-7a744b1516a7.wav
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-07 07:27:53.610754 aiZero-0.0.1a1/aiZero/static/js/
+-rw-r--r--   0 emhang     (501) staff       (20)    35418 2024-04-10 09:16:03.000000 aiZero-0.0.1a1/aiZero/static/js/marked.min.js
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-07 07:27:53.611287 aiZero-0.0.1a1/aiZero/templates/
+-rw-r--r--   0 emhang     (501) staff       (20)    28097 2024-04-17 06:07:29.000000 aiZero-0.0.1a1/aiZero/templates/index.html
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-07 07:27:53.608721 aiZero-0.0.1a1/aiZero.egg-info/
+-rw-r--r--   0 emhang     (501) staff       (20)     9594 2024-05-07 07:27:53.000000 aiZero-0.0.1a1/aiZero.egg-info/PKG-INFO
+-rw-r--r--   0 emhang     (501) staff       (20)      319 2024-05-07 07:27:53.000000 aiZero-0.0.1a1/aiZero.egg-info/SOURCES.txt
+-rw-r--r--   0 emhang     (501) staff       (20)        1 2024-05-07 07:27:53.000000 aiZero-0.0.1a1/aiZero.egg-info/dependency_links.txt
+-rw-r--r--   0 emhang     (501) staff       (20)       48 2024-05-07 07:27:53.000000 aiZero-0.0.1a1/aiZero.egg-info/requires.txt
+-rw-r--r--   0 emhang     (501) staff       (20)        7 2024-05-07 07:27:53.000000 aiZero-0.0.1a1/aiZero.egg-info/top_level.txt
+-rw-r--r--   0 emhang     (501) staff       (20)       38 2024-05-07 07:27:53.611906 aiZero-0.0.1a1/setup.cfg
+-rw-r--r--   0 emhang     (501) staff       (20)      828 2024-05-07 07:27:34.000000 aiZero-0.0.1a1/setup.py
```

### Comparing `aiZero-0.0.1a0/PKG-INFO` & `aiZero-0.0.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiZero
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: A simple and easy-to-use library that connects to common artificial intelligence interfaces, allowing for quick development of local web applications. It includes mainstream AI capabilities such as LLM text interaction, image understanding, audio understanding, image generation, speech recognition, and speech synthesis.
 Home-page: UNKNOWN
 Author: emhang
 Author-email: emhang@126.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -24,15 +24,15 @@
 app = AIWebApp(title='人工智能助手')    # 初始化web应用
 app.set_apikey('YOUR_API_KEY')    # 设定AI接口的api key
 app.add_input_text()    # 在页面中添加一个输入文本框
 app.add_submit(my_ai_function)    # 添加一个提交按钮，点击后执行函数
 app.run(port=6060)    # 启动应用，设定端口，默认为5000
 ```
 
-启动后，你将可以在浏览器中访问http://127.0.0.1:6060/查看搭建好的web应用。
+启动后，你将可以在浏览器中访问http://127.0.0.1:6060/ 查看搭建好的web应用。
 
 如果需要实现AI功能的可视化呈现，你只需要将`'YOUR_API_KEY'`替换为真实的api key，并完善`my_ai_function`函数即可。
 
 ### AI功能实现例子
 
 #### 大模型文字交互
```

### Comparing `aiZero-0.0.1a0/README.md` & `aiZero-0.0.1a1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 app = AIWebApp(title='人工智能助手')    # 初始化web应用
 app.set_apikey('YOUR_API_KEY')    # 设定AI接口的api key
 app.add_input_text()    # 在页面中添加一个输入文本框
 app.add_submit(my_ai_function)    # 添加一个提交按钮，点击后执行函数
 app.run(port=6060)    # 启动应用，设定端口，默认为5000
 ```
 
-启动后，你将可以在浏览器中访问http://127.0.0.1:6060/查看搭建好的web应用。
+启动后，你将可以在浏览器中访问http://127.0.0.1:6060/ 查看搭建好的web应用。
 
 如果需要实现AI功能的可视化呈现，你只需要将`'YOUR_API_KEY'`替换为真实的api key，并完善`my_ai_function`函数即可。
 
 ### AI功能实现例子
 
 #### 大模型文字交互
```

### Comparing `aiZero-0.0.1a0/aiZero/__init__.py` & `aiZero-0.0.1a1/aiZero/__init__.py`

 * *Files identical despite different names*

### Comparing `aiZero-0.0.1a0/aiZero/static/audios/1a32d899-90f3-46e7-a26c-7a744b1516a7.wav` & `aiZero-0.0.1a1/aiZero/static/audios/1a32d899-90f3-46e7-a26c-7a744b1516a7.wav`

 * *Files identical despite different names*

### Comparing `aiZero-0.0.1a0/aiZero/static/js/marked.min.js` & `aiZero-0.0.1a1/aiZero/static/js/marked.min.js`

 * *Files identical despite different names*

### Comparing `aiZero-0.0.1a0/aiZero/templates/index.html` & `aiZero-0.0.1a1/aiZero/templates/index.html`

 * *Files identical despite different names*

### Comparing `aiZero-0.0.1a0/aiZero.egg-info/PKG-INFO` & `aiZero-0.0.1a1/aiZero.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiZero
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: A simple and easy-to-use library that connects to common artificial intelligence interfaces, allowing for quick development of local web applications. It includes mainstream AI capabilities such as LLM text interaction, image understanding, audio understanding, image generation, speech recognition, and speech synthesis.
 Home-page: UNKNOWN
 Author: emhang
 Author-email: emhang@126.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -24,15 +24,15 @@
 app = AIWebApp(title='人工智能助手')    # 初始化web应用
 app.set_apikey('YOUR_API_KEY')    # 设定AI接口的api key
 app.add_input_text()    # 在页面中添加一个输入文本框
 app.add_submit(my_ai_function)    # 添加一个提交按钮，点击后执行函数
 app.run(port=6060)    # 启动应用，设定端口，默认为5000
 ```
 
-启动后，你将可以在浏览器中访问http://127.0.0.1:6060/查看搭建好的web应用。
+启动后，你将可以在浏览器中访问http://127.0.0.1:6060/ 查看搭建好的web应用。
 
 如果需要实现AI功能的可视化呈现，你只需要将`'YOUR_API_KEY'`替换为真实的api key，并完善`my_ai_function`函数即可。
 
 ### AI功能实现例子
 
 #### 大模型文字交互
```

### Comparing `aiZero-0.0.1a0/setup.py` & `aiZero-0.0.1a1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="aiZero",
-    version="0.0.1a",
+    version="0.0.1a1",
     author="emhang",
     author_email="emhang@126.com",
     description="A simple and easy-to-use library that connects to common artificial intelligence interfaces, "
                 "allowing for quick development of local web applications. "
                 "It includes mainstream AI capabilities such as LLM text interaction, image understanding, audio understanding, image generation, speech recognition, and speech synthesis.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

