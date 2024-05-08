# Comparing `tmp/th-influx-sdk-1.0.7.tar.gz` & `tmp/th-influx-sdk-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "th-influx-sdk-1.0.7.tar", last modified: Mon Apr 29 07:34:20 2024, max compression
+gzip compressed data, was "th-influx-sdk-1.0.8.tar", last modified: Wed May  8 07:22:15 2024, max compression
```

## Comparing `th-influx-sdk-1.0.7.tar` & `th-influx-sdk-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 07:34:20.821048 th-influx-sdk-1.0.7/
--rw-rw-rw-   0        0        0      300 2024-04-29 07:34:20.820050 th-influx-sdk-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       39 2024-04-19 06:33:19.000000 th-influx-sdk-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 07:34:20.810040 th-influx-sdk-1.0.7/ThInfluxSDK/
--rw-rw-rw-   0        0        0       25 2024-04-19 05:50:15.000000 th-influx-sdk-1.0.7/ThInfluxSDK/__init__.py
--rw-rw-rw-   0        0        0    18677 2024-04-29 07:33:24.000000 th-influx-sdk-1.0.7/ThInfluxSDK/influxSDK.py
--rw-rw-rw-   0        0        0       42 2024-04-29 07:34:20.821048 th-influx-sdk-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      553 2024-04-29 07:33:49.000000 th-influx-sdk-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:34:20.818055 th-influx-sdk-1.0.7/th_influx_sdk.egg-info/
--rw-rw-rw-   0        0        0      300 2024-04-29 07:34:20.000000 th-influx-sdk-1.0.7/th_influx_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-04-29 07:34:20.000000 th-influx-sdk-1.0.7/th_influx_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 07:34:20.000000 th-influx-sdk-1.0.7/th_influx_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-29 07:34:20.000000 th-influx-sdk-1.0.7/th_influx_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-29 07:34:20.000000 th-influx-sdk-1.0.7/th_influx_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 07:22:15.685640 th-influx-sdk-1.0.8/
+-rw-rw-rw-   0        0        0      300 2024-05-08 07:22:15.682648 th-influx-sdk-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       39 2024-04-19 06:33:19.000000 th-influx-sdk-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 07:22:15.666731 th-influx-sdk-1.0.8/ThInfluxSDK/
+-rw-rw-rw-   0        0        0       25 2024-04-19 05:50:15.000000 th-influx-sdk-1.0.8/ThInfluxSDK/__init__.py
+-rw-rw-rw-   0        0        0    22653 2024-05-08 03:42:11.000000 th-influx-sdk-1.0.8/ThInfluxSDK/influxSDK.py
+-rw-rw-rw-   0        0        0       42 2024-05-08 07:22:15.685640 th-influx-sdk-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      553 2024-05-08 07:21:10.000000 th-influx-sdk-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:22:15.679654 th-influx-sdk-1.0.8/th_influx_sdk.egg-info/
+-rw-rw-rw-   0        0        0      300 2024-05-08 07:22:15.000000 th-influx-sdk-1.0.8/th_influx_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-05-08 07:22:15.000000 th-influx-sdk-1.0.8/th_influx_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 07:22:15.000000 th-influx-sdk-1.0.8/th_influx_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-08 07:22:15.000000 th-influx-sdk-1.0.8/th_influx_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-08 07:22:15.000000 th-influx-sdk-1.0.8/th_influx_sdk.egg-info/top_level.txt
```

### Comparing `th-influx-sdk-1.0.7/ThInfluxSDK/influxSDK.py` & `th-influx-sdk-1.0.8/ThInfluxSDK/influxSDK.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from dateutil.tz import tzutc
 from collections import OrderedDict
 from itertools import groupby
 from operator import itemgetter
 import csv
 import json
 from typing import Optional
