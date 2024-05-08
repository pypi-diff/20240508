# Comparing `tmp/colorful_terminal-0.1.4.tar.gz` & `tmp/colorful_terminal-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorful_terminal-0.1.4.tar", last modified: Mon Mar  4 15:56:39 2024, max compression
+gzip compressed data, was "colorful_terminal-0.1.5.tar", last modified: Wed May  8 20:19:32 2024, max compression
```

## Comparing `colorful_terminal-0.1.4.tar` & `colorful_terminal-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-04 15:56:39.809554 colorful_terminal-0.1.4/
--rw-rw-rw-   0        0        0     1091 2023-01-07 18:23:21.000000 colorful_terminal-0.1.4/LICENSE
--rw-rw-rw-   0        0        0    10014 2024-03-04 15:56:39.809554 colorful_terminal-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     8991 2024-02-26 00:54:44.000000 colorful_terminal-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-04 15:56:39.799523 colorful_terminal-0.1.4/colorful_terminal/
--rw-rw-rw-   0        0        0      260 2024-03-04 15:55:43.000000 colorful_terminal-0.1.4/colorful_terminal/__init__.py
--rw-rw-rw-   0        0        0    31917 2024-03-03 22:11:30.000000 colorful_terminal-0.1.4/colorful_terminal/definitions.py
-drwxrwxrwx   0        0        0        0 2024-03-04 15:56:39.806546 colorful_terminal-0.1.4/colorful_terminal.egg-info/
--rw-rw-rw-   0        0        0    10014 2024-03-04 15:56:39.000000 colorful_terminal-0.1.4/colorful_terminal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2024-03-04 15:56:39.000000 colorful_terminal-0.1.4/colorful_terminal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-04 15:56:39.000000 colorful_terminal-0.1.4/colorful_terminal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-03-04 15:56:39.000000 colorful_terminal-0.1.4/colorful_terminal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-04 15:56:39.810560 colorful_terminal-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1976 2024-03-04 15:55:48.000000 colorful_terminal-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 20:19:32.256815 colorful_terminal-0.1.5/
+-rw-rw-rw-   0        0        0     1091 2023-01-07 18:23:21.000000 colorful_terminal-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0    10014 2024-05-08 20:19:32.255820 colorful_terminal-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8991 2024-02-26 00:54:44.000000 colorful_terminal-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 20:19:32.245584 colorful_terminal-0.1.5/colorful_terminal/
+-rw-rw-rw-   0        0        0      260 2024-05-08 20:18:33.000000 colorful_terminal-0.1.5/colorful_terminal/__init__.py
+-rw-rw-rw-   0        0        0    33410 2024-05-08 20:17:10.000000 colorful_terminal-0.1.5/colorful_terminal/definitions.py
+drwxrwxrwx   0        0        0        0 2024-05-08 20:19:32.253816 colorful_terminal-0.1.5/colorful_terminal.egg-info/
+-rw-rw-rw-   0        0        0    10014 2024-05-08 20:19:31.000000 colorful_terminal-0.1.5/colorful_terminal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2024-05-08 20:19:32.000000 colorful_terminal-0.1.5/colorful_terminal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 20:19:31.000000 colorful_terminal-0.1.5/colorful_terminal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-08 20:19:31.000000 colorful_terminal-0.1.5/colorful_terminal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 20:19:32.257817 colorful_terminal-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1976 2024-05-08 20:18:37.000000 colorful_terminal-0.1.5/setup.py
```

### Comparing `colorful_terminal-0.1.4/LICENSE` & `colorful_terminal-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `colorful_terminal-0.1.4/PKG-INFO` & `colorful_terminal-0.1.5/colorful_terminal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: colorful_terminal
-Version: 0.1.4
+Name: colorful-terminal
+Version: 0.1.5
 Summary: Print with color, style your output and take full control of your terminal.
 Home-page: https://github.com/ICreedenI/colorful_terminal
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python,print,color,colour,colored,coloured,rainbow,terminal,console,colorama
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
```

