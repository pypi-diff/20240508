# Comparing `tmp/rushcards-0.1.2.tar.gz` & `tmp/rushcards-0.1.3.tar.gz`

## Comparing `rushcards-0.1.2.tar` & `rushcards-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    13155 2020-02-02 00:00:00.000000 rushcards-0.1.2/docs/images/sample.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rushcards-0.1.2/rushcards/__init__.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 rushcards-0.1.2/rushcards/__main__.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 rushcards-0.1.2/rushcards/base.py
--rw-r--r--   0        0        0     4480 2020-02-02 00:00:00.000000 rushcards-0.1.2/rushcards/cli.py
--rw-r--r--   0        0        0     6554 2020-02-02 00:00:00.000000 rushcards-0.1.2/rushcards/draw.py
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 rushcards-0.1.2/rushcards/puzzle.py
--rw-r--r--   0        0        0 20737698 2020-02-02 00:00:00.000000 rushcards-0.1.2/rushcards/puzzles.pickle
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rushcards-0.1.2/rushcards/tools/__init__.py
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 rushcards-0.1.2/rushcards/tools/mkpuzzles.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 rushcards-0.1.2/rushcards/tools/statistics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rushcards-0.1.2/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 rushcards-0.1.2/LICENSE.md
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 rushcards-0.1.2/README.md
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 rushcards-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 rushcards-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 rushcards-0.1.3/docs/images/sample.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rushcards-0.1.3/rushcards/__init__.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 rushcards-0.1.3/rushcards/__main__.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 rushcards-0.1.3/rushcards/base.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 rushcards-0.1.3/rushcards/cli.py
+-rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 rushcards-0.1.3/rushcards/draw.py
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 rushcards-0.1.3/rushcards/puzzle.py
+-rw-r--r--   0        0        0 20737698 2020-02-02 00:00:00.000000 rushcards-0.1.3/rushcards/puzzles.pickle
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rushcards-0.1.3/rushcards/tools/__init__.py
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 rushcards-0.1.3/rushcards/tools/mkpuzzles.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 rushcards-0.1.3/rushcards/tools/statistics.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 rushcards-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 rushcards-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 rushcards-0.1.3/README.md
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 rushcards-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 rushcards-0.1.3/PKG-INFO
```

### Comparing `rushcards-0.1.2/rushcards/base.py` & `rushcards-0.1.3/rushcards/base.py`

 * *Files identical despite different names*

### Comparing `rushcards-0.1.2/rushcards/cli.py` & `rushcards-0.1.3/rushcards/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         file_uri = Path(outfile.name).resolve().as_uri()
         print_debug(f"Opening {file_uri}", debug)
         webbrowser.open_new_tab(file_uri)
 
 
 # Converts string difficulties into a list of integers. The special case of
 # "_" is converted to None.
-def difficulty_type(difficulty_str):
-    difficulties_parts = [d.strip() for d in difficulty_str.split(",")]
+def difficulties_type(difficulties_str):
+    difficulties_parts = [d.strip() for d in difficulties_str.split(",")]
     difficulties_raw = [None if d == "_" else int(d) for d in difficulties_parts]
 
     if any(type(d) is int and not 1 <= d <= DIFFICULTY_STEPS for d in difficulties_raw):
         raise ValueError(f"Difficulty must be between 1 and {DIFFICULTY_STEPS}")
 
     return difficulties_raw
 
