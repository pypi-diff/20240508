# Comparing `tmp/listpicker-0.2.0.tar.gz` & `tmp/listpicker-0.3.0.tar.gz`

## Comparing `listpicker-0.2.0.tar` & `listpicker-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 listpicker-0.2.0/src/listpicker/__init__.py
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 listpicker-0.2.0/src/listpicker/keyboard.py
--rw-r--r--   0        0        0    20641 2020-02-02 00:00:00.000000 listpicker-0.2.0/src/listpicker/listpicker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 listpicker-0.2.0/src/listpicker/py.typed
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 listpicker-0.2.0/src/listpicker/util.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 listpicker-0.2.0/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 listpicker-0.2.0/LICENSE
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 listpicker-0.2.0/README.md
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 listpicker-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 listpicker-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 listpicker-0.3.0/src/listpicker/__init__.py
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 listpicker-0.3.0/src/listpicker/keyboard.py
+-rw-r--r--   0        0        0    21202 2020-02-02 00:00:00.000000 listpicker-0.3.0/src/listpicker/listpicker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 listpicker-0.3.0/src/listpicker/py.typed
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 listpicker-0.3.0/src/listpicker/util.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 listpicker-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 listpicker-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 listpicker-0.3.0/README.md
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 listpicker-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 listpicker-0.3.0/PKG-INFO
```

### Comparing `listpicker-0.2.0/src/listpicker/__init__.py` & `listpicker-0.3.0/src/listpicker/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -63,22 +63,33 @@
 
 def pick_multiple(
     prompt: str,
     options: Sequence[str],
     *,
     force_prompt: bool = False,
     minimum: int = 1,
+    preselected: Optional[Sequence[str]] = None,
     infile: TextIO = sys.stdin,
     outfile: TextIO = sys.stdout,
 ) -> list[str]:
     """
     Prompt user to select a subset of "options". If len(options) <= minimum,
     the same options are returned in a new list without prompting the user.
     Pass force_prompt=True to always prompt the user when len(options) == minimum.
 
+    Preselected options can be passed with the "preselected" keyword argument.
+
     This function always returns a new list that contains a subsequence of
     "options" (i.e. same ordering).
     """
     if len(options) < minimum or len(options) == minimum and not force_prompt:
         return list(options)
 
-    return ListPicker(prompt, options, multiselect=True, minimum=minimum, infile=infile, outfile=outfile).pick()
+    return ListPicker(
+        prompt,
+        options,
+        multiselect=True,
+        minimum=minimum,
+        preselected=preselected,
+        infile=infile,
+        outfile=outfile,
+    ).pick()
```

### Comparing `listpicker-0.2.0/src/listpicker/keyboard.py` & `listpicker-0.3.0/src/listpicker/keyboard.py`

 * *Files identical despite different names*

### Comparing `listpicker-0.2.0/src/listpicker/listpicker.py` & `listpicker-0.3.0/src/listpicker/listpicker.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,34 +163,43 @@
     def __init__(
         self,
         prompt: str,
         options: Sequence[str],
         *,
         multiselect: bool = False,
         minimum: int = 0,
+        preselected: Optional[Sequence[str]] = None,
         infile: TextIO = sys.stdin,
         outfile: TextIO = sys.stdout,
     ):
         self._prompt = prompt.rstrip("\n").split("\n")
         self._all_options = [Option(i + 1, o) for i, o in enumerate(options)]
         self._options = self._all_options
         self._option_index_width = len("%d." % (self._all_options[-1].number))
         self._multiselect = multiselect
         self._multiselect_minimum = minimum
         self._infile = infile
         self._outfile = outfile
         self._selected_options = set()
+        self._preselected_options = set(preselected) if preselected else set()
         self._option_window = range(len(self._all_options))
 
         if self._multiselect_minimum > 0:
             if not self._multiselect:
                 raise ValueError("minimum > 0 has no effect unless multiselect=True")
             if len(self._all_options) < self._multiselect_minimum:
                 raise ValueError("not enough options to satisfy minimum constraint")
 
