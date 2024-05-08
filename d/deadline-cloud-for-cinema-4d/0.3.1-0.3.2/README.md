# Comparing `tmp/deadline_cloud_for_cinema_4d-0.3.1.tar.gz` & `tmp/deadline_cloud_for_cinema_4d-0.3.2.tar.gz`

## Comparing `deadline_cloud_for_cinema_4d-0.3.1.tar` & `deadline_cloud_for_cinema_4d-0.3.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/_version.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/_version.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/Cinema4DAdaptor.json
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/__init__.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/__main__.py
--rw-r--r--   0        0        0    17059 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/adaptor.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/schemas/init_data.schema.json
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/schemas/run_data.schema.json
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DClient/__init__.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DClient/cinema4d_client.py
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DClient/cinema4d_handler.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DClient/plugin/DeadlineCloudClient.pyp
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/_version.py
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/adaptor_cinema4d_job_template.yaml
--rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/adaptor_override_environment.yaml
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/assets.py
--rw-r--r--   0        0        0    14924 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/cinema4d_render_submitter.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/data_classes.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/default_cinema4d_job_template.yaml
--rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/scene.py
--rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/style.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/takes.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/ui/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/ui/components/__init__.py
--rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/ui/components/scene_settings_tab.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/NOTICE
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/README.md
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/hatch.toml
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/_version.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_adaptor/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_adaptor/_version.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/Cinema4DAdaptor.json
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/__init__.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/__main__.py
+-rw-r--r--   0        0        0    17059 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/adaptor.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/schemas/init_data.schema.json
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/schemas/run_data.schema.json
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_adaptor/Cinema4DClient/__init__.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_adaptor/Cinema4DClient/cinema4d_client.py
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_adaptor/Cinema4DClient/cinema4d_handler.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_adaptor/Cinema4DClient/plugin/DeadlineCloudClient.pyp
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_submitter/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_submitter/_version.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_submitter/adaptor_cinema4d_job_template.yaml
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_submitter/adaptor_override_environment.yaml
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_submitter/assets.py
+-rw-r--r--   0        0        0    14916 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_submitter/cinema4d_render_submitter.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_submitter/data_classes.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_submitter/default_cinema4d_job_template.yaml
+-rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_submitter/scene.py
+-rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_submitter/style.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_submitter/takes.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_submitter/ui/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_submitter/ui/components/__init__.py
+-rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_submitter/ui/components/scene_settings_tab.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/NOTICE
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/README.md
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/hatch.toml
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 deadline_cloud_for_cinema_4d-0.3.2/PKG-INFO
```

### Comparing `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/__main__.py` & `deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/__main__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/adaptor.py` & `deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_adaptor/Cinema4DAdaptor/adaptor.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DClient/cinema4d_client.py` & `deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_adaptor/Cinema4DClient/cinema4d_client.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DClient/cinema4d_handler.py` & `deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_adaptor/Cinema4DClient/cinema4d_handler.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_adaptor/Cinema4DClient/plugin/DeadlineCloudClient.pyp` & `deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_adaptor/Cinema4DClient/plugin/DeadlineCloudClient.pyp`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/adaptor_cinema4d_job_template.yaml` & `deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_submitter/adaptor_cinema4d_job_template.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/adaptor_override_environment.yaml` & `deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_submitter/adaptor_override_environment.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/assets.py` & `deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_submitter/assets.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/cinema4d_render_submitter.py` & `deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_submitter/cinema4d_render_submitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 from typing import Any, Optional
 import yaml  # type: ignore[import]
 from copy import deepcopy
 from dataclasses import dataclass
 
 import c4d
 
-from PySide2 import QtWidgets
+from qtpy import QtWidgets
 
 from deadline.client.job_bundle.submission import AssetReferences
 from deadline.client.job_bundle._yaml import deadline_yaml_dump
 from deadline.client.ui.dialogs.submit_job_to_deadline_dialog import (  # pylint: disable=import-error
     SubmitJobToDeadlineDialog,
     JobBundlePurpose,
 )
 from deadline.client.exceptions import DeadlineOperationError
-from PySide2.QtCore import Qt  # pylint: disable=import-error
+from qtpy.QtCore import Qt  # type: ignore[attr-defined]
 
 from .data_classes import (
     RenderSubmitterUISettings,
 )
 from .ui.components.scene_settings_tab import SceneSettingsWidget
 from .scene import Animation, Scene
 from .assets import AssetIntrospector
```

### Comparing `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/data_classes.py` & `deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_submitter/data_classes.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/default_cinema4d_job_template.yaml` & `deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_submitter/default_cinema4d_job_template.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/scene.py` & `deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_submitter/scene.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/style.py` & `deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_submitter/style.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.1/src/deadline/cinema4d_submitter/ui/components/scene_settings_tab.py` & `deadline_cloud_for_cinema_4d-0.3.2/src/deadline/cinema4d_submitter/ui/components/scene_settings_tab.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 import os
 
-from PySide2.QtCore import QSize, Qt  # type: ignore
-from PySide2.QtWidgets import (  # type: ignore
+from qtpy.QtCore import QSize, Qt  # type: ignore
+from qtpy.QtWidgets import (  # type: ignore
     QCheckBox,
     QComboBox,
     QFileDialog,
     QGridLayout,
     QHBoxLayout,
     QLabel,
     QLineEdit,
@@ -35,15 +35,14 @@
             raise ValueError("")
 
         self.file_format = file_format
         self.directory_only = directory_only
 
         lyt = QHBoxLayout(self)
         lyt.setContentsMargins(0, 0, 0, 0)
-        lyt.setMargin(0)
 
         self.edit = QLineEdit(self)
         self.btn = QPushButton("...", parent=self)
         self.btn.setMaximumSize(QSize(100, 40))
         self.btn.clicked.connect(self.get_file)
 
         lyt.addWidget(self.edit)
```

### Comparing `deadline_cloud_for_cinema_4d-0.3.1/LICENSE` & `deadline_cloud_for_cinema_4d-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.1/README.md` & `deadline_cloud_for_cinema_4d-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.1/hatch.toml` & `deadline_cloud_for_cinema_4d-0.3.2/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.1/pyproject.toml` & `deadline_cloud_for_cinema_4d-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_cinema_4d-0.3.1/PKG-INFO` & `deadline_cloud_for_cinema_4d-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline-cloud-for-cinema-4d
-Version: 0.3.1
+Version: 0.3.2
 Summary: AWS Deadline Cloud for Cinema 4D
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud-for-cinema-4d
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud-for-cinimema-4d
 Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
```

