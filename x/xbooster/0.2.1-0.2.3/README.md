# Comparing `tmp/xbooster-0.2.1.tar.gz` & `tmp/xbooster-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbooster-0.2.1.tar", max compression
+gzip compressed data, was "xbooster-0.2.3.tar", max compression
```

## Comparing `xbooster-0.2.1.tar` & `xbooster-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2024-02-14 10:37:37.681440 xbooster-0.2.1/LICENSE.md
--rw-r--r--   0        0        0    16771 2024-05-03 11:06:56.522410 xbooster-0.2.1/README.md
--rw-r--r--   0        0        0      746 2024-05-03 13:12:08.560315 xbooster-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-02-13 14:22:51.544451 xbooster-0.2.1/xbooster/.DS_Store
--rw-r--r--   0        0        0       17 2024-02-13 21:49:27.431142 xbooster-0.2.1/xbooster/__init__.py
--rw-r--r--   0        0        0     6911 2024-02-13 21:49:27.456857 xbooster-0.2.1/xbooster/_parser.py
--rw-r--r--   0        0        0    12457 2024-04-30 18:54:22.550733 xbooster-0.2.1/xbooster/_utils.py
--rw-r--r--   0        0        0    28641 2024-02-14 09:53:56.565516 xbooster-0.2.1/xbooster/constructor.py
--rw-r--r--   0        0        0    41429 2024-05-02 10:43:56.668725 xbooster-0.2.1/xbooster/explainer.py
--rw-r--r--   0        0        0    17755 1970-01-01 00:00:00.000000 xbooster-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-02-14 10:37:37.681440 xbooster-0.2.3/LICENSE.md
+-rw-r--r--   0        0        0    11652 2024-05-08 11:50:55.816269 xbooster-0.2.3/README.md
+-rw-r--r--   0        0        0      742 2024-05-08 10:50:46.838482 xbooster-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-05-08 11:49:10.572404 xbooster-0.2.3/xbooster/.DS_Store
+-rw-r--r--   0        0        0       17 2024-02-13 21:49:27.431142 xbooster-0.2.3/xbooster/__init__.py
+-rw-r--r--   0        0        0     6911 2024-02-13 21:49:27.456857 xbooster-0.2.3/xbooster/_parser.py
+-rw-r--r--   0        0        0    12457 2024-04-30 18:54:22.550733 xbooster-0.2.3/xbooster/_utils.py
+-rw-r--r--   0        0        0    28641 2024-02-14 09:53:56.565516 xbooster-0.2.3/xbooster/constructor.py
+-rw-r--r--   0        0        0    41832 2024-05-08 11:46:28.409171 xbooster-0.2.3/xbooster/explainer.py
+-rw-r--r--   0        0        0    12632 1970-01-01 00:00:00.000000 xbooster-0.2.3/PKG-INFO
```

### Comparing `xbooster-0.2.1/LICENSE.md` & `xbooster-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `xbooster-0.2.1/pyproject.toml` & `xbooster-0.2.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "xbooster"
-version = "0.2.1"
+version = "0.2.3"
 description = "Explainable Boosted Scoring"
-authors = ["Denis Burakov <dennyemb@gmail.com>"]
+authors = ["xRiskLab <contact@xrisklab.ai>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 black = {extras = ["jupyter"], version = "^24.2.0"}
 duckdb = "^0.9.2"
```

