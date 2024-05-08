# Comparing `tmp/nrtk-0.4.0.tar.gz` & `tmp/nrtk-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrtk-0.4.0.tar", max compression
+gzip compressed data, was "nrtk-0.4.1.tar", max compression
```

## Comparing `nrtk-0.4.0.tar` & `nrtk-0.4.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    10173 2024-05-06 20:03:32.927344 nrtk-0.4.0/LICENSE
--rw-r--r--   0        0        0      554 2024-05-06 20:03:32.927344 nrtk-0.4.0/NOTICE
--rw-r--r--   0        0        0     2006 2024-05-06 20:03:32.931344 nrtk-0.4.0/README.md
--rw-r--r--   0        0        0      246 2024-05-06 20:03:32.959344 nrtk-0.4.0/nrtk/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/impls/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/impls/gen_object_detector_blackbox_response/__init__.py
--rw-r--r--   0        0        0     1986 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/gen_object_detector_blackbox_response/simple_generic_generator.py
--rw-r--r--   0        0        0     3302 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/gen_object_detector_blackbox_response/simple_pybsm_generator.py
--rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/impls/perturb_image/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/impls/perturb_image/generic/PIL/__init__.py
--rw-r--r--   0        0        0     4774 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/perturb_image/generic/PIL/enhance.py
--rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/impls/perturb_image/generic/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/impls/perturb_image/generic/cv2/__init__.py
--rw-r--r--   0        0        0     2702 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/perturb_image/generic/cv2/blur.py
--rw-r--r--   0        0        0      706 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/perturb_image/generic/nop_perturber.py
--rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/impls/perturb_image/generic/skimage/__init__.py
--rw-r--r--   0        0        0     6560 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/perturb_image/generic/skimage/random_noise.py
--rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/impls/perturb_image/pybsm/__init__.py
--rw-r--r--   0        0        0     3569 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/perturb_image/pybsm/perturber.py
--rw-r--r--   0        0        0     5067 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/perturb_image/pybsm/scenario.py
--rw-r--r--   0        0        0     8611 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/perturb_image/pybsm/sensor.py
--rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/impls/perturb_image_factory/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/impls/perturb_image_factory/generic/__init__.py
--rw-r--r--   0        0        0     1656 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/perturb_image_factory/generic/step.py
--rw-r--r--   0        0        0     3160 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/perturb_image_factory/pybsm.py
--rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/impls/score_detections/__init__.py
--rw-r--r--   0        0        0     2661 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/score_detections/class_agnostic_pixelwise_iou_scorer.py
--rw-r--r--   0        0        0     4277 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/score_detections/coco_scorer.py
--rw-r--r--   0        0        0     1346 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/score_detections/nop_scorer.py
--rw-r--r--   0        0        0     1617 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/impls/score_detections/random_scorer.py
--rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/interfaces/__init__.py
--rw-r--r--   0        0        0     2836 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/interfaces/gen_blackbox_response.py
--rw-r--r--   0        0        0     5401 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/interfaces/gen_classifier_blackbox_response.py
--rw-r--r--   0        0        0     5394 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/interfaces/gen_object_detector_blackbox_response.py
--rw-r--r--   0        0        0     1121 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/interfaces/perturb_image.py
--rw-r--r--   0        0        0     2750 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/interfaces/perturb_image_factory.py
--rw-r--r--   0        0        0     1345 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/interfaces/score_classifications.py
--rw-r--r--   0        0        0     1572 2024-05-06 20:03:32.963344 nrtk-0.4.0/nrtk/interfaces/score_detections.py
--rw-r--r--   0        0        0        0 2024-05-06 20:11:48.487575 nrtk-0.4.0/nrtk/interop/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 20:11:48.491575 nrtk-0.4.0/nrtk/py.typed
--rw-r--r--   0        0        0        0 2024-05-06 20:11:48.491575 nrtk-0.4.0/nrtk/utils/__init__.py
--rw-r--r--   0        0        0     2855 2024-05-06 20:03:32.967344 nrtk-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3525 1970-01-01 00:00:00.000000 nrtk-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    10173 2024-05-08 17:36:32.920911 nrtk-0.4.1/LICENSE
+-rw-r--r--   0        0        0      554 2024-05-08 17:36:32.920911 nrtk-0.4.1/NOTICE
+-rw-r--r--   0        0        0     2006 2024-05-08 17:36:32.920911 nrtk-0.4.1/README.md
+-rw-r--r--   0        0        0      246 2024-05-08 17:36:32.964911 nrtk-0.4.1/nrtk/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:36:33.020912 nrtk-0.4.1/nrtk/impls/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:36:33.020912 nrtk-0.4.1/nrtk/impls/gen_object_detector_blackbox_response/__init__.py
+-rw-r--r--   0        0        0     1986 2024-05-08 17:36:32.964911 nrtk-0.4.1/nrtk/impls/gen_object_detector_blackbox_response/simple_generic_generator.py
+-rw-r--r--   0        0        0     3302 2024-05-08 17:36:32.964911 nrtk-0.4.1/nrtk/impls/gen_object_detector_blackbox_response/simple_pybsm_generator.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:36:33.020912 nrtk-0.4.1/nrtk/impls/perturb_image/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:36:33.020912 nrtk-0.4.1/nrtk/impls/perturb_image/generic/PIL/__init__.py
+-rw-r--r--   0        0        0     4774 2024-05-08 17:36:32.964911 nrtk-0.4.1/nrtk/impls/perturb_image/generic/PIL/enhance.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:36:33.020912 nrtk-0.4.1/nrtk/impls/perturb_image/generic/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:36:33.020912 nrtk-0.4.1/nrtk/impls/perturb_image/generic/cv2/__init__.py
+-rw-r--r--   0        0        0     2702 2024-05-08 17:36:32.964911 nrtk-0.4.1/nrtk/impls/perturb_image/generic/cv2/blur.py
+-rw-r--r--   0        0        0      706 2024-05-08 17:36:32.964911 nrtk-0.4.1/nrtk/impls/perturb_image/generic/nop_perturber.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:36:33.020912 nrtk-0.4.1/nrtk/impls/perturb_image/generic/skimage/__init__.py
+-rw-r--r--   0        0        0     6560 2024-05-08 17:36:32.964911 nrtk-0.4.1/nrtk/impls/perturb_image/generic/skimage/random_noise.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:36:33.020912 nrtk-0.4.1/nrtk/impls/perturb_image/pybsm/__init__.py
+-rw-r--r--   0        0        0     4534 2024-05-08 17:36:32.964911 nrtk-0.4.1/nrtk/impls/perturb_image/pybsm/perturber.py
+-rw-r--r--   0        0        0     5065 2024-05-08 17:36:32.964911 nrtk-0.4.1/nrtk/impls/perturb_image/pybsm/scenario.py
+-rw-r--r--   0        0        0     9671 2024-05-08 17:36:32.964911 nrtk-0.4.1/nrtk/impls/perturb_image/pybsm/sensor.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:36:33.020912 nrtk-0.4.1/nrtk/impls/perturb_image_factory/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:36:33.020912 nrtk-0.4.1/nrtk/impls/perturb_image_factory/generic/__init__.py
+-rw-r--r--   0        0        0     1656 2024-05-08 17:36:32.968911 nrtk-0.4.1/nrtk/impls/perturb_image_factory/generic/step.py
+-rw-r--r--   0        0        0     4065 2024-05-08 17:36:32.968911 nrtk-0.4.1/nrtk/impls/perturb_image_factory/pybsm.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:36:33.020912 nrtk-0.4.1/nrtk/impls/score_detections/__init__.py
+-rw-r--r--   0        0        0     2661 2024-05-08 17:36:32.968911 nrtk-0.4.1/nrtk/impls/score_detections/class_agnostic_pixelwise_iou_scorer.py
+-rw-r--r--   0        0        0     4277 2024-05-08 17:36:32.968911 nrtk-0.4.1/nrtk/impls/score_detections/coco_scorer.py
+-rw-r--r--   0        0        0     1346 2024-05-08 17:36:32.968911 nrtk-0.4.1/nrtk/impls/score_detections/nop_scorer.py
+-rw-r--r--   0        0        0     1617 2024-05-08 17:36:32.968911 nrtk-0.4.1/nrtk/impls/score_detections/random_scorer.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:36:33.020912 nrtk-0.4.1/nrtk/interfaces/__init__.py
+-rw-r--r--   0        0        0     2836 2024-05-08 17:36:32.968911 nrtk-0.4.1/nrtk/interfaces/gen_blackbox_response.py
+-rw-r--r--   0        0        0     5401 2024-05-08 17:36:32.968911 nrtk-0.4.1/nrtk/interfaces/gen_classifier_blackbox_response.py
+-rw-r--r--   0        0        0     5394 2024-05-08 17:36:32.968911 nrtk-0.4.1/nrtk/interfaces/gen_object_detector_blackbox_response.py
+-rw-r--r--   0        0        0     1121 2024-05-08 17:36:32.968911 nrtk-0.4.1/nrtk/interfaces/perturb_image.py
+-rw-r--r--   0        0        0     2750 2024-05-08 17:36:32.968911 nrtk-0.4.1/nrtk/interfaces/perturb_image_factory.py
+-rw-r--r--   0        0        0     1345 2024-05-08 17:36:32.968911 nrtk-0.4.1/nrtk/interfaces/score_classifications.py
+-rw-r--r--   0        0        0     1572 2024-05-08 17:36:32.968911 nrtk-0.4.1/nrtk/interfaces/score_detections.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:36:33.020912 nrtk-0.4.1/nrtk/interop/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:36:33.020912 nrtk-0.4.1/nrtk/py.typed
+-rw-r--r--   0        0        0        0 2024-05-08 17:36:33.020912 nrtk-0.4.1/nrtk/utils/__init__.py
+-rw-r--r--   0        0        0     4204 2024-05-08 17:36:32.972911 nrtk-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3525 1970-01-01 00:00:00.000000 nrtk-0.4.1/PKG-INFO
```

### Comparing `nrtk-0.4.0/LICENSE` & `nrtk-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.0/NOTICE` & `nrtk-0.4.1/NOTICE`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.0/README.md` & `nrtk-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.0/nrtk/impls/gen_object_detector_blackbox_response/simple_generic_generator.py` & `nrtk-0.4.1/nrtk/impls/gen_object_detector_blackbox_response/simple_generic_generator.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.0/nrtk/impls/gen_object_detector_blackbox_response/simple_pybsm_generator.py` & `nrtk-0.4.1/nrtk/impls/gen_object_detector_blackbox_response/simple_pybsm_generator.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.0/nrtk/impls/perturb_image/generic/PIL/enhance.py` & `nrtk-0.4.1/nrtk/impls/perturb_image/generic/PIL/enhance.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.0/nrtk/impls/perturb_image/generic/cv2/blur.py` & `nrtk-0.4.1/nrtk/impls/perturb_image/generic/cv2/blur.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.0/nrtk/impls/perturb_image/generic/nop_perturber.py` & `nrtk-0.4.1/nrtk/impls/perturb_image/generic/nop_perturber.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.0/nrtk/impls/perturb_image/generic/skimage/random_noise.py` & `nrtk-0.4.1/nrtk/impls/perturb_image/generic/skimage/random_noise.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.0/nrtk/impls/perturb_image/pybsm/perturber.py` & `nrtk-0.4.1/nrtk/impls/perturb_image/pybsm/perturber.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from __future__ import annotations
 import copy
-from typing import Any, Dict
-
 import numpy as np
 from pybsm.simulation import RefImage, simulate_image
+from typing import Any, Dict, Type
+
+from smqtk_core.configuration import to_config_dict, from_config_dict, make_default_config
 
 from nrtk.impls.perturb_image.pybsm.sensor import PybsmSensor
 from nrtk.impls.perturb_image.pybsm.scenario import PybsmScenario
 from nrtk.interfaces.perturb_image import PerturbImage
 
 
 class PybsmPerturber(PerturbImage):
@@ -90,20 +92,46 @@
 
     def __str__(self) -> str:
         return self.sensor.name + " " + self.scenario.name
 
     def __repr__(self) -> str:
         return self.sensor.name + " " + self.scenario.name
 
+    @classmethod
+    def get_default_config(cls) -> Dict[str, Any]:
+        cfg = super().get_default_config()
+        cfg["sensor"] = make_default_config([PybsmSensor])
+        cfg["scenario"] = make_default_config([PybsmScenario])
+        cfg["reflectance_range"] = cfg["reflectance_range"].tolist()
+
+        return cfg
+
+    @classmethod
+    def from_config(
+        cls: Type[PybsmPerturber],
+        config_dict: Dict,
+        merge_default: bool = True
+    ) -> PybsmPerturber:
+        config_dict = dict(config_dict)
+
+        config_dict["sensor"] = from_config_dict(
+            config_dict["sensor"],
+            [PybsmSensor]
+        )
+        config_dict["scenario"] = from_config_dict(
+            config_dict["scenario"],
+            [PybsmScenario]
+        )
+
+        # Convert input data to expected constructor types
+        config_dict["reflectance_range"] = np.array(config_dict["reflectance_range"])
+
+        return super().from_config(config_dict, merge_default=merge_default)
+
     def get_config(self) -> Dict[str, Any]:
         config = {
-            'sensor': self.sensor.get_config(),
-            'scenario': self.scenario.get_config(),
-            'reflectance_range': self.reflectance_range
+            'sensor': to_config_dict(self.sensor),
+            'scenario': to_config_dict(self.scenario),
+            'reflectance_range': self.reflectance_range.tolist()
         }
 
-        for k in self.sensor.__dict__:
-            config[k] = getattr(self.sensor, k)
-        for k in self.scenario.__dict__:
-            config[k] = getattr(self.scenario, k)
-
         return config
```

