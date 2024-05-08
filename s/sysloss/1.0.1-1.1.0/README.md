# Comparing `tmp/sysloss-1.0.1.tar.gz` & `tmp/sysloss-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysloss-1.0.1.tar", max compression
+gzip compressed data, was "sysloss-1.1.0.tar", max compression
```

## Comparing `sysloss-1.0.1.tar` & `sysloss-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2024-04-29 15:01:39.280490 sysloss-1.0.1/LICENSE
--rw-r--r--   0        0        0     2488 2024-04-29 15:01:39.280490 sysloss-1.0.1/README.md
--rw-r--r--   0        0        0     1585 2024-04-29 15:01:50.184508 sysloss-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-29 15:01:39.288490 sysloss-1.0.1/src/sysloss/__init__.py
--rw-r--r--   0        0        0    29244 2024-04-29 15:01:39.288490 sysloss-1.0.1/src/sysloss/components.py
--rw-r--r--   0        0        0    46897 2024-04-29 15:01:39.288490 sysloss-1.0.1/src/sysloss/system.py
--rw-r--r--   0        0        0     3390 1970-01-01 00:00:00.000000 sysloss-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-08 16:12:08.645780 sysloss-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2621 2024-05-08 16:12:08.645780 sysloss-1.1.0/README.md
+-rw-r--r--   0        0        0     1620 2024-05-08 16:12:18.625846 sysloss-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-08 16:12:18.625846 sysloss-1.1.0/src/sysloss/__init__.py
+-rw-r--r--   0        0        0    29244 2024-05-08 16:12:08.653780 sysloss-1.1.0/src/sysloss/components.py
+-rw-r--r--   0        0        0    51609 2024-05-08 16:12:08.653780 sysloss-1.1.0/src/sysloss/system.py
+-rw-r--r--   0        0        0     3574 1970-01-01 00:00:00.000000 sysloss-1.1.0/PKG-INFO
```

### Comparing `sysloss-1.0.1/LICENSE` & `sysloss-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sysloss-1.0.1/README.md` & `sysloss-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 <p align="center">
 <a href="https://github.com/geddy11/sysloss/actions"><img alt="Actions Status" src="https://github.com/geddy11/sysloss/actions/workflows/ci-cd.yml/badge.svg"></a>
 <a href="https://codecov.io/github/geddy11/sysloss"><img src="https://codecov.io/github/geddy11/sysloss/graph/badge.svg?token=9L1ZMN0UET"/></a>
 <a><img alt="PyPI" src="https://img.shields.io/pypi/v/sysloss"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 <a href="https://www.conventionalcommits.org"><img alt="Conv. commits" src="https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white"></a>
+<a href="https://doi.org/10.5281/zenodo.11086061"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.11086061.svg" alt="DOI"></a>
 </p>
 
 # sysLoss
 sysLoss is a tool for analyzing system power and losses. From the smallest IoT sensor to large industrial installations. The tool is efficient and easy to use, the analysis result provides a detailed report on voltages, currents, power and efficiency for every component defined in the system. Output format is Pandas DataFrame: Create charts, plots and export to Excel and other formats. 
 
 ## Installation
 ```bash
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 ![](https://github.com/geddy11/sysloss/raw/main/docs/sysloss.svg)
        _[_A_c_t_i_o_n_s_ _S_t_a_t_u_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_i_t_h_u_b_/_g_e_d_d_y_1_1_/_s_y_s_l_o_s_s_/_g_r_a_p_h_/
-      _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_9_L_1_Z_M_N_0_U_E_T_][PyPI]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_C_o_n_v_._ _c_o_m_m_i_t_s_]
+   _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_9_L_1_Z_M_N_0_U_E_T_][PyPI]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_C_o_n_v_._ _c_o_m_m_i_t_s_]_[_D_O_I_]
 # sysLoss sysLoss is a tool for analyzing system power and losses. From the
 smallest IoT sensor to large industrial installations. The tool is efficient
 and easy to use, the analysis result provides a detailed report on voltages,
 currents, power and efficiency for every component defined in the system.
 Output format is Pandas DataFrame: Create charts, plots and export to Excel and
 other formats. ## Installation ```bash $ pip install sysloss ``` ## Usage
 ```python from sysloss.components import * from sysloss.system import System
```

### Comparing `sysloss-1.0.1/pyproject.toml` & `sysloss-1.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 [tool.poetry]
 name = "sysloss"