### Comparing `xbooster-0.2.1/xbooster/.DS_Store` & `xbooster-0.2.3/xbooster/.DS_Store`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
-00000010: 0000 1000 0000 0108 0000 0000 0000 0000  ................
+00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0004  ................
-00000050: 0000 0001 0000 1000 0073 0065 0072 002e  .........s.e.r..
-00000060: 0070 0079 0000 0000 0000 0000 0000 0000  .p.y............
+00000040: 0000 0000 0000 0002 0000 0000 0000 0005  ................
+00000050: 0000 0001 0000 1000 0069 0074 005f 005f  .........i.t._._
+00000060: 002e 0070 0000 0000 0000 0000 0000 0000  ...p............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000100: 0000 0000 0000 0000 0000 0004 0000 000a  ................
-00000110: 005f 0070 0061 0072 0073 0065 0072 002e  ._.p.a.r.s.e.r..
-00000120: 0070 0079 496c 6f63 626c 6f62 0000 0010  .p.yIlocblob....
-00000130: ffff ffff ffff ffff ffff ffff ffff ffff  ................
-00000140: 0000 0009 005f 0075 0074 0069 006c 0073  ....._.u.t.i.l.s
-00000150: 002e 0070 0079 496c 6f63 626c 6f62 0000  ...p.yIlocblob..
-00000160: 0010 ffff ffff ffff ffff ffff ffff ffff  ................
-00000170: ffff 0000 000e 0063 006f 006e 0073 0074  .......c.o.n.s.t
-00000180: 0072 0075 0063 0074 006f 0072 002e 0070  .r.u.c.t.o.r...p
-00000190: 0079 496c 6f63 626c 6f62 0000 0010 ffff  .yIlocblob......
-000001a0: ffff ffff ffff ffff ffff ffff ffff 0000  ................
-000001b0: 000c 0065 0078 0070 006c 0061 0069 006e  ...e.x.p.l.a.i.n
-000001c0: 0065 0072 002e 0070 0079 496c 6f63 626c  .e.r...p.yIlocbl
-000001d0: 6f62 0000 0010 ffff ffff ffff ffff ffff  ob..............
-000001e0: ffff ffff ffff 0000 0000 0000 0000 0000  ................
+00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000200: 0000 0000 0000 0000 0000 0005 0000 000b  ................
+00000210: 005f 005f 0069 006e 0069 0074 005f 005f  ._._.i.n.i.t._._
+00000220: 002e 0070 0079 496c 6f63 626c 6f62 0000  ...p.yIlocblob..
+00000230: 0010 0000 0041 0000 002e ffff ffff ffff  .....A..........
+00000240: 0000 0000 000a 005f 0070 0061 0072 0073  ......._.p.a.r.s
+00000250: 0065 0072 002e 0070 0079 496c 6f63 626c  .e.r...p.yIlocbl
+00000260: 6f62 0000 0010 0000 011d 0000 002e ffff  ob..............
+00000270: ffff ffff 0000 0000 0009 005f 0075 0074  ..........._.u.t
+00000280: 0069 006c 0073 002e 0070 0079 496c 6f63  .i.l.s...p.yIloc
+00000290: 626c 6f62 0000 0010 0000 018b 0000 002e  blob............
+000002a0: ffff ffff ffff 0000 0000 000e 0063 006f  .............c.o
+000002b0: 006e 0073 0074 0072 0075 0063 0074 006f  .n.s.t.r.u.c.t.o
+000002c0: 0072 002e 0070 0079 496c 6f63 626c 6f62  .r...p.yIlocblob
+000002d0: 0000 0010 0000 01f9 0000 002e ffff ffff  ................
+000002e0: ffff 0000 0000 000c 0065 0078 0070 006c  .........e.x.p.l
+000002f0: 0061 0069 006e 0065 0072 002e 0070 0079  .a.i.n.e.r...p.y
+00000300: 496c 6f63 626c 6f62 0000 0010 0000 0267  Ilocblob.......g
+00000310: 0000 002e ffff ffff ffff 0000 0000 0000  ................
 00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -251,15 +251,15 @@
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0003 0000 0000 0000 100b  ................
-00001010: 0000 0045 0000 0108 0000 0000 0000 0000  ...E............
+00001010: 0000 0045 0000 0209 0000 0000 0000 0000  ...E............
 00001020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -318,15 +318,15 @@
 000013d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
 00001410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
 00001420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
-00001440: 0100 0000 8000 0000 0000 0000 0100 0002  ................
+00001440: 0100 0000 8000 0000 0100 0001 0000 0000  ................
 00001450: 0000 0000 0100 0004 0000 0000 0200 0008  ................
 00001460: 0000 0018 0000 0000 0000 0000 0100 0020  ............... 
 00001470: 0000 0000 0100 0040 0000 0000 0100 0080  .......@........
 00001480: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001490: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 000014a0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 000014b0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
```

### Comparing `xbooster-0.2.1/xbooster/_parser.py` & `xbooster-0.2.3/xbooster/_parser.py`

 * *Files identical despite different names*

### Comparing `xbooster-0.2.1/xbooster/_utils.py` & `xbooster-0.2.3/xbooster/_utils.py`

 * *Files identical despite different names*

### Comparing `xbooster-0.2.1/xbooster/constructor.py` & `xbooster-0.2.3/xbooster/constructor.py`

 * *Files identical despite different names*

### Comparing `xbooster-0.2.1/xbooster/explainer.py` & `xbooster-0.2.3/xbooster/explainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,27 +297,31 @@
     ] = None,
     metric: str = "Likelihood",
     normalize: bool = True,
     method: Optional[str] = None,
     dataframe: Optional[pd.DataFrame] = None,
     fontfamily: Optional[str] = "Monospace",
     fontsize: Optional[int] = 12,
