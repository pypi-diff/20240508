# Comparing `tmp/movie-downloader-0.1.7.tar.gz` & `tmp/movie-downloader-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\movie-downloader-0.1.7.tar", last modified: Mon Jun 27 10:06:55 2022, max compression
+gzip compressed data, was "C:\projects\movie-downloader\dist\tmpgo646vgl\movie-downloader-0.2.5.tar", last modified: Wed May  8 02:17:24 2024, max compression
```

## Comparing `movie-downloader-0.1.7.tar` & `movie-downloader-0.2.5.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxrwxrwx   0        0        0        0 2022-06-27 10:06:55.000000 movie-downloader-0.1.7/
--rw-rw-rw-   0        0        0      177 2022-05-24 02:08:13.000000 movie-downloader-0.1.7/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2022-06-27 10:06:55.000000 movie-downloader-0.1.7/mdl/
--rw-rw-rw-   0        0        0     1100 2022-06-12 05:02:24.000000 movie-downloader-0.1.7/mdl/commons.py
-drwxrwxrwx   0        0        0        0 2022-06-27 10:06:55.000000 movie-downloader-0.1.7/mdl/conf/
--rw-rw-rw-   0        0        0     1870 2022-06-01 04:53:01.000000 movie-downloader-0.1.7/mdl/conf/dlops.conf
--rw-rw-rw-   0        0        0      253 2022-05-24 02:08:13.000000 movie-downloader-0.1.7/mdl/conf/misc.conf
--rw-rw-rw-   0        0        0    11991 2022-06-12 05:02:24.000000 movie-downloader-0.1.7/mdl/downloader.py
-drwxrwxrwx   0        0        0        0 2022-06-27 10:06:55.000000 movie-downloader-0.1.7/mdl/js/
--rw-rw-rw-   0        0        0    10624 2022-06-01 04:55:02.000000 movie-downloader-0.1.7/mdl/js/vqq.js
-drwxrwxrwx   0        0        0        0 2022-06-27 10:06:55.000000 movie-downloader-0.1.7/mdl/log/
--rw-rw-rw-   0        0        0        0 2022-06-27 10:06:55.000000 movie-downloader-0.1.7/mdl/log/mdl.log
-drwxrwxrwx   0        0        0        0 2022-06-27 10:06:55.000000 movie-downloader-0.1.7/mdl/sites/
--rw-rw-rw-   0        0        0    12552 2022-05-08 11:07:18.000000 movie-downloader-0.1.7/mdl/sites/m1905.py
--rw-rw-rw-   0        0        0    32336 2022-06-25 08:54:15.000000 movie-downloader-0.1.7/mdl/sites/vqq.py
--rw-rw-rw-   0        0        0      360 2022-05-24 02:08:13.000000 movie-downloader-0.1.7/mdl/sites/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-27 10:06:55.000000 movie-downloader-0.1.7/mdl/third_parties/
-drwxrwxrwx   0        0        0        0 2022-06-27 10:06:55.000000 movie-downloader-0.1.7/mdl/third_parties/aria2/
--rw-rw-rw-   0        0        0      101 2022-06-12 03:41:05.000000 movie-downloader-0.1.7/mdl/third_parties/aria2/README
-drwxrwxrwx   0        0        0        0 2022-06-27 10:06:55.000000 movie-downloader-0.1.7/mdl/third_parties/ckey/
--rw-rw-rw-   0        0        0      161 2022-05-24 02:08:13.000000 movie-downloader-0.1.7/mdl/third_parties/ckey/README
-drwxrwxrwx   0        0        0        0 2022-06-27 10:06:55.000000 movie-downloader-0.1.7/mdl/third_parties/ffmpeg/
--rw-rw-rw-   0        0        0       76 2021-11-15 11:57:06.000000 movie-downloader-0.1.7/mdl/third_parties/ffmpeg/README
-drwxrwxrwx   0        0        0        0 2022-06-27 10:06:55.000000 movie-downloader-0.1.7/mdl/third_parties/mkvtoolnix/
--rw-rw-rw-   0        0        0      102 2022-06-12 03:41:05.000000 movie-downloader-0.1.7/mdl/third_parties/mkvtoolnix/README
-drwxrwxrwx   0        0        0        0 2022-06-27 10:06:55.000000 movie-downloader-0.1.7/mdl/third_parties/node/
--rw-rw-rw-   0        0        0       69 2022-05-24 02:08:13.000000 movie-downloader-0.1.7/mdl/third_parties/node/README
-drwxrwxrwx   0        0        0        0 2022-06-27 10:06:55.000000 movie-downloader-0.1.7/mdl/third_parties/setupext_janitor/
--rw-rw-rw-   0        0        0     7217 2022-03-03 03:10:20.000000 movie-downloader-0.1.7/mdl/third_parties/setupext_janitor/janitor.py
--rw-rw-rw-   0        0        0     5228 2021-11-15 11:57:06.000000 movie-downloader-0.1.7/mdl/third_parties/setupext_janitor/README.rst
--rw-rw-rw-   0        0        0    13647 2022-06-27 07:16:09.000000 movie-downloader-0.1.7/mdl/third_parties/__init__.py
--rw-rw-rw-   0        0        0      338 2021-11-15 11:57:06.000000 movie-downloader-0.1.7/mdl/third_parties/__main__.py
--rw-rw-rw-   0        0        0     5640 2022-06-01 04:53:01.000000 movie-downloader-0.1.7/mdl/utils.py
--rw-rw-rw-   0        0        0     3052 2022-05-24 02:08:13.000000 movie-downloader-0.1.7/mdl/videoconfig.py
--rw-rw-rw-   0        0        0     6857 2022-05-24 02:08:13.000000 movie-downloader-0.1.7/mdl/__init__.py
--rw-rw-rw-   0        0        0      392 2021-11-15 11:57:06.000000 movie-downloader-0.1.7/mdl/__main__.py
--rw-rw-rw-   0        0        0     7253 2022-06-27 10:06:55.000000 movie-downloader-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     6091 2022-05-24 02:08:13.000000 movie-downloader-0.1.7/README.md
--rw-rw-rw-   0        0        0       97 2022-05-24 02:08:13.000000 movie-downloader-0.1.7/requirements.txt
--rw-rw-rw-   0        0        0       58 2022-06-27 10:06:55.000000 movie-downloader-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     2738 2022-05-24 02:08:13.000000 movie-downloader-0.1.7/setup.py
--rw-rw-rw-   0        0        0        5 2022-06-27 09:40:30.000000 movie-downloader-0.1.7/VERSION
+drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/
+-rw-rw-rw-   0        0        0      177 2022-05-24 02:08:13.000000 movie-downloader-0.2.5/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/
+-rw-rw-rw-   0        0        0     2137 2023-03-17 08:17:40.000000 movie-downloader-0.2.5/mdl/commons.py
+drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/conf/
+-rw-rw-rw-   0        0        0     4229 2024-04-12 05:39:22.000000 movie-downloader-0.2.5/mdl/conf/dlops.conf
+-rw-rw-rw-   0        0        0      253 2022-05-24 02:08:13.000000 movie-downloader-0.2.5/mdl/conf/misc.conf
+-rw-rw-rw-   0        0        0    12875 2024-04-04 15:37:04.000000 movie-downloader-0.2.5/mdl/downloader.py
+drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/js/
+-rw-rw-rw-   0        0        0    29485 2023-05-24 09:09:12.000000 movie-downloader-0.2.5/mdl/js/vqq_ckey-8.1.js
+-rw-rw-rw-   0        0        0    31710 2023-09-26 16:39:11.000000 movie-downloader-0.2.5/mdl/js/vqq_ckey-8.5.js
+-rw-rw-rw-   0        0        0    10669 2023-05-24 11:42:29.000000 movie-downloader-0.2.5/mdl/js/vqq_ckey-9.1.js
+drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/log/
+-rw-rw-rw-   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/log/mdl.log
+drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/sites/
+-rw-rw-rw-   0        0        0    14343 2024-03-08 16:14:06.000000 movie-downloader-0.2.5/mdl/sites/m1905.py
+-rw-rw-rw-   0        0        0    45194 2024-04-12 05:39:22.000000 movie-downloader-0.2.5/mdl/sites/vqq.py
+-rw-rw-rw-   0        0        0      360 2022-05-24 02:08:13.000000 movie-downloader-0.2.5/mdl/sites/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/third_parties/
+drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/third_parties/aria2/
+-rw-rw-rw-   0        0        0      101 2022-06-12 03:41:05.000000 movie-downloader-0.2.5/mdl/third_parties/aria2/README
+drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/third_parties/ckey/
+-rw-rw-rw-   0        0        0      161 2022-05-24 02:08:13.000000 movie-downloader-0.2.5/mdl/third_parties/ckey/README
+drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/third_parties/ffmpeg/
+-rw-rw-rw-   0        0        0       76 2021-11-15 11:57:06.000000 movie-downloader-0.2.5/mdl/third_parties/ffmpeg/README
+drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/third_parties/mkvtoolnix/
+-rw-rw-rw-   0        0        0      102 2022-06-12 03:41:05.000000 movie-downloader-0.2.5/mdl/third_parties/mkvtoolnix/README
+drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/third_parties/node/
+-rw-rw-rw-   0        0        0       69 2022-05-24 02:08:13.000000 movie-downloader-0.2.5/mdl/third_parties/node/README
+drwxrwxrwx   0        0        0        0 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/mdl/third_parties/setupext_janitor/
+-rw-rw-rw-   0        0        0     7217 2022-03-03 03:10:20.000000 movie-downloader-0.2.5/mdl/third_parties/setupext_janitor/janitor.py
+-rw-rw-rw-   0        0        0     5228 2021-11-15 11:57:06.000000 movie-downloader-0.2.5/mdl/third_parties/setupext_janitor/README.rst
+-rw-rw-rw-   0        0        0    13647 2022-11-11 05:46:23.000000 movie-downloader-0.2.5/mdl/third_parties/__init__.py
+-rw-rw-rw-   0        0        0      338 2021-11-15 11:57:06.000000 movie-downloader-0.2.5/mdl/third_parties/__main__.py
+-rw-rw-rw-   0        0        0     5640 2022-06-01 04:53:01.000000 movie-downloader-0.2.5/mdl/utils.py
+-rw-rw-rw-   0        0        0     3965 2024-04-05 10:09:24.000000 movie-downloader-0.2.5/mdl/videoconfig.py
+-rw-rw-rw-   0        0        0     6893 2024-03-30 04:55:37.000000 movie-downloader-0.2.5/mdl/__init__.py
+-rw-rw-rw-   0        0        0      392 2021-11-15 11:57:06.000000 movie-downloader-0.2.5/mdl/__main__.py
+-rw-rw-rw-   0        0        0     7269 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6107 2024-05-07 09:22:21.000000 movie-downloader-0.2.5/README.md
+-rw-rw-rw-   0        0        0      213 2024-05-07 04:13:17.000000 movie-downloader-0.2.5/requirements.txt
+-rw-rw-rw-   0        0        0       58 2024-05-08 02:17:24.000000 movie-downloader-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     2745 2024-05-07 04:13:17.000000 movie-downloader-0.2.5/setup.py
+-rw-rw-rw-   0        0        0        5 2024-05-08 01:47:52.000000 movie-downloader-0.2.5/VERSION
```

### Comparing `movie-downloader-0.1.7/mdl/downloader.py` & `movie-downloader-0.2.5/mdl/downloader.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,73 +5,83 @@
 import errno
 import logging
 from math import trunc, log10
 
 from certifi import where
 from bdownload.download import requests_retry_session
 
