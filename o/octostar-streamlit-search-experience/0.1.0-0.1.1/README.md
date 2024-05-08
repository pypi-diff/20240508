# Comparing `tmp/octostar_streamlit_search_experience-0.1.0.tar.gz` & `tmp/octostar_streamlit_search_experience-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octostar_streamlit_search_experience-0.1.0.tar", max compression
+gzip compressed data, was "octostar_streamlit_search_experience-0.1.1.tar", max compression
```

## Comparing `octostar_streamlit_search_experience-0.1.0.tar` & `octostar_streamlit_search_experience-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      769 2024-05-06 21:21:27.822014 octostar_streamlit_search_experience-0.1.0/README.md
--rw-r--r--   0        0        0     1964 2024-05-08 17:42:01.973106 octostar_streamlit_search_experience-0.1.0/octostar_streamlit_search_experience/__init__.py
--rw-r--r--   0        0        0      436 2024-05-06 19:56:14.704927 octostar_streamlit_search_experience-0.1.0/octostar_streamlit_search_experience/frontend/.eslintrc.cjs
--rw-r--r--   0        0        0      253 2024-05-06 19:56:14.705546 octostar_streamlit_search_experience-0.1.0/octostar_streamlit_search_experience/frontend/.gitignore
--rw-r--r--   0        0        0     1300 2024-05-06 19:56:14.705182 octostar_streamlit_search_experience-0.1.0/octostar_streamlit_search_experience/frontend/README.md
--rw-r--r--   0        0        0      366 2024-05-06 19:56:14.705921 octostar_streamlit_search_experience-0.1.0/octostar_streamlit_search_experience/frontend/index.html
--rw-r--r--   0        0        0   131645 2024-05-06 19:59:47.585426 octostar_streamlit_search_experience-0.1.0/octostar_streamlit_search_experience/frontend/package-lock.json
--rw-r--r--   0        0        0      824 2024-05-06 19:59:47.541094 octostar_streamlit_search_experience-0.1.0/octostar_streamlit_search_experience/frontend/package.json
--rw-r--r--   0        0        0       33 2024-05-06 20:49:37.529891 octostar_streamlit_search_experience-0.1.0/octostar_streamlit_search_experience/frontend/src/App.css
--rw-r--r--   0        0        0      860 2024-05-06 20:53:21.988684 octostar_streamlit_search_experience-0.1.0/octostar_streamlit_search_experience/frontend/src/App.tsx
--rw-r--r--   0        0        0      215 2024-05-06 20:48:31.521496 octostar_streamlit_search_experience-0.1.0/octostar_streamlit_search_experience/frontend/src/main.tsx
--rw-r--r--   0        0        0       38 2024-05-06 19:56:14.708711 octostar_streamlit_search_experience-0.1.0/octostar_streamlit_search_experience/frontend/src/vite-env.d.ts
--rw-r--r--   0        0        0      605 2024-05-06 19:56:14.709077 octostar_streamlit_search_experience-0.1.0/octostar_streamlit_search_experience/frontend/tsconfig.json
--rw-r--r--   0        0        0      233 2024-05-06 19:56:14.709733 octostar_streamlit_search_experience-0.1.0/octostar_streamlit_search_experience/frontend/tsconfig.node.json
--rw-r--r--   0        0        0      178 2024-05-08 17:55:47.277413 octostar_streamlit_search_experience-0.1.0/octostar_streamlit_search_experience/frontend/vite.config.ts
--rw-r--r--   0        0        0      389 2024-05-06 19:50:40.901011 octostar_streamlit_search_experience-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1481 1970-01-01 00:00:00.000000 octostar_streamlit_search_experience-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      769 2024-05-06 21:21:27.822014 octostar_streamlit_search_experience-0.1.1/README.md
+-rw-r--r--   0        0        0     2351 2024-05-08 19:05:10.951970 octostar_streamlit_search_experience-0.1.1/octostar_streamlit_search_experience/__init__.py
+-rw-r--r--   0        0        0      436 2024-05-06 19:56:14.704927 octostar_streamlit_search_experience-0.1.1/octostar_streamlit_search_experience/frontend/.eslintrc.cjs
+-rw-r--r--   0        0        0      253 2024-05-06 19:56:14.705546 octostar_streamlit_search_experience-0.1.1/octostar_streamlit_search_experience/frontend/.gitignore
+-rw-r--r--   0        0        0     1300 2024-05-06 19:56:14.705182 octostar_streamlit_search_experience-0.1.1/octostar_streamlit_search_experience/frontend/README.md
+-rw-r--r--   0        0        0      366 2024-05-06 19:56:14.705921 octostar_streamlit_search_experience-0.1.1/octostar_streamlit_search_experience/frontend/index.html
+-rw-r--r--   0        0        0   131645 2024-05-06 19:59:47.585426 octostar_streamlit_search_experience-0.1.1/octostar_streamlit_search_experience/frontend/package-lock.json
+-rw-r--r--   0        0        0      824 2024-05-06 19:59:47.541094 octostar_streamlit_search_experience-0.1.1/octostar_streamlit_search_experience/frontend/package.json
+-rw-r--r--   0        0        0       33 2024-05-06 20:49:37.529891 octostar_streamlit_search_experience-0.1.1/octostar_streamlit_search_experience/frontend/src/App.css
+-rw-r--r--   0        0        0      926 2024-05-08 19:10:07.541449 octostar_streamlit_search_experience-0.1.1/octostar_streamlit_search_experience/frontend/src/App.tsx
+-rw-r--r--   0        0        0      215 2024-05-06 20:48:31.521496 octostar_streamlit_search_experience-0.1.1/octostar_streamlit_search_experience/frontend/src/main.tsx
+-rw-r--r--   0        0        0       38 2024-05-06 19:56:14.708711 octostar_streamlit_search_experience-0.1.1/octostar_streamlit_search_experience/frontend/src/vite-env.d.ts
+-rw-r--r--   0        0        0      605 2024-05-06 19:56:14.709077 octostar_streamlit_search_experience-0.1.1/octostar_streamlit_search_experience/frontend/tsconfig.json
+-rw-r--r--   0        0        0      233 2024-05-06 19:56:14.709733 octostar_streamlit_search_experience-0.1.1/octostar_streamlit_search_experience/frontend/tsconfig.node.json
+-rw-r--r--   0        0        0      178 2024-05-08 17:55:47.277413 octostar_streamlit_search_experience-0.1.1/octostar_streamlit_search_experience/frontend/vite.config.ts
+-rw-r--r--   0        0        0      409 2024-05-08 19:11:29.534690 octostar_streamlit_search_experience-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1522 1970-01-01 00:00:00.000000 octostar_streamlit_search_experience-0.1.1/PKG-INFO
```

### Comparing `octostar_streamlit_search_experience-0.1.0/README.md` & `octostar_streamlit_search_experience-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `octostar_streamlit_search_experience-0.1.0/octostar_streamlit_search_experience/__init__.py` & `octostar_streamlit_search_experience-0.1.1/octostar_streamlit_search_experience/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import os
+from typing import Dict, List, Union
+import uuid
 import streamlit.components.v1 as components
+from pydantic import BaseModel
 
 
 # Create a _RELEASE constant. We'll set this to False while we're developing
 # the component, and True when we're ready to package and distribute it.
 # (This is, of course, optional - there are innumerable ways to manage your
 # release process.)
 _RELEASE = os.environ.get("OCTOSTAR_STREAMLIT_RELEASE", "true").lower() == "true"
@@ -35,7 +38,20 @@
 else:
     # When we're distributing a production version of the component, we'll
     # replace the `url` param with `path`, and point it to the component's
     # build directory:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/dist")
     _component_func = components.declare_component(component_name, path=build_dir)
+
+
+class SearchExperienceButtonParams(BaseModel):
+    button_text: Union[str, None] = None
+
+
+def search_experience_button(
+    params: SearchExperienceButtonParams, key=None
+) -> List[Dict]:
+    if key is None:
+        key = str(uuid.uuid4())
+
+    return _component_func(params=params.model_dump(), key=key)
```