### Comparing `nrtk-0.4.0/nrtk/impls/perturb_image/pybsm/scenario.py` & `nrtk-0.4.1/nrtk/impls/perturb_image/pybsm/scenario.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any
 from typing import Dict, Optional
 
 from pybsm.simulation.scenario import Scenario
-from smqtk_core import Plugfigurable
+from smqtk_core import Configurable
 
 
-class PybsmScenario(Plugfigurable):
+class PybsmScenario(Configurable):
     """
     Wrapper for pybsm.scenario.
 
     ihaze:
         MODTRAN code for visibility, valid options are ihaze = 1 (Rural extinction with 23 km visibility)
         or ihaze = 2 (Rural extinction with 5 km visibility)
     altitude:
```

### Comparing `nrtk-0.4.0/nrtk/impls/perturb_image/pybsm/sensor.py` & `nrtk-0.4.1/nrtk/impls/perturb_image/pybsm/sensor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 from typing import Any
-from typing import Dict, Optional
+from typing import Dict, Optional, Type
 
 import numpy as np
 from pybsm.simulation.sensor import Sensor
-from smqtk_core import Plugfigurable
+from smqtk_core import Configurable
 
 
-class PybsmSensor(Plugfigurable):
+class PybsmSensor(Configurable):
     """
     Wrapper for pybsm.sensor.
 
     Attributes (the first four are mandatory):
     ------------------------------------------
     name :
         name of the sensor (string)
