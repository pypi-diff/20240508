# Comparing `tmp/playsound3-2.1.6.tar.gz` & `tmp/playsound3-2.2.0.tar.gz`

## Comparing `playsound3-2.1.6.tar` & `playsound3-2.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 playsound3-2.1.6/.github/workflows/check-code-quality.yaml
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 playsound3-2.1.6/.github/workflows/check-with-pytest-linux.yaml
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 playsound3-2.1.6/.github/workflows/check-with-pytest-macos.yaml
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 playsound3-2.1.6/.github/workflows/check-with-pytest-windows.yaml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 playsound3-2.1.6/.idea/.gitignore
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 playsound3-2.1.6/.idea/misc.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 playsound3-2.1.6/.idea/modules.xml
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 playsound3-2.1.6/.idea/playsound3.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 playsound3-2.1.6/.idea/vcs.xml
--rw-r--r--   0        0        0    23894 2020-02-02 00:00:00.000000 playsound3-2.1.6/.idea/workspace.xml
--rw-r--r--   0        0        0     9348 2020-02-02 00:00:00.000000 playsound3-2.1.6/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 playsound3-2.1.6/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 playsound3-2.1.6/playsound3/__init__.py
--rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 playsound3-2.1.6/playsound3/playsound3.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 playsound3-2.1.6/tests/test_playsound.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 playsound3-2.1.6/.gitignore
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 playsound3-2.1.6/LICENSE
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 playsound3-2.1.6/README.md
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 playsound3-2.1.6/pyproject.toml
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 playsound3-2.1.6/PKG-INFO
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 playsound3-2.2.0/.github/workflows/check-code-quality.yaml
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 playsound3-2.2.0/.github/workflows/check-with-pytest-linux.yaml
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 playsound3-2.2.0/.github/workflows/check-with-pytest-macos.yaml
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 playsound3-2.2.0/.github/workflows/check-with-pytest-windows.yaml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 playsound3-2.2.0/.idea/.gitignore
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 playsound3-2.2.0/.idea/misc.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 playsound3-2.2.0/.idea/modules.xml
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 playsound3-2.2.0/.idea/playsound3.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 playsound3-2.2.0/.idea/vcs.xml
+-rw-r--r--   0        0        0    23777 2020-02-02 00:00:00.000000 playsound3-2.2.0/.idea/workspace.xml
+-rw-r--r--   0        0        0     9348 2020-02-02 00:00:00.000000 playsound3-2.2.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 playsound3-2.2.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 playsound3-2.2.0/playsound3/__init__.py
+-rw-r--r--   0        0        0     9242 2020-02-02 00:00:00.000000 playsound3-2.2.0/playsound3/playsound3.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 playsound3-2.2.0/tests/test_playsound.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 playsound3-2.2.0/.gitignore
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 playsound3-2.2.0/LICENSE
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 playsound3-2.2.0/README.md
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 playsound3-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 playsound3-2.2.0/PKG-INFO
```

### Comparing `playsound3-2.1.6/.github/workflows/check-code-quality.yaml` & `playsound3-2.2.0/.github/workflows/check-code-quality.yaml`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.6/.github/workflows/check-with-pytest-linux.yaml` & `playsound3-2.2.0/.github/workflows/check-with-pytest-linux.yaml`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.6/.github/workflows/check-with-pytest-macos.yaml` & `playsound3-2.2.0/.github/workflows/check-with-pytest-macos.yaml`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.6/.github/workflows/check-with-pytest-windows.yaml` & `playsound3-2.2.0/.github/workflows/check-with-pytest-windows.yaml`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.6/.idea/workspace.xml` & `playsound3-2.2.0/.idea/workspace.xml`

 * *Files 4% similar despite different names*

#### Comparing `playsound3-2.1.6/.idea/workspace.xml` & `playsound3-2.2.0/.idea/workspace.xml`

```diff
@@ -1,15 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="4fbee7df-bfbf-4326-aa56-dc3a718f551b" name="Changes" comment="Update comments in a test">
-      <change beforePath="$PROJECT_DIR$/playsound3/playsound3.py" beforeDir="false" afterPath="$PROJECT_DIR$/playsound3/playsound3.py" afterDir="false"/>
+    <list default="true" id="4fbee7df-bfbf-4326-aa56-dc3a718f551b" name="Changes" comment="Add backend selection">
+      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
@@ -20,28 +20,28 @@
 }</component>
   <component name="ProjectId" id="2g5sXLf8F18eSiUiNloeaQqPaCM"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
     <option name="sortKey" value="BY_TIME_DESCENDING"/>
   </component>