### Comparing `colorful_terminal-0.1.4/README.md` & `colorful_terminal-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `colorful_terminal-0.1.4/colorful_terminal/definitions.py` & `colorful_terminal-0.1.5/colorful_terminal/definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,14 +182,28 @@
                         s += Fore.rgb(*rgb[counter])
                         counter += 1
                     everyxcounter += 1
                 s += c
                 newstring += s
             return newstring
 
+    def color(string: str, color=(255, 255, 255)):
+        """Get a colored string ending with Fore.RESET.
+
+        Args:
+            string (str): Your string
+            color (tuple|str): The color to be used, either (red, green, blue) or a string from Fore.RED / .GREEN / .YELLOW / .BLUE / ...
+        Returns:
+            str: colored string with Fore.RESET ending
+        """
+        if isinstance(color, tuple):
+            return Fore.rgb(*color) + string + Fore.RESET
+        else:
+            return color + string + Fore.RESET
+
 
 class BackroundColor:
     BLACK = select_graphic_rendition(40)
     RED = select_graphic_rendition(41)
     GREEN = select_graphic_rendition(42)
     YELLOW = select_graphic_rendition(43)
     BLUE = select_graphic_rendition(44)
@@ -333,14 +347,28 @@
                         s += Back.rgb(*rgb[counter])
                         counter += 1
                     everyxcounter += 1
                 s += c
                 newstring += s
             return newstring
 
+    def color(string: str, color=(255, 255, 255)):
+        """Get a colored string ending with Back.RESET.
+
+        Args:
+            string (str): Your string
+            color (tuple|str): The color to be used, either (red, green, blue) or a string from Back.RED / .GREEN / .YELLOW / .BLUE / ...
+        Returns:
+            str: colored string with Back.RESET ending
+        """
+        if isinstance(color, tuple):
+            return Back.rgb(*color) + string + Back.RESET
+        else:
+            return color + string + Back.RESET
+
 
 class Styling:
     RESET_ALL = select_graphic_rendition(0)
     BOLD = select_graphic_rendition(1)
     DIM = select_graphic_rendition(2)
     ITALIC = select_graphic_rendition(3)
     UNDERLINED = select_graphic_rendition(4)
@@ -382,14 +410,25 @@
             )
         if not 0 <= blue <= 255:
             raise ValueError(
                 "blue needs to be an integer from 0 to 255 including both end points."
             )
         return select_graphic_rendition(f"58;2;{red};{green};{blue}")
 
+    def underline_color(string: str, rgb=(255, 255, 255)):
+        """Get a colored string ending with Fore.RESET.
+
+        Args:
+            string (str): Your string
+            color (tuple): The color to be used as (red, green, blue).
+        Returns:
+            str: colored string with Fore.RESET ending
+        """
+        return Fore.rgb(*rgb) + string + Fore.RESET
+
 
 class TerminalActions:
     cursor_up = "\033[A"
     """Moves the cursor 1 cell in the given direction. If the cursor is already at the edge of the screen, this has no effect."""
 
     cursor_down = "\033[B"
     """Moves the cursor 1 cell in the given direction. If the cursor is already at the edge of the screen, this has no effect."""
```

### Comparing `colorful_terminal-0.1.4/colorful_terminal.egg-info/PKG-INFO` & `colorful_terminal-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: colorful-terminal
-Version: 0.1.4
+Name: colorful_terminal
+Version: 0.1.5
 Summary: Print with color, style your output and take full control of your terminal.
 Home-page: https://github.com/ICreedenI/colorful_terminal
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python,print,color,colour,colored,coloured,rainbow,terminal,console,colorama
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
```

### Comparing `colorful_terminal-0.1.4/setup.py` & `colorful_terminal-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.1.4"
+VERSION = "0.1.5"
 DESCRIPTION = (
     "Print with color, style your output and take full control of your terminal."
 )
 
 # Setting up
 setup(
     name="colorful_terminal",
```

