# Comparing `tmp/emunium-1.5.0.tar.gz` & `tmp/emunium-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emunium-1.5.0.tar", last modified: Sun Apr 21 05:26:24 2024, max compression
+gzip compressed data, was "emunium-2.0.0.tar", last modified: Tue May  7 06:21:54 2024, max compression
```

## Comparing `emunium-1.5.0.tar` & `emunium-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 05:26:24.000730 emunium-1.5.0/
--rw-rw-rw-   0        0        0     1080 2024-04-19 11:50:43.000000 emunium-1.5.0/LICENSE
--rw-rw-rw-   0        0        0       34 2024-04-19 11:50:43.000000 emunium-1.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4270 2024-04-21 05:26:24.000730 emunium-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     3462 2024-04-21 05:00:46.000000 emunium-1.5.0/README.MD
-drwxrwxrwx   0        0        0        0 2024-04-21 05:26:23.993750 emunium-1.5.0/emunium/
--rw-rw-rw-   0        0        0       22 2024-04-19 11:50:43.000000 emunium-1.5.0/emunium/__init__.py
--rw-rw-rw-   0        0        0     7276 2024-04-21 05:25:05.000000 emunium-1.5.0/emunium/emunium.py
-drwxrwxrwx   0        0        0        0 2024-04-21 05:26:23.999733 emunium-1.5.0/emunium.egg-info/
--rw-rw-rw-   0        0        0     4270 2024-04-21 05:26:23.000000 emunium-1.5.0/emunium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2024-04-21 05:26:23.000000 emunium-1.5.0/emunium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 05:26:23.000000 emunium-1.5.0/emunium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-21 05:26:23.000000 emunium-1.5.0/emunium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-21 05:26:23.000000 emunium-1.5.0/emunium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 05:26:24.001727 emunium-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1096 2024-04-21 05:10:00.000000 emunium-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:21:54.378263 emunium-2.0.0/
+-rw-rw-rw-   0        0        0     1080 2024-05-07 03:40:54.000000 emunium-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0      119 2024-05-07 06:18:07.000000 emunium-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6692 2024-05-07 06:21:54.378263 emunium-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5995 2024-05-07 06:16:57.000000 emunium-2.0.0/README.MD
+drwxrwxrwx   0        0        0        0 2024-05-07 06:21:54.373949 emunium-2.0.0/emunium/
+-rw-rw-rw-   0        0        0       79 2024-05-07 06:01:28.000000 emunium-2.0.0/emunium/__init__.py
+-rw-rw-rw-   0        0        0     4527 2024-05-07 05:58:13.000000 emunium-2.0.0/emunium/base.py
+-rw-rw-rw-   0        0        0     4571 2024-05-07 06:01:47.000000 emunium-2.0.0/emunium/browsers.py
+-rw-rw-rw-   0        0        0     2305 2024-05-07 06:02:03.000000 emunium-2.0.0/emunium/standalone.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:21:54.377240 emunium-2.0.0/emunium.egg-info/
+-rw-rw-rw-   0        0        0     6692 2024-05-07 06:21:54.000000 emunium-2.0.0/emunium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2024-05-07 06:21:54.000000 emunium-2.0.0/emunium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 06:21:54.000000 emunium-2.0.0/emunium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-07 06:21:54.000000 emunium-2.0.0/emunium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-07 06:21:54.000000 emunium-2.0.0/emunium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 06:21:54.378263 emunium-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      987 2024-05-07 06:19:10.000000 emunium-2.0.0/setup.py
```

### Comparing `emunium-1.5.0/LICENSE` & `emunium-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `emunium-1.5.0/emunium/emunium.py` & `emunium-2.0.0/emunium/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,186 +6,123 @@
 import time
 import struct
 
 import keyboard
 import pyautogui
 import pyclick
 
+from enum import Enum
+
+class ClickType(Enum):
+    LEFT = 0
+    RIGHT = 1
+    MIDDLE = 2
+    DOUBLE = 3
+
 def get_image_size(file_path):
     with open(file_path, 'rb') as file:
         file.seek(16)
         width_bytes = file.read(4)
         height_bytes = file.read(4)
         width = struct.unpack('>I', width_bytes)[0]
         height = struct.unpack('>I', height_bytes)[0]
         return (width, height,)
 
-class EmuniumSelenium:
-    def __init__(self, driver):
-        self.driver = driver
+
+class EmuniumBase:
+    def __init__(self):
         self.clicker = pyclick.HumanClicker()
+        self._extend_clicker()
         self.browser_offsets = ()
         self.browser_inner_window = ()
-        
-    def _get_browser_properties_if_not_found(self):
+
+    def _extend_clicker(self):
+        def right_click(self):
+            pyautogui.click(button='right')
+
+        def middle_click(self):
+            pyautogui.click(button='middle')
+
+        def double_click(self):
+            pyautogui.doubleClick()
+
+        self.clicker.right_click = right_click.__get__(self.clicker)
+        self.clicker.middle_click = middle_click.__get__(self.clicker)
+        self.clicker.double_click = double_click.__get__(self.clicker)
+
+    async def _get_browser_properties_if_not_found(self, screenshot_func):
         if not self.browser_offsets or not self.browser_inner_window:
             with tempfile.NamedTemporaryFile(suffix='.png', delete=False) as temp_file:
                 temp_screen_path = temp_file.name
-            self.driver.save_screenshot(temp_screen_path)
+            if asyncio.iscoroutinefunction(screenshot_func):
+                await screenshot_func(temp_screen_path)
+            else:
+                screenshot_func(temp_screen_path)
             location = pyautogui.locateOnScreen(temp_screen_path, confidence=0.8)
             self.browser_offsets = (location.left, location.top,)
             self.browser_inner_window = get_image_size(temp_screen_path)
             os.remove(temp_screen_path)
 
-    def get_center(self, element):
-        self._get_browser_properties_if_not_found()
-
-        element_location = element.location
+    def _get_center(self, element_location, element_size):
         offset_to_screen_x, offset_to_screen_y = self.browser_offsets
         element_x = element_location['x'] + offset_to_screen_x
         element_y = element_location['y'] + offset_to_screen_y
 
-        element_size = element.size
         centered_x = element_x + (element_size['width'] // 2)
         centered_y = element_y + (element_size['height'] // 2)
-    
+
         return {
             'x': centered_x,
             'y': centered_y
         }
 
-    def find_and_move(self, element, click=False, offset_x=random.uniform(0.0, 1.5), offset_y=random.uniform(0.0, 1.5)):
-        center = self.get_center(element)
+    def _move(self, center, offset_x=random.uniform(0.0, 1.5), offset_y=random.uniform(0.0, 1.5)):
         target_x, target_y = round(center['x'] + offset_x), round(center['y'] + offset_y)
 
         current_x, current_y = pyautogui.position()
         distance = math.sqrt((target_x - current_x) ** 2 + (target_y - current_y) ** 2)
 
         speed = max(random.uniform(0.3, 0.6), min(random.uniform(2.0, 2.5), distance / random.randint(500, 700)))
 
         self.clicker.move((target_x, target_y), speed)
 
-        if click:
+    def _click(self, click_type=ClickType.LEFT):
+        if click_type == ClickType.LEFT:
             self.clicker.click()
+        elif click_type == ClickType.RIGHT:
+            self.clicker.right_click()
+        elif click_type == ClickType.MIDDLE:
+            self.clicker.middle_click()
+        elif click_type == ClickType.DOUBLE:
+            self.clicker.double_click()
 
     def silent_type(self, text, characters_per_minute=280, offset=20):
         total_chars = len(text)
         time_per_char = 60 / characters_per_minute
 
         for i, char in enumerate(text):
             randomized_offset = random.uniform(-offset, offset) / 1000
             delay = time_per_char + randomized_offset
 
             keyboard.write(char)
             time.sleep(delay)
 
-    def scroll_smoothly_to_element(self, element):
-        self._get_browser_properties_if_not_found()
-
-        element_rect = element.rect        
+    def _scroll_smoothly_to_element(self, element_rect):
         window_width = self.browser_inner_window[0]
         window_height = self.browser_inner_window[1]
-        
+
         scroll_amount = element_rect['y'] - window_height // 2
         scroll_steps = abs(scroll_amount) // 100
-        
+
         if scroll_amount > 0:
             scroll_direction = -1
         else:
             scroll_direction = 1
-        
+
         for _ in range(scroll_steps):
             pyautogui.scroll(scroll_direction * 100)
             time.sleep(random.uniform(0.05, 0.1))
-        
-        remaining_scroll = scroll_amount % 100
-        if remaining_scroll != 0:
-            pyautogui.scroll(scroll_direction * remaining_scroll)
-            time.sleep(random.uniform(0.05, 0.1))
 
-class EmuniumPpeteer:
-    def __init__(self, page):
-        self.page = page        
-        self.clicker = pyclick.HumanClicker()
-        self.browser_offsets = ()
-        self.browser_inner_window = ()
-
-    async def _get_browser_properties_if_not_found(self):
-        if not self.browser_offsets or not self.browser_inner_window:
-            with tempfile.NamedTemporaryFile(suffix='.png', delete=False) as temp_file:
-                temp_screen_path = temp_file.name
-            await self.page.screenshot(path=temp_screen_path)
-            location = pyautogui.locateOnScreen(temp_screen_path, confidence=0.8)
-            self.browser_offsets = (location.left, location.top,)
-            self.browser_inner_window = get_image_size(temp_screen_path)
-            os.remove(temp_screen_path)
-
-    async def get_center(self, element):
-        await self._get_browser_properties_if_not_found()
-
-        rect = await element.boundingBox()
-        if rect is None:
-            return None
-
-        offset_to_screen_x, offset_to_screen_y = self.browser_offsets
-        element_x = rect['x'] + offset_to_screen_x
-        element_y = rect['y'] + offset_to_screen_y
-        element_width = rect['width']
-        element_height = rect['height']
-        centered_x = element_x + (element_width // 2)
-        centered_y = element_y + (element_height // 2)
-        return {
-            'x': centered_x,
-            'y': centered_y
-        }
-
-    async def find_and_move(self, element, click=False, offset_x=random.uniform(0.0, 1.5), offset_y=random.uniform(0.0, 1.5)):
-        center = await self.get_center(element)        
-        target_x, target_y = round(center['x'] + offset_x), round(center['y'] + offset_y)
-
-        current_x, current_y = pyautogui.position()
-        distance = math.sqrt((target_x - current_x) ** 2 + (target_y - current_y) ** 2)
-
-        speed = max(random.uniform(0.3, 0.6), min(random.uniform(2.0, 2.5), distance / random.randint(500, 700)))
-
-        self.clicker.move((target_x, target_y), speed)
-
-        if click:
-            self.clicker.click()
-
-    async def silent_type(self, text, characters_per_minute=280, offset=20):
-        total_chars = len(text)
-        time_per_char = 60 / characters_per_minute
-
-        for i, char in enumerate(text):
-            randomized_offset = random.uniform(-offset, offset) / 1000
-            delay = time_per_char + randomized_offset
-
-            keyboard.write(char)
-            await asyncio.sleep(delay)
-
-    async def scroll_smoothly_to_element(self, element):
-        await self._get_browser_properties_if_not_found()
-
-        element_rect = await element.boundingBox()
-        if element_rect is None:
-            return None
-
-        window_width = self.browser_inner_window[0]
-        window_height = self.browser_inner_window[1]
-        
-        scroll_amount = element_rect['y'] - window_height // 2
-        scroll_steps = abs(scroll_amount) // 100
-        
-        if scroll_amount > 0:
-            scroll_direction = -1
-        else:
-            scroll_direction = 1
-        
-        for _ in range(scroll_steps):
-            pyautogui.scroll(scroll_direction * 100)
-            await asyncio.sleep(random.uniform(0.05, 0.1))
-        
         remaining_scroll = scroll_amount % 100
         if remaining_scroll != 0:
             pyautogui.scroll(scroll_direction * remaining_scroll)
-            await asyncio.sleep(random.uniform(0.05, 0.1))
+            time.sleep(random.uniform(0.05, 0.1))
```

### Comparing `emunium-1.5.0/setup.py` & `emunium-2.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='emunium',
-    version='1.5.0',
+    version='2.0.0',
     author='Maehdakvan',
     author_email='visitanimation@google.com',
-    description='A Python module for automating interactions to mimic human behavior in browsers when using Selenium or Pyppeteer. Provides utilities to programmatically move the mouse cursor, click on page elements, type text, and scroll as if performed by a human user.',
+    description='A Python module for automating interactions to mimic human behavior in standalone apps or browsers when using Selenium, Pyppeteer, or Playwright.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/DedInc/emunium',
     project_urls={
         'Bug Tracker': 'https://github.com/DedInc/emunium/issues',
     },
     classifiers=[
```