-  <component name="PropertiesComponent">{
-  &quot;keyToString&quot;: {
-    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
-    &quot;git-widget-placeholder&quot;: &quot;main&quot;,
-    &quot;last_opened_file_path&quot;: &quot;/home/gaha/workspace/python/playsound3/.github/workflows&quot;,
-    &quot;node.js.detected.package.eslint&quot;: &quot;true&quot;,
-    &quot;node.js.detected.package.tslint&quot;: &quot;true&quot;,
-    &quot;node.js.selected.package.eslint&quot;: &quot;(autodetect)&quot;,
-    &quot;node.js.selected.package.tslint&quot;: &quot;(autodetect)&quot;,
-    &quot;nodejs_package_manager_path&quot;: &quot;npm&quot;,
-    &quot;settings.editor.selected.configurable&quot;: &quot;preferences.sourceCode&quot;,
-    &quot;vue.rearranger.settings.migration&quot;: &quot;true&quot;
+  <component name="PropertiesComponent"><![CDATA[{
+  "keyToString": {
+    "RunOnceActivity.ShowReadmeOnStart": "true",
+    "git-widget-placeholder": "develop",
+    "last_opened_file_path": "/home/gaha/workspace/python/playsound3/.github/workflows",
+    "node.js.detected.package.eslint": "true",
+    "node.js.detected.package.tslint": "true",
+    "node.js.selected.package.eslint": "(autodetect)",
+    "node.js.selected.package.tslint": "(autodetect)",
+    "nodejs_package_manager_path": "npm",
+    "settings.editor.selected.configurable": "preferences.sourceCode",
+    "vue.rearranger.settings.migration": "true"
   }
-}</component>
+}]]></component>
   <component name="PyConsoleOptionsProvider">
     <option name="myPythonConsoleState">
       <console-settings custom-start-script="%load_ext autoreload
 %autoreload 2
 
 import sys; print('Python %s on %s' % (sys.version, sys.platform))
 sys.path.extend([WORKING_DIR_AND_PYTHON_PATHS])
@@ -90,167 +90,17 @@
       <workItem from="1715028902191" duration="292000"/>
       <workItem from="1715029948125" duration="587000"/>
       <workItem from="1715030546044" duration="41000"/>
       <workItem from="1715030697321" duration="9000"/>
       <workItem from="1715035744281" duration="106000"/>
       <workItem from="1715035857578" duration="3880000"/>
       <workItem from="1715073679361" duration="15313000"/>
-      <workItem from="1715089410611" duration="1567000"/>
-    </task>
-    <task id="LOCAL-00038" summary="Install gstreamer for test">
-      <option name="closed" value="true"/>
-      <created>1715081784901</created>
-      <option name="number" value="00038"/>
-      <option name="presentableId" value="LOCAL-00038"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1715081784901</updated>
-    </task>
-    <task id="LOCAL-00039" summary="Add separate tests for Windows and Mac OS">
-      <option name="closed" value="true"/>
-      <created>1715082103842</created>
-      <option name="number" value="00039"/>
-      <option name="presentableId" value="LOCAL-00039"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1715082103842</updated>
-    </task>
-    <task id="LOCAL-00040" summary="Remove 3.7 runner from Mac OS">
-      <option name="closed" value="true"/>
-      <created>1715082277170</created>
-      <option name="number" value="00040"/>
-      <option name="presentableId" value="LOCAL-00040"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1715082277170</updated>
-    </task>
-    <task id="LOCAL-00041" summary="Update workflows">
-      <option name="closed" value="true"/>
-      <created>1715083003371</created>
-      <option name="number" value="00041"/>
-      <option name="presentableId" value="LOCAL-00041"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1715083003371</updated>
-    </task>
-    <task id="LOCAL-00042" summary="Update workflows">
-      <option name="closed" value="true"/>
-      <created>1715083188627</created>
-      <option name="number" value="00042"/>
-      <option name="presentableId" value="LOCAL-00042"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1715083188627</updated>
-    </task>
-    <task id="LOCAL-00043" summary="Update workflows">
-      <option name="closed" value="true"/>
-      <created>1715083251898</created>
-      <option name="number" value="00043"/>
-      <option name="presentableId" value="LOCAL-00043"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1715083251898</updated>
-    </task>
-    <task id="LOCAL-00044" summary="Update workflows">
-      <option name="closed" value="true"/>
-      <created>1715083304184</created>
-      <option name="number" value="00044"/>
-      <option name="presentableId" value="LOCAL-00044"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1715083304184</updated>
-    </task>
-    <task id="LOCAL-00045" summary="Update workflows">
-      <option name="closed" value="true"/>
-      <created>1715083337529</created>
-      <option name="number" value="00045"/>
-      <option name="presentableId" value="LOCAL-00045"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1715083337529</updated>
-    </task>
-    <task id="LOCAL-00046" summary="Update workflows">
-      <option name="closed" value="true"/>
-      <created>1715083408493</created>
-      <option name="number" value="00046"/>
-      <option name="presentableId" value="LOCAL-00046"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1715083408493</updated>
-    </task>
-    <task id="LOCAL-00047" summary="Update workflows - force install">
-      <option name="closed" value="true"/>
-      <created>1715083498513</created>
-      <option name="number" value="00047"/>
-      <option name="presentableId" value="LOCAL-00047"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1715083498513</updated>
-    </task>
-    <task id="LOCAL-00048" summary="Update workflows - force install">
-      <option name="closed" value="true"/>
-      <created>1715083564971</created>
-      <option name="number" value="00048"/>
-      <option name="presentableId" value="LOCAL-00048"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1715083564971</updated>
-    </task>
-    <task id="LOCAL-00049" summary="Revert to setup-gstreamer action">
-      <option name="closed" value="true"/>
-      <created>1715083667376</created>
-      <option name="number" value="00049"/>
-      <option name="presentableId" value="LOCAL-00049"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1715083667376</updated>
-    </task>
-    <task id="LOCAL-00050" summary="Revert to setup-gstreamer action">
-      <option name="closed" value="true"/>
-      <created>1715083883233</created>
-      <option name="number" value="00050"/>
-      <option name="presentableId" value="LOCAL-00050"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1715083883233</updated>
-    </task>
-    <task id="LOCAL-00051" summary="Revert to setup-gstreamer action">
-      <option name="closed" value="true"/>
-      <created>1715083949015</created>
-      <option name="number" value="00051"/>
-      <option name="presentableId" value="LOCAL-00051"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1715083949015</updated>
-    </task>
-    <task id="LOCAL-00052" summary="Revert to setup-gstreamer action">
-      <option name="closed" value="true"/>
-      <created>1715084012716</created>
-      <option name="number" value="00052"/>
-      <option name="presentableId" value="LOCAL-00052"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1715084012716</updated>
-    </task>
-    <task id="LOCAL-00053" summary="Revert to setup-gstreamer action">
-      <option name="closed" value="true"/>
-      <created>1715084136253</created>
-      <option name="number" value="00053"/>
-      <option name="presentableId" value="LOCAL-00053"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1715084136253</updated>
-    </task>
-    <task id="LOCAL-00054" summary="Revert to setup-gstreamer action">
-      <option name="closed" value="true"/>
-      <created>1715084367717</created>
-      <option name="number" value="00054"/>
-      <option name="presentableId" value="LOCAL-00054"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1715084367717</updated>
-    </task>
-    <task id="LOCAL-00055" summary="Github actions - add dummy output device for linux">
-      <option name="closed" value="true"/>
-      <created>1715084519162</created>
-      <option name="number" value="00055"/>
-      <option name="presentableId" value="LOCAL-00055"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1715084519162</updated>
-    </task>
-    <task id="LOCAL-00056" summary="Github actions - add timeout and verbosity">
-      <option name="closed" value="true"/>
-      <created>1715084686654</created>
-      <option name="number" value="00056"/>
-      <option name="presentableId" value="LOCAL-00056"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1715084686654</updated>
+      <workItem from="1715089410611" duration="1698000"/>
+      <workItem from="1715092844590" duration="65000"/>
+      <workItem from="1715104032924" duration="5932000"/>
     </task>
     <task id="LOCAL-00057" summary="Github actions - add local sound files">
       <option name="closed" value="true"/>
       <created>1715084997443</created>
       <option name="number" value="00057"/>
       <option name="presentableId" value="LOCAL-00057"/>
       <option name="project" value="LOCAL"/>
@@ -484,15 +334,167 @@
       <option name="closed" value="true"/>
       <created>1715090571937</created>
       <option name="number" value="00086"/>
       <option name="presentableId" value="LOCAL-00086"/>
       <option name="project" value="LOCAL"/>
       <updated>1715090571937</updated>
     </task>
-    <option name="localTasksCounter" value="87"/>
+    <task id="LOCAL-00087" summary="Allow setting up LOGLEVEL from env variable">
+      <option name="closed" value="true"/>
+      <created>1715091065398</created>
+      <option name="number" value="00087"/>
+      <option name="presentableId" value="LOCAL-00087"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715091065398</updated>
+    </task>
+    <task id="LOCAL-00088" summary="Bump version for release">
+      <option name="closed" value="true"/>
+      <created>1715091100461</created>
+      <option name="number" value="00088"/>
+      <option name="presentableId" value="LOCAL-00088"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715091100461</updated>
+    </task>
+    <task id="LOCAL-00089" summary="Add backend selection">
+      <option name="closed" value="true"/>
+      <created>1715106087024</created>
+      <option name="number" value="00089"/>
+      <option name="presentableId" value="LOCAL-00089"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715106087024</updated>
+    </task>
+    <task id="LOCAL-00090" summary="Add backend selection">
+      <option name="closed" value="true"/>
+      <created>1715107430827</created>
+      <option name="number" value="00090"/>
+      <option name="presentableId" value="LOCAL-00090"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715107430827</updated>
+    </task>
+    <task id="LOCAL-00091" summary="Update linux tests with new backends">
+      <option name="closed" value="true"/>
+      <created>1715107442275</created>
+      <option name="number" value="00091"/>
+      <option name="presentableId" value="LOCAL-00091"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715107442275</updated>
+    </task>
+    <task id="LOCAL-00092" summary="Remove timeout from Mac OS and Windows tests">
+      <option name="closed" value="true"/>
+      <created>1715107681229</created>
+      <option name="number" value="00092"/>
+      <option name="presentableId" value="LOCAL-00092"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715107681229</updated>
+    </task>
+    <task id="LOCAL-00093" summary="Extend linux test names">
+      <option name="closed" value="true"/>
+      <created>1715107714227</created>
+      <option name="number" value="00093"/>
+      <option name="presentableId" value="LOCAL-00093"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715107714227</updated>
+    </task>
+    <task id="LOCAL-00094" summary="Add ffmpeg installation to the test">
+      <option name="closed" value="true"/>
+      <created>1715107899040</created>
+      <option name="number" value="00094"/>
+      <option name="presentableId" value="LOCAL-00094"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715107899040</updated>
+    </task>
+    <task id="LOCAL-00095" summary="Add alsa installation to the test">
+      <option name="closed" value="true"/>
+      <created>1715108002876</created>
+      <option name="number" value="00095"/>
+      <option name="presentableId" value="LOCAL-00095"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715108002876</updated>
+    </task>
+    <task id="LOCAL-00096" summary="Add pulseaudio installation to all Linux tests">
+      <option name="closed" value="true"/>
+      <created>1715108165898</created>
+      <option name="number" value="00096"/>
+      <option name="presentableId" value="LOCAL-00096"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715108165898</updated>
+    </task>
+    <task id="LOCAL-00097" summary="Add file suffix when saving file from web">
+      <option name="closed" value="true"/>
+      <created>1715108478826</created>
+      <option name="number" value="00097"/>
+      <option name="presentableId" value="LOCAL-00097"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715108478826</updated>
+    </task>
+    <task id="LOCAL-00098" summary="Add file suffix when saving file from web">
+      <option name="closed" value="true"/>
+      <created>1715108491497</created>
+      <option name="number" value="00098"/>
+      <option name="presentableId" value="LOCAL-00098"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715108491497</updated>
+    </task>
+    <task id="LOCAL-00099" summary="Rollback to single Linux test">
+      <option name="closed" value="true"/>
+      <created>1715108963867</created>
+      <option name="number" value="00099"/>
+      <option name="presentableId" value="LOCAL-00099"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715108963867</updated>
+    </task>
+    <task id="LOCAL-00100" summary="Rollback to single Linux test">
+      <option name="closed" value="true"/>
+      <created>1715108968066</created>
+      <option name="number" value="00100"/>
+      <option name="presentableId" value="LOCAL-00100"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715108968066</updated>
+    </task>
+    <task id="LOCAL-00101" summary="Rollback to single Linux test">
+      <option name="closed" value="true"/>
+      <created>1715108971617</created>
+      <option name="number" value="00101"/>
+      <option name="presentableId" value="LOCAL-00101"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715108971617</updated>
+    </task>
+    <task id="LOCAL-00102" summary="Fix typo">
+      <option name="closed" value="true"/>
+      <created>1715108980422</created>
+      <option name="number" value="00102"/>
+      <option name="presentableId" value="LOCAL-00102"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715108980422</updated>
+    </task>
+    <task id="LOCAL-00103" summary="Documentation updates">
+      <option name="closed" value="true"/>
+      <created>1715109388477</created>
+      <option name="number" value="00103"/>
+      <option name="presentableId" value="LOCAL-00103"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715109388477</updated>
+    </task>
+    <task id="LOCAL-00104" summary="Better error handling">
+      <option name="closed" value="true"/>
+      <created>1715109718199</created>
+      <option name="number" value="00104"/>
+      <option name="presentableId" value="LOCAL-00104"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715109718199</updated>
+    </task>
+    <task id="LOCAL-00105" summary="Add backend selection">
+      <option name="closed" value="true"/>
+      <created>1715109890231</created>
+      <option name="number" value="00105"/>
+      <option name="presentableId" value="LOCAL-00105"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1715109890231</updated>
+    </task>
+    <option name="localTasksCounter" value="106"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
@@ -502,35 +504,35 @@
             <State/>
           </value>
         </entry>
       </map>
     </option>
   </component>
   <component name="VcsManagerConfiguration">
-    <MESSAGE value="Updating legacy download function"/>
-    <MESSAGE value="Fix missing certificates for download"/>
-    <MESSAGE value="Install and use certifi by default"/>
-    <MESSAGE value="Add tests and github workflows"/>
-    <MESSAGE value="Isort and Black formatting"/>
-    <MESSAGE value="Install gstreamer for test"/>
-    <MESSAGE value="Add separate tests for Windows and Mac OS"/>
-    <MESSAGE value="Remove 3.7 runner from Mac OS"/>
-    <MESSAGE value="Update workflows"/>
-    <MESSAGE value="Update workflows - force install"/>
-    <MESSAGE value="Revert to setup-gstreamer action"/>
-    <MESSAGE value="Github actions - add dummy output device for linux"/>
-    <MESSAGE value="Github actions - add timeout and verbosity"/>
     <MESSAGE value="Github actions - add local sound files"/>
     <MESSAGE value="Github actions - other fixes"/>
     <MESSAGE value="Skip windows test"/>
     <MESSAGE value="Update README"/>
     <MESSAGE value="Use URLs in blocking test"/>
     <MESSAGE value="Remove audio samples"/>
     <MESSAGE value="Modify Linux backend"/>
     <MESSAGE value="Remove unsued dependency"/>
     <MESSAGE value="Change backend naming"/>
     <MESSAGE value="Remove unnecessary note"/>
-    <MESSAGE value="Bump version for release"/>
     <MESSAGE value="Update comments in a test"/>
-    <option name="LAST_COMMIT_MESSAGE" value="Update comments in a test"/>
+    <MESSAGE value="Allow setting up LOGLEVEL from env variable"/>
+    <MESSAGE value="Bump version for release"/>
+    <MESSAGE value="Update linux tests with new backends"/>
+    <MESSAGE value="Remove timeout from Mac OS and Windows tests"/>
+    <MESSAGE value="Extend linux test names"/>
+    <MESSAGE value="Add ffmpeg installation to the test"/>
+    <MESSAGE value="Add alsa installation to the test"/>
+    <MESSAGE value="Add pulseaudio installation to all Linux tests"/>
+    <MESSAGE value="Add file suffix when saving file from web"/>
+    <MESSAGE value="Rollback to single Linux test"/>
+    <MESSAGE value="Fix typo"/>
+    <MESSAGE value="Documentation updates"/>
+    <MESSAGE value="Better error handling"/>
+    <MESSAGE value="Add backend selection"/>
+    <option name="LAST_COMMIT_MESSAGE" value="Add backend selection"/>
   </component>
 </project>
```

### Comparing `playsound3-2.1.6/.idea/inspectionProfiles/Project_Default.xml` & `playsound3-2.2.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.6/tests/test_playsound.py` & `playsound3-2.2.0/tests/test_playsound.py`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.6/.gitignore` & `playsound3-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.6/LICENSE` & `playsound3-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `playsound3-2.1.6/README.md` & `playsound3-2.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -24,31 +24,38 @@
 
 # or use directly on URLs
 playsound("http://url/to/sound/file.mp3")
 ```
 
 ## Documentation
 
-The playsound module contains only one thing - the function (also named) playsound:
+The `playsound3` module contains a single function named `playsound`:
 
 ```python
-def playsound(sound, block: bool = True) -> None:
+def playsound(sound, block=True, backend=None) -> None:
     """Play a sound file using an audio backend availabile in your system.
 
     Args:
         sound: Path or URL to the sound file. Can be a string or pathlib.Path.
         block: If True, the function will block execution until the sound finishes playing.
                If False, sound will play in a background thread.
+        backend: Name of the audio backend to use. Use None for automatic selection.
     """
     ...
 ```
 
-It requires one argument - the path to the file with the sound you'd like to play.
+It requires one argument: `sound` - the path to the file with the sound you'd like to play.
 This should be a local file or a URL.
-There's an optional second argument, block, which is set to True by default.
-Setting it to False makes the function run asynchronously.
+There's an optional second argument: `block` which is set to `True` by default.
+Setting it to `False` makes the function run asynchronously.
+You can manually specify a backend by passing its name as the third argument.
+You can browse available backends by using `playsound3.AVAILABLE_BACKENDS`.
+It is recommended to use the default value of `None` to let the library choose the best backend available.
 
 ## Supported systems
 
-* Linux, using GStreamer (built-in on Linux distributions)
-* Windows, using winmm.dll (built-in on Windows)
-* OS X, using afplay utility (built-in on OS X)
+* **Linux** using one of the below backends, whichever is available:
+    * GStreamer
+    * FFmpeg
+    * aplay for .wav and mpg123 .mp3
+* **Windows** using winmm.dll (built-in on Windows)
+* **OS X** using afplay utility (built-in on OS X)
```

### Comparing `playsound3-2.1.6/pyproject.toml` & `playsound3-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "playsound3"
-version = "2.1.6"
+version = "2.2.0"
 requires-python = ">=3.7"
 authors = [
     { name = "Szymon Mikler", email = "sjmikler@gmail.com" },
     { name = "Taylor Marks", email = "taylor@marksfam.com" },
 ]
 maintainers = [
     { name = "Szymon Mikler", email = "sjmikler@gmail.com" },
```

### Comparing `playsound3-2.1.6/PKG-INFO` & `playsound3-2.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: playsound3
-Version: 2.1.6
+Version: 2.2.0
 Summary: Cross-platform library to play audio files
 Project-URL: Repository, https://github.com/sjmikler/playsound3
 Project-URL: Issues, https://github.com/sjmikler/playsound3/issues
 Project-URL: Documentation, https://github.com/sjmikler/playsound3?tab=readme-ov-file#documentation
 Author-email: Szymon Mikler <sjmikler@gmail.com>, Taylor Marks <taylor@marksfam.com>
 Maintainer-email: Szymon Mikler <sjmikler@gmail.com>
 License: MIT License
@@ -54,31 +54,38 @@
 
 # or use directly on URLs
 playsound("http://url/to/sound/file.mp3")
 ```
 
 ## Documentation
 
-The playsound module contains only one thing - the function (also named) playsound:
+The `playsound3` module contains a single function named `playsound`:
 
 ```python
-def playsound(sound, block: bool = True) -> None:
+def playsound(sound, block=True, backend=None) -> None:
     """Play a sound file using an audio backend availabile in your system.
 
     Args:
         sound: Path or URL to the sound file. Can be a string or pathlib.Path.
         block: If True, the function will block execution until the sound finishes playing.
                If False, sound will play in a background thread.
+        backend: Name of the audio backend to use. Use None for automatic selection.
     """
     ...
 ```
 
-It requires one argument - the path to the file with the sound you'd like to play.
+It requires one argument: `sound` - the path to the file with the sound you'd like to play.
 This should be a local file or a URL.
-There's an optional second argument, block, which is set to True by default.
-Setting it to False makes the function run asynchronously.
+There's an optional second argument: `block` which is set to `True` by default.
+Setting it to `False` makes the function run asynchronously.
+You can manually specify a backend by passing its name as the third argument.
+You can browse available backends by using `playsound3.AVAILABLE_BACKENDS`.
+It is recommended to use the default value of `None` to let the library choose the best backend available.
 
 ## Supported systems
 
-* Linux, using GStreamer (built-in on Linux distributions)
-* Windows, using winmm.dll (built-in on Windows)
-* OS X, using afplay utility (built-in on OS X)
+* **Linux** using one of the below backends, whichever is available:
+    * GStreamer
+    * FFmpeg
+    * aplay for .wav and mpg123 .mp3
+* **Windows** using winmm.dll (built-in on Windows)
+* **OS X** using afplay utility (built-in on OS X)
```

