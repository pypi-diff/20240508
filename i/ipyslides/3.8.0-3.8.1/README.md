# Comparing `tmp/ipyslides-3.8.0.tar.gz` & `tmp/ipyslides-3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyslides-3.8.0.tar", last modified: Mon May  6 20:08:00 2024, max compression
+gzip compressed data, was "ipyslides-3.8.1.tar", last modified: Wed May  8 00:54:13 2024, max compression
```

## Comparing `ipyslides-3.8.0.tar` & `ipyslides-3.8.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 20:08:00.052967 ipyslides-3.8.0/
--rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.8.0/LICENSE
--rw-rw-rw-   0        0        0     5382 2024-05-06 20:08:00.052967 ipyslides-3.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.8.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 20:08:00.018868 ipyslides-3.8.0/ipyslides/
--rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.8.0/ipyslides/__init__.py
--rw-rw-rw-   0        0        0       25 2024-05-06 20:00:02.000000 ipyslides-3.8.0/ipyslides/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 20:08:00.052967 ipyslides-3.8.0/ipyslides/_base/
--rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.8.0/ipyslides/_base/__init__.py
--rw-rw-rw-   0        0        0    41405 2024-05-06 16:18:36.000000 ipyslides-3.8.0/ipyslides/_base/_layout_css.py
--rw-rw-rw-   0        0        0     5191 2024-05-02 17:09:40.000000 ipyslides-3.8.0/ipyslides/_base/_widgets.py
--rw-rw-rw-   0        0        0    33097 2024-05-06 19:59:42.000000 ipyslides-3.8.0/ipyslides/_base/base.py
--rw-rw-rw-   0        0        0     7547 2024-04-30 19:43:44.000000 ipyslides-3.8.0/ipyslides/_base/export_html.py
--rw-rw-rw-   0        0        0     6572 2024-02-21 00:10:04.000000 ipyslides-3.8.0/ipyslides/_base/export_template.py
--rw-rw-rw-   0        0        0    12175 2024-05-03 23:26:00.000000 ipyslides-3.8.0/ipyslides/_base/icons.py
--rw-rw-rw-   0        0        0    12178 2024-05-02 17:12:13.000000 ipyslides-3.8.0/ipyslides/_base/intro.py
-drwxrwxrwx   0        0        0        0 2024-05-06 20:08:00.052967 ipyslides-3.8.0/ipyslides/_base/js/
--rw-rw-rw-   0        0        0    12184 2024-05-02 17:09:03.000000 ipyslides-3.8.0/ipyslides/_base/js/interaction.js
--rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.8.0/ipyslides/_base/js/notes.js
--rw-rw-rw-   0        0        0     3737 2024-01-23 22:26:12.000000 ipyslides-3.8.0/ipyslides/_base/navigation.py
--rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.8.0/ipyslides/_base/notes.py
--rw-rw-rw-   0        0        0    13157 2024-05-02 15:59:52.000000 ipyslides-3.8.0/ipyslides/_base/screenshot.py
--rw-rw-rw-   0        0        0    21960 2024-05-04 00:50:24.000000 ipyslides-3.8.0/ipyslides/_base/settings.py
--rw-rw-rw-   0        0        0    28848 2024-05-02 18:42:52.000000 ipyslides-3.8.0/ipyslides/_base/slide.py
--rw-rw-rw-   0        0        0    28513 2024-05-06 19:55:40.000000 ipyslides-3.8.0/ipyslides/_base/styles.py
--rw-rw-rw-   0        0        0    15593 2024-05-06 16:29:40.000000 ipyslides-3.8.0/ipyslides/_base/widgets.py
--rw-rw-rw-   0        0        0    15373 2024-05-02 19:35:56.000000 ipyslides-3.8.0/ipyslides/_demo.py
--rw-rw-rw-   0        0        0    49425 2024-05-06 16:22:38.000000 ipyslides-3.8.0/ipyslides/core.py
--rw-rw-rw-   0        0        0    18477 2024-05-06 18:06:44.000000 ipyslides-3.8.0/ipyslides/formatters.py
--rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.8.0/ipyslides/source.py
--rw-rw-rw-   0        0        0    29143 2024-03-08 03:23:55.000000 ipyslides-3.8.0/ipyslides/utils.py
--rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.8.0/ipyslides/writer.py
--rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.8.0/ipyslides/xmd.py
-drwxrwxrwx   0        0        0        0 2024-05-06 20:08:00.034422 ipyslides-3.8.0/ipyslides.egg-info/
--rw-rw-rw-   0        0        0     5382 2024-05-06 20:07:59.000000 ipyslides-3.8.0/ipyslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      854 2024-05-06 20:07:59.000000 ipyslides-3.8.0/ipyslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 20:07:59.000000 ipyslides-3.8.0/ipyslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-05-06 20:07:59.000000 ipyslides-3.8.0/ipyslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-06 20:07:59.000000 ipyslides-3.8.0/ipyslides.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 20:08:00.052967 ipyslides-3.8.0/setup.cfg
--rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 00:54:13.263394 ipyslides-3.8.1/
+-rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.8.1/LICENSE
+-rw-rw-rw-   0        0        0     5382 2024-05-08 00:54:13.263394 ipyslides-3.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.8.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 00:54:13.225254 ipyslides-3.8.1/ipyslides/
+-rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.8.1/ipyslides/__init__.py
+-rw-rw-rw-   0        0        0       25 2024-05-08 00:53:42.000000 ipyslides-3.8.1/ipyslides/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 00:54:13.259032 ipyslides-3.8.1/ipyslides/_base/
+-rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.8.1/ipyslides/_base/__init__.py
+-rw-rw-rw-   0        0        0    41405 2024-05-06 16:18:36.000000 ipyslides-3.8.1/ipyslides/_base/_layout_css.py
+-rw-rw-rw-   0        0        0     5191 2024-05-02 17:09:40.000000 ipyslides-3.8.1/ipyslides/_base/_widgets.py
+-rw-rw-rw-   0        0        0    33098 2024-05-08 00:50:58.000000 ipyslides-3.8.1/ipyslides/_base/base.py
+-rw-rw-rw-   0        0        0     7547 2024-04-30 19:43:44.000000 ipyslides-3.8.1/ipyslides/_base/export_html.py
+-rw-rw-rw-   0        0        0     6572 2024-02-21 00:10:04.000000 ipyslides-3.8.1/ipyslides/_base/export_template.py
+-rw-rw-rw-   0        0        0    12175 2024-05-03 23:26:00.000000 ipyslides-3.8.1/ipyslides/_base/icons.py
+-rw-rw-rw-   0        0        0    12178 2024-05-02 17:12:13.000000 ipyslides-3.8.1/ipyslides/_base/intro.py
+drwxrwxrwx   0        0        0        0 2024-05-08 00:54:13.259032 ipyslides-3.8.1/ipyslides/_base/js/
+-rw-rw-rw-   0        0        0    12184 2024-05-02 17:09:03.000000 ipyslides-3.8.1/ipyslides/_base/js/interaction.js
+-rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.8.1/ipyslides/_base/js/notes.js
+-rw-rw-rw-   0        0        0     3737 2024-01-23 22:26:12.000000 ipyslides-3.8.1/ipyslides/_base/navigation.py
+-rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.8.1/ipyslides/_base/notes.py
+-rw-rw-rw-   0        0        0    13157 2024-05-02 15:59:52.000000 ipyslides-3.8.1/ipyslides/_base/screenshot.py
+-rw-rw-rw-   0        0        0    21960 2024-05-04 00:50:24.000000 ipyslides-3.8.1/ipyslides/_base/settings.py
+-rw-rw-rw-   0        0        0    28852 2024-05-08 00:37:24.000000 ipyslides-3.8.1/ipyslides/_base/slide.py
+-rw-rw-rw-   0        0        0    28513 2024-05-06 19:55:40.000000 ipyslides-3.8.1/ipyslides/_base/styles.py
+-rw-rw-rw-   0        0        0    15593 2024-05-08 00:49:46.000000 ipyslides-3.8.1/ipyslides/_base/widgets.py
+-rw-rw-rw-   0        0        0    15373 2024-05-02 19:35:56.000000 ipyslides-3.8.1/ipyslides/_demo.py
+-rw-rw-rw-   0        0        0    49426 2024-05-08 00:37:34.000000 ipyslides-3.8.1/ipyslides/core.py
+-rw-rw-rw-   0        0        0    18477 2024-05-06 18:06:44.000000 ipyslides-3.8.1/ipyslides/formatters.py
+-rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.8.1/ipyslides/source.py
+-rw-rw-rw-   0        0        0    29143 2024-03-08 03:23:55.000000 ipyslides-3.8.1/ipyslides/utils.py
+-rw-rw-rw-   0        0        0    14485 2024-05-06 19:28:00.000000 ipyslides-3.8.1/ipyslides/writer.py
+-rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.8.1/ipyslides/xmd.py
+drwxrwxrwx   0        0        0        0 2024-05-08 00:54:13.243625 ipyslides-3.8.1/ipyslides.egg-info/
+-rw-rw-rw-   0        0        0     5382 2024-05-08 00:54:12.000000 ipyslides-3.8.1/ipyslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2024-05-08 00:54:13.000000 ipyslides-3.8.1/ipyslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 00:54:12.000000 ipyslides-3.8.1/ipyslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-05-08 00:54:12.000000 ipyslides-3.8.1/ipyslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-08 00:54:12.000000 ipyslides-3.8.1/ipyslides.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 00:54:13.263394 ipyslides-3.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.8.1/setup.py
```

### Comparing `ipyslides-3.8.0/LICENSE` & `ipyslides-3.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.0/PKG-INFO` & `ipyslides-3.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.8.0
+Version: 3.8.1
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.8.0/README.md` & `ipyslides-3.8.1/README.md`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.0/ipyslides/_base/_layout_css.py` & `ipyslides-3.8.1/ipyslides/_base/_layout_css.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.0/ipyslides/_base/_widgets.py` & `ipyslides-3.8.1/ipyslides/_base/_widgets.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.0/ipyslides/_base/base.py` & `ipyslides-3.8.1/ipyslides/_base/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
         return self._dynamic_private(func, tag = '_has_widgets', hide_refresher = False)
     
     def _dynamic_private(self, func, tag = None, hide_refresher = False):
         "Not for user use, internal function for other dynamic content decorators with their own tags."
         self.verify_running('Dynamic content can only be used inside slide constructor!')
         return self.running._dynamic_private(func, tag = tag, hide_refresher = hide_refresher)
         
-    def update_tmp_output(self, *objs):
+    def _update_tmp_output(self, *objs):
         "Used for CSS/animations etc. HTML widget does not work properly."
         if self.is_jupyter_session():
             self.widgets._tmp_out.clear_output(wait=True)
             with self.widgets._tmp_out:
                 display(*objs)
         
     def from_markdown(self, start, content, trusted = False):
```

