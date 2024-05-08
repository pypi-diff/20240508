# Comparing `tmp/libgunshotmatch_mpl-0.5.2.tar.gz` & `tmp/libgunshotmatch_mpl-0.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libgunshotmatch_mpl-0.5.2.tar", last modified: Wed Mar 20 12:09:28 2024, max compression
+gzip compressed data, was "libgunshotmatch_mpl-0.6.0b1.tar", last modified: Wed May  8 15:40:18 2024, max compression
```

## Comparing `libgunshotmatch_mpl-0.5.2.tar` & `libgunshotmatch_mpl-0.6.0b1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-20 12:09:28.363255 libgunshotmatch_mpl-0.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-03-20 12:09:28.367255 libgunshotmatch_mpl-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-03-20 12:09:28.363255 libgunshotmatch_mpl-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-03-20 12:09:28.363255 libgunshotmatch_mpl-0.5.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-20 12:09:28.359255 libgunshotmatch_mpl-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-03-20 12:09:04.251184 libgunshotmatch_mpl-0.5.2/libgunshotmatch_mpl/peakviewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-03-20 12:09:04.251184 libgunshotmatch_mpl-0.5.2/libgunshotmatch_mpl/combined_chromatogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-03-20 12:09:04.251184 libgunshotmatch_mpl-0.5.2/libgunshotmatch_mpl/chromatogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-03-20 12:09:04.251184 libgunshotmatch_mpl-0.5.2/libgunshotmatch_mpl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 12:09:04.251184 libgunshotmatch_mpl-0.5.2/libgunshotmatch_mpl/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-08 15:40:18.942627 libgunshotmatch_mpl-0.6.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-08 15:40:18.942627 libgunshotmatch_mpl-0.6.0b1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-08 15:40:18.946627 libgunshotmatch_mpl-0.6.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-08 15:40:18.942627 libgunshotmatch_mpl-0.6.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-08 15:40:18.942627 libgunshotmatch_mpl-0.6.0b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-05-08 15:39:54.726563 libgunshotmatch_mpl-0.6.0b1/libgunshotmatch_mpl/chromatogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-08 15:39:54.726563 libgunshotmatch_mpl-0.6.0b1/libgunshotmatch_mpl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:39:54.726563 libgunshotmatch_mpl-0.6.0b1/libgunshotmatch_mpl/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-08 15:39:54.726563 libgunshotmatch_mpl-0.6.0b1/libgunshotmatch_mpl/peakviewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-05-08 15:39:54.726563 libgunshotmatch_mpl-0.6.0b1/libgunshotmatch_mpl/combined_chromatogram.py
```

### Comparing `libgunshotmatch_mpl-0.5.2/PKG-INFO` & `libgunshotmatch_mpl-0.6.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.2
 Name: libgunshotmatch-mpl
-Version: 0.5.2
+Version: 0.6.0b1
 Summary: Matplotlib intergration for GunShotMatch.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Home-page: https://github.com/GunShotMatch/libgunshotmatch-mpl
 Project-URL: Issue Tracker, https://github.com/GunShotMatch/libgunshotmatch-mpl/issues
 Project-URL: Source Code, https://github.com/GunShotMatch/libgunshotmatch-mpl
 Project-URL: Documentation, https://libgunshotmatch-mpl.readthedocs.io/en/latest
@@ -123,15 +123,15 @@
 .. |license| image:: https://img.shields.io/github/license/GunShotMatch/libgunshotmatch-mpl
 	:target: https://github.com/GunShotMatch/libgunshotmatch-mpl/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/GunShotMatch/libgunshotmatch-mpl
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/libgunshotmatch-mpl/v0.5.2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/libgunshotmatch-mpl/v0.6.0b1
 	:target: https://github.com/GunShotMatch/libgunshotmatch-mpl/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/GunShotMatch/libgunshotmatch-mpl
 	:target: https://github.com/GunShotMatch/libgunshotmatch-mpl/commit/master
 	:alt: GitHub last commit