@@ -65,16 +65,16 @@
 
 
 def rushcards_cli():
     parser = argparse.ArgumentParser(
         prog="rushcards", description="Generate puzzle cards for the game Rush Hour."
     )
     parser.add_argument(
-        "difficulty",
-        type=difficulty_type,
+        "difficulties",
+        type=difficulties_type,
         help=f"comma-separated list of difficulties (1-{DIFFICULTY_STEPS} or _ for random)",
     )
     parser.add_argument(
         "-l",
         "--layout",
         type=layout_type,
         help="card layout expressed as [rows]x[cols]",
@@ -93,37 +93,40 @@
     parser.add_argument(
         "--debug",
         action="store_true",
         help=argparse.SUPPRESS,
     )
     args = parser.parse_args()
 
-    if args.layout and len(args.difficulty) > (args.layout.rows * args.layout.cols):
+    difficulties_raw = args.difficulties
+    num_specified = len(difficulties_raw)
+    if args.layout and num_specified > (args.layout.rows * args.layout.cols):
         parser.error("Too many puzzles requested for given layout")
 
-    # If there is only one difficulty but layout is provided, create as many
-    # puzzles with that difficulty as necessary to fill the layout.
-    difficulties_raw = args.difficulty
-    if len(difficulties_raw) == 1 and args.layout:
-        difficulties_raw *= args.layout.rows * args.layout.cols
+    # If a layout wasn't provided, create one to fit at least the requested number of
+    # puzzles (showing preference for more columns and fewer rows).
+    layout = args.layout
+    if not layout:
+        cols = math.ceil(math.sqrt(num_specified))
+        rows = math.ceil(num_specified / cols)
+        layout = Layout(rows, cols)
+
+    # Repeat the sequence of specified difficulties as many times as needed
+    # to fill the layout.
+    num_needed = layout.rows * layout.cols
+    if num_specified < num_needed:
+        difficulties_raw *= math.ceil(num_needed / num_specified)
+        difficulties_raw = difficulties_raw[:num_needed]
 
     # Insert random difficulties where requested.
     difficulties = [
         d if d is not None else random.randrange(1, DIFFICULTY_STEPS + 1)
         for d in difficulties_raw
     ]
 
-    # If a layout wasn't provided, create one to fit the requested number of puzzles
-    # (showing preference for more columns and fewer rows).
-    layout = args.layout
-    if not layout:
-        cols = int(math.ceil(math.sqrt(len(difficulties))))
-        rows = int(math.ceil(len(difficulties) / cols))
-        layout = Layout(rows, cols)
-
     do_open = not args.no_open
 
     # There are three possible write destinations.
     if args.outfile == "-":
         outfile = open(sys.stdout.fileno(), "wb", closefd=False)
         do_open = False  # Can't open data passed to stdout
     elif args.outfile:
```

### Comparing `rushcards-0.1.2/rushcards/draw.py` & `rushcards-0.1.3/rushcards/draw.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,23 +14,25 @@
 BOARD_GRID_WIDTH = 2
 PAGE_BACKGROUND_COLOR = "#FFFFFF"
 BOARD_BORDER_COLOR = "#909090"
 BOARD_GRID_COLOR = "#E8E8E8"
 EXIT_SIZE = CELL_WIDTH // 6
 BOARD_PADDING = EXIT_SIZE
 
-CAR_PADDING_WIDTH = CELL_WIDTH // 12
-CAR_WIDTH = CELL_WIDTH - 2 * CAR_PADDING_WIDTH
+CAR_PADDING = CELL_WIDTH // 12
+CAR_WIDTH = CELL_WIDTH - 2 * CAR_PADDING
 CAR_BORDER_RADIUS = CAR_WIDTH // 4
-BOARD_BORDER_RADIUS = CAR_BORDER_RADIUS + CAR_PADDING_WIDTH  # Match rounded corners
+BOARD_BORDER_RADIUS = CAR_BORDER_RADIUS + CAR_PADDING  # Match rounded corners
 
 TEXT_COLOR = "#555555"
-TEXT_HEIGHT = CELL_WIDTH  # This is fairly arbitrary
-FONT_SIZE = CELL_WIDTH // 4
-DEBUG_FONT_SIZE = CELL_WIDTH // 6
+TEXT_BOX_HEIGHT = CELL_WIDTH  # This is fairly arbitrary
+TEXT_BOX_TOP_PADDING = CELL_WIDTH // 6
+TEXT_BOX_LEFT_PADDING = CELL_WIDTH // 8
+TEXT_FONT_SIZE = CELL_WIDTH // 3
+TEXT_DEBUG_FONT_SIZE = CELL_WIDTH // 5
 
 
 # Draw the board border, grid lines, and exit mark.
 def draw_board(drawer, debug):
     # Draw the grid lines first so board border is drawn over them.
     for line_num in range(1, BOARD_SIZE):
         # Draw both a horizontal and a vertical line.
@@ -68,23 +70,23 @@
     )
 
 
 # Draw the car with the provided color.
 def draw_car(drawer, car, color):
     # The start pixel is determined solely by the Car's position but
     # the end pixel depends on its orientation as well.
