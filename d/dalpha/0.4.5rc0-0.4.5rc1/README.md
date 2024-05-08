# Comparing `tmp/dalpha-0.4.5rc0.tar.gz` & `tmp/dalpha-0.4.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha-0.4.5rc0.tar", max compression
+gzip compressed data, was "dalpha-0.4.5rc1.tar", max compression
```

## Comparing `dalpha-0.4.5rc0.tar` & `dalpha-0.4.5rc1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.4.5rc0/README.md
--rw-r--r--   0        0        0     1862 2024-05-02 07:23:00.795089 dalpha-0.4.5rc0/dalpha/__init__.py
--rw-r--r--   0        0        0    29060 2024-05-02 07:23:00.795089 dalpha-0.4.5rc0/dalpha/agent.py
--rw-r--r--   0        0        0      548 2024-04-19 16:22:01.493908 dalpha-0.4.5rc0/dalpha/cobra_cls.py
--rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.4.5rc0/dalpha/context.py
--rw-r--r--   0        0        0     3036 2024-05-02 07:23:00.795089 dalpha-0.4.5rc0/dalpha/data_update_cls.py
--rw-r--r--   0        0        0      940 2024-05-02 07:23:00.795089 dalpha-0.4.5rc0/dalpha/dto.py
--rw-r--r--   0        0        0      521 2024-05-02 07:23:00.795089 dalpha-0.4.5rc0/dalpha/exception.py
--rw-r--r--   0        0        0     6098 2024-05-02 07:23:00.795089 dalpha-0.4.5rc0/dalpha/inference_cls.py
--rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.4.5rc0/dalpha/kafka_cli.py
--rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.4.5rc0/dalpha/logging/__init__.py
--rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.4.5rc0/dalpha/logging/events.py
--rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.4.5rc0/dalpha/logging/log_formatter.py
--rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.4.5rc0/dalpha/logging/utils.py
--rw-r--r--   0        0        0     1702 2024-05-02 07:23:00.795089 dalpha-0.4.5rc0/dalpha/openai_cls.py
--rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.4.5rc0/dalpha/redis_cli.py
--rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.4.5rc0/dalpha/redis_cls.py
--rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.4.5rc0/dalpha/signal_handler.py
--rw-r--r--   0        0        0      881 2024-05-02 07:23:00.795089 dalpha-0.4.5rc0/pyproject.toml
--rw-r--r--   0        0        0     1321 1970-01-01 00:00:00.000000 dalpha-0.4.5rc0/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.4.5rc1/README.md
+-rw-r--r--   0        0        0     1862 2024-05-02 07:23:00.795089 dalpha-0.4.5rc1/dalpha/__init__.py
+-rw-r--r--   0        0        0    28968 2024-05-08 06:25:10.211719 dalpha-0.4.5rc1/dalpha/agent.py
+-rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.4.5rc1/dalpha/cobra_cls.py
+-rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.4.5rc1/dalpha/context.py
+-rw-r--r--   0        0        0     3036 2024-05-02 07:23:00.795089 dalpha-0.4.5rc1/dalpha/data_update_cls.py
+-rw-r--r--   0        0        0      940 2024-05-02 07:23:00.795089 dalpha-0.4.5rc1/dalpha/dto.py
+-rw-r--r--   0        0        0      521 2024-05-02 07:23:00.795089 dalpha-0.4.5rc1/dalpha/exception.py
+-rw-r--r--   0        0        0     6098 2024-05-02 07:23:00.795089 dalpha-0.4.5rc1/dalpha/inference_cls.py
+-rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.4.5rc1/dalpha/kafka_cli.py
+-rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.4.5rc1/dalpha/logging/__init__.py
+-rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.4.5rc1/dalpha/logging/events.py
+-rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.4.5rc1/dalpha/logging/log_formatter.py
+-rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.4.5rc1/dalpha/logging/utils.py
+-rw-r--r--   0        0        0     1702 2024-05-02 07:23:00.795089 dalpha-0.4.5rc1/dalpha/openai_cls.py
+-rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.4.5rc1/dalpha/redis_cli.py
+-rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.4.5rc1/dalpha/redis_cls.py
+-rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.4.5rc1/dalpha/signal_handler.py
+-rw-r--r--   0        0        0      881 2024-05-08 06:25:10.211719 dalpha-0.4.5rc1/pyproject.toml
+-rw-r--r--   0        0        0     1321 1970-01-01 00:00:00.000000 dalpha-0.4.5rc1/PKG-INFO
```

### Comparing `dalpha-0.4.5rc0/README.md` & `dalpha-0.4.5rc1/README.md`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.5rc0/dalpha/__init__.py` & `dalpha-0.4.5rc1/dalpha/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.5rc0/dalpha/agent.py` & `dalpha-0.4.5rc1/dalpha/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,15 +265,14 @@
                 self.poll_time = time.time()
                 return ret
 
         elif self.use_sqs:
             response = self.sqs.receive_message(
                 QueueUrl = self.queue_url,
                 MaxNumberOfMessages = max_number_of_messages,  # 가져올 메시지의 최대 수 (1개 이상 설정 가능)
-                WaitTimeSeconds = 0       # 긴 폴링을 위한 대기 시간 (초 단위)
             )
             ret = []
             messages = response.get('Messages', [])
             for message in messages:
                 message_body = message['Body']
                 try:
                     # message_body를 딕셔너리로 변환
```

