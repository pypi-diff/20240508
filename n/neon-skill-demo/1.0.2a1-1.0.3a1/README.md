# Comparing `tmp/neon-skill-demo-1.0.2a1.tar.gz` & `tmp/neon-skill-demo-1.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-demo-1.0.2a1.tar", last modified: Tue Dec 19 00:47:28 2023, max compression
+gzip compressed data, was "neon-skill-demo-1.0.3a1.tar", last modified: Wed May  8 18:52:50 2024, max compression
```

## Comparing `neon-skill-demo-1.0.2a1.tar` & `neon-skill-demo-1.0.3a1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 00:47:28.502242 neon-skill-demo-1.0.2a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2023-12-19 00:47:28.498242 neon-skill-demo-1.0.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      776 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    13461 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 00:47:28.494243 neon-skill-demo-1.0.2a1/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 00:47:28.498242 neon-skill-demo-1.0.2a1/locale/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/locale/en-us/ask_demo.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/locale/en-us/ask_demo_next_time.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/locale/en-us/confirm_demo_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/locale/en-us/confirm_demo_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      162 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/locale/en-us/demo.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/locale/en-us/finished_demo.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/locale/en-us/mall_demo.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/locale/en-us/show_demo.intent
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/locale/en-us/starting_demo.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 00:47:28.498242 neon-skill-demo-1.0.2a1/locale/uk-ua/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/locale/uk-ua/ask_demo.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/locale/uk-ua/ask_demo_next_time.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/locale/uk-ua/confirm_demo_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/locale/uk-ua/confirm_demo_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      340 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/locale/uk-ua/demo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/locale/uk-ua/finished_demo.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      212 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/locale/uk-ua/show_demo.intent
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/locale/uk-ua/starting_demo.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 00:47:28.498242 neon-skill-demo-1.0.2a1/neon_skill_demo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2023-12-19 00:47:28.000000 neon-skill-demo-1.0.2a1/neon_skill_demo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      887 2023-12-19 00:47:28.000000 neon-skill-demo-1.0.2a1/neon_skill_demo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 00:47:28.000000 neon-skill-demo-1.0.2a1/neon_skill_demo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-12-19 00:47:28.000000 neon-skill-demo-1.0.2a1/neon_skill_demo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2023-12-19 00:47:28.000000 neon-skill-demo-1.0.2a1/neon_skill_demo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-19 00:47:28.000000 neon-skill-demo-1.0.2a1/neon_skill_demo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 00:47:28.502242 neon-skill-demo-1.0.2a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 00:47:28.498242 neon-skill-demo-1.0.2a1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     6236 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2023-12-19 00:47:25.000000 neon-skill-demo-1.0.2a1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:52:50.765175 neon-skill-demo-1.0.3a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 18:52:50.765175 neon-skill-demo-1.0.3a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13420 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:52:50.761175 neon-skill-demo-1.0.3a1/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:52:50.765175 neon-skill-demo-1.0.3a1/locale/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/locale/en-us/ask_demo.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/locale/en-us/ask_demo_next_time.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/locale/en-us/confirm_demo_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/locale/en-us/confirm_demo_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/locale/en-us/demo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/locale/en-us/finished_demo.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/locale/en-us/mall_demo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/locale/en-us/show_demo.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/locale/en-us/starting_demo.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:52:50.765175 neon-skill-demo-1.0.3a1/locale/uk-ua/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/locale/uk-ua/ask_demo.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/locale/uk-ua/ask_demo_next_time.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/locale/uk-ua/confirm_demo_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/locale/uk-ua/confirm_demo_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/locale/uk-ua/demo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/locale/uk-ua/finished_demo.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/locale/uk-ua/show_demo.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/locale/uk-ua/starting_demo.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:52:50.765175 neon-skill-demo-1.0.3a1/neon_skill_demo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 18:52:50.000000 neon-skill-demo-1.0.3a1/neon_skill_demo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-08 18:52:50.000000 neon-skill-demo-1.0.3a1/neon_skill_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:52:50.000000 neon-skill-demo-1.0.3a1/neon_skill_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-08 18:52:50.000000 neon-skill-demo-1.0.3a1/neon_skill_demo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 18:52:50.000000 neon-skill-demo-1.0.3a1/neon_skill_demo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 18:52:50.000000 neon-skill-demo-1.0.3a1/neon_skill_demo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:52:50.765175 neon-skill-demo-1.0.3a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:52:50.765175 neon-skill-demo-1.0.3a1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     6236 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-08 18:52:47.000000 neon-skill-demo-1.0.3a1/version.py
```

### Comparing `neon-skill-demo-1.0.2a1/LICENSE.md` & `neon-skill-demo-1.0.3a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-demo-1.0.2a1/PKG-INFO` & `neon-skill-demo-1.0.3a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-demo
-Version: 1.0.2a1
+Version: 1.0.3a1
 Home-page: https://github.com/NeonGeckoCom/skill-demo
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-demo-1.0.2a1/README.md` & `neon-skill-demo-1.0.3a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-demo-1.0.2a1/__init__.py` & `neon-skill-demo-1.0.3a1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,28 +40,39 @@
 from neon_utils.message_utils import get_message_user, dig_for_message
 from neon_utils.signal_utils import wait_for_signal_clear
 from neon_utils.skills import NeonSkill
 from neon_utils.user_utils import get_user_prefs
 from neon_utils.file_utils import load_commented_file
 from ovos_config.locations import get_xdg_data_save_path
 from ovos_plugin_manager.templates import TTS