+        if self._preselected_options:
+            if not self._multiselect:
+                raise ValueError("preselected options require multiselect=True")
+
+            if invalid_options := self._preselected_options - set(options):
+                raise ValueError(f"unknown preselected options: {invalid_options!r}")
+
     @property
     def _header_height(self) -> int:
         return len(self._prompt) + 1  # Plus one for filter bar
 
     def _clear_buffer_commands(self) -> str:
         return "\r" + (CSI_CURSOR_MOVE_UP % self._draw_height) + CSI_CLEAR_TO_BOTTOM
 
@@ -487,14 +496,15 @@
             case ListPickerState.CONFIRMATION:
                 self._state = self._handle_confirmation_input(key)
             case _:
                 raise RuntimeError("impossible value for _state: %r" % self._state)
 
     def _run(self) -> None:
         self._selected_options.clear()
+        self._selected_options.update(o for o in self._all_options if o.value in self._preselected_options)
         self._set_filter("")
         self._columns, self._lines = os.get_terminal_size(self._outfile.fileno())
 
         try:
             self._write_screen("\r\n" + CSI_CURSOR_HIDE)
             original_sigwinch_handler = signal.getsignal(signal.SIGWINCH)
             signal.signal(signal.SIGWINCH, self._sigwinch_handler)
```

### Comparing `listpicker-0.2.0/src/listpicker/util.py` & `listpicker-0.3.0/src/listpicker/util.py`

 * *Files identical despite different names*

### Comparing `listpicker-0.2.0/LICENSE` & `listpicker-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `listpicker-0.2.0/README.md` & `listpicker-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 - Paging for long lists
 - Common navigation keybindings (vi, emacs, arrow keys, Home/End, etc)
 - Direct terminal manipulation with CSI commands (i.e. no curses)
 - Draw to main screen buffer without clearing the screen
 - Proper truncation of long lines with SGR color sequences
 - Redraw on terminal resize (SIGWINCH)
 - Help menu and multiselect confirmation prompt
+- Preselected options in multiselect prompts
 
 Screenshots
 -----------
 
 ![timezones](https://github.com/guns/python-listpicker/assets/55776/f7e6629b-77ba-4f99-a9f6-0de15485c2dd)
 ![helpmenu](https://github.com/guns/python-listpicker/assets/55776/78a966e7-4023-4d52-bfa9-87acac89b73e)
 ![filtering](https://github.com/guns/python-listpicker/assets/55776/ae01150c-cead-42f3-898e-2d631d3ba83a)
```

### Comparing `listpicker-0.2.0/pyproject.toml` & `listpicker-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "listpicker"
 description = "Interactive list selection and multiselect for POSIX terminals (non-curses)"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
     {name = "Sung Pae", email = "self@sungpae.com"},
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `listpicker-0.2.0/PKG-INFO` & `listpicker-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: listpicker
-Version: 0.2.0
+Version: 0.3.0
 Summary: Interactive list selection and multiselect for POSIX terminals (non-curses)
 Project-URL: Homepage, https://github.com/guns/python-listpicker
 Project-URL: Repository, https://github.com/guns/python-listpicker.git
 Author-email: Sung Pae <self@sungpae.com>
 License: The MIT License (MIT)
         
         Copyright © 2024 Sung Pae <self@sungpae.com>
@@ -61,14 +61,15 @@
 - Paging for long lists
 - Common navigation keybindings (vi, emacs, arrow keys, Home/End, etc)
 - Direct terminal manipulation with CSI commands (i.e. no curses)
 - Draw to main screen buffer without clearing the screen
 - Proper truncation of long lines with SGR color sequences
 - Redraw on terminal resize (SIGWINCH)
 - Help menu and multiselect confirmation prompt
+- Preselected options in multiselect prompts
 
 Screenshots
 -----------
 
 ![timezones](https://github.com/guns/python-listpicker/assets/55776/f7e6629b-77ba-4f99-a9f6-0de15485c2dd)
 ![helpmenu](https://github.com/guns/python-listpicker/assets/55776/78a966e7-4023-4d52-bfa9-87acac89b73e)
 ![filtering](https://github.com/guns/python-listpicker/assets/55776/ae01150c-cead-42f3-898e-2d631d3ba83a)
```