### Comparing `ipyslides-3.8.0/ipyslides/_base/export_html.py` & `ipyslides-3.8.1/ipyslides/_base/export_html.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.0/ipyslides/_base/export_template.py` & `ipyslides-3.8.1/ipyslides/_base/export_template.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.0/ipyslides/_base/icons.py` & `ipyslides-3.8.1/ipyslides/_base/icons.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.0/ipyslides/_base/intro.py` & `ipyslides-3.8.1/ipyslides/_base/intro.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.0/ipyslides/_base/js/interaction.js` & `ipyslides-3.8.1/ipyslides/_base/js/interaction.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.0/ipyslides/_base/js/notes.js` & `ipyslides-3.8.1/ipyslides/_base/js/notes.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.0/ipyslides/_base/navigation.py` & `ipyslides-3.8.1/ipyslides/_base/navigation.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.0/ipyslides/_base/notes.py` & `ipyslides-3.8.1/ipyslides/_base/notes.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.0/ipyslides/_base/screenshot.py` & `ipyslides-3.8.1/ipyslides/_base/screenshot.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.0/ipyslides/_base/settings.py` & `ipyslides-3.8.1/ipyslides/_base/settings.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.0/ipyslides/_base/slide.py` & `ipyslides-3.8.1/ipyslides/_base/slide.py`

 * *Files 1% similar despite different names*