+    dpi: Optional[int] = 100,
+    title: Optional[str] = "Feature importance",
     **kwargs: Any,
 ) -> None:
     """
     Plots the importance of features based on the XGBoost scorecard.
 
     Args:
         scorecard_constructor: XGBoost scorecard constructor.
         metric: Metric to plot ("Likelihood" (default), "NegLogLikelihood", "IV", or "Points").
         normalize: Whether to normalize the importance values (default: True).
         method: The method to use for plotting the importance ("global" or "local").
         dataframe: The dataframe containing features and labels.
         fontfamily: Font family for text elements like xlabel, title, etc.
         fontsize: Font size for text elements like xlabel, title, etc.
+        dpi: Dots per inch for the plot.
+        title: The title of the plot.
         **kwargs: Additional Matplotlib parameters.
 
     Returns:
         None
 
     Raises:
         ValueError: If scorecard_constructor is not provided.
@@ -426,22 +430,22 @@
         )
 
     color = kwargs.pop("color", "#7950f2")
 
     with plt.rc_context(
         {"font.family": fontfamily, "font.size": fontsize}
     ):
-        _, ax = plt.subplots(figsize=(5, 5), dpi=100)
+        _, ax = plt.subplots(dpi=dpi, **kwargs)
         importance_data.plot(
             kind="barh",
             width=0.75,
             ax=ax,
             fontsize=12,
             color=color,
-            **kwargs,
+            **kwargs
         )  # type: ignore
 
         ax.set_ylabel(None)
         ax.set_xlabel(
             (
                 "NegLogLikelihood"
                 if metric == "WOE"
@@ -449,15 +453,17 @@
             ),
             fontsize=12,
         )
         ax.xaxis.set_ticks_position("bottom")
         ax.yaxis.set_ticks_position("none")
         ax.spines["right"].set_visible(False)
         ax.spines["top"].set_visible(False)
-
+        
+        if title:
+            plt.title(f"{title}")
         plt.show()
 
 
 def plot_score_distribution(
     y_true: pd.Series = None,  # type: ignore
     y_pred: pd.Series = None,  # type: ignore
     n_bins: int = 25,  # type: ignore
@@ -551,21 +557,22 @@
         plt.gca().spines["right"].set_visible(False)
         plt.grid(alpha=0.2)
         plt.xlabel("Score")
         plt.title("Score distribution")
         plt.legend()
         plt.show()
 
-
 # pylint: disable=too-many-statements, too-many-locals
 def plot_local_importance(
     scorecard_constructor,
     X: pd.DataFrame,  # pylint: disable=C0103
     fontfamily: Optional[str] = "Monospace",
     fontsize: Optional[int] = 12,
+    boxstyle: Optional[str] = "round, pad=-0.001,rounding_size=0.01",
+    title: Optional[str] = "Local feature importance",
     **kwargs: Any,
 ) -> None:
     # sourcery skip: extract-method
     """
     Plot local importance based on the provided scorecard constructor and a sample
     which needs to be explanation.
 
@@ -581,14 +588,16 @@
     For boosters with max_depth > 1, we construct interaction splits using the split
     and count method, which essentially returns the WOE for each feature in the split.
 
     Args:
         scorecard_constructor: The scorecard constructor object.
         X: A single row (or rows) of the dataset to explain.
         fontsize: Font size for text elements like xlabel, title, etc.
+        boxstyle: The style of the rounding box.
+        title: The title of the plot.
         **kwargs: Additional parameters to pass to the matplotlib function.
 
     Returns:
         None
     """
     if not isinstance(X, pd.DataFrame):
         raise ValueError(
@@ -722,15 +731,15 @@
         for patch in ax.patches:
             bb = patch.get_bbox()  # type: ignore
             color = patch.get_facecolor()
             p_bbox = FancyBboxPatch(
                 (bb.xmin, bb.ymin),
                 abs(bb.width),
                 abs(bb.height),
-                boxstyle="round, pad=-0.001,rounding_size=0.01",
+                boxstyle=f"{boxstyle}",
                 ec="black",
                 linewidth=0.5,
                 fc=color,
                 mutation_aspect=1.5,
             )
             ax.add_patch(p_bbox)
             patch.remove()
@@ -753,15 +762,15 @@
                     legend_colors, legend_labels
                 )
             ],
             loc="upper left",
         )
         plt.gca().spines["top"].set_visible(False)
         plt.gca().spines["right"].set_visible(False)
-        plt.title("Local explanation")
+        plt.title(f"{title}")
         plt.xlabel("mean(WOE)")
         plt.grid(axis="y", linestyle="--", alpha=0.5)
         plt.xticks(rotation=45)
         plt.axvline(x=0, color="black", linewidth=0.7)
         plt.show()
 
 
@@ -773,15 +782,15 @@
         parse_xgb_output: Parses the XGBoost model output to construct a tree representation.
         plot_tree: Plot the decision tree(s) using the provided scorecard constructor.
     """
 
     def __init__(
         self,
         metrics: Optional[List[str]] = None,
-        precision: int = None,
+        precision: int = None, # type: ignore
     ):
         self.scorecard_constructor: Optional[
             XGBScorecardConstructor
         ] = None
         self.tree_dump: Optional[Dict[str, Any]] = None
         self.scorecard_frame: Optional[pd.DataFrame] = None
         self.metrics: List[str] = (
```