@@ -202,31 +202,55 @@
         self
     ) -> Sensor:
         """
         Alias for :meth:`.StoreSensor.sensor`.
         """
         return self.create_sensor()
 
+    @classmethod
+    def from_config(
+        cls: Type[PybsmSensor],
+        config_dict: Dict,
+        merge_default: bool = True
+    ) -> PybsmSensor:
+        config_dict = dict(config_dict)
+
+        # Convert input data to expected constructor types
+        config_dict["optTransWavelengths"] = np.array(config_dict["optTransWavelengths"])
+
+        # Non-JSON type arguments with defaults (so they might not be there)
+        opticsTransmission = config_dict.get("opticsTransmission", None)
+        if opticsTransmission is not None:
+            config_dict["opticsTransmission"] = np.array(config_dict["opticsTransmission"])
+        qewavelengths = config_dict.get("qewavelengths", None)
+        if qewavelengths is not None:
+            config_dict["qewavelengths"] = np.array(config_dict["qewavelengths"])
+        qe = config_dict.get("qe", None)
+        if qe is not None:
+            config_dict["qe"] = np.array(config_dict["qe"])
+
+        return super().from_config(config_dict, merge_default=merge_default)
+
     def get_config(self) -> Dict[str, Any]:
         return {
             'name': self.name,
             'D': self.D,
             'f': self.f,
             'px': self.px,
-            'optTransWavelengths': self.optTransWavelengths,
-            'opticsTransmission': self.opticsTransmission,
+            'optTransWavelengths': self.optTransWavelengths.tolist(),
+            'opticsTransmission': self.opticsTransmission.tolist(),
             'eta': self.eta,
             'wx': self.wx,
             'wy': self.wy,
             'intTime': self.intTime,
             'darkCurrent': self.darkCurrent,
             'readNoise': self.readNoise,
             'maxN': self.maxN,
             'bitdepth': self.bitdepth,
             'maxWellFill': self.maxWellFill,
             'sx': self.sx,
             'sy': self.sy,
             'dax': self.dax,
             'day': self.day,
-            'qewavelengths': self.qewavelengths,
-            'qe': self.qe,
+            'qewavelengths': self.qewavelengths.tolist(),
+            'qe': self.qe.tolist(),
         }