```diff
@@ -402,15 +402,15 @@
             display(*self.contents)
             for dp in self._dproxies.values(): 
                 dp.update_display() # Update display to show new output as well
 
             self._handle_refs()
         
         # Update corresponding CSS but avoid animation here for faster and clean update
-        self._app.update_tmp_output(self.css)
+        self._app._update_tmp_output(self.css)
         self.set_dom_classes('SlideArea', 'SlideArea') # Hard refresh, removes first and add later
 
     def _handle_refs(self):
         if hasattr(self, '_refs'): # from some previous settings and change
             delattr(self, '_refs') # added later  only if need
         
         if self._app.cite_mode == 'footnote': # don't do in inline mode
@@ -522,15 +522,15 @@
         self._css = _format_css(css_dict, allow_root_attrs = True)
         
         # See effect of changes
         if not self._app.running: # Otherwise it has side effects
             if self._app._slidelabel != self.label:
                 self._app._slidelabel = self.label # Go there to see effects
             else:
-                self._app.update_tmp_output(self.animation, self._css)
+                self._app._update_tmp_output(self.animation, self._css)
 
     def set_dom_classes(self, add=None, remove=None):
         "Sett CSS classes on this slide separated by space. classes are remove first and add after it."
         if remove is not None: # remove first to enable toggle
             if not isinstance(remove, str):
                 raise TypeError("CSS classes should be a string with each class separated by space")
             for c in remove.split():
@@ -571,28 +571,28 @@
         if frame is None:
             self.__class__._animations['frame'] = ''
         elif frame in styles.animations:
             self.__class__._animations['frame'] = self._instance_animation(frame)
         else:
             raise KeyError(f'Animation {frame!r} not found. Use None to remove animation or one of {tuple(styles.animations.keys())}')
         
-        self._app.update_tmp_output(self.animation, self.css) # See effect
+        self._app._update_tmp_output(self.animation, self.css) # See effect
             
     def set_animation(self, name):
         "Set animation of this slide. Provide None if need to stop animation."
         if name is None:
             self._animation = html('style', '')
         elif isinstance(name,str) and name in styles.animations:
             self._animation = html('style',self._instance_animation(name))
             # See effect of changes
             if not self._app.running: # Otherwise it has side effects
                 if self._app._slidelabel != self.label:
                     self._app._slidelabel = self.label # Go there to see effects
                 else:
-                    self._app.update_tmp_output(self._animation, self.css)
+                    self._app._update_tmp_output(self._animation, self.css)
         else:
             self._animation = None # It should be None, not '' or don't throw error here
        
     def _rebuild_all(self):
         "Update all slides in optimal way when a new slide is added."
         self._app.refresh()
         self._app._slidelabel = self.label # Go there after setting children
```