-from .commons import VIDEO_DEFINITIONS, VideoTypes, DEFAULT_YEAR
+from .commons import pick_highest_definition, VideoTypes, DEFAULT_YEAR
 from .sites import get_all_sites_vcs
 from .utils import logging_with_pipe, normalize_filename
 
 
-cert_path = where()
-
-
 class MDownloader(object):
     def __init__(self, args=None, confs=None):
         self._vcs = get_all_sites_vcs()
         self.args = args
         self.confs = confs
 
         logger_name = '.'.join(['MDL', 'MDownloader'])  # 'MDL.MDownloader'
         self._logger = logging.getLogger(logger_name)
 
     def download(self, urls):
         for url in urls:
-            cover_info = self.extract_config_info(url)
-            if cover_info:
-                cover_dir, episodes = self.dwnld_videos_with_aria2(
-                    cover_info, save_dir=self.confs[cover_info["vc_name"]]["dir"],
-                    defn=self.confs[cover_info["vc_name"]]['definition'])
+            vci, cover_info = self.extract_config_info(url)
+            if not cover_info or not cover_info.get('normal_ids'):
+                self._logger.warning("No files to download for '{}'.".format(url))
+                continue
+
+            # download the list of videos in batches, instead of all at once
+            batch_size = int(self.confs[vci.VC_NAME]['episode_batch_size'])
+            batch_cover_info = cover_info.copy()
+            video_list = cover_info['normal_ids']
+
+            for batch_start in range(0, len(video_list), batch_size):
+                batch_cover_info['normal_ids'] = video_list[batch_start:batch_start + batch_size]
+
+                vci.update_video_dwnld_info(batch_cover_info)
+                cover_dir, episodes = self.dwnld_videos_with_aria2(batch_cover_info,
+                                                                   save_dir=self.confs[vci.VC_NAME]['dir'],
+                                                                   defn=self.confs[vci.VC_NAME]['definition'])
+
                 self.join_videos(cover_dir, episodes)
 
     def extract_config_info(self, url):
         for name, vc in self._vcs.items():
             vcc = vc['class']
             if not vcc.is_url_valid(url):
                 continue
 
             vci = vc.get('instance')
             if vci is None:
-                requester = requests_retry_session()
+                verify = vcc.make_ca_bundle(self.args, self.confs)
+                if not verify:
+                    verify = True
+                else:
+                    self.confs[vcc.VC_NAME]['ca_cert'] = verify
+                requester = requests_retry_session(verify=verify)
                 vci = vcc(requester, self.args, self.confs)
                 vc['instance'] = vci
 
             cover_info = vci.get_video_config_info(url)
             if cover_info:
-                cover_info["source_name"] = vcc.SOURCE_NAME
-                cover_info["vc_name"] = vcc.VC_NAME
-            return cover_info
+                cover_info['source_name'] = vcc.SOURCE_NAME
+                cover_info['vc_name'] = vcc.VC_NAME
+            return vci, cover_info
         else:
             # check site domain name against URL
             self._logger.error("Video URL {!r} is invalid".format(url))
-            return None
+            return None, None
 
     def dwnld_videos_with_aria2(self, cover_info, save_dir='.', defn=None):
         """
         :returns:
         (abs_cover_dir, [(abs_episode1_dir, [fname1.1.mp4, fname1.2.mp4]),(abs_episode2_dir, [fname2.1.mp4, fname2.2.mp4])])
         """
 
-        def pick_highest_definition(defns):
-            for definition in VIDEO_DEFINITIONS:
-                if defns.get(definition):
-                    return definition
-
         def pick_format(formats):
             for format in formats:
                 if format['ext'] != 'ts':
                     return format
 
             return formats[0]
 
@@ -86,16 +96,16 @@
             ep_cnt = sum([1 for vi in normal_ids if vi.get('defns') and any(vi['defns'].values())])  # number of valid episodes
             numbering = False if (total_ep and total_ep == 1) or (not total_ep and ep_cnt == 1) else True
 
             return numbering, width
 
         video_list = cover_info.get('normal_ids')
         if video_list:
-            cover_name = '.'.join([cover_info.get('title') if cover_info.get('title') else cover_info['source_name'] + '_' + cover_info.get('cover_id', ''),
-                                   cover_info.get('year', DEFAULT_YEAR)])
+            cover_name = '.'.join([cover_info.get('title') or cover_info['source_name'] + '_' + (cover_info.get('cover_id') or ''),
+                                   (cover_info.get('year') or DEFAULT_YEAR)])
             cover_name = normalize_filename(cover_name, repl='_')
             cover_default_dir = '.'.join([cover_name, cover_info.get('type', VideoTypes.MOVIE)])
             cover_dir = os.path.abspath(os.path.join(save_dir, cover_default_dir))
 
             urls = []  # URLs file info for aria2c
             episodes = []  # [(abs_episode1_dir, [fname1.1.mp4, fname1.2.mp4]), ]
 
@@ -141,14 +151,17 @@
             mcd = self.confs[cover_info['vc_name']]['max_concurrent_downloads']
             mss = self.confs[cover_info['vc_name']]['min_split_size']
             split = self.confs[cover_info['vc_name']]['split']
             mcps = self.confs[cover_info['vc_name']]['max_connection_per_server']
             retry_wait = self.confs[cover_info['vc_name']]['retry_wait']
             speed_limit = self.confs[cover_info['vc_name']]['lowest_speed_limit']
             referer = cover_info['referrer']
+            cert_path = self.confs[cover_info['vc_name']]['ca_cert']
+            if not cert_path:
+                cert_path = where()
 
             cmd_aria2c = [aria2c, '-c', '-j', mcd,  '-k', mss, '-s', split, '-x', mcps, '--max-file-not-found=5000', '-m0',
                           '--retry-wait', retry_wait, '--lowest-speed-limit', speed_limit, '--no-conf', '-i-',
                           '--console-log-level=warn', '--download-result=hide', '--summary-interval=0', '--uri-selector=adaptive',
                           '--referer', referer, '--ca-certificate', cert_path, '-U', user_agent, '--all-proxy', proxy,
                           '--retry-on-400=true', '--retry-on-403=true', '--retry-on-406=true', '--retry-on-unknown=true']
             try:
```

### Comparing `movie-downloader-0.1.7/mdl/js/vqq.js` & `movie-downloader-0.2.5/mdl/js/vqq_ckey-9.1.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
     URL: "",
     referrer: ""
 }
 
 var window = {
     document: document,
     navigator: {
-        userAgent: "Mozilla/5.0 (Linux; U; Android 2.3.7; zh-cn) AppleWebKit/533.1 (KHTML, like Gecko) Version/4.0 Mobile Safari/533.1",
+        userAgent: "Mozilla/5.0 (Linux; U; Android 9; zh-cn) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Safari/537.36",
         appCodeName: "Mozilla",
         appName: "Netscape",
         platform: "Linux"
     },
 };
 
 
@@ -394,31 +394,34 @@
         b += d;
     }
     return b;
 }
 
 /////////////////////////
 