```

### Comparing `nrtk-0.4.0/nrtk/impls/perturb_image_factory/generic/step.py` & `nrtk-0.4.1/nrtk/impls/perturb_image_factory/generic/step.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.0/nrtk/impls/score_detections/class_agnostic_pixelwise_iou_scorer.py` & `nrtk-0.4.1/nrtk/impls/score_detections/class_agnostic_pixelwise_iou_scorer.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.0/nrtk/impls/score_detections/coco_scorer.py` & `nrtk-0.4.1/nrtk/impls/score_detections/coco_scorer.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.0/nrtk/impls/score_detections/nop_scorer.py` & `nrtk-0.4.1/nrtk/impls/score_detections/nop_scorer.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.0/nrtk/impls/score_detections/random_scorer.py` & `nrtk-0.4.1/nrtk/impls/score_detections/random_scorer.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.0/nrtk/interfaces/gen_blackbox_response.py` & `nrtk-0.4.1/nrtk/interfaces/gen_blackbox_response.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.0/nrtk/interfaces/gen_classifier_blackbox_response.py` & `nrtk-0.4.1/nrtk/interfaces/gen_classifier_blackbox_response.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.0/nrtk/interfaces/gen_object_detector_blackbox_response.py` & `nrtk-0.4.1/nrtk/interfaces/gen_object_detector_blackbox_response.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.0/nrtk/interfaces/perturb_image.py` & `nrtk-0.4.1/nrtk/interfaces/perturb_image.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.0/nrtk/interfaces/perturb_image_factory.py` & `nrtk-0.4.1/nrtk/interfaces/perturb_image_factory.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.0/nrtk/interfaces/score_classifications.py` & `nrtk-0.4.1/nrtk/interfaces/score_classifications.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.0/nrtk/interfaces/score_detections.py` & `nrtk-0.4.1/nrtk/interfaces/score_detections.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.4.0/PKG-INFO` & `nrtk-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrtk
-Version: 0.4.0
+Version: 0.4.1
 Summary: An open source toolkit for evaluating the natural robustness of computer vision algorithms.
 License: Apache-2.0
 Author: Kitware, Inc.
 Author-email: nrtk@kitware.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