-from ovos_utils.sound import play_wav
+from ovos_utils.sound import play_audio
 from ovos_workshop.decorators import intent_handler
 from ovos_workshop.resource_files import find_resource
 
 
 class DemoSkill(NeonSkill):
     def __init__(self, **kwargs):
         NeonSkill.__init__(self, **kwargs)
         self._active_demos = dict()
         self._audio_output_done = Event()
         self._prompt_handled = Event()
         self._last_response = None
         self._data_path = get_xdg_data_save_path()
 
+        # When demo prompt enabled, wait for load and prompt user
+        if self.prompt_on_start:
+            self.add_event('mycroft.ready', self._show_demo_prompt)
+        self.add_event("recognizer_loop:audio_output_start",
+                       self._audio_started)
+        self.add_event("recognizer_loop:audio_output_end",
+                       self._audio_stopped)
+        self.add_event("mycroft.mic.listen", self._mic_listen)
+        self.add_event("mycroft.skill.handler.complete",
+                       self._handler_complete)
+
     @classproperty
     def runtime_requirements(self):
         return RuntimeRequirements(network_before_load=False,
                                    internet_before_load=False,
                                    gui_before_load=False,
                                    requires_internet=False,
                                    requires_network=False,
@@ -99,24 +110,14 @@
         """
         return self.settings.get("filename") or "demo.txt"
 
     @property
     def prompt_on_start(self):
         return self.settings.get("prompt_on_start", True)
 
-    def initialize(self):
-        # When demo prompt enabled, wait for load and prompt user
-        if self.settings.get("prompt_on_start"):
-            self.bus.once('mycroft.ready', self._show_demo_prompt)
-        self.add_event("recognizer_loop:audio_output_start",
-                       self._audio_started)
-        self.add_event("recognizer_loop:audio_output_end", self._audio_stopped)
-        self.add_event("mycroft.mic.listen", self._mic_listen)
-        self.add_event("mycroft.skill.handler.complete", self._handler_complete)
-
     def _audio_started(self, _):
         # TODO: Handle audio per-user
         self._audio_output_done.clear()
 
     def _audio_stopped(self, _):
         # TODO: Handle audio per-user
         self._audio_output_done.set()
@@ -263,17 +264,16 @@
         :param prompter: Speaker config to use for spoken prompts
         """
         self._audio_output_done.wait(self.speak_timeout)
         if tts:
             # If available, use skill-managed TTS
             _, output_file = mkstemp()
             wav_file, _ = tts.get_tts(prompt, output_file)
-            # TODO: If server, self.send_with_audio
-            play_wav(wav_file,
-                     self.config_core.get("play_wav_cmdline")).wait(
+            play_audio(wav_file,
+                       self.config_core.get("play_wav_cmdline")).wait(
                 self.speak_timeout)
         else:
             # Else fallback to audio module (probably same voice
             self.speak(prompt, speaker=prompter)
             self._audio_output_done.wait(self.speak_timeout)
 
     def _get_demo_tts(self, lang: str = None) -> Optional[TTS]:
```

### Comparing `neon-skill-demo-1.0.2a1/neon_skill_demo.egg-info/PKG-INFO` & `neon-skill-demo-1.0.3a1/neon_skill_demo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-demo
-Version: 1.0.2a1
+Version: 1.0.3a1
 Home-page: https://github.com/NeonGeckoCom/skill-demo
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-demo-1.0.2a1/neon_skill_demo.egg-info/SOURCES.txt` & `neon-skill-demo-1.0.3a1/neon_skill_demo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-demo-1.0.2a1/setup.py` & `neon-skill-demo-1.0.3a1/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-demo-1.0.2a1/skill.json` & `neon-skill-demo-1.0.3a1/skill.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978354978354979%*

 * *Differences: {"'requirements'": "{'python': {insert: [(1, 'neon-utils~=1.8'), (4, 'ovos-utils~=0.0, "*

 * *                   ">=0.0.28')], delete: [4, 1]}}"}*

```diff
@@ -24,18 +24,18 @@
         "ia64",
         "arm64",
         "arm"
     ],
     "requirements": {
         "python": [
             "neon-tts-plugin-audiofiles~=0.0.2",
-            "neon-utils~=1.0,>=1.2.2",
+            "neon-utils~=1.8",
             "ovos-bus-client~=0.0.3",
             "ovos-plugin-manager~=0.0.21",
-            "ovos-utils~=0.0.28"
+            "ovos-utils~=0.0, >=0.0.28"
         ],
         "skill": [],
         "system": {}
     },
     "short_description": "Skill to demo Neon capabilities",
     "skillname": "skill-demo",
     "summary": "Skill to demo Neon capabilities",
```

### Comparing `neon-skill-demo-1.0.2a1/test/test_skill.py` & `neon-skill-demo-1.0.3a1/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-demo-1.0.2a1/version.py` & `neon-skill-demo-1.0.3a1/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.2a1"
+__version__ = "1.0.3a1"
```