-    start_x = car.position.x * CELL_WIDTH + CAR_PADDING_WIDTH
-    start_y = car.position.y * CELL_WIDTH + CAR_PADDING_WIDTH
+    start_x = car.position.x * CELL_WIDTH + CAR_PADDING
+    start_y = car.position.y * CELL_WIDTH + CAR_PADDING
     end_x = (
-        (car.position.x + car.size) * CELL_WIDTH - CAR_PADDING_WIDTH
+        (car.position.x + car.size) * CELL_WIDTH - CAR_PADDING
         if car.orientation is Orientation.HORIZONTAL
         else start_x + CAR_WIDTH
     )
     end_y = (
-        (car.position.y + car.size) * CELL_WIDTH - CAR_PADDING_WIDTH
+        (car.position.y + car.size) * CELL_WIDTH - CAR_PADDING
         if car.orientation is Orientation.VERTICAL
         else start_y + CAR_WIDTH
     )
 
     drawer.rounded_rectangle(
         (start_x, start_y, end_x, end_y),
         fill=color,
@@ -105,63 +107,61 @@
 
 
 # Draw the puzzle text. This is just the difficulty unless debug=True, in
 # which case we also draw the puzzle_def.
 def draw_text(drawer, puzzle, debug):
     text = f"Difficulty: {puzzle.difficulty}"
 
-    # Just use the default font, not worth packaging one.
-    drawer.text((0, FONT_SIZE), text, fill=TEXT_COLOR, font_size=FONT_SIZE)
+    # Just use the default font, it's not worth packaging one.
+    drawer.text((TEXT_BOX_LEFT_PADDING, TEXT_BOX_TOP_PADDING), text, fill=TEXT_COLOR, font_size=TEXT_FONT_SIZE)
 
     if debug:
         debug_text = puzzle.puzzle_def
         drawer.text(
-            (0, 3 * FONT_SIZE),
+            (TEXT_BOX_LEFT_PADDING, TEXT_BOX_TOP_PADDING * 2 + TEXT_FONT_SIZE),
             debug_text,
             fill=TEXT_COLOR,
-            font_size=DEBUG_FONT_SIZE,
+            font_size=TEXT_DEBUG_FONT_SIZE,
         )
 
 
 # Return an Image representing a single puzzle. Draw the board, then the cars, then
 # the difficulty text. For convenience we draw different parts as separate images and
 # then combine them in the end.
 def draw_puzzle(puzzle, debug):
     board_image = Image.new(
         "RGB", (BOARD_WIDTH + EXIT_SIZE, BOARD_WIDTH), PAGE_BACKGROUND_COLOR
     )
     board_drawer = ImageDraw.Draw(board_image, mode="RGBA")
     draw_board(board_drawer, debug)
     draw_cars(board_drawer, puzzle.cars, debug)
 
-    text_image = Image.new("RGB", (BOARD_WIDTH, TEXT_HEIGHT), PAGE_BACKGROUND_COLOR)
+    text_image = Image.new("RGB", (BOARD_WIDTH, TEXT_BOX_HEIGHT), PAGE_BACKGROUND_COLOR)
     text_drawer = ImageDraw.Draw(text_image, mode="RGBA")
     draw_text(text_drawer, puzzle, debug)
 
     # Before saving we want to add padding on the left and top matching the right
     # so that the final image is centered.
     final_image = Image.new(
         "RGB",
         (
             BOARD_PADDING + BOARD_WIDTH + EXIT_SIZE,
-            BOARD_PADDING + BOARD_WIDTH + TEXT_HEIGHT,
+            BOARD_PADDING + BOARD_WIDTH + TEXT_BOX_HEIGHT,
         ),
         PAGE_BACKGROUND_COLOR,
     )
     final_image.paste(board_image, (BOARD_PADDING, BOARD_PADDING))
     final_image.paste(text_image, (BOARD_PADDING, BOARD_PADDING + BOARD_WIDTH))
     return final_image
 
 
 # Return a single image (as a string of bytes) showing all the puzzles
 # represented by puzzles in the layout represented by layout.
-#
-# We trust the caller on layout, even if it's larger than needed for the number of puzzles.
 def draw_puzzles(puzzles, layout, image_format, debug):
-    assert len(puzzles) > 0, puzzles
+    assert len(puzzles) == layout.rows * layout.cols, puzzles
 
     # Draw an image for each puzzle.
     puzzle_images = [draw_puzzle(puzzle, debug) for puzzle in puzzles]
 
     # Create a composite image with each puzzle image placed as specified by layout.
     puzzle_size = puzzle_images[0].size  # Assumes all images are the same size
     composite_size = (puzzle_size[0] * layout.cols, puzzle_size[1] * layout.rows)
```

### Comparing `rushcards-0.1.2/rushcards/puzzle.py` & `rushcards-0.1.3/rushcards/puzzle.py`

 * *Files identical despite different names*

### Comparing `rushcards-0.1.2/rushcards/puzzles.pickle` & `rushcards-0.1.3/rushcards/puzzles.pickle`

 * *Files identical despite different names*

### Comparing `rushcards-0.1.2/rushcards/tools/mkpuzzles.py` & `rushcards-0.1.3/rushcards/tools/mkpuzzles.py`

 * *Files identical despite different names*

### Comparing `rushcards-0.1.2/rushcards/tools/statistics.py` & `rushcards-0.1.3/rushcards/tools/statistics.py`

 * *Files identical despite different names*

### Comparing `rushcards-0.1.2/LICENSE.md` & `rushcards-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `rushcards-0.1.2/README.md` & `rushcards-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Rush Cards
 
 ![Sample Rush Cards puzzle](https://raw.githubusercontent.com/marfire/rushcards/main/docs/images/sample.png)
 
 Rush Cards provides a Python command line application for generating puzzle cards 
 for the game [Rush Hour](https://en.wikipedia.org/wiki/Rush_Hour_(puzzle)). It 
-builds on [a project](https://www.michaelfogleman.com/rush/) by Michael Fogelman to 
+    builds on [a project](https://www.michaelfogleman.com/rush/) by Michael Fogleman to 
 identify all possible Rush Hour puzzles. Put simply, this project takes that 
 database of puzzles, keeps the puzzles that can be expressed in the standard board 
 game, maps a 1-10 difficulty scale onto them, and provides an interface to generate 
 endless puzzle cards.
 
 ## Installation
 
@@ -19,50 +19,51 @@
 ## Usage
 
 Cards are generated from the command line using either `rushcards` or `python -m 
 rushcards`.
 
     $ rushcards 5
 
-This will generate a single card representing a random puzzle with difficulty `5`; save 
-the PNG image to a temporary directory; then open it in a native image-viewing 
-application chosen by the operating system.
+This will generate a single card representing a random puzzle of difficulty `5`, save 
+the PNG image to a temporary directory, then open it in a native image-viewing 
+application.
 
 In addition to numbers `1` through `10` you can also specify `_` (underscore) to 
 choose a random difficulty.
 
 To put multiple cards into the same image use a comma-separated list of difficulties.
 
     $ # Create a single image with 6 puzzles in a 2x3 layout.
     $ rushcards 2,_,4,5,6,10
 
-A compact layout will be chosen automatically, but you can also specify a layout 
+A compact layout will be chosen automatically, but you can also specify the layout 
 with the `--layout` option.
 
-    $ # Create a single image with 6 rows of 1 puzzle each.
+    $ # Create an image with 6 rows of 1 puzzle each.
     $ rushcards 2,_,4,5,6,10 --layout 6x1
 
-As a special case, if you specify a single difficulty but a larger layout, enough 
-puzzles with that difficulty will be chosen to fill the layout.
+Regardless of how the layout is chosen, enough puzzles will be generated to 
+completely fill it. This is done by repeating the sequence of difficulties as many 
+times as necessary.
 
-    $ # Create an image with 8 puzzles of difficulty 5.
-    $ rushcards 5 --layout 2x4.
+    $ # Create an image with 8 puzzles alternating between difficulties 2 and 3.
+    $ rushcards 2,3 --layout 2x4
 
 Use the `--outfile` option to specify an output file.
 
     $ # Save the image to a file.
     $ rushcards 5 --outfile puzzle.png
 
-Specify the file as `-` (hyphen) to output to stdout.
+Specify the file as `-` (hyphen) to output to `stdout`.
 
     $ # Send the image to stdout and pipe it to another program.
     $ rushcards 5 --outfile - | wc -c
     7987
 
-Note that when writing to stdout the image can't be opened automatically. You can 
+Note that when writing to `stdout` the image can't be opened automatically. You can 
 also manually suppress opening the file with the `--no-open` option.
 
     $ # Write the puzzle to a file but don't open it.
     $ rushcards 5 --outfile puzzle.png --no-open
 
 ## Notes
```

### Comparing `rushcards-0.1.2/pyproject.toml` & `rushcards-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rushcards"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Kevin Christopher Henry", email="k@severian.com" },
 ]
 description = "A Python command line application for generating Rush Hour puzzle cards."
 license = "MIT"
 readme="README.md"
 requires-python = ">=3.6"