### Comparing `octostar_streamlit_search_experience-0.1.0/octostar_streamlit_search_experience/frontend/README.md` & `octostar_streamlit_search_experience-0.1.1/octostar_streamlit_search_experience/frontend/README.md`

 * *Files identical despite different names*

### Comparing `octostar_streamlit_search_experience-0.1.0/octostar_streamlit_search_experience/frontend/package-lock.json` & `octostar_streamlit_search_experience-0.1.1/octostar_streamlit_search_experience/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `octostar_streamlit_search_experience-0.1.0/octostar_streamlit_search_experience/frontend/package.json` & `octostar_streamlit_search_experience-0.1.1/octostar_streamlit_search_experience/frontend/package.json`

 * *Files identical despite different names*

### Comparing `octostar_streamlit_search_experience-0.1.0/octostar_streamlit_search_experience/frontend/src/App.tsx` & `octostar_streamlit_search_experience-0.1.1/octostar_streamlit_search_experience/frontend/src/App.tsx`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 import { desktopApi } from "@octostar/platform-api"
 import { useEffect } from 'react'
 import { ComponentProps, Streamlit, withStreamlitConnection } from "streamlit-component-lib"
 import './App.css'
 
 type ArgsType = {
-  buttonText?: string;
-}
+  params?: {
+    button_text?: string;
+  };
+};
 
 function App(props: ComponentProps) {
-  const {buttonText = 'Search'}: ArgsType = props.args;
-  
+  const args: ArgsType = props.args;
+  const { button_text = "Search" } = args.params || {};
+
   useEffect(() => {
-    Streamlit.setFrameHeight()
-  }, [])
+    Streamlit.setFrameHeight();
+  }, []);
 
   const handleSearchClick = async () => {
-    const result = await desktopApi().searchXperience()
+    const result = await desktopApi().searchXperience();
 
-    console.log('search result', result)
+    console.log("search result", result);
 
-    Streamlit.setComponentValue(result)
-    Streamlit.setFrameHeight()
-  }
+    Streamlit.setComponentValue(result);
+    Streamlit.setFrameHeight();
+  };
 
   return (
     <button onClick={handleSearchClick} className="search-btn">
-      {buttonText}
+      {button_text}
     </button>
-  )
+  );
 }
 
 const ConnectedApp = withStreamlitConnection(App)
 
 ConnectedApp.displayName = 'SearchExperience';
 
 export default ConnectedApp
```

### Comparing `octostar_streamlit_search_experience-0.1.0/octostar_streamlit_search_experience/frontend/tsconfig.json` & `octostar_streamlit_search_experience-0.1.1/octostar_streamlit_search_experience/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `octostar_streamlit_search_experience-0.1.0/PKG-INFO` & `octostar_streamlit_search_experience-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: octostar-streamlit-search-experience
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: streamlit (>=1.34.0,<2.0.0)
 Requires-Dist: streamlit-octostar-research (>=0.1.22,<0.2.0)
 Description-Content-Type: text/markdown
 
 # Octostar search experience streamlit component
 
 Motivation to create a separate project for the component is to address problems with complex bidirectional components in Streamlit. The problem with the current search experience implementation is that Streamlit resets the state of the application each time a component returns a value what makes usage of conditions with UI components difficult.
```