### Comparing `dalpha-0.4.5rc0/dalpha/cobra_cls.py` & `dalpha-0.4.5rc1/dalpha/cobra_cls.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,10 +10,10 @@
         pass
 
     def __call__(self, func_or_cls):
         # 이 데코레이터는 함수나 클래스를 그대로 반환합니다.
         return func_or_cls
     
     @classmethod
-    def block(cls, label):
+    def block(cls, label = None):
         # 새 인스턴스를 생성하고, 이 인스턴스는 __call__을 통해 함수나 클래스를 그대로 반환합니다.
         return cls(label)
```

### Comparing `dalpha-0.4.5rc0/dalpha/context.py` & `dalpha-0.4.5rc1/dalpha/context.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.5rc0/dalpha/data_update_cls.py` & `dalpha-0.4.5rc1/dalpha/data_update_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.5rc0/dalpha/dto.py` & `dalpha-0.4.5rc1/dalpha/dto.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.5rc0/dalpha/exception.py` & `dalpha-0.4.5rc1/dalpha/exception.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.5rc0/dalpha/inference_cls.py` & `dalpha-0.4.5rc1/dalpha/inference_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.5rc0/dalpha/logging/__init__.py` & `dalpha-0.4.5rc1/dalpha/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.5rc0/dalpha/logging/log_formatter.py` & `dalpha-0.4.5rc1/dalpha/logging/log_formatter.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.5rc0/dalpha/logging/utils.py` & `dalpha-0.4.5rc1/dalpha/logging/utils.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.5rc0/dalpha/openai_cls.py` & `dalpha-0.4.5rc1/dalpha/openai_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.5rc0/dalpha/redis_cli.py` & `dalpha-0.4.5rc1/dalpha/redis_cli.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.5rc0/dalpha/redis_cls.py` & `dalpha-0.4.5rc1/dalpha/redis_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.5rc0/pyproject.toml` & `dalpha-0.4.5rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dalpha"
-version = "0.4.5rc0"
+version = "0.4.5rc1"
 description = ""
 authors = ["devops <devops@dalpha.so>"]
 readme = "README.md"
 packages = [{include = "dalpha"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -16,15 +16,15 @@
 kafka-python = "^2.0.2"
 
 [tool.poetry.group.dev.dependencies]
 twine = "^4.0.2"
 
 [project]
 name = "dalpha"
-version = "0.4.5rc0"
+version = "0.4.5rc1"
 authors = [
   { name="Beomseok", email="beomseok.kim@dalpha.so" },
 ]
 description = "Dalpha internal sdk"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `dalpha-0.4.5rc0/PKG-INFO` & `dalpha-0.4.5rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalpha
-Version: 0.4.5rc0
+Version: 0.4.5rc1
 Summary: 
 Author: devops
 Author-email: devops@dalpha.so
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