+import pytz
 
 
 def get_influx_db_connection(host, port, username, password, timeout):
     """
     获取InfluxDB连接，使用完必须使用close()关闭。
 
     :param host: 数据库连接地址ip，必填参数
@@ -128,37 +129,53 @@
     # 将UTC时间转换为北京时间（东八区）
     beijing_aware = utc_aware + timedelta(hours=8)
     # 格式化时间为指定格式
     beijing_time_str = beijing_aware.strftime('%Y-%m-%d %H:%M:%S')
     return beijing_time_str
 
 
+def convert_beijing_time_to_utc(beijing_time_str):
+    # 解析北京时间字符串
+    beijing_time = datetime.strptime(beijing_time_str, "%Y-%m-%d %H:%M:%S")
+    # 设置北京时区
+    beijing_tz = pytz.timezone('Asia/Shanghai')
+    # 将北京时间转换为带有时区的datetime对象
+    beijing_datetime = beijing_tz.localize(beijing_time)
+    # 转换为UTC时间
+    utc_datetime = beijing_datetime.astimezone(pytz.UTC)
+    # 转换为ISO 8601格式（包含Z结尾）
+    utc_time_str = utc_datetime.isoformat().replace('+00:00', 'Z')
+
+    return utc_time_str
+
+
 def get_new_set_data(database: str, tableName: str, pointList: List[str],
                      influxDB: InfluxDBClient, queryTime: Optional[str] = None) -> str:
     """
         查询最新的测点数据或查询某个时刻的测点数据（需时间对齐）。
 
         Args:
             database (str): 数据库名。必填参数
             tableName (str): 表名。必填参数
             queryTime (str, optional): 查询时刻。默认值为None，表示查询最新时间。
-                格式要求：'YYYY-MM-DDTHH:MM:SSZ'。
+                格式要求：'YYYY-MM-DD HH:mm:ss'。
             pointList (list[str]): 一个或多个点号。必填参数，表示查询所有点。
             influxDB (InfluxDBClient): 数据库连接对象。必填参数，表示使用默认连接。
 
         Returns:
             Any: 查询结果，具体类型取决于查询内容和返回的数据结构。
 
         说明：
             本函数可同时满足以下四个场景要求：
             1. 获取一个点的最新值。
             2. 获取一个点在特定时刻的值。
             3. 获取多个点的最新值。
             4. 获取多个点在特定时刻的值。
         """
+    queryTime = convert_beijing_time_to_utc(queryTime)
     # 1. 初始化 resultList
     resultList = []
     # 2. 使用join方法将pointList中的字符串用'|'连接起来
     pointStr = '|'.join(pointList)
     # 3. 构建SQL查询字符串
     SQLForMaxTime = f"SELECT LAST(VALUE), UUID FROM {tableName} WHERE UUID =~ /^{pointStr}$/"
 
@@ -286,14 +303,83 @@
         pointList (list of str): 一个或多个点号列表，必填参数，表示查询所有点。
         interval (int, optional): 时间间隔（单位秒），默认为None，表示不使用间隔查询。
         influxDB (InfluxDBClient): InfluxDB连接对象，必填参数，表示使用默认连接。
 
     Returns:
         dict: 包含查询结果的字典，具体结构根据实际应用情况确定。
     """
+    startTime = convert_beijing_time_to_utc(startTime)
+    endTime = convert_beijing_time_to_utc(endTime)
+    # 构建点号字符串
+    point_str = '|'.join(pointList)
+
+    # 构建查询语句
+    query = f"SELECT LAST(VALUE), UUID FROM {tableName} WHERE UUID =~ /^{point_str}$/ AND time>='{startTime}' AND time<='{endTime}' GROUP BY UUID, time({interval}s) FILL(previous) "
+
+    # 执行查询
+    result = influxDB.query(query, database=database)
+
+    # 获取数据映射，这里需要相应的Python实现
+    map_data = get_new_data_map(database, tableName, startTime, pointList, influxDB)
+
+    timeList = get_time_list(utc_get_time(startTime), utc_get_time(endTime), interval)
+
+    result_value_map = OrderedDict()
+    for series in result.raw['series']:
+        result_value_map[series['tags']['UUID']] = series['values']
+
+    map_record = OrderedDict()
+    sb = '['
+    index = 0
+    for time_stamp in timeList:
+        map_record['time'] = time_stamp  # 添加时间戳
+        for point in pointList:
+            values_list = result_value_map.get(point)
+            if values_list and values_list[index][1]:
+                # 假设 values_list 是一个包含时间戳和值的元组列表
+                map_record[point] = values_list[index][1]
+            elif point in map_data:
+                map_record[point] = map_data[point]
+            else:
+                map_record[point] = ''
+
+        if index >= 1:
+            sb += ','
+        sb += json.dumps(map_record)
+        index += 1
+    sb += ']'
+
+    return sb
+
+
+def get_his_set_data_by_complete_FQ(database: str, tableName: str, startTime: str, endTime: str, pointList: List[str],
+                                 influxDB: InfluxDBClient, interval: Optional[int] = None):
+    """
+    查询历史时间段一个或多个测点数据（进行数据补齐）
+
+    可同时满足下面4个场景要求：
+    1、获取一个[点]的[开始，结束]段的历史数据;
+    2、获取一个[点]的[开始，结束]段的[间隔秒]的历史数据;
+    3、获取多个[点...] 的[开始，结束] 段的历史数据;
+    4、获取多个[点...] 的[开始，结束] 段的[间隔秒] 的历史数据;
+
+    Args:
+        database (str): 数据库名，必填参数
+        tableName (str): 表名，必填参数
+        startTime (str): 开始时间，必填参数，表示使用当前时间。格式应为ISO 8601。
+        endTime (str): 结束时间，必填参数，表示使用当前时间。格式应为ISO 8601。
+        pointList (list of str): 一个或多个点号列表，必填参数，表示查询所有点。
+        interval (int, optional): 时间间隔（单位秒），默认为None，表示不使用间隔查询。
+        influxDB (InfluxDBClient): InfluxDB连接对象，必填参数，表示使用默认连接。
+
+    Returns:
+        dict: 包含查询结果的字典，具体结构根据实际应用情况确定。
+    """
+    startTime = convert_beijing_time_to_utc(startTime)
+    endTime = convert_beijing_time_to_utc(endTime)
     # 构建点号字符串
     point_str = '|'.join(pointList)
 
     # 构建查询语句
     query = f"SELECT LAST(VALUE), UUID FROM {tableName} WHERE UUID =~ /^{point_str}$/ AND time>='{startTime}' AND time<='{endTime}' GROUP BY UUID, time({interval}s) FILL(previous) "
 
     # 执行查询