-function processRequest(recordLine) {
+async function processRequest(recordLine) {
     var req = recordLine.trim().split(' '); // Input Record Format: < platform appVer vid vURL referrer >
     setDocument(req[3], req[4]);
     var flowid = flowGuid + "_" + req[0];
+
+    await delay((Math.floor(Math.random() * 2) + 1) * 1000); // sleep for 1 or 2s
     var tm = Math.floor(Date.now() / 1000);
     var cKey = getCkey(req[0], req[1], req[2], "", guid, tm);
 
-    delay((Math.floor(Math.random() * 2) + 1) * 1000); // 'sleep' (busy-waiting) 1 or 2s
-
     var resp = [cKey, tm, guid, flowid];
     process.stdout.write(resp.join(' ')); // Output Record Format: < cKey tm guid flowid >
     process.stdout.write('\n');
 }
 
-function delay(millis) {
-    const start = Date.now();
-    while ((Date.now() - start) < millis) {}
+async function delay(millis) {
+    return new Promise((resolve, reject) => {
+        setTimeout(() => {
+            resolve();
+        }, millis);
+    });
 }
 
 var guid = createGUID();
 var flowGuid = createGUID(); // + "_" + platform
 
 process.stdin.setEncoding('utf8');
 process.stdout.setEncoding('utf8');
```

### Comparing `movie-downloader-0.1.7/mdl/sites/m1905.py` & `movie-downloader-0.2.5/mdl/sites/m1905.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 import json
 import time
 import re
 import random
 import hashlib
-from urllib.parse import quote as urllib_parse_quote
+from urllib.parse import quote as urllib_parse_quote, urlencode
 from math import floor as math_floor
 
 # from requests.cookies import RequestsCookieJar
+from requests import RequestException
 
 from ..videoconfig import VideoConfig
 from ..commons import VideoTypes
 from ..utils import json_path_get
 
 
 class M1905VC(VideoConfig):
     _VIDEO_URL_PATS = [
-        {'pat': r'^https?://www\.1905\.com/vod/play/(\d+)\.shtml',
+        {'pat': r'^https?://www\.1905\.com/(?:vod|video)/play/(\d+)\.shtml',
          'eg': 'https://www.1905.com/vod/play/1287886.shtml'}, # 'video_episode_sd'
         {'pat': r'^https?://www\.1905\.com/mdb/film/(\d+)/?',
          'eg': 'https://www.1905.com/mdb/film/2245563'},  # 'video_cover'
         {'pat': r'https?://vip\.1905\.com/play/(\d+)\.shtml',
          'eg': 'https://vip.1905.com/play/535547.shtml'}  # 'VIP: video_episode_hd'
     ]
     SOURCE_NAME = "m1905"
     VC_NAME = "m1905"
     #_VIP_TOKEN = {}
 
-    _M1905_DEFINITION = ['uhd', 'hd', 'sd']  # decremental! FIXME: VIP user
-    _M1905_DEFN_MAP_I2S = {'uhd': 'shd', 'hd': 'hd', 'sd': 'sd'}  # internal format name -> standard format name
-    _M1905_DEFN_MAP_S2I = {'fhd': 'fhd', 'shd': 'uhd', 'hd': 'hd', 'sd': 'sd'}  # standard -> internal | FIXME: VIP fhd?
+    _M1905_DEFINITION = ['fhd', 'uhd', 'hd', 'sd']  # decremental! FIXME: VIP user
+    _M1905_DEFN_MAP_I2S = {'fhd': 'fhd', 'uhd': 'shd', 'hd': 'hd', 'sd': 'sd'}  # internal format name -> standard format name
+    _M1905_DEFN_MAP_S2I = {'dolby': 'fhd', 'sfr_hdr': 'fhd', 'hdr10': 'fhd', 'uhd': 'fhd', 'fhd': 'fhd', 'shd': 'uhd', 'hd': 'hd', 'sd': 'sd'}  # standard -> internal | FIXME: VIP fhd?
 
     def __init__(self, requester, args, confs):
         super().__init__(requester, args, confs)
 
         self._SD_CONF_PAT_RE = re.compile(
-            r"VODCONFIG.*vid\s*:\s*\"(\d+)\".*title\s*:\s*\"(.*?)\".*mdbfilmid\s*:\s*\"(\d+)\".*apikey\s*:\s*\"(.*?)\"",
+            r"(?:VODCONFIG|VIDEOCONFIG).*vid\s*:\s*\"(\d+)\".*?(?<!vip)title\s*:\s*\"(.*?)\".*?apikey\s*:\s*\"(.*?)\"",  # (mdbfilmid\s*:\s*\"(\d+)\")?
             re.MULTILINE | re.DOTALL | re.IGNORECASE
         )
         self._COVER_YEAR_RE = re.compile(r"header-wrapper-h1.*?\(\s*(\d+)\s*\)",
                                          re.MULTILINE | re.DOTALL | re.IGNORECASE
                                          )
         self._ONLINE_COVER_RE = re.compile(
             r"class\s*=\s*\"\s*watch-online.+?正片.+?(<ul\s+class\s*=\s*\"watch-online-list.*?</ul>)",
@@ -81,39 +82,53 @@
                 query += "&" + q if query else q
 
         return hashlib.sha1((query + "." + appid).encode("utf-8")).hexdigest()
 
     def _get_episode_info_sd(self, epurl):
         info = None
 
-        r = self._requester.get(epurl, allow_redirects=True)
-        if r.status_code == 200:  # requests.codes.ok
-            r.encoding = 'utf-8'
-            conf_match = self._SD_CONF_PAT_RE.search(r.text)
-            if conf_match:
-                info = {'vid': conf_match.group(1), 'title': conf_match.group(2), 'cover_id': conf_match.group(3)}
-                # info['year'] = video_info.get('year')  # extract it from the cover page
-
-                self._apikey = conf_match.group(4)
+        try:
+            r = self._requester.get(epurl)
+            if r.status_code == 200:  # requests.codes.ok
+                r.encoding = 'utf-8'
+                conf_match = self._SD_CONF_PAT_RE.search(r.text)
+                if conf_match:
+                    info = {'vid': conf_match.group(1), 'title': conf_match.group(2)}
+                    # info['year'] = video_info.get('year')  # extract it from the cover page
+                    self._apikey = conf_match.group(3)
+
+                    video_config = conf_match.group(0)  # VODCONFIG | VIDEOCONFIG
+                    re_cover_id = r"mdbfilmid\s*:\s*\"(\d+)\""
+                    cover_id_match = re.search(re_cover_id, video_config, flags=re.MULTILINE | re.DOTALL | re.IGNORECASE)
+                    info['cover_id'] = cover_id_match.group(1) if cover_id_match else ""
+            else:
+                raise RequestException("Unexpected status code %i" % r.status_code)
+        except RequestException as e:
+            self._logger.error("Request webpage '%s' failed: '%r'", epurl, e)
 
         return info
 
     def _get_episode_info_hd(self, epurl):
         """Parse VIP webpage"""
 
         info = None
         regex_vip = r"movie-title\s*\"\s*>(?P<title>[^<]+)</h1>.*?年份[^\d]+(?P<year>\d+).*?www\.1905\.com/mdb/film/(?P<cover_id>\d+)"
 
-        r = self._requester.get(epurl, allow_redirects=True)
-        if r.status_code == 200:
-            r.encoding = 'utf-8'
-            conf_match = re.search(regex_vip, r.text, flags=re.MULTILINE|re.DOTALL|re.IGNORECASE)
-            if conf_match:
-                info = {'title': conf_match.group('title'), 'year': conf_match.group('year'),
-                        'cover_id': conf_match.group('cover_id'), 'vid': epurl.split('/')[-1].split('.')[0]}
+        try:
+            r = self._requester.get(epurl)
+            if r.status_code == 200:
+                r.encoding = 'utf-8'
+                conf_match = re.search(regex_vip, r.text, flags=re.MULTILINE|re.DOTALL|re.IGNORECASE)
+                if conf_match:
+                    info = {'title': conf_match.group('title'), 'year': conf_match.group('year'),
+                            'cover_id': conf_match.group('cover_id'), 'vid': epurl.split('/')[-1].split('.')[0]}
+            else:
+                raise RequestException("Unexpected status code %i" % r.status_code)
+        except RequestException as e:
+            self._logger.error("Request webpage '%s' failed: '%r'", epurl, e)
 
         return info
 
     def _get_cover_info(self, cvurl):
         """
 
         :param cvurl:
@@ -122,46 +137,50 @@
         year = ""
         defns = {
             "VIP免广告": "hd",
             "免费": "sd"
         }
         urls = {}
 
-        r = self._requester.get(cvurl)
-        if r.status_code == 200:
-            r.encoding = 'utf-8'
-            year_match = self._COVER_YEAR_RE.search(r.text)
-            if year_match:
-                year = year_match.group(1)
-                cover_match = self._ONLINE_COVER_RE.search(r.text[year_match.end(0):])
+        try:
+            r = self._requester.get(cvurl)
+            if r.status_code == 200:
+                r.encoding = 'utf-8'
+                year_match = self._COVER_YEAR_RE.search(r.text)
+                if year_match:
+                    year = year_match.group(1)
+                    cover_match = self._ONLINE_COVER_RE.search(r.text[year_match.end(0):])
+                else:
+                    cover_match = self._ONLINE_COVER_RE.search(r.text)
+
+                if cover_match:
+                    episodes_match = self._ONLINE_EPISODE_RE.finditer(cover_match.group(1))
+                    for mo in episodes_match:
+                        urls[defns[mo.group(2)]] = mo.group(1)
             else:
-                cover_match = self._ONLINE_COVER_RE.search(r.text)
-
-            if cover_match:
-                episodes_match = self._ONLINE_EPISODE_RE.finditer(cover_match.group(1))
-                for mo in episodes_match:
-                    urls[defns[mo.group(2)]] = mo.group(1)
-        else:
-            print("Request webpage failed: {}".format(cvurl))  # logging
+                raise RequestException("Unexpected status code %i" % r.status_code)
+        except RequestException as e:
+            self._logger.error("Request webpage '%s' failed: '%r'", cvurl, e)
 
         return year, urls
 
     def get_cover_info(self, url):
         cover_info = None
         episode_info = None
 
         for typ, pat in enumerate(self._VIDEO_URL_PATS, 1):
             match = pat['cpat'].match(url)
             if match:
                 cover_info = {}
                 if typ == 1:  # 'video_episode_sd'
                     episode_info = self._get_episode_info_sd(url)
                     if episode_info:
-                        year, _ = self._get_cover_info(self._VIDEO_COVER_FORMAT.format(episode_info['cover_id']))
-                        episode_info['year'] = year
+                        if episode_info['cover_id']:
+                            year, _ = self._get_cover_info(self._VIDEO_COVER_FORMAT.format(episode_info['cover_id']))
+                            episode_info['year'] = year
 
                         cover_info["normal_ids"] = [dict(V=episode_info['vid'], E=1, vip=False, defns={}, page=url)]
                 elif typ == 2:  # 'video_cover'
                     year, urls_dict = self._get_cover_info(self._VIDEO_COVER_FORMAT.format(match.group(1)))
                     if urls_dict:
                         cover_info["normal_ids"] = []
                         ep_num = 0
@@ -179,18 +198,18 @@
                                 cover_info["normal_ids"].append(dict(V=episode_info['vid'], E=ep_num, vip=True, defns={}, page=urls_dict['hd']))
                 else:  # video_episode_hd
                     episode_info = self._get_episode_info_hd(url)
                     if episode_info:
                         cover_info["normal_ids"] = [dict(V=episode_info['vid'], E=1, vip=True, defns={}, page=url)]
 
                 if episode_info:
-                    cover_info["title"] = episode_info["title"]
-                    cover_info["year"] = episode_info["year"]
+                    cover_info["title"] = episode_info.get("title") or ""
+                    cover_info["year"] = episode_info.get("year") or ""
                     cover_info["type"] = VideoTypes.MOVIE
-                    cover_info["cover_id"] = episode_info["cover_id"]
+                    cover_info["cover_id"] = episode_info.get("cover_id") or ""
                     cover_info["episode_all"] = len(cover_info["normal_ids"])
                     cover_info["referrer"] = url
 
                 break
 
         return cover_info
 
@@ -231,18 +250,20 @@
                         if line:
                             if line.startswith("#EXT-X-STREAM-INF:"):  # in master playlist
                                 _, m3u = self._pick_highest_bandwidth_m3u8(r.text)
                                 playlist = "%s/%s" % (url_prefix, m3u)
                                 break
                             elif line.startswith("#EXTINF:"):  # in media playlist
                                 mpeg_urls = ["%s/%s" % (url_prefix, ts) for ts in r.text.splitlines() if
-                                             ts and not ts.startswith('#')]
+                                             ts and not ts.startswith('#') and ts.endswith('.ts')]
                                 return mpeg_urls
-        except Exception:
-            print("Failed to fetch {!r}".format(m3u8_url))  # logging
+                else:
+                    raise RequestException("Unexpected status code %i" % r.status_code)
+        except RequestException as e:
+            self._logger.error("Failed to fetch '%s': '%r'", playlist, e)
 
     def _update_video_dwnld_info_sd(self, vi):
         """
         :param vi: item of cover_info['normal_ids'].
         """
         nonce = math_floor(time.time())
         params = {
@@ -252,46 +273,50 @@
             'page': vi['page'],
             'playerid': self._random_string().replace('-', '')[5:20],
             'type': "hls",
             'uuid': self._random_string()
         }
         params['signature'] = self._signature(params, self._appid)
 
-        r = self._requester.get(self._PROFILE_CONFIG_URL, params=params)
-        if r.status_code == 200:
-            # cookie_jar = RequestsCookieJar()
-            # set_cookie = r.headers.get("Set-Cookie")
-            # if set_cookie:
-            #     cookie_info = set_cookie.split(";")
-            #     name, val = cookie_info[0].split("=")
-            #     _, path = cookie_info[-2].split("=")
-            #     _, domain = cookie_info[-1].split("=")
-            #     cookie_jar.set(name, val, path=path, domain=domain)
-            try:
-                data = json.loads(r.text[len("null("):-1]).get('data')
-            except json.JSONDecodeError:
-                return
-
-            playlist_m3u8 = ""
-            defn = self._M1905_DEFN_MAP_S2I[self.preferred_defn]
-            defns = [defn] if json_path_get(data, ['sign', defn]) else self._M1905_DEFINITION
-            for defn in defns:
-                host = json_path_get(data, ['quality', defn, 'host'])
-                sign = json_path_get(data, ['sign', defn, 'sign'])
-                path = json_path_get(data, ['path', defn, 'path'])
-
-                if host and sign and path:
-                    playlist_m3u8 = (host + sign + path).replace('\\', '')
-                    break
-
-            if playlist_m3u8:
-                mpeg_urls = self._get_ts_playlist(playlist_m3u8)
-                if mpeg_urls:
-                    std_defn = self._M1905_DEFN_MAP_I2S[defn]
-                    vi["defns"].setdefault(std_defn, []).append(dict(ext="ts", urls=mpeg_urls))
+        try:
+            r = self._requester.get(self._PROFILE_CONFIG_URL, params=params)
+            if r.status_code == 200:
+                # cookie_jar = RequestsCookieJar()
+                # set_cookie = r.headers.get("Set-Cookie")
+                # if set_cookie:
+                #     cookie_info = set_cookie.split(";")
+                #     name, val = cookie_info[0].split("=")
+                #     _, path = cookie_info[-2].split("=")
+                #     _, domain = cookie_info[-1].split("=")
+                #     cookie_jar.set(name, val, path=path, domain=domain)
+                try:
+                    data = json.loads(r.text[len("null("):-1]).get('data')
+                except json.JSONDecodeError:
+                    return
+
+                defn = self._M1905_DEFN_MAP_S2I[self.preferred_defn]
+                defns = [defn] if json_path_get(data, ['sign', defn]) else self._M1905_DEFINITION
+                for defn in defns:
+                    host = json_path_get(data, ['quality', defn, 'host'])
+                    sign = json_path_get(data, ['sign', defn, 'sign'])
+                    path = json_path_get(data, ['path', defn, 'path'])
+
+                    if host and sign and path:
+                        playlist_m3u8 = (host + sign + path).replace('\\', '')
+                        mpeg_urls = self._get_ts_playlist(playlist_m3u8)
+                        if mpeg_urls:
+                            std_defn = self._M1905_DEFN_MAP_I2S[defn]
+                            vi["defns"].setdefault(std_defn, []).append(dict(ext="ts", urls=mpeg_urls))
+
+                            break
+            else:
+                raise RequestException("Unexpected status code %i" % r.status_code)
+        except RequestException as e:
+            request_url = "%s?%s" % (self._PROFILE_CONFIG_URL, urlencode(params))
+            self._logger.error("Failed to fetch '%s': '%r'", request_url, e)
 
     def _update_video_dwnld_info_hd(self, vi):
         pass
 
     def update_video_dwnld_info(self, cover_info):
         vl = cover_info.get('normal_ids', [])
         for vi in vl:
```

### Comparing `movie-downloader-0.1.7/mdl/sites/vqq.py` & `movie-downloader-0.2.5/mdl/sites/vqq.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import json
 import re
 import os
 import subprocess
 
 from urllib.parse import urlencode
 
-from ..commons import VideoTypeCodes, VideoTypes, DEFAULT_YEAR
+from requests import RequestException
+
+from ..commons import pick_highest_definition, sort_definitions, VideoTypeCodes, VideoTypes, DEFAULT_YEAR
 from ..videoconfig import VideoConfig
 from ..utils import json_path_get, build_cookiejar_from_kvp
 
 mdl_dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
 
 class QQVideoPlatforms:
@@ -30,16 +32,19 @@
         {'pat': r'^https?://v\.qq\.com/x/page/(\w+)\.html',
          'eg': 'https://v.qq.com/x/page/d00249ld45q.html'}  # 'video_page'
     ]
     SOURCE_NAME = "Tencent"
     VC_NAME = "QQVideo"
     # _VIP_TOKEN = {}
 
-    APP_VER = '3.5.57'
-    ENCRYPT_VER = '9.1'
+    _ENCRYPTVER_to_APPVER = {
+        '8.1': '3.5.57',
+        '9.1': '3.5.57',
+        '8.5': '1.27.3'
+    }
 
     _VQQ_TYPE_CODES = {
         VideoTypeCodes.MOVIE: VideoTypes.MOVIE,
         VideoTypeCodes.TV: VideoTypes.TV,
         VideoTypeCodes.CARTOON: VideoTypes.CARTOON,
         VideoTypeCodes.SPORTS: VideoTypes.SPORTS,
         VideoTypeCodes.ENTMT: VideoTypes.ENTMT,
@@ -61,26 +66,29 @@
         VideoTypeCodes.CHILD: VideoTypes.CHILD,
         VideoTypeCodes.ART: VideoTypes.ART
         # default: VideoTypes.MOVIE
     }
 
     _VQQ_FORMAT_IDS_DEFAULT = {
         QQVideoPlatforms.P10901: {
+            'uhd': 10208,  # fixme
             'fhd': 10209,
             'shd': 10201,
             'hd': 10212,  # 10202
             'sd': 10203
         },
         QQVideoPlatforms.P10801: {
+            'uhd': 321005,  # fixme
             'fhd': 321004,
             'shd': 321003,
             'hd': 321002,
             'sd': 321001
         },
         QQVideoPlatforms.P10201: {
+            'uhd': 10219,  # fixme
             'fhd': 10218,
             'shd': 10217,
             'hd': 2,
             'sd': 100001
         }
     }
 
@@ -93,56 +101,67 @@
 
         self._COVER_PAT_RE = re.compile(r"var\s+COVER_INFO\s*=\s*(.+?);?var\s+COLUMN_INFO"
                                         r"|\"coverInfo\"\s*:\s*(.+?),\s*\"videoInfo\"",
                                         re.MULTILINE | re.DOTALL | re.IGNORECASE)
         self._VIDEO_INFO_RE = re.compile(r"var\s+VIDEO_INFO\s*=\s*(.+?);?</script>"
                                          r"|\"episodeSinglePlay\".+?\"item_params\"\s*:\s*({.+?})\s*,\s*\"\s*sub_items",
                                          re.MULTILINE | re.DOTALL | re.IGNORECASE)
-        self._ALL_LOADED_INFO_RE = re.compile(r"window\.__pinia\s*=\s*(.+?);?</script>",
+        self._ALL_LOADED_INFO_RE = re.compile(r"window\.__PINIA__\s*=\s*(.+?);?</script>",
                                               re.MULTILINE | re.DOTALL | re.IGNORECASE)
+        self._EP_LIST_RE = re.compile(r"(?:\[{\"list\":)?Array\.prototype\.slice\.call\({\"\d+\":(?:{\"list\":\[)?\[(.+?})\]\]?,.*?\"length\":\d+}\).*?(?=,\"listMeta\")",
+                                      re.MULTILINE | re.DOTALL | re.IGNORECASE)
         self._VIDEO_COVER_PREFIX = 'https://v.qq.com/x/cover/'
+        self._VIDEO_CONFIG_URL = 'https://vd.l.qq.com/proxyhttp'
 
         # make sure _VIDEO_URL_PATS has a compiled version, which should have been done in @classmethod is_url_valid
         for pat in self._VIDEO_URL_PATS:
             if pat.get('cpat') is None:
                 pat['cpat'] = re.compile(pat['pat'], re.IGNORECASE)
 
         # get user tokens/cookies from configuration file
         self._regular_token = build_cookiejar_from_kvp(confs[self.VC_NAME]['regular_user_token'])
         self._vip_token = build_cookiejar_from_kvp(confs[self.VC_NAME]['vip_user_token'])
         self.user_token = self._vip_token if self._vip_token else self._regular_token
         self.has_vip = True if self._vip_token else False
         self.login_token = self._get_logintoken_from_cookies(self.user_token)
 
-        self.jsfile = os.path.join(mdl_dir, 'js', 'vqq.js')
+        self.encrypt_ver = confs[self.VC_NAME]['ckey_ver']
+        ckey_js = 'vqq_ckey-' + self.encrypt_ver + '.js'
+        self.jsfile = os.path.join(mdl_dir, 'js', ckey_js)
+
+        self.app_ver = self._ENCRYPTVER_to_APPVER[self.encrypt_ver]
 
         # parse cmdline args and config file for "QQVideo" site
         no_logo_default = 'True'
         no_logo = args.QQVideo_no_logo or confs[self.VC_NAME]['no_logo'] or no_logo_default
         self.no_logo = True if no_logo.lower() == 'true' else False
 
+        probe_mode_default = 'False'
+        probe_mode = confs[self.VC_NAME].get('probe_mode') or probe_mode_default
+        self.probe_mode = True if probe_mode.lower() == 'true' else False
+
         use_cdn = confs[self.VC_NAME].get('use_cdn')
         self.use_cdn = True if use_cdn and use_cdn.lower() == 'true' else False
 
         cdn_blacklist = confs[self.VC_NAME].get('cdn_blacklist')
         self.cdn_blacklist = tuple(cdn_blacklist.split()) if cdn_blacklist else ()
 
         self.preferred_defn = confs[self.VC_NAME]['definition']
 
     # @classmethod
     # def is_url_valid(cls, url):
     #     return super().is_url_valid(url)
 
     @staticmethod
     def _get_logintoken_from_cookies(cookies):
-        login_token = {'openid': None, 'appid': None, 'access_token': None, 'vuserid': None, 'vusession': None}
+        login_token = {'openid': '', 'appid': '', 'access_token': '', 'vuserid': '', 'vusession': ''}
 
         if cookies:
             for cookie_name in login_token:
-                login_token.update({cookie_name: cookies.get('vqq_' + cookie_name)})
+                login_token.update({cookie_name: cookies.get('vqq_' + cookie_name, '')})
 
         login_token['main_login'] = 'qq'
 
         return login_token
 
     def _get_video_urls_p10801(self, vid, definition, vurl, referrer):
         urls = []
@@ -211,15 +230,15 @@
                 if ext == 'ts':
                     if drm == 1 and not preview and not self.has_vip:
                         return format_name, ext, urls
 
                     for idx in range(start, fc + 1):
                         vfilename_new = '.'.join([vfn[0], str(idx), 'ts'])
                         url_mirrors = '\t'.join(
-                            ['%s%s' % (prefix, vfilename_new) for prefix in chosen_url_prefixes])
+                            ['%s%s?sdtfrom=v1010' % (prefix, vfilename_new) for prefix in chosen_url_prefixes])
                         urls.append(url_mirrors)
                 else:  # 'mp4'
                     if drm == 1 and not self.has_vip:
                         return format_name, ext, urls
 
                     logo = json_path_get(data, ['vl', 'vi', 0, 'logo'])
                     if logo == 0:  # logo == 0 or drm == 1
@@ -359,55 +378,62 @@
         ext = None
         format_name = None
 
         nodejs = self.confs['progs']['node']
         cmd_nodejs = [nodejs, self.jsfile]
         with subprocess.Popen(cmd_nodejs, bufsize=1, universal_newlines=True, encoding='utf-8',
                               stdin=subprocess.PIPE, stdout=subprocess.PIPE) as node_proc:
-            ckey_req = ' '.join([QQVideoPlatforms.P10201, self.APP_VER, vid, vurl, referrer])
+            ckey_req = ' '.join([QQVideoPlatforms.P10201, self.app_ver, vid, vurl, referrer])
             node_proc.stdin.write(ckey_req)
             node_proc.stdin.write(r'\n')
             node_proc.stdin.flush()
             ckey_resp = node_proc.stdout.readline().rstrip(r'\r\n')
             ckey, tm, guid, flowid = ckey_resp.split()
 
             vinfoparam = {
                 'otype': 'ojson',
-                'isHLS': 0,
+                'isHLS': 1,
                 'charge': 0,
                 'fhdswitch': 0,
                 'show1080p': 1,
-                'defnpayver': 1,
+                'defnpayver': 7,
                 'sdtfrom': 'v1010',
                 'host': 'v.qq.com',
                 'vid': vid,
                 'defn': definition,
                 'platform': QQVideoPlatforms.P10201,
-                'appVer': self.APP_VER,
+                'appVer': self.app_ver,
                 'refer': referrer,
                 'ehost': vurl,
-                'logintoken': self.login_token,
-                'encryptVer': self.ENCRYPT_VER,
+                'logintoken': json.dumps(self.login_token, separators=(',', ':')),
+                'encryptVer': self.encrypt_ver,
                 'guid': guid,
                 'flowid': flowid,
                 'tm': tm,
-                'cKey': ckey
+                'cKey': ckey,
+                'dtype': 1,
+                #'drm': 40
             }
             params = {
                 'buid': 'vinfoad',
                 'vinfoparam': urlencode(vinfoparam)
             }
-            r = self._requester.post('https://vd.l.qq.com/proxyhttp', json=params, cookies=self.user_token)
-            if r.status_code == 200:
+
+            try:
+                r = self._requester.post(self._VIDEO_CONFIG_URL, json=params, cookies=self.user_token)
+                r.raise_for_status()
+                if r.status_code != 200:
+                    raise RequestException("Unexpected status code %i" % r.status_code)
+
                 try:
                     data = json.loads(r.text)
                     if data:
                         data = json.loads(data.get('vinfo'))
-                except json.JSONDecodeError:
-                    # logging
+                except json.JSONDecodeError as e:
+                    self._logger.error("Received ill-formed video config info for '%i': '%r'", vid, e)
                     return format_name, ext, urls
 
                 if data and data.get('dltype'):
                     url_prefixes = []
                     for url_dic in json_path_get(data, ['vl', 'vi', 0, 'ul', 'ui'], []):
                         if isinstance(url_dic, dict):
                             url = url_dic.get('url')
@@ -424,102 +450,324 @@
                         cdn = [prefix for prefix in url_prefixes if prefix not in chosen_url_prefixes]
                         chosen_url_prefixes += cdn
 
                     # drm = json_path_get(data, ['vl', 'vi', 0, 'drm'])
 
                     # pick the best matched definition from available formats
                     formats = {fmt.get('name'): fmt.get('id') for fmt in json_path_get(data, ['fl', 'fi'], [])}
-                    ret_defn = definition  # not necessarily equal to requested `definition`
+                    ret_defn = definition  # not necessarily the requested `definition`
                     if ret_defn not in formats:
-                        for defn in self._VQQ_FORMAT_IDS_DEFAULT[QQVideoPlatforms.P10201]:
-                            if defn in formats:
-                                ret_defn = defn
-                                break
+                        ret_defn = pick_highest_definition(formats)
 
-                    format_id = formats.get(ret_defn) or self._VQQ_FORMAT_IDS_DEFAULT[QQVideoPlatforms.P10201][ret_defn]
+                    new_format_id = formats.get(ret_defn) or self._VQQ_FORMAT_IDS_DEFAULT[QQVideoPlatforms.P10201][ret_defn]
                     vfilename = json_path_get(data, ['vl', 'vi', 0, 'fn'], '')
                     vfn = vfilename.split('.')  # e.g. ['egmovie', 'p201', 'mp4'], ['egmovie', 'mp4']
                     ext = vfn[-1]  # video extension, e.g. 'mp4'
-                    # vfmt = vfn[1]  # e.g. 'p201'
-                    # fmt_prefix = vfmt[0]  # e.g. 'p' in 'p201'
-                    vfmt_new = vfn[1][0] + str(format_id % 10000) if len(vfn) == 3 else ''
+                    fmt_prefix = vfn[1][0] if len(vfn) == 3 else 'p'  # e.g. 'p' in 'p201'
+                    vfmt_new = fmt_prefix + str(new_format_id % 10000)
 
                     # fvkey = json_path_get(data, ['vl', 'vi', 0, 'fvkey'])
                     fc = json_path_get(data, ['vl', 'vi', 0, 'cl', 'fc'])
-                    keyids = [chap.get('keyid') for chap in json_path_get(data, ['vl', 'vi', 0, 'cl', 'ci'], [])] if fc \
-                        else [json_path_get(data, ['vl', 'vi', 0, 'cl', 'keyid'])]
+                    keyid = json_path_get(data, ['vl', 'vi', 0, 'cl', 'ci', 0, 'keyid']) if fc else json_path_get(data, ['vl', 'vi', 0, 'cl', 'keyid'])
+                    orig_format_id = int(keyid.split('.')[1])
 
-                    for keyid in keyids:
+                    max_fc = 80  # large enough try limit such that we don't miss any clip
+                    for idx in range(1, max_fc + 1):
                         keyid_new = keyid.split('.')
+                        keyid_new[0] = vfn[0]
                         if len(keyid_new) == 3:
-                            keyid_new[1] = vfmt_new
+                            keyid_new[1:] = [vfmt_new, str(idx)]
                             keyid_new = '.'.join(keyid_new)
                         else:
-                            if len(vfn) == 3 and int(keyid_new[1]) != format_id:
-                                vfn[1] = vfn[1][0] + str(format_id)
+                            if int(keyid_new[1]) != new_format_id:
+                                if len(vfn) == 3:
+                                    vfn[1] = vfn[1][0] + str(new_format_id)
+                                else:
+                                    vfn.insert(1, vfmt_new)
                             keyid_new = '.'.join(vfn[:-1])
                         cfilename = keyid_new + '.' + ext
 
-                        ckey_req = ' '.join([QQVideoPlatforms.P10201, self.APP_VER, vid, vurl, referrer, r'\n'])
+                        ckey_req = ' '.join([QQVideoPlatforms.P10201, self.app_ver, vid, vurl, referrer, r'\n'])
                         node_proc.stdin.write(ckey_req)
                         node_proc.stdin.flush()
                         ckey_resp = node_proc.stdout.readline().rstrip(r'\r\n')
                         ckey, tm, guid, flowid = ckey_resp.split()
 
                         vkeyparam = {
                             'otype': 'ojson',
                             'vid': vid,
-                            'format': format_id,
+                            'format': new_format_id,
                             'filename': cfilename,
                             'platform': QQVideoPlatforms.P10201,
-                            'appVer': self.APP_VER,
+                            'appVer': self.app_ver,
                             'sdtfrom': 'v1010',
                             'guid': guid,
                             'flowid': flowid,
                             'tm': tm,
                             'refer': referrer,
                             'ehost': vurl,
-                            'logintoken': self.login_token,
-                            'encryptVer': self.ENCRYPT_VER,
+                            'logintoken': json.dumps(self.login_token, separators=(',', ':')),
+                            'encryptVer': self.encrypt_ver,
                             'cKey': ckey
                         }
                         params = {
                             'buid': 'onlyvkey',
                             'vkeyparam': urlencode(vkeyparam)
                         }
-                        r = self._requester.post('https://vd.l.qq.com/proxyhttp', json=params, cookies=self.user_token)
-                        if r.status_code == 200:
+
+                        try:
+                            r = self._requester.post(self._VIDEO_CONFIG_URL, json=params, cookies=self.user_token)
+                            r.raise_for_status()
+                            if r.status_code != 200:
+                                raise RequestException("Unexpected status code %i" % r.status_code)
+
                             try:
                                 key_data = json.loads(r.text)
                                 if key_data:
                                     key_data = json.loads(key_data.get('vkey'))
-                            except json.JSONDecodeError:
-                                # logging
+                            except json.JSONDecodeError as e:
+                                self._logger.error("Received ill-formed video key data for the clip '%s' from video '%i': '%r'", cfilename, vid, e)
                                 return format_name, ext, urls
 
                             if key_data and isinstance(key_data, dict):
                                 vkey = key_data.get('key')
                                 if not vkey:
-                                    return format_name, ext, urls
-                                if not fc:
-                                    cfilename = key_data.get('filename', cfilename)
+                                    break
+
+                                keyid = key_data.get('keyid')
+                                keyid_nseg = len(keyid.split('.'))
+                                ffilename = key_data.get('filename')
+                                if ffilename:
+                                    if keyid_nseg == 3:
+                                        cfilename = ffilename.split('.')
+                                        cfilename.insert(-1, str(idx))
+                                        cfilename = '.'.join(cfilename)
+                                    else:
+                                        cfilename = ffilename
+
                                 url_mirrors = '\t'.join(['%s%s?sdtfrom=v1010&vkey=%s' % (url_prefix, cfilename, vkey)
                                                         for url_prefix in chosen_url_prefixes])
                                 if url_mirrors:
                                     urls.append(url_mirrors)
 
-                    # check if the URLs for the file parts have all been successfully obtained
-                    if len(keyids) == len(urls):
+                                if ((orig_format_id == new_format_id or not self.probe_mode) and fc == idx) or (not fc and keyid_nseg != 3):
+                                    break
+                        except RequestException as e:
+                            self._logger.error("Error while requesting the key for the clip '%s' from video '%i': '%r'", cfilename, vid, e)
+                            return format_name, ext, urls
+
+                    # hopefully the URLs for the file parts have all been successfully obtained
+                    if len(urls) > 0:
                         format_name = ret_defn
+            except RequestException as e:
+                self._logger.error("Error while requesting the config info of video '%i': '%r'", vid, e)
+
+        return format_name, ext, urls
+
+    def _get_video_urls_p10201_ts(self, vid, definition, vurl, referrer):
+        urls = []
+        ext = None
+        format_name = None
+
+        nodejs = self.confs['progs']['node']
+        cmd_nodejs = [nodejs, self.jsfile]
+        with subprocess.Popen(cmd_nodejs, bufsize=1, universal_newlines=True, encoding='utf-8',
+                              stdin=subprocess.PIPE, stdout=subprocess.PIPE) as node_proc:
+            ckey_req = ' '.join([QQVideoPlatforms.P10201, self.app_ver, vid, vurl, referrer])
+            node_proc.stdin.write(ckey_req)
+            node_proc.stdin.write(r'\n')
+            node_proc.stdin.flush()
+            ckey_resp = node_proc.stdout.readline().rstrip(r'\r\n')
+            ckey, tm, guid, flowid = ckey_resp.split()
+
+            vinfoparam = {
+                'otype': 'ojson',
+                'isHLS': 1,
+                'charge': 0,
+                'fhdswitch': 0,
+                'show1080p': 1,
+                'defnpayver': 7,
+                'sdtfrom': 'v1010',
+                'host': 'v.qq.com',
+                'vid': vid,
+                'defn': definition,
+                'platform': QQVideoPlatforms.P10201,
+                'appVer': self.app_ver,
+                'refer': referrer,
+                'ehost': vurl,
+                'logintoken': json.dumps(self.login_token, separators=(',', ':')),
+                'encryptVer': self.encrypt_ver,
+                'guid': guid,
+                'flowid': flowid,
+                'tm': tm,
+                'cKey': ckey,
+                'dtype': 3,
+                'spau': 1,
+                'spaudio': 68,
+                'spwm': 1,
+                'sphls': 2,
+                'sphttps': 1,
+                'clip': 4,
+                'spsrt': 2,
+                'spvvpay': 1,
+                'spadseg': 3,
+                'spav1': 15,
+                'hevclv': 28,
+                'spsfrhdr': 100,
+                'spvideo': 1044,
+                # 'drm': 40,
+                # 'spm3u8tag': 67,
+                # 'spmasterm3u8': 3
+            }
+            params = {
+                'buid': 'vinfoad',
+                'vinfoparam': urlencode(vinfoparam)
+            }
+
+            try:
+                r = self._requester.post(self._VIDEO_CONFIG_URL, json=params, cookies=self.user_token)
+                r.raise_for_status()
+                if r.status_code != 200:
+                    raise RequestException("Unexpected status code %i" % r.status_code)
+
+                try:
+                    data = json.loads(r.text)
+                    if data:
+                        data = json.loads(data.get('vinfo'))
+                except json.JSONDecodeError as e:
+                    self._logger.error("Received ill-formed video config info for '%i': '%r'", vid, e)
+                    return format_name, ext, urls
+
+                if data and data.get('dltype'):
+                    url_prefixes = []
+                    for url_dic in json_path_get(data, ['vl', 'vi', 0, 'ul', 'ui'], []):
+                        if isinstance(url_dic, dict):
+                            url = url_dic.get('url')
+                            if url and not url.startswith(self.cdn_blacklist):
+                                if not url.endswith('/'):
+                                    url = url[:url.rfind('/')+1]
+                                url_prefixes.append(url)
+
+                    chosen_url_prefixes = [prefix for prefix in url_prefixes if
+                                           prefix[:prefix.find('/', 8)].endswith('.tc.qq.com')]
+                    if not chosen_url_prefixes:
+                        chosen_url_prefixes = url_prefixes
+
+                    if self.use_cdn:
+                        # use all URL prefixes but with default servers coming before CDN mirrors
+                        cdn = [prefix for prefix in url_prefixes if prefix not in chosen_url_prefixes]
+                        chosen_url_prefixes += cdn
+
+                    drm = json_path_get(data, ['vl', 'vi', 0, 'drm'])
+                    preview = data.get('preview')
+
+                    formats_id2nm = {fmt.get('id'): fmt.get('name') for fmt in json_path_get(data, ['fl', 'fi'], [])}
+                    formats_nm2id = {fmt_nm: fmt_id for fmt_id, fmt_nm in formats_id2nm.items()}
+                    keyid = json_path_get(data, ['vl', 'vi', 0, 'keyid'], '')
+
+                    vfilename = json_path_get(data, ['vl', 'vi', 0, 'fn'], '')
+                    vfn = vfilename.rpartition('.')  # e.g. ['egmovie.f323013001', '.', 'ts']
+                    ext = vfn[-1]  # video extension, e.g. 'ts' 'mp4'
+
+                    ret_defn = ''  # not necessarily equal to requested `definition`
+
+                    if ext == 'ts':
+                        if drm == 1 and not preview and not self.has_vip:
+                            return format_name, ext, urls
+
+                        # determine the true definition `ret_defn` from the returned formats
+                        key_format_id = keyid.split('.')[-1]
+                        try:
+                            key_format_id = int(key_format_id)
+                            ret_defn = formats_id2nm.get(key_format_id) or ret_defn
+                        except ValueError:
+                            pass
+
+                        if not ret_defn:
+                            for format_defn in sort_definitions(formats_nm2id):
+                                format_id = formats_nm2id.get(format_defn)
+                                ckey_req = ' '.join([QQVideoPlatforms.P10201, self.app_ver, vid, vurl, referrer, r'\n'])
+                                node_proc.stdin.write(ckey_req)
+                                node_proc.stdin.flush()
+                                ckey_resp = node_proc.stdout.readline().rstrip(r'\r\n')
+                                ckey, tm, guid, flowid = ckey_resp.split()
+
+                                vkeyparam = {
+                                    'otype': 'ojson',
+                                    'vid': vid,
+                                    'format': format_id,
+                                    'filename': vfilename,
+                                    'platform': QQVideoPlatforms.P10201,
+                                    'appVer': self.app_ver,
+                                    'sdtfrom': 'v1010',
+                                    'guid': guid,
+                                    'flowid': flowid,
+                                    'tm': tm,
+                                    'refer': referrer,
+                                    'ehost': vurl,
+                                    'logintoken': json.dumps(self.login_token, separators=(',', ':')),
+                                    'encryptVer': self.encrypt_ver,
+                                    'cKey': ckey
+                                }
+                                params = {
+                                    'buid': 'onlyvkey',
+                                    'vkeyparam': urlencode(vkeyparam)
+                                }
+
+                                try:
+                                    r = self._requester.post(self._VIDEO_CONFIG_URL, json=params, cookies=self.user_token)
+                                    if r.status_code != 200:
+                                        raise RequestException("Unexpected status code %i" % r.status_code)
+
+                                    try:
+                                        key_data = json.loads(r.text)
+                                        if key_data:
+                                            key_data = json.loads(key_data.get('vkey'))
+                                    except json.JSONDecodeError as e:
+                                        self._logger.error("Received ill-formed video key data for the file '%s' of video '%i': '%r'", vfilename, vid, e)
+                                        return format_name, ext, urls
+
+                                    if key_data and isinstance(key_data, dict):
+                                        vkey = key_data.get('key')
+                                        if not vkey:
+                                            return format_name, ext, urls
+
+                                        cfilename = key_data.get('filename', '')
+                                        if cfilename and cfilename == vfilename:
+                                            ret_defn = format_defn
+                                            break
+                                except RequestException as e:
+                                    self._logger.error("Error while requesting the key for the file '%s' of video '%i': '%r'", vfilename, vid, e)
+                                    return format_name, ext, urls
+
+                        fc = json_path_get(data, ['vl', 'vi', 0, 'fc'])  # always >= 1?
+                        # start = 0 if fc == 0 else 1  # start counting number of the video clip file indexes
+                        start = 1
+
+                        for idx in range(start, fc + 1):
+                            vfilename_new = '.'.join([vfn[0], str(idx), 'ts'])
+                            url_mirrors = '\t'.join(
+                                ['%s%s?sdtfrom=v1010' % (prefix, vfilename_new) for prefix in chosen_url_prefixes])
+                            urls.append(url_mirrors)
+                    else:  # 'mp4'
+                        if drm == 1 and not self.has_vip:
+                            return format_name, ext, urls
+
+                        return self._get_video_urls_p10201(vid, definition, vurl, referrer)
+
+                    format_name = ret_defn
+            except RequestException as e:
+                self._logger.error("Error while requesting the config info of video '%i': '%r'", vid, e)
 
         return format_name, ext, urls
 
     def _get_video_urls(self, vid, definition, vurl, referrer):
         if self.no_logo:
-            return self._get_video_urls_p10801(vid, definition, vurl, referrer)
+            # return self._get_video_urls_p10801(vid, definition, vurl, referrer)
+            return self._get_video_urls_p10201_ts(vid, definition, vurl, referrer)
         else:
             # return self._get_video_urls_p10901(vid, definition)
             return self._get_video_urls_p10201(vid, definition, vurl, referrer)
 
     def _extract_video_cover_info(self, regex, text):
         result = (None, None)
 
@@ -529,57 +777,58 @@
             cover_group = cover_match.group(1) or cover_match.group(2)
             try:
                 cover_info = json.loads(cover_group.replace('undefined', 'null'))
             except json.JSONDecodeError:
                 return result
             if cover_info and isinstance(cover_info, dict):
                 info['title'] = cover_info.get('title', '') or cover_info.get('title_new', '')
-                info['year'] = cover_info.get('year', DEFAULT_YEAR)
+                info['year'] = cover_info.get('year') or (cover_info.get('publish_date') or '').split('-')[0]
                 info['cover_id'] = cover_info.get('cover_id', '')
 
                 type_id = int(cover_info.get('type') or VideoTypeCodes.MOVIE)
                 info['type'] = self._VQQ_TYPE_CODES.get(type_id, VideoTypes.MOVIE)
 
                 video_id = cover_info.get('vid')
                 if video_id is None:
                     video_ids = cover_info.get('video_ids') or []
                     normal_ids = [{'V': vid, 'E': ep} for ep, vid in enumerate(video_ids, start=1)]
                 else:
                     normal_ids = [{"V": video_id, "E": 1}]
                 info['normal_ids'] = normal_ids
 
-                result = (info, cover_match.end)
+                result = (info, cover_match.end())
 
         return result
 
     def _update_video_cover_info(self, cover_info, regex, text):
         match = regex.search(text)
         if match:
-            matched = match.group(1).replace('undefined', 'null')
+            matched = match.group(1)
+            matched_norm = re.sub(self._EP_LIST_RE, r'[{"list":[[\1]]}]', matched).replace('undefined', 'null')
             try:
-                conf_info = json.loads(matched)
+                conf_info = json.loads(matched_norm)
             except json.JSONDecodeError:
                 return
 
             if conf_info:
-                cover_info['year'] = json_path_get(conf_info, ['introduction', 'introData', 'list', 0, 'item_params', 'cover_year'])\
-                                     or json_path_get(conf_info, ['introduction', 'introData', 'list', 0, 'item_params', 'year'])\
-                                     or json_path_get(conf_info, ['introduction', 'introData', 'list', 0, 'item_params', 'show_year'])\
-                                     or cover_info['year']
+                year = json_path_get(conf_info, ['introduction', 'introData', 'list', 0, 'item_params', 'year']) \
+                       or json_path_get(conf_info, ['introduction', 'introData', 'list', 0, 'item_params', 'show_year'])
+                if year and (not cover_info['year'] or cover_info['year'] != year):
+                    cover_info['year'] = year
 
                 # set to the probably more specific title
-                ep_list = json_path_get(conf_info, ['episodeMain', 'listData'], [])
+                ep_list = json_path_get(conf_info, ['episodeMain', 'listData', 0, 'list'], [])
                 if not ep_list:
                     return
                 ep_list = ep_list[0]
 
                 if len(ep_list) >= len(cover_info['normal_ids']):  # ensure the full list of episodes
-                    cover_info['normal_ids'] = [{'V': item['item_params']['vid'],
+                    cover_info['normal_ids'] = [{'V': item['vid'],
                                                  'E': ep,
-                                                 'title': json_path_get(item, ['item_params', 'play_title']) or json_path_get(item, ['item_params', 'title'])
+                                                 'title': item.get('playTitle') or item.get('title', '')
                                                  # exclude the types of videos that are unlikely to have meaningful episode names
                                                  if cover_info['type'] not in [VideoTypes.TV, ] else ''}
                                                 for ep, item in enumerate(ep_list, start=1)]
 
     def _get_cover_info(self, cover_url):
         """"{
         "referrer": "https://v.qq.com/x/cover/nhtfh14i9y1egge.html",
@@ -597,29 +846,34 @@
             "E": 2,
             # "title": ""
         }]
         }"""
 
         info = None
 
-        r = self._requester.get(cover_url)
-        if r.status_code == 200:
+        try:
+            r = self._requester.get(cover_url)
+            if r.status_code != 200:
+                raise RequestException("Unexpected status code %i" % r.status_code)
+
             r.encoding = 'utf-8'
             info, pos_end = self._extract_video_cover_info(self._COVER_PAT_RE, r.text)
             if info:
                 if not info['normal_ids']:
                     info, _ = self._extract_video_cover_info(self._VIDEO_INFO_RE, r.text[pos_end:])
             else:
                 info, _ = self._extract_video_cover_info(self._VIDEO_INFO_RE, r.text)
 
-        if info:
-            self._update_video_cover_info(info, self._ALL_LOADED_INFO_RE, r.text)
+            if info:
+                self._update_video_cover_info(info, self._ALL_LOADED_INFO_RE, r.text)
 
-            info['episode_all'] = len(info['normal_ids']) if info['normal_ids'] else 1
-            info['referrer'] = cover_url  # set the Referer to the address of the cover web page
+                info['episode_all'] = len(info['normal_ids']) if info['normal_ids'] else 1
+                info['referrer'] = cover_url  # set the Referer to the address of the cover web page
+        except RequestException as e:
+            self._logger.error("Error while requesting the webpage '%s': '%r'", cover_url, e)
 
         return info
 
     def get_cover_info(self, videourl):
         cover_info = None
         for typ, pat in enumerate(self._VIDEO_URL_PATS, 1):
             match = pat['cpat'].match(videourl)
```

### Comparing `movie-downloader-0.1.7/mdl/third_parties/setupext_janitor/janitor.py` & `movie-downloader-0.2.5/mdl/third_parties/setupext_janitor/janitor.py`

 * *Files identical despite different names*

### Comparing `movie-downloader-0.1.7/mdl/third_parties/setupext_janitor/README.rst` & `movie-downloader-0.2.5/mdl/third_parties/setupext_janitor/README.rst`

 * *Files identical despite different names*

### Comparing `movie-downloader-0.1.7/mdl/third_parties/__init__.py` & `movie-downloader-0.2.5/mdl/third_parties/__init__.py`

 * *Files identical despite different names*

### Comparing `movie-downloader-0.1.7/mdl/utils.py` & `movie-downloader-0.2.5/mdl/utils.py`

 * *Files identical despite different names*

### Comparing `movie-downloader-0.1.7/mdl/__init__.py` & `movie-downloader-0.2.5/mdl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 
 def arg_parser():
     parser = ArgumentParser()
 
     parser.add_argument('url', nargs='+', help='Episode or cover/playlist web page URL(s)')
     parser.add_argument('-D', '--dir', default='', dest='dir', help='path to downloaded videos')
-    parser.add_argument('-d', '--definition', default='', dest='definition', choices=['fhd', 'shd', 'hd', 'sd'])
+    parser.add_argument('-d', '--definition', default='', dest='definition', choices=['dolby', 'sfr_hdr', 'hdr10', 'uhd', 'fhd', 'shd', 'hd', 'sd'])
     parser.add_argument('-p', '--proxy', dest='proxy', help='proxy in the form of "http://[user:password@]host:port"')
     parser.add_argument('--playlist-items', default='', dest='playlist_items', type=_segment_playlist_items,
                         help='desired episode indices in a playlist separated by commas, while the playlists are separated by semicolons,'
                              'e.g. "--playlist-items 1,2,5-10", "--playlist-items 1,2,5-10;3-", and "--playlist-items 1,2,5-10;;-20"')
 
     parser.add_argument('--QQVideo-no-logo', dest='QQVideo_no_logo', default='', choices=['True', 'False'])
 
@@ -125,15 +125,15 @@
     con_log_level = getattr(logging, con_log_level.upper())
 
     confs['misc']['log_level'] = con_log_level
 
 
 def parse_dlops_default(args, confs):
     save_dir_default = '.'
-    definition_default = 'fhd'
+    definition_default = 'uhd'
 
     for site in confs:
         if site not in ('misc', 'progs'):
             save_dir = args.dir or confs[site]['dir'] or save_dir_default
             confs[site]['dir'] = save_dir
             # Validate the file save directory
             if not (os.path.exists(save_dir) and os.path.isdir(save_dir)):
```

### Comparing `movie-downloader-0.1.7/PKG-INFO` & `movie-downloader-0.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: movie-downloader
-Version: 0.1.7
+Version: 0.2.5
 Summary: A fast movie downloader using Aria2
 Home-page: https://github.com/Jesseatgao/movie-downloader
 Author: Jesse Gao
 Author-email: changxigao@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Intended Audience :: End Users/Desktop
@@ -72,28 +72,28 @@
         https://www.johnvansickle.com/ffmpeg/old-releases/ffmpeg-4.2.2-amd64-static.tar.xz
         
 * [MKVToolnix(mkvmerge)](https://github.com/Jesseatgao/MKVToolNix-static-builds)
     * For Windows:
     
         i686 32-bit version:
     
-        https://github.com/Jesseatgao/MKVToolNix-static-builds/releases/download/v47.0.0-mingw-w64-win32v1.0/mkvtoolnix-i686-win.zip
+        https://github.com/Jesseatgao/MKVToolNix-static-builds/releases/download/v58.0.0-mingw-w64-win32v1.4/mkvtoolnix-i686-win.zip
         
         x86_64 64-bit version:
         
-        https://github.com/Jesseatgao/MKVToolNix-static-builds/releases/download/v47.0.0-mingw-w64-win32v1.0/mkvtoolnix-x86_64-win.zip
+        https://github.com/Jesseatgao/MKVToolNix-static-builds/releases/download/v58.0.0-mingw-w64-win32v1.4/mkvtoolnix-x86_64-win.zip
     * For Linux:
     
         i686 32-bit version:
         
-        https://github.com/Jesseatgao/MKVToolNix-static-builds/releases/download/v47.0.0-mingw-w64-win32v1.0/mkvtoolnix-i686-linux.tar.xz
+        https://github.com/Jesseatgao/MKVToolNix-static-builds/releases/download/v58.0.0-mingw-w64-win32v1.4/mkvtoolnix-i686-linux.tar.xz
 
         x86_64 64-bit version:
         
-        https://github.com/Jesseatgao/MKVToolNix-static-builds/releases/download/v47.0.0-mingw-w64-win32v1.0/mkvtoolnix-x86_64-linux.tar.xz
+        https://github.com/Jesseatgao/MKVToolNix-static-builds/releases/download/v58.0.0-mingw-w64-win32v1.4/mkvtoolnix-x86_64-linux.tar.xz
         
 * [node](https://nodejs.org)
     * For Windows:
     
         i686 32-bit version:
     
         https://nodejs.org/dist/v16.15.0/node-v16.15.0-win-x86.zip
@@ -135,24 +135,24 @@
 
   Download, unzip and extract `aria2`, `ffmpeg`, `mkvmerge`, `node` and `ckey` into the directory
  `third_parties/aria2/`, `third_parties/ffmpeg/`, `third_parties/mkvtoolnix/`, `third_parties/node/` and `third_parties/ckey/`
  according to the target platform, respectively.
 
 ### Usage
 ```
-mdl [-h] [-D DIR] [-d {fhd,shd,hd,sd}] [-p PROXY] [--QQVideo-no-logo {True,False}]
+mdl [-h] [-D DIR] [-d {uhd,fhd,shd,hd,sd}] [-p PROXY] [--QQVideo-no-logo {True,False}]
     [-A ARIA2C] [-F FFMPEG] [-M MKVMERGE] [-N NODE] [-L {debug,info,warning,error,critical}]
     url [url ...] [--playlist-items PLAYLIST_ITEMS]
 ```
 
 **Description**:
 
 `-D DIR`: specify _DIR_ to save downloaded videos.
 
-`-d {fhd,shd,hd,sd}`: specify the definition of the video to download. `fhd,shd,hd,sd` correspond to `1080P, 720P, 480P, 270P` respectively.
+`-d {uhd,fhd,shd,hd,sd}`: specify the definition of the video to download. `uhd,fhd,shd,hd,sd` correspond to `4K, 1080P, 720P, 480P, 270P` respectively.
 
 `-p PROXY`: specify the proxy server _PROXY_ (in the form of `http://[user:password@]host:port`)
     used to get web pages or download videos (if configured in `conf/dlops.conf`).
 
 `--QQVideo-no-logo {True,False}`: indicate whether we're trying to download no-watermarked QQVideos or not.
 
 `-A ARIA2C`: specify the absolute path to `aria2c` executable, which takes precedence over the configuration in `conf/misc.conf`
```

### Comparing `movie-downloader-0.1.7/README.md` & `movie-downloader-0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,28 +47,28 @@
         https://www.johnvansickle.com/ffmpeg/old-releases/ffmpeg-4.2.2-amd64-static.tar.xz
         
 * [MKVToolnix(mkvmerge)](https://github.com/Jesseatgao/MKVToolNix-static-builds)
     * For Windows:
     
         i686 32-bit version:
     
-        https://github.com/Jesseatgao/MKVToolNix-static-builds/releases/download/v47.0.0-mingw-w64-win32v1.0/mkvtoolnix-i686-win.zip
+        https://github.com/Jesseatgao/MKVToolNix-static-builds/releases/download/v58.0.0-mingw-w64-win32v1.4/mkvtoolnix-i686-win.zip
         
         x86_64 64-bit version:
         
-        https://github.com/Jesseatgao/MKVToolNix-static-builds/releases/download/v47.0.0-mingw-w64-win32v1.0/mkvtoolnix-x86_64-win.zip
+        https://github.com/Jesseatgao/MKVToolNix-static-builds/releases/download/v58.0.0-mingw-w64-win32v1.4/mkvtoolnix-x86_64-win.zip
     * For Linux:
     
         i686 32-bit version:
         
-        https://github.com/Jesseatgao/MKVToolNix-static-builds/releases/download/v47.0.0-mingw-w64-win32v1.0/mkvtoolnix-i686-linux.tar.xz
+        https://github.com/Jesseatgao/MKVToolNix-static-builds/releases/download/v58.0.0-mingw-w64-win32v1.4/mkvtoolnix-i686-linux.tar.xz
 
         x86_64 64-bit version:
         
-        https://github.com/Jesseatgao/MKVToolNix-static-builds/releases/download/v47.0.0-mingw-w64-win32v1.0/mkvtoolnix-x86_64-linux.tar.xz
+        https://github.com/Jesseatgao/MKVToolNix-static-builds/releases/download/v58.0.0-mingw-w64-win32v1.4/mkvtoolnix-x86_64-linux.tar.xz
         
 * [node](https://nodejs.org)
     * For Windows:
     
         i686 32-bit version:
     
         https://nodejs.org/dist/v16.15.0/node-v16.15.0-win-x86.zip
@@ -110,24 +110,24 @@
 
   Download, unzip and extract `aria2`, `ffmpeg`, `mkvmerge`, `node` and `ckey` into the directory
  `third_parties/aria2/`, `third_parties/ffmpeg/`, `third_parties/mkvtoolnix/`, `third_parties/node/` and `third_parties/ckey/`
  according to the target platform, respectively.
 
 ### Usage
 ```
-mdl [-h] [-D DIR] [-d {fhd,shd,hd,sd}] [-p PROXY] [--QQVideo-no-logo {True,False}]
+mdl [-h] [-D DIR] [-d {uhd,fhd,shd,hd,sd}] [-p PROXY] [--QQVideo-no-logo {True,False}]
     [-A ARIA2C] [-F FFMPEG] [-M MKVMERGE] [-N NODE] [-L {debug,info,warning,error,critical}]
     url [url ...] [--playlist-items PLAYLIST_ITEMS]
 ```
 
 **Description**:
 
 `-D DIR`: specify _DIR_ to save downloaded videos.
 
-`-d {fhd,shd,hd,sd}`: specify the definition of the video to download. `fhd,shd,hd,sd` correspond to `1080P, 720P, 480P, 270P` respectively.
+`-d {uhd,fhd,shd,hd,sd}`: specify the definition of the video to download. `uhd,fhd,shd,hd,sd` correspond to `4K, 1080P, 720P, 480P, 270P` respectively.
 
 `-p PROXY`: specify the proxy server _PROXY_ (in the form of `http://[user:password@]host:port`)
     used to get web pages or download videos (if configured in `conf/dlops.conf`).
 
 `--QQVideo-no-logo {True,False}`: indicate whether we're trying to download no-watermarked QQVideos or not.
 
 `-A ARIA2C`: specify the absolute path to `aria2c` executable, which takes precedence over the configuration in `conf/misc.conf`
```

### Comparing `movie-downloader-0.1.7/setup.py` & `movie-downloader-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 setup(
     name='movie-downloader',
     version=version,
     package_dir={'': '.'},
     packages=find_packages(where='.'),
     python_requires='>=3.6',
-    install_requires=['bdownload'],
+    install_requires=['bdownload>=0.2.0'],
     include_package_data=True,
     package_data={
         'mdl': [
             'log/mdl.log',
             'conf/*.conf',
             'js/*',
             'third_parties/aria2/README',
```