```

### Comparing `rushcards-0.1.2/PKG-INFO` & `rushcards-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rushcards
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python command line application for generating Rush Hour puzzle cards.
 Project-URL: Homepage, https://github.com/marfire/rushcards
 Project-URL: Issues, https://github.com/marfire/rushcards/issues
 Author-email: Kevin Christopher Henry <k@severian.com>
 License-Expression: MIT
 License-File: LICENSE.md
 Keywords: games,rush,rush-hour
@@ -28,15 +28,15 @@
 
 # Rush Cards
 
 ![Sample Rush Cards puzzle](https://raw.githubusercontent.com/marfire/rushcards/main/docs/images/sample.png)
 
 Rush Cards provides a Python command line application for generating puzzle cards 
 for the game [Rush Hour](https://en.wikipedia.org/wiki/Rush_Hour_(puzzle)). It 
-builds on [a project](https://www.michaelfogleman.com/rush/) by Michael Fogelman to 
+    builds on [a project](https://www.michaelfogleman.com/rush/) by Michael Fogleman to 
 identify all possible Rush Hour puzzles. Put simply, this project takes that 
 database of puzzles, keeps the puzzles that can be expressed in the standard board 
 game, maps a 1-10 difficulty scale onto them, and provides an interface to generate 
 endless puzzle cards.
 
 ## Installation
 
@@ -47,50 +47,51 @@
 ## Usage
 
 Cards are generated from the command line using either `rushcards` or `python -m 
 rushcards`.
 
     $ rushcards 5
 
-This will generate a single card representing a random puzzle with difficulty `5`; save 
-the PNG image to a temporary directory; then open it in a native image-viewing 
-application chosen by the operating system.
+This will generate a single card representing a random puzzle of difficulty `5`, save 
+the PNG image to a temporary directory, then open it in a native image-viewing 
+application.
 
 In addition to numbers `1` through `10` you can also specify `_` (underscore) to 
 choose a random difficulty.
 
 To put multiple cards into the same image use a comma-separated list of difficulties.
 
     $ # Create a single image with 6 puzzles in a 2x3 layout.
     $ rushcards 2,_,4,5,6,10
 
-A compact layout will be chosen automatically, but you can also specify a layout 
+A compact layout will be chosen automatically, but you can also specify the layout 
 with the `--layout` option.
 
-    $ # Create a single image with 6 rows of 1 puzzle each.
+    $ # Create an image with 6 rows of 1 puzzle each.
     $ rushcards 2,_,4,5,6,10 --layout 6x1
 
-As a special case, if you specify a single difficulty but a larger layout, enough 
-puzzles with that difficulty will be chosen to fill the layout.
+Regardless of how the layout is chosen, enough puzzles will be generated to 
+completely fill it. This is done by repeating the sequence of difficulties as many 
+times as necessary.
 
-    $ # Create an image with 8 puzzles of difficulty 5.
-    $ rushcards 5 --layout 2x4.
+    $ # Create an image with 8 puzzles alternating between difficulties 2 and 3.
+    $ rushcards 2,3 --layout 2x4
 
 Use the `--outfile` option to specify an output file.
 
     $ # Save the image to a file.
     $ rushcards 5 --outfile puzzle.png
 
-Specify the file as `-` (hyphen) to output to stdout.
+Specify the file as `-` (hyphen) to output to `stdout`.
 
     $ # Send the image to stdout and pipe it to another program.
     $ rushcards 5 --outfile - | wc -c
     7987
 
-Note that when writing to stdout the image can't be opened automatically. You can 
+Note that when writing to `stdout` the image can't be opened automatically. You can 
 also manually suppress opening the file with the `--no-open` option.
 
     $ # Write the puzzle to a file but don't open it.
     $ rushcards 5 --outfile puzzle.png --no-open
 
 ## Notes
```