@@ -353,23 +439,25 @@
                      pointList: List[str], influxDB: InfluxDBClient) -> str:
     """
     查询历史一个或多个测点数据（不进行数据补齐）
 
     Args:
         database (str): 数据库名，必填参数
         tableName (str): 表名，必填参数
-        startTime (str): 开始时间，必填参数(格式要求："2023-12-27T13:42:00Z")
-        endTime (str): 结束时间，必填参数(格式要求："2023-12-27T13:42:00Z")
+        startTime (str): 开始时间，必填参数(格式要求："2023-12-27 13:42:00")
+        endTime (str): 结束时间，必填参数(格式要求："2023-12-27 13:42:00")
         pointList (List[str]): 一个或多个点号，必填参数
         influxDB (InfluxDBClient): 数据库连接，必填参数
 
     Returns:
         str: 查询结果
 
     """
+    startTime = convert_beijing_time_to_utc(startTime)
+    endTime = convert_beijing_time_to_utc(endTime)
     # 将点号列表转换为str
     pointStr = '|'.join(pointList)
 
     # 构建查询语句
     query = f"SELECT time,VALUE, UUID FROM {tableName} WHERE UUID =~ /{pointStr}/ AND time>='{startTime}' AND time<='{endTime}' "
 
     # 执行查询
@@ -400,21 +488,23 @@
     2、获取一个点的[开始，结束]段的[间隔秒]的历史数据;
     3、获取多个点...的[开始，结束]段的历史数据;
     4、获取多个点...的[开始，结束]段的[间隔秒]的历史数据;
 
     Args:
         database (str): 数据库名，必填参数
         tableName (str): 表名，必填参数 (在InfluxDB中通常是measurement名)
-        startTime (str): 开始时间，必填参数(格式要求："YYYY-MM-DDTHH:mm:ssZ")
-        endTime (str): 结束时间，必填参数(格式要求："YYYY-MM-DDTHH:mm:ssZ")
+        startTime (str): 开始时间，必填参数(格式要求："YYYY-MM-DD HH:mm:ss")
+        endTime (str): 结束时间，必填参数(格式要求："YYYY-MM-DD HH:mm:ss")
         pointList (List[str]): 一个或多个点号（测点标识），必填参数
         interval (int): 时间间隔（单位秒），必填参数
         influxDB (InfluxDBClient): InfluxDB客户端连接，必填参数
         filePath (str): 文件路径，必填参数，例如："D:\\temp\\202401.csv" 或 "/opt/202401.csv"
     """
+    startTime = convert_beijing_time_to_utc(startTime)
+    endTime = convert_beijing_time_to_utc(endTime)
     # 打开文件以写入CSV数据
     with open(filePath, mode='w', newline='') as file:
         csv_writer = csv.writer(file)
         # 写头信息（测点点号）
         title_list = ['timestamp']
         for point in pointList:
             title_list.append(point)
```

### Comparing `th-influx-sdk-1.0.7/setup.py` & `th-influx-sdk-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
 setup(
     name='th-influx-sdk',
-    version='1.0.7',
+    version='1.0.8',
     description='A SDK for influxDb',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='xiongyi',
     author_email='15679191752@163.com',
     packages=find_packages(),
     install_requires=[
```