-version = "1.0.1"
+version = "1.1.0"
 description = "Power analysis of circuits and systems."
 authors = ["Geir Drange"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/geddy11/sysloss"
 repository = "https://github.com/geddy11/sysloss"
 documentation = "https://sysloss.readthedocs.io/en/latest/Getting%20started.html#"
 keywords = ["system", "power" , "loss", "efficiency", "energy", "component"]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 scipy = "^1.9.0"
 pandas = "^2.0.0"
 rustworkx = "^0.13.0"
 rich = "^12.0.0"
 toml = "^0.10.2"
 matplotlib = "^3.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^4.0.0"
 matplotlib = "^3.0.0"
 jupyter-book = "^1.0.0"
 toml = "^0.10.2"
 pandas = "^2.0.0"
+tqdm = "^4.63.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 scipy = "^1.9.0"
 pandas = "^2.0.0"
 rustworkx = "^0.13.0"
 rich = "^12.0.0"
 toml = "^0.10.2"
 matplotlib = "^3.0.0"
+tqdm = "^4.63.0"
 
 [tool.semantic_release]
 allow_zero_version = false
 version_toml = [
     "pyproject.toml:tool.poetry.version",
 ]                                                    # version location
-version_variable = [
+version_variables = [
     "src/sysloss/__init__.py:__version__"
 ]
 branch = "main"                                      # branch to make releases of
 changelog_file = "CHANGELOG.md"                      # changelog file
 build_command = "pip install poetry && poetry build" # build dists 
 
 [build-system]
```

### Comparing `sysloss-1.0.1/src/sysloss/components.py` & `sysloss-1.1.0/src/sysloss/components.py`

 * *Files identical despite different names*

### Comparing `sysloss-1.0.1/src/sysloss/system.py` & `sysloss-1.1.0/src/sysloss/system.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,26 +28,34 @@
 from rich.tree import Tree
 import json
 import pandas as pd
 import matplotlib
 import matplotlib.pyplot as plt
 from matplotlib.ticker import LinearLocator
 from scipy.interpolate import LinearNDInterpolator
+from typing import Callable
+import warnings
+from tqdm import TqdmExperimentalWarning
+
+warnings.filterwarnings("ignore", category=TqdmExperimentalWarning)
+from tqdm.autonotebook import tqdm
+
 from sysloss.components import *
 from sysloss.components import (
     _ComponentTypes,
     _get_opt,
     _get_mand,
     _get_eff,
     _Interp0d,
     _Interp1d,
     _Interp2d,
     RS_DEFAULT,
     LIMITS_DEFAULT,
 )
+import sysloss
 
 
 class System:
     """System to be analyzed. The first component of a system must always be a :py:class:`~components.Source`.
 
     Parameters
     ----------
@@ -614,15 +622,15 @@
         *,
         vtol: float = 1e-6,
         itol: float = 1e-6,
         maxiter: int = 10000,
         quiet: bool = True,
         phase: str = "",
         energy: bool = False,
-        tags: dict = {}
+        tags: dict = {},
     ) -> pd.DataFrame:
         """Analyze steady-state of system.
 
         Parameters
         ----------
         vtol : float, optional
             Voltage tolerance., by default 1e-6
@@ -658,15 +666,15 @@
                 raise ValueError(
                     "The specified phase '{}' is not defined".format(phase)
                 )
             phase_list = [phase]
         elif len(list(self._g.attrs["phases"].keys())) > 0:
             phase_list = list(self._g.attrs["phases"].keys())
         # solve
-        ppwr, ploss, peff, ptime, pener = [], [], [], [], []
+        ppwr, ploss, peff, ptime, pener, pcurr = [], [], [], [], [], []
         frames = []
         for ph in phase_list:
             v, i, iters = self._solve(vtol, itol, maxiter, quiet, ph)
             if iters > maxiter:
                 raise RuntimeError(
                     "Steady-state not achieved after {} iterations".format(iters - 1)
                 )
@@ -775,18 +783,22 @@
             res["Loss (W)"] = loss
             res["Efficiency (%)"] = eff
             if energy:
                 res["24h energy (Wh)"] = ener
             res["Warnings"] = warn
             df = pd.DataFrame(res)
 
-            # update subsystem power/loss/efficiency/energy
+            # update subsystem current/power/loss/efficiency/energy
             for d in range(len(sources)):
                 src = list(sources.keys())[d]
                 idx = df[df.Component == "Subsystem {}".format(src)].index[0]
+                curr = df[(df.Domain == src) & (df.Type == "SOURCE")][
+                    "Iout (A)"
+                ].values[0]
+                df.at[idx, "Iout (A)"] = curr
                 pwr = df[(df.Domain == src) & (df.Type == "SOURCE")][
                     "Power (W)"
                 ].values[0]
                 df.at[idx, "Power (W)"] = pwr
                 loss = df[df.Domain == src]["Loss (W)"].sum()
                 df.at[idx, "Loss (W)"] = loss
                 df.at[idx, "Efficiency (%)"] = _get_eff(pwr, pwr - loss)
@@ -798,35 +810,41 @@
             idx = df.index[-1]
             df.at[idx, "Power (W)"] = pwr
             loss = df[(df.Domain == "") & (df["Loss (W)"] != "")]["Loss (W)"].sum()
             df.at[idx, "Loss (W)"] = loss
             df.at[idx, "Efficiency (%)"] = _get_eff(pwr, pwr - loss)
             if energy:
                 df.at[idx, "24h energy (Wh)"] = self._calc_energy(ph, pwr)
+            if len(sources) < 2:
+                df.at[idx, "Iout (A)"] = curr
             if len(phase_list) > 1:
                 ploss += [loss]
                 ppwr += [pwr]
                 peff += [_get_eff(pwr, pwr - loss)]
+                pcurr += [curr]
                 ptime += [self._g.attrs["phases"][ph]]
                 pener += [self._calc_energy(ph, pwr)]
-
             # if only one subsystem, delete subsystem row and domain column
             if len(sources) < 2:
                 df.drop(len(df) - 2, inplace=True)
                 df.drop(columns="Domain", inplace=True)
                 df.reset_index(inplace=True, drop=True)
             frames += [df]
 
         if len(phase_list) > 1:
             ttot = np.sum(np.asarray(ptime))
             apwr = np.sum(np.multiply(np.asarray(ppwr), np.asarray(ptime))) / ttot
             aloss = np.sum(np.multiply(np.asarray(ploss), np.asarray(ptime))) / ttot
             aeff = np.sum(np.multiply(np.asarray(peff), np.asarray(ptime))) / ttot
+            acurr = np.sum(np.multiply(np.asarray(pcurr), np.asarray(ptime))) / ttot
             vals = ["System average", apwr, aloss, aeff]
             idxs = ["Component", "Power (W)", "Loss (W)", "Efficiency (%)"]
+            if len(sources) < 2:
+                vals += [acurr]
+                idxs += ["Iout (A)"]
             if energy:
                 vals += [self._calc_energy("", apwr)]
                 idxs += ["24h energy (Wh)"]
             if tags != {}:
                 for key in tags.keys():
                     idxs += [key]
                     vals += [tags[key]]
@@ -945,15 +963,15 @@
 
         Raises
         ------
         ValueError
             If the dict contains less than two load phases or 'N/A' is used as
             a phase name.
         """
-        if len(list(phases.keys())) < 2:
+        if len(list(phases.keys())) < 2 and phases != {}:
             raise ValueError("There must be at least two phases!")
         if "N/A" in list(phases.keys()):
             raise ValueError('"N/A" is a reserved name!')
         self._g.attrs["phases"] = phases
 
     def get_sys_phases(self) -> dict:
         """Get the system level load phases.
@@ -1093,19 +1111,19 @@
         indent : int, optional
             Indentation to use in .json file, by default 4
         """
         self._rel_update()
         sys = {
             "system": {
                 "name": self._g.attrs["name"],
-                "version": "1.0.0",
+                "version": sysloss.__version__,
                 "phases": self._g.attrs["phases"],
                 "phase_conf": self._g.attrs["phase_conf"],
             }
-        }  # TODO: version
+        }
         ridx = self._get_sources()
         root = [self._g[n]._params["name"] for n in ridx]
         for r in range(len(ridx)):
             tree = self._get_childs_tree(ridx[r])
             cdict = {}
             if tree != {}:
                 for e in tree:
@@ -1131,15 +1149,15 @@
 
     def plot_interp(
         self,
         name: str,
         *,
         cmap: matplotlib.colors.Colormap = "viridis",
         inpdata: bool = True,
-        plot3d: bool = False
+        plot3d: bool = False,
     ) -> matplotlib.figure.Figure | None:
         """Plot 1D or 2D interpolation data.
 
         If a component has a parameter defined as either 1D or 2D interpolation data,
         a figure is returned with linear interpolation shown. 1D data is plotted as an
         interpolated line. 2D data can be shown as 2D color map or 3D surface. The
         interpolated data is extended to +/-15% outside of input data points.
@@ -1246,7 +1264,110 @@
                 )
             else:
                 plt.title("{} voltage drop".format(name))
             return fig
         else:
             print("Component does not have interpolation data")
             return None
+
+    def batt_life(
+        self,
+        battery: str,
+        *,
+        cutoff: float,
+        pfunc: Callable[[], tuple[float, float, float]],
+        dfunc: Callable[[float, float], tuple[float, float, float]],
+    ) -> pd.DataFrame:
+        """Estimate battery life.
+
+        Battery life estimation requires an external battery model. The battery model is
+        accessed using two callback functions - one for battery probing and one for
+        battery depletion. If system load phases have been defined, the estimation process
+        loops through the phases until the battery is depleted or the cutoff voltage has been
+        reached. In a system without load phases the process depletes the battery in ~1000
+        time steps.
+
+        Parameters
+        ----------
+        battery : str
+            Name of battery (source) to be depleted
+        cutoff : float
+            End simulation when battery voltage reaches cutoff or capacity is depleted,
+            whichever comes first.
+        pfunc : Callable[[], tuple[float, float, float]]
+            Battery probe callback function, must return tuple with remaining capacity (Ah),
+            battery voltage (V) and battery impedance (Ohm)
+        dfunc : Callable[[float, float], tuple[float, float, float]]
+            Battery deplete callback function. Function arguments are time (s) and
+            current (A). Must return tuple with same format as pfunc.
+
+        Returns
+        -------
+        pd.DataFrame
+            Battery depletion data.
+
+        Raises
+        ------
+        ValueError
+            If battery name is not found or component is not a source.
+        """
+        # check for valid source
+        self._chk_parent(battery)
+        pidx = self._get_index(battery)
+        if not isinstance(self._g[pidx], Source):
+            raise ValueError("Battery must be a source!")
+        # keep current source params
+        vo_org = self._g[pidx]._params["vo"]
+        rs_org = self._g[pidx]._params["rs"]
+        # probe/deplete returns (capacity, voltage, rs)
+        state = pfunc()
+        t = [0.0]
+        cap = [state[0]]
+        volt = [state[1]]
+        rs = [state[2]]
+        phase_list = [""]
+        if len(list(self._g.attrs["phases"].keys())) > 0:
+            phase_list = list(self._g.attrs["phases"].keys())
+        # deplete args: time, current
+        unit, mult = "Ah", 1.0
+        if state[0] < 100.0:
+            unit, mult = "mAh", 1000.0
+        self._rel_update()
+        cdelta = 0.0
+        phidx = 0
+        with tqdm(
+            range(int(mult * cap[0])),
+            desc="Battery depletion ({})".format(unit),
+            unit=unit,
+            unit_scale=True,
+            unit_divisor=1000,
+        ) as pbar:
+            while state[0] > 0.0 and state[1] > cutoff:
+                self._g[pidx]._params["vo"] = state[1]
+                self._g[pidx]._params["rs"] = state[2]
+                _, i, _ = self._solve(phase=phase_list[phidx])
+                if phase_list == [""]:
+                    deltat = (cap[0] / i[pidx]) * 3.6
+                else:
+                    deltat = self._g.attrs["phases"][phase_list[phidx]]
+                state = dfunc(deltat, i[pidx])
+                cdelta += (cap[-1] - state[0]) * mult
+                pbar.update(int(cdelta))
+                cdelta -= int(cdelta)
+                phidx = (phidx + 1) % len(phase_list)
+                if state[0] > 0.0 and state[1] > cutoff:
+                    t += [t[-1] + deltat]
+                    cap += [state[0]]
+                    volt += [state[1]]
+                    rs += [state[2]]
+            pbar.total = int(mult * cap[0] - cdelta)
+            pbar.close()
+        # restore source params
+        self._g[pidx]._params["vo"] = vo_org
+        self._g[pidx]._params["rs"] = rs_org
+        # result
+        res = {}
+        res["Time (s)"] = t
+        res["Capacity (Ah)"] = cap
+        res["Voltage (V)"] = volt
+        res["Resistance (Ohm)"] = rs
+        return pd.DataFrame(res)
```

### Comparing `sysloss-1.0.1/PKG-INFO` & `sysloss-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: sysloss
-Version: 1.0.1
+Version: 1.1.0
 Summary: Power analysis of circuits and systems.
 Home-page: https://github.com/geddy11/sysloss
 License: MIT
 Keywords: system,power,loss,efficiency,energy,component
 Author: Geir Drange
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: matplotlib (>=3.0.0,<4.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: rich (>=12.0.0,<13.0.0)
 Requires-Dist: rustworkx (>=0.13.0,<0.14.0)
 Requires-Dist: scipy (>=1.9.0,<2.0.0)
@@ -26,14 +27,15 @@
 
 <p align="center">
 <a href="https://github.com/geddy11/sysloss/actions"><img alt="Actions Status" src="https://github.com/geddy11/sysloss/actions/workflows/ci-cd.yml/badge.svg"></a>
 <a href="https://codecov.io/github/geddy11/sysloss"><img src="https://codecov.io/github/geddy11/sysloss/graph/badge.svg?token=9L1ZMN0UET"/></a>
 <a><img alt="PyPI" src="https://img.shields.io/pypi/v/sysloss"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 <a href="https://www.conventionalcommits.org"><img alt="Conv. commits" src="https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white"></a>
+<a href="https://doi.org/10.5281/zenodo.11086061"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.11086061.svg" alt="DOI"></a>
 </p>
 
 # sysLoss
 sysLoss is a tool for analyzing system power and losses. From the smallest IoT sensor to large industrial installations. The tool is efficient and easy to use, the analysis result provides a detailed report on voltages, currents, power and efficiency for every component defined in the system. Output format is Pandas DataFrame: Create charts, plots and export to Excel and other formats. 
 
 ## Installation
 ```bash
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: sysloss Version: 1.0.1 Summary: Power analysis of
+Metadata-Version: 2.1 Name: sysloss Version: 1.1.0 Summary: Power analysis of
 circuits and systems. Home-page: https://github.com/geddy11/sysloss License:
 MIT Keywords: system,power,loss,efficiency,energy,component Author: Geir Drange
-Requires-Python: >=3.11,<4.0 Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: matplotlib (>=3.0.0,<4.0.0) Requires-Dist: pandas
-(>=2.0.0,<3.0.0) Requires-Dist: rich (>=12.0.0,<13.0.0) Requires-Dist:
-rustworkx (>=0.13.0,<0.14.0) Requires-Dist: scipy (>=1.9.0,<2.0.0) Requires-
-Dist: toml (>=0.10.2,<0.11.0) Project-URL: Documentation, https://
-sysloss.readthedocs.io/en/latest/Getting%20started.html# Project-URL:
-Repository, https://github.com/geddy11/sysloss Description-Content-Type: text/
-markdown ![](https://github.com/geddy11/sysloss/raw/main/docs/sysloss.svg)
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Requires-Dist: matplotlib
+(>=3.0.0,<4.0.0) Requires-Dist: pandas (>=2.0.0,<3.0.0) Requires-Dist: rich
+(>=12.0.0,<13.0.0) Requires-Dist: rustworkx (>=0.13.0,<0.14.0) Requires-Dist:
+scipy (>=1.9.0,<2.0.0) Requires-Dist: toml (>=0.10.2,<0.11.0) Project-URL:
+Documentation, https://sysloss.readthedocs.io/en/latest/Getting%20started.html#
+Project-URL: Repository, https://github.com/geddy11/sysloss Description-
+Content-Type: text/markdown ![](https://github.com/geddy11/sysloss/raw/main/
+docs/sysloss.svg)
        _[_A_c_t_i_o_n_s_ _S_t_a_t_u_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_i_t_h_u_b_/_g_e_d_d_y_1_1_/_s_y_s_l_o_s_s_/_g_r_a_p_h_/
-      _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_9_L_1_Z_M_N_0_U_E_T_][PyPI]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_C_o_n_v_._ _c_o_m_m_i_t_s_]
+   _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_9_L_1_Z_M_N_0_U_E_T_][PyPI]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_C_o_n_v_._ _c_o_m_m_i_t_s_]_[_D_O_I_]
 # sysLoss sysLoss is a tool for analyzing system power and losses. From the
 smallest IoT sensor to large industrial installations. The tool is efficient
 and easy to use, the analysis result provides a detailed report on voltages,
 currents, power and efficiency for every component defined in the system.
 Output format is Pandas DataFrame: Create charts, plots and export to Excel and
 other formats. ## Installation ```bash $ pip install sysloss ``` ## Usage
 ```python from sysloss.components import * from sysloss.system import System
```