```

### Comparing `libgunshotmatch_mpl-0.5.2/pyproject.toml` & `libgunshotmatch_mpl-0.6.0b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "libgunshotmatch-mpl"
-version = "0.5.2"
+version = "0.6.0b1"
 description = "Matplotlib intergration for GunShotMatch."
 readme = "README.rst"
 keywords = []
 dynamic = []
 dependencies = [
     "domdf-python-tools>=3.8.0.post2",
     "libgunshotmatch>=0.7.0",
@@ -30,22 +30,21 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 requires-python = ">=3.8"
 
+[project.license]
+file = "LICENSE"
+
 [[project.authors]]
 name = "Dominic Davis-Foster"
 email = "dominic@davis-foster.co.uk"
 
-
-[project.license]
-file = "LICENSE"
-
 [project.urls]
 Homepage = "https://github.com/GunShotMatch/libgunshotmatch-mpl"
 "Issue Tracker" = "https://github.com/GunShotMatch/libgunshotmatch-mpl/issues"
 "Source Code" = "https://github.com/GunShotMatch/libgunshotmatch-mpl"
 Documentation = "https://libgunshotmatch-mpl.readthedocs.io/en/latest"
 
 [tool.whey]
@@ -78,26 +77,24 @@
     "sphinxcontrib.toctree_plus",
     "sphinx_toolbox.tweaks.latex_layout",
     "sphinx_toolbox.tweaks.latex_toc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
     "sphinxcontrib.extras_require",
     "sphinx.ext.todo",
-    "sphinxemoji.sphinxemoji",
     "notfound.extension",
     "sphinx_copybutton",
     "sphinxcontrib.default_values",
     "sphinx_debuginfo",
     "sphinx_licenseinfo",
     "seed_intersphinx_mapping",
     "html_section",
     "local_extension",
     "sphinx_toolbox.more_autosummary.column_widths",
 ]
-sphinxemoji_style = "twemoji"
 gitstamp_fmt = "%d %b %Y"
 templates_path = [ "_templates",]
 html_static_path = [ "_static",]
 source_suffix = ".rst"
 master_doc = "index"
 suppress_warnings = [ "image.nonlocal_uri",]
 pygments_style = "default"
@@ -149,30 +146,30 @@
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
 [tool.snippet-fmt]
 directives = [ "code-block",]
 
+[tool.snippet-fmt.languages.python]
+reformat = true
+
+[tool.snippet-fmt.languages.TOML]
+reformat = true
+
+[tool.snippet-fmt.languages.ini]
+
+[tool.snippet-fmt.languages.json]
+
 [tool.importcheck]
 always = [ "libgunshotmatch_mpl", "libgunshotmatch_mpl.peakviewer", "libgunshotmatch_mpl.chromatogram",]
 
 [tool.dependency-dash."requirements.txt"]
 order = 10
 
 [tool.dependency-dash."tests/requirements.txt"]
 order = 20
 include = false
 
 [tool.dependency-dash."doc-source/requirements.txt"]
 order = 30
 include = false
-
-[tool.snippet-fmt.languages.python]
-reformat = true
-
-[tool.snippet-fmt.languages.TOML]
-reformat = true
-
-[tool.snippet-fmt.languages.ini]
-
-[tool.snippet-fmt.languages.json]
```

### Comparing `libgunshotmatch_mpl-0.5.2/README.rst` & `libgunshotmatch_mpl-0.6.0b1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 .. |license| image:: https://img.shields.io/github/license/GunShotMatch/libgunshotmatch-mpl
 	:target: https://github.com/GunShotMatch/libgunshotmatch-mpl/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/GunShotMatch/libgunshotmatch-mpl
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/libgunshotmatch-mpl/v0.5.2
+.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/libgunshotmatch-mpl/v0.6.0b1
 	:target: https://github.com/GunShotMatch/libgunshotmatch-mpl/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/GunShotMatch/libgunshotmatch-mpl
 	:target: https://github.com/GunShotMatch/libgunshotmatch-mpl/commit/master
 	:alt: GitHub last commit