### Comparing `ipyslides-3.8.0/ipyslides/_base/styles.py` & `ipyslides-3.8.1/ipyslides/_base/styles.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.0/ipyslides/_base/widgets.py` & `ipyslides-3.8.1/ipyslides/_base/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
 @dataclass(frozen=True)
 class _Sliders:
     """
     Instantiate under `Widgets` class only.
     """
     progress = ipw.SelectionSlider(options=[('0',0)], value=0, continuous_update=False,readout=True)
-    width    = ipw.IntSlider(**describe('Width (vw)'),min=20,max=100, value = 70,continuous_update=False).add_class('Width-Slider') 
+    width    = ipw.IntSlider(**describe('Width (vw)'),min=20,max=100, value = 55,continuous_update=False).add_class('Width-Slider') 
     fontsize = ipw.IntSlider(**describe('Font Size'),min=8,max=64,step=1, value = 20,continuous_update=False, tooltip="If you need more larger/smaller font size, use `Slides.settings.set_font_size`")
 
 @dataclass(frozen=True)
 class _Dropdowns:
     """
     Instantiate under `Widgets` class only.
     """
```

### Comparing `ipyslides-3.8.0/ipyslides/_demo.py` & `ipyslides-3.8.1/ipyslides/_demo.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.0/ipyslides/core.py` & `ipyslides-3.8.1/ipyslides/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -609,15 +609,15 @@
                 "style",
                 f"{uclass} .toc-item.s{self._sectionindex} {{font-weight:bold;background:var(--primary-bg);}}",
             )]
 
         if self.screenshot.capturing == False:
             _objs.append(self._iterable[new_index].animation)
 
-        self.update_tmp_output(*_objs)
+        self._update_tmp_output(*_objs)
         self.widgets.update_progressbar()
 
         if (old_index + 1) > len(self.widgets.slidebox.children):
             old_index = new_index  # Just safe
 
         self.widgets.slidebox.children[old_index].layout.visibility = 'hidden'
         self.widgets.slidebox.children[new_index].layout.visibility = 'visible'
```

### Comparing `ipyslides-3.8.0/ipyslides/formatters.py` & `ipyslides-3.8.1/ipyslides/formatters.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.0/ipyslides/source.py` & `ipyslides-3.8.1/ipyslides/source.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.0/ipyslides/utils.py` & `ipyslides-3.8.1/ipyslides/utils.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.0/ipyslides/writer.py` & `ipyslides-3.8.1/ipyslides/writer.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.0/ipyslides/xmd.py` & `ipyslides-3.8.1/ipyslides/xmd.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.0/ipyslides.egg-info/PKG-INFO` & `ipyslides-3.8.1/ipyslides.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.8.0
+Version: 3.8.1
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.8.0/ipyslides.egg-info/SOURCES.txt` & `ipyslides-3.8.1/ipyslides.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyslides-3.8.0/setup.py` & `ipyslides-3.8.1/setup.py`

 * *Files identical despite different names*

