# Comparing `tmp/zzd-cli-0.2.0.tar.gz` & `tmp/zzd-cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zzd-cli-0.2.0.tar", last modified: Mon Apr 29 07:29:39 2024, max compression
+gzip compressed data, was "zzd-cli-0.3.0.tar", last modified: Wed May  8 08:15:48 2024, max compression
```

## Comparing `zzd-cli-0.2.0.tar` & `zzd-cli-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 qinyiqi    (501) staff       (20)        0 2024-04-29 07:29:39.071671 zzd-cli-0.2.0/
--rw-r--r--   0 qinyiqi    (501) staff       (20)      210 2024-04-29 07:29:39.071581 zzd-cli-0.2.0/PKG-INFO
--rw-r--r--   0 qinyiqi    (501) staff       (20)     3508 2024-03-08 10:29:30.000000 zzd-cli-0.2.0/README.md
--rw-r--r--   0 qinyiqi    (501) staff       (20)       38 2024-04-29 07:29:39.071702 zzd-cli-0.2.0/setup.cfg
--rw-r--r--   0 qinyiqi    (501) staff       (20)      496 2024-04-29 07:29:31.000000 zzd-cli-0.2.0/setup.py
-drwxr-xr-x   0 qinyiqi    (501) staff       (20)        0 2024-04-29 07:29:39.070878 zzd-cli-0.2.0/zzd/
--rw-r--r--   0 qinyiqi    (501) staff       (20)        0 2024-02-24 09:26:56.000000 zzd-cli-0.2.0/zzd/__init__.py
--rw-r--r--   0 qinyiqi    (501) staff       (20)    37655 2024-04-29 07:21:06.000000 zzd-cli-0.2.0/zzd/cli.py
-drwxr-xr-x   0 qinyiqi    (501) staff       (20)        0 2024-04-29 07:29:39.071466 zzd-cli-0.2.0/zzd_cli.egg-info/
--rw-r--r--   0 qinyiqi    (501) staff       (20)      210 2024-04-29 07:29:39.000000 zzd-cli-0.2.0/zzd_cli.egg-info/PKG-INFO
--rw-r--r--   0 qinyiqi    (501) staff       (20)      233 2024-04-29 07:29:39.000000 zzd-cli-0.2.0/zzd_cli.egg-info/SOURCES.txt
--rw-r--r--   0 qinyiqi    (501) staff       (20)        1 2024-04-29 07:29:39.000000 zzd-cli-0.2.0/zzd_cli.egg-info/dependency_links.txt
--rw-r--r--   0 qinyiqi    (501) staff       (20)       55 2024-04-29 07:29:39.000000 zzd-cli-0.2.0/zzd_cli.egg-info/entry_points.txt
--rw-r--r--   0 qinyiqi    (501) staff       (20)       55 2024-04-29 07:29:39.000000 zzd-cli-0.2.0/zzd_cli.egg-info/requires.txt
--rw-r--r--   0 qinyiqi    (501) staff       (20)        4 2024-04-29 07:29:39.000000 zzd-cli-0.2.0/zzd_cli.egg-info/top_level.txt
+drwxr-xr-x   0 qinyiqi    (501) staff       (20)        0 2024-05-08 08:15:48.664560 zzd-cli-0.3.0/
+-rw-r--r--   0 qinyiqi    (501) staff       (20)      210 2024-05-08 08:15:48.664472 zzd-cli-0.3.0/PKG-INFO
+-rw-r--r--   0 qinyiqi    (501) staff       (20)     3508 2024-03-08 10:29:30.000000 zzd-cli-0.3.0/README.md
+-rw-r--r--   0 qinyiqi    (501) staff       (20)       38 2024-05-08 08:15:48.664593 zzd-cli-0.3.0/setup.cfg
+-rw-r--r--   0 qinyiqi    (501) staff       (20)      496 2024-05-08 08:14:50.000000 zzd-cli-0.3.0/setup.py
+drwxr-xr-x   0 qinyiqi    (501) staff       (20)        0 2024-05-08 08:15:48.663781 zzd-cli-0.3.0/zzd/
+-rw-r--r--   0 qinyiqi    (501) staff       (20)        0 2024-02-24 09:26:56.000000 zzd-cli-0.3.0/zzd/__init__.py
+-rw-r--r--   0 qinyiqi    (501) staff       (20)    38326 2024-05-08 08:10:01.000000 zzd-cli-0.3.0/zzd/cli.py
+drwxr-xr-x   0 qinyiqi    (501) staff       (20)        0 2024-05-08 08:15:48.664356 zzd-cli-0.3.0/zzd_cli.egg-info/
+-rw-r--r--   0 qinyiqi    (501) staff       (20)      210 2024-05-08 08:15:48.000000 zzd-cli-0.3.0/zzd_cli.egg-info/PKG-INFO
+-rw-r--r--   0 qinyiqi    (501) staff       (20)      233 2024-05-08 08:15:48.000000 zzd-cli-0.3.0/zzd_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 qinyiqi    (501) staff       (20)        1 2024-05-08 08:15:48.000000 zzd-cli-0.3.0/zzd_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 qinyiqi    (501) staff       (20)       55 2024-05-08 08:15:48.000000 zzd-cli-0.3.0/zzd_cli.egg-info/entry_points.txt
+-rw-r--r--   0 qinyiqi    (501) staff       (20)       55 2024-05-08 08:15:48.000000 zzd-cli-0.3.0/zzd_cli.egg-info/requires.txt
+-rw-r--r--   0 qinyiqi    (501) staff       (20)        4 2024-05-08 08:15:48.000000 zzd-cli-0.3.0/zzd_cli.egg-info/top_level.txt
```

### Comparing `zzd-cli-0.2.0/README.md` & `zzd-cli-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `zzd-cli-0.2.0/zzd/cli.py` & `zzd-cli-0.3.0/zzd/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,40 @@
+# from pprint36 import pprint
+
 # built-in
 import os
 import re
 import base64
 
 import platform
 import socket
 
 import click
 import requests
 import json
 
 # third-party
-# from pprint36 import pprint
 import chardet
 from bs4 import BeautifulSoup
 
 # brew update && brew upgrade openssl
 # pip install urllib3==1.26.16
 
 
 # PATTERN = r'(?<!zzd.one:8000)(/media/)'
 # BASE = "http://zzd.one:8000/"
 # CODEBASE = "http://code.zzd.one:8000/"
 PATTERN = r'(?<!zzd.show)(/media/)'
 BASE = "https://zzd.show/"
 CODEBASE = "https://code.zzd.show/"
 
+DEBUG = True
+# DEBUG = False
+
+
 ENDPOINTS = {
     'web': 'users/cli/', 
     'tokenverify': 'users/cli/tokenverify/',
     'login': 'users/cli/login/',
     'list': 'shows/cli/list/',
     'clone': 'shows/cli/clone/',
     'info': 'shows/cli/info/',
@@ -104,47 +109,47 @@
     data_file_path = os.path.join(script_dir, 'data.json')
     token = None
     if os.path.isfile(data_file_path):
         try:
             data = json.loads(read_and_convert_to_utf8(data_file_path))
             token = data['token']
         except Exception as e:
-            # raise e
-            pass
+            if DEBUG:
+                raise e
     if not token:
         click.echo('您尚未登录，请先通过\nzzd login\n登录')
         return
     try:
         response = requests.post(ENDPOINTS['list'], data={
             'token': token, 
         })
         if response.status_code == 200:
             data = response.json()['data']
             click.echo(data)
         elif response.status_code == 402 and data['username']:
             click.echo(f'API冷却当中，我们暂时无法核验该操作。\n若您需要核验登录状态，请在30秒后重试')
             return
     except Exception as e:
-        # print(e)
-        # raise e   
+        if DEBUG:
+            raise e   
         click.echo("抱歉，您的网络不稳定或者服务器流量过大，请稍后重试")
         return
 
 
 @zzd.command(help="唯一参数，可以是一个序号或者一个链接")
 @click.argument('demo', type=str)
 def info(demo):
     """调取demo基本信息"""
     def extractPk(inp):
         try:
             if str(int(inp)) == str(inp):
                 return int(inp)
         except Exception as e:
-            # raise e
-            pass
+            if DEBUG:
+                raise e
         match = re.search(r'/(?P<int>\d+)', inp)
         if match:
             return int(match.group('int'))
         else:
             return None
 
     pk = extractPk(demo)
@@ -156,16 +161,16 @@
     data_file_path = os.path.join(script_dir, 'data.json')
     token = None
     if os.path.isfile(data_file_path):
         try:
             data = json.loads(read_and_convert_to_utf8(data_file_path))
             token = data['token']
         except Exception as e:
-            # raise e
-            pass
+            if DEBUG:
+                raise e
     if not token:
         click.echo('您尚未登录，请先通过\nzzd login\n登录')
         return
 
     """ error messages
     400 internal server error
     401 auth failed id or passcode
@@ -183,16 +188,16 @@
             click.echo(response.json()['data'])
             return
         elif response.status_code == 402:
             click.echo('API冷却当中，请过30秒再进行操作')
         else:
             click.echo('抱歉API调用失败，可能是登录密匙已过期')
     except Exception as e:
-        # print(e)
-        raise e
+        if DEBUG:
+            raise e
         click.echo("抱歉，您的网络不稳定或者服务器流量过大，请稍后重试")
         return
 
 
 @zzd.command()
 def login():
     """登录您的账号, 请前往官网查询id以及passcode"""
@@ -213,19 +218,19 @@
                 if response.status_code == 200:
                     still_working = True
                     username = response.json()['username']
                 elif response.status_code == 402 and data['username']:
                     click.echo(f'API冷却当中，我们暂时无法核验该操作。\n若您需要核验登录状态，请在30秒后重试')
                     return
             except Exception as e:
-                # raise e
-                pass
+                if DEBUG:
+                    raise e
         except Exception as e:
-            # print(e)
-            # raise e   
+            if DEBUG:
+                raise e
             click.echo("抱歉，您的网络不稳定或者服务器流量过大，请稍后重试")
             return
     if still_working and username:
         click.echo(f'您已以{username}登录, 若需要切换账号或者重新登录，请先使用\nzzd logout\n退出当前账号')
         return
     click.echo('登录您的账号, 使用id以及passcode')
     tut_site = ENDPOINTS['web']
@@ -259,21 +264,21 @@
                     json.dump({'token': data['msg'], 'username': username}, file)
                 click.echo(f"\n登陆成功，欢迎{username}\n您可以使用 \nzzd --help\n 查看命令帮助")
             else:
                 st = '抱歉登录失败，可能是由于API冷却中，可能是您的登录信息错误'
                 try:
                     st = data['msg']
                 except Exception as e:
-                    # raise e
-                    pass
+                    if DEBUG:
+                        raise e
                 click.echo(st)
                 return
     except Exception as e:
-        # print(e)
-        # raise e
+        if DEBUG:
+            raise e
         click.echo("抱歉，您的网络不稳定或者服务器流量过大，请稍后重试")
         return
 
 @zzd.command()
 def logout():
     """退出您的账号本地登录"""
     # Assuming you're using a token that needs to be invalidated
@@ -312,15 +317,15 @@
 
 # div{
 #     background: url('/media/portray/ksenia.jpg');
 # }
 # '''))
 # exit()
 
-def html_embrace(compiled: bool, cdndt, title, _html, css_refs, js_refs):
+def html_embrace(compiled: bool, cdndt, title, _html, css_refs, js_all):
     html = process_media_links(_html)
     css_blocks = '\n'
     js_blocks = '\n'
     if cdndt:
         cdn_css = cdndt.get('css')
         cdn_js = cdndt.get('js')
         if cdn_css:
@@ -337,21 +342,24 @@
         for i, href in enumerate(css_refs):
             href = '../' + href
             if compiled:
                 href = '../' + href
             css_blocks += f'<link rel="stylesheet" href="{href}" />'
             if i != len(css_refs) - 1:
                 css_blocks += '\n'
-    if js_refs:
-        for i, src in enumerate(js_refs):
-            src = '../' + src
+    if js_all:
+        for i, dt in enumerate(js_all):
+            src = '../' + dt['path']
             if compiled:
                 src = '../' + src
-            js_blocks += f'<script src="{src}"></script>'
-            if i != len(js_refs) - 1:
+            js_blocks += f'<script src="{src}"'
+            if dt.get('is_module', None):
+                js_blocks +=  ' type="module"'
+            js_blocks += '></script>'
+            if i != len(js_all) - 1:
                 js_blocks += '\n'
     if ('</head>' in html) and ('</body>' in html):
         sld = html.split('</head>')
         sld[0] += css_blocks
         t1 = '</head>'.join(sld)
 
         sld2 = t1.split('</body>')
@@ -417,16 +425,17 @@
     # click.echo(data)  
     # return
     if commit: os.makedirs(data['title'], exist_ok=True)
     dirpath = os.path.join(data['title'])
     # narrative
     writeLog(data, True)
     # file parse 
-    js_refs = []
     css_refs = []
+    js_refs = []
+    js_all = []
     for generic, ddt in data['textcode'].items():
         if generic == 'html': continue
         generic_dir = os.path.join(dirpath, generic)
         if commit: os.makedirs(generic_dir, exist_ok=True)
         for filename, dt in ddt.items():
             unplug = dt.get('unplug')
             raw = dt.get('raw')
@@ -446,22 +455,30 @@
                 _sld = compiled_path.split('/')
                 _sld.pop(0)
                 relative_path = '/'.join(_sld)
                 if generic == 'css':
                     css_refs.append(relative_path)
                 elif generic == 'js':
                     js_refs.append(relative_path)
+                    js_all.append({
+                        'path': relative_path,
+                        'is_module': dt.get('is_module', 0), 
+                    })
             else:
                 _sld = filepath.split('/')
                 _sld.pop(0)
                 relative_path = '/'.join(_sld)
                 if generic == 'css':
                     css_refs.append(relative_path)
                 elif generic == 'js':
                     js_refs.append(relative_path)
+                    js_all.append({
+                        'path': relative_path,
+                        'is_module': dt.get('is_module', 0), 
+                    })
             # print(generic, filename, unplug, raw, compiled)
     html = data['textcode'].get('html')
     if not html:
         html = {'index.html': {'raw': '', 'compiled': '', 'unplug': 0}}
     generic = 'html'
     generic_dir = os.path.join(dirpath, generic)
     if commit: os.makedirs(generic_dir, exist_ok=True)
@@ -473,20 +490,20 @@
         if compiled:
             compiled_dir = os.path.join(generic_dir, 'compiled')
             compiled_name = get_compiled_name(filename, generic)
             compiled_path = os.path.join(compiled_dir, compiled_name)
             if commit:
                     os.makedirs(compiled_dir, exist_ok=True)
                     with open(compiled_path, 'w', encoding="utf-8") as f:
-                        f.write(html_embrace(True, data['cdns'], data['title'], compiled, css_refs, js_refs))
+                        f.write(html_embrace(True, data['cdns'], data['title'], compiled, css_refs, js_all))
         if commit:
             with open(filepath, 'w', encoding="utf-8") as f:
                 if not compiled:
                     # html
-                    f.write(html_embrace(False, data['cdns'], data['title'], raw, css_refs, js_refs))
+                    f.write(html_embrace(False, data['cdns'], data['title'], raw, css_refs, js_all))
                 else:
                     # pug, etc (handled in previous condition, only compiled parsed)
                     f.write(process_media_links(raw))
 
 
 # exit()
 
@@ -495,16 +512,16 @@
 def clone(demo):
     """将demo复制到本地"""
     def extractPk(inp):
         try:
             if str(int(inp)) == str(inp):
                 return int(inp)
         except Exception as e:
-            # raise e
-            pass
+            if DEBUG:
+                raise e
         match = re.search(r'/(?P<int>\d+)', inp)
         if match:
             return int(match.group('int'))
         else:
             return None
 
     pk = extractPk(demo)
@@ -516,16 +533,16 @@
     data_file_path = os.path.join(script_dir, 'data.json')
     token = None
     if os.path.isfile(data_file_path):
         try:
             data = json.loads(read_and_convert_to_utf8(data_file_path))
             token = data['token']
         except Exception as e:
-            # raise e
-            pass
+            if DEBUG:
+                raise e
     if not token:
         click.echo('您尚未登录，请先通过\nzzd login\n登录')
         return
 
     """ error messages
     400 internal server error
     401 auth failed id or passcode
@@ -553,20 +570,20 @@
         elif response.status_code == 402:
             click.echo('API冷却当中，请过30秒再进行操作')
         else:
             msg = '抱歉API调用失败，可能是登录密匙已过期'
             try:
                 msg = response.json()['msg']
             except Exception as e:
-                # raise e
-                pass
+                if DEBUG:
+                    raise e
             click.echo(msg)
     except Exception as e:
-        # print(e)
-        # raise e
+        if DEBUG:
+            raise e
         click.echo("抱歉，您的网络不稳定或者服务器流量过大，请稍后重试")
         return
 
 @zzd.command()
 def push():
     # """将本地更改同步到服务器数据库"""
     # # inspect: dirs check
@@ -583,16 +600,16 @@
     data_file_path = os.path.join(script_dir, 'data.json')
     token = None
     if os.path.isfile(data_file_path):
         try:
             data = json.loads(read_and_convert_to_utf8(data_file_path))
             token = data['token']
         except Exception as e:
-            # raise e
-            pass
+            if DEBUG:
+                raise e
     if not token:
         click.echo('您尚未登录，请先通过\nzzd login\n登录')
         return
 
     # ===== inspect =====
     supported_exts = {
         'html': {
@@ -778,15 +795,16 @@
             headers = {'Authorization': f'Bearer {token}'}
             try:
                 response = requests.post(ENDPOINTS['static-upload'], headers=headers, data={
                     'action': 'force' if force else '', 
                     'overwrites': json.dumps(overwrites, ensure_ascii=False), 
                 }, files=files)
             except Exception as e:
-                # raise e
+                if DEBUG:
+                    raise e
                 click.echo("抱歉，您的网络不稳定或者服务器流量过大，请稍后重试")
                 exit()
             if response.status_code == 201:
                 # ok but has dups
                 dups = response.json()['dups']
                 # print(dups)
                 ignore_files = []
@@ -839,15 +857,16 @@
                     click.echo(msg)
                     # show feed back in api, where to go to fix the issue
                     link = mdt.get('link')
                     if link:
                         click.echo(f'请前往{link}\n查看解决方案')
                     exit()
                 except Exception as e:
-                    raise e
+                    if DEBUG:
+                        raise e
                     click.echo('static静态文件上传失败')
 
         # upload static first
         static_paths = []
         if os.path.isdir(static_dir):
             for static_name in os.listdir(static_dir):
                 static_path = os.path.join(static_dir, static_name)
@@ -894,15 +913,16 @@
                                 soup_prewarn(soup_warned)
                                 extract_body = click.prompt(f'{filename}上传前是否进行简化处理，只上传body内部内容？(y/n)（默认为是）', type=bool, default=True)
                             if has_script:
                                 soup_prewarn(soup_warned)
                                 remove_scripts = click.prompt(f'{filename}上传前是否将所有相对路径的script移除？(y/n)（默认为是）', type=bool, default=True)
                             raw = soup_html(raw, extract_body, remove_scripts)
                     except Exception as e:
-                        raise e
+                        if DEBUG:
+                            raise e
                         click.echo(f'此文件无法被读取，请确保编码为utf-8或者其他可读取的类型 {filepath}')
                         exit()
                     if relative_switches and len(relative_switches):
                         for endname, url in relative_switches.items():
                             data[filename] = raw.replace(endname, url)
                     else:
                         data[filename] = raw
@@ -962,16 +982,16 @@
                 try:
                     msg = response.json()['msg']
                 except:
                     pass
                 click.echo(msg)
                 return        
         except Exception as e:
-            # print(e)
-            raise e
+            if DEBUG:
+                raise e
             click.echo("抱歉，您的网络不稳定或者服务器流量过大，请稍后重试")
         return
 
 
 if __name__ == '__main__':
     zzd()
```