```

### Comparing `libgunshotmatch_mpl-0.5.2/LICENSE` & `libgunshotmatch_mpl-0.6.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `libgunshotmatch_mpl-0.5.2/libgunshotmatch_mpl/peakviewer.py` & `libgunshotmatch_mpl-0.6.0b1/libgunshotmatch_mpl/peakviewer.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 #  IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 #  DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 # stdlib
-import sys
 from typing import List
 
 # 3rd party
+import numpy
 from domdf_python_tools.paths import PathLike
 from libgunshotmatch.project import Project
 from matplotlib.axes import Axes  # type: ignore[import]
 from matplotlib.figure import Figure  # type: ignore[import]
 
 # this package
 from libgunshotmatch_mpl.chromatogram import draw_peak_vlines
@@ -66,56 +66,51 @@
 			raise UnsupportedProject(f"Repeat.qualified_peaks is unset for {name!r}")
 		if repeat.datafile.intensity_matrix is None:
 			raise UnsupportedProject(f"Datafile.intensity_matrix is unset for {name!r}")
 
 	return project
 
 
-def draw_peaks(project: Project, peak_idx: int, figure: Figure, axes: List[Axes]) -> None:
+def draw_peaks(project: Project, retention_times: List[float], figure: Figure, axes: List[Axes]) -> None:
 	"""
-	Draw the peaks at ``peak_idx`` for each repeat in the project.
+	Draw the peaks at the given retention time for each repeat in the project.
 
 	:param project:
-	:param peak_idx:
+	:param retention_times: List of retention times for each repeat in the project.
 	:param figure:
 	:param axes:
-	"""
 
-	min_rt: float = sys.maxsize
-	max_rt: float = 0
-	for repeat_idx, (_, repeat) in enumerate(project.datafile_data.items()):
-		assert repeat.qualified_peaks is not None
-		peak = repeat.qualified_peaks[peak_idx]
-		# print(name, peak)
+	.. versionchanged:: 0.6.0  Replaced ``peak_idx`` argument with ``retention_times``
+	"""
 
-		min_rt = min(min_rt, peak.rt - 20)
-		max_rt = max(max_rt, peak.rt + 20)
+	min_rt: float = numpy.nanmin(retention_times) - 20
+	max_rt: float = numpy.nanmax(retention_times) + 20
 
 	for repeat_idx, (_, repeat) in enumerate(project.datafile_data.items()):
-		assert repeat.qualified_peaks is not None
-		peak = repeat.qualified_peaks[peak_idx]
 		assert repeat.datafile.intensity_matrix is not None
 		im = repeat.datafile.intensity_matrix
 		tic = im.tic
 
 		# Get subset of timelist within RT range
 		time_list = []
 		intensity_list = []
 		for rt, intensity in zip(tic.time_list, tic.intensity_array):
 			if min_rt <= rt <= max_rt:
 				time_list.append(rt / 60)
 				intensity_list.append(intensity)
 
 		axes[repeat_idx].plot(time_list, intensity_list)
-		draw_peak_vlines(axes[repeat_idx], peak.rt / 60, intensity_list[time_list.index(peak.rt / 60)])
-		axes[repeat_idx].text(
-				peak.rt / 60,
-				axes[repeat_idx].get_ylim()[1] * 0.2,
-				f" {peak.rt/60:0.3f}",
-				)
+		peak_rt = retention_times[repeat_idx]
+		if not numpy.isnan(peak_rt):
+			draw_peak_vlines(axes[repeat_idx], peak_rt / 60, intensity_list[time_list.index(peak_rt / 60)])
+			axes[repeat_idx].text(
+					peak_rt / 60,
+					axes[repeat_idx].get_ylim()[1] * 0.2,
+					f" {peak_rt/60:0.3f}",
+					)
 	figure.supylabel("Intensity", fontsize="medium")
 	axes[0].autoscale()
 	axes[-1].set_xlabel("Retention Time (mins)")
 	for ax, repeat_name in zip(axes, project.datafile_data):
 		ax.ticklabel_format(axis='y', scilimits=(0, 0), useMathText=True)
 		ax.set_ylim(bottom=0)
 		# xmin, xmax = ax.get_xlim()
```

### Comparing `libgunshotmatch_mpl-0.5.2/libgunshotmatch_mpl/combined_chromatogram.py` & `libgunshotmatch_mpl-0.6.0b1/libgunshotmatch_mpl/combined_chromatogram.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,16 +85,16 @@
 	:param use_peak_height: Show the peak height and not the peak area.
 	"""
 
 	if use_peak_height:
 		areas = []
 		ms: Optional["MassSpectrum"]
 		for ms in peak.ms_list:
-			assert ms is not None
-			areas.append(sum(ms.intensity_list))
+			if ms is not None:
+				areas.append(sum(ms.intensity_list))
 	else:
 		areas = peak.area_list
 
 	if use_median:
 		area: float = numpy.nanmedian(areas)
 		_25th_percentile: float = numpy.nanpercentile(areas, 25)
 		_75th_percentile: float = numpy.nanpercentile(areas, 75)
```

### Comparing `libgunshotmatch_mpl-0.5.2/libgunshotmatch_mpl/chromatogram.py` & `libgunshotmatch_mpl-0.6.0b1/libgunshotmatch_mpl/chromatogram.py`

 * *Files identical despite different names*

### Comparing `libgunshotmatch_mpl-0.5.2/libgunshotmatch_mpl/__init__.py` & `libgunshotmatch_mpl-0.6.0b1/libgunshotmatch_mpl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,9 +25,9 @@
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2023-2024 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.5.2"
+__version__: str = "0.6.0b1"
 __email__: str = "dominic@davis-foster.co.uk"
```

