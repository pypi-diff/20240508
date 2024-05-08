# Comparing `tmp/jupyter_collaboration_ui-1.0.0a1.tar.gz` & `tmp/jupyter_collaboration_ui-1.0.0a2.tar.gz`

## Comparing `jupyter_collaboration_ui-1.0.0a1.tar` & `jupyter_collaboration_ui-1.0.0a2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/install.json
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/setup.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/_version.py
--rw-r--r--   0        0        0     3750 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/package.json
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/schemas/@jupyter/collaboration-extension/package.json.orig
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/schemas/@jupyter/collaboration-extension/shared-link.json
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/schemas/@jupyter/collaboration-extension/user-menu-bar.json
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/341.2e8e5b6b71bf13a327e4.js
--rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/422.c33fd4bf2f8b13b1f430.js
--rw-r--r--   0        0        0    11313 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/44.0ba472088663f425d307.js
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/722.542e750613dbd427da59.js
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/784.1e2f345c812db2777387.js
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/842.5f0d12cba5fc800873b2.js
--rw-r--r--   0        0        0     8224 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/944.0167e5870ff1c1e28b32.js
--rw-r--r--   0        0        0     9385 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/952.e3c8e98af75bf2e2b0f2.js
--rw-r--r--   0        0        0     9326 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/remoteEntry.0faaa3f9527c21590e28.js
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/style.js
--rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/README.md
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/package.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/tsconfig.json
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/collaboratorspanel.tsx
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/components.tsx
--rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/cursors.ts
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/index.ts
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/menu.ts
--rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/sharedlink.ts
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/tokens.ts
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/userinfopanel.tsx
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/style/base.css
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/style/index.css
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/style/index.js
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/style/menu.css
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration/style/sidepanel.css
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/README.md
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/package.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/tsconfig.json
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/schema/shared-link.json
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/schema/user-menu-bar.json
--rw-r--r--   0        0        0     5807 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/src/collaboration.ts
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/src/index.ts
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/src/sharedlink.ts
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/style/index.css
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/style/index.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/babel.config.js
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/jest.config.js
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/package.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/tsconfig.json
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/tsconfig.test.json
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/awareness.ts
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/index.ts
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/requests.ts
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/tokens.ts
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/utils.ts
--rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/ydrive.ts
--rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/yprovider.ts
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/__tests__/yprovider.spec.ts
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/README.md
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/package.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/tsconfig.json
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/src/executor.ts
--rw-r--r--   0        0        0     9449 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/src/filebrowser.ts
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/src/index.ts
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/style/index.css
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/style/index.js
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/LICENSE
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/README.md
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/install.json
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/setup.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/_version.py
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/package.json
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/schemas/@jupyter/collaboration-extension/package.json.orig
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/schemas/@jupyter/collaboration-extension/shared-link.json
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/schemas/@jupyter/collaboration-extension/user-menu-bar.json
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/static/341.2c1235edd98d4fcf3370.js
+-rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/static/422.c33fd4bf2f8b13b1f430.js
+-rw-r--r--   0        0        0    11312 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/static/44.0dea17119570f524d364.js
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/static/722.0acbe11e1d6267433136.js
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/static/784.1e2f345c812db2777387.js
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/static/842.733246f866c208234c5d.js
+-rw-r--r--   0        0        0     8224 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/static/944.0167e5870ff1c1e28b32.js
+-rw-r--r--   0        0        0     9385 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/static/952.e3c8e98af75bf2e2b0f2.js
+-rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/static/remoteEntry.264cc5bbcf3df58d111b.js
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/static/style.js
+-rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration/README.md
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration/package.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration/tsconfig.json
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration/src/collaboratorspanel.tsx
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration/src/components.tsx
+-rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration/src/cursors.ts
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration/src/index.ts
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration/src/menu.ts
+-rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration/src/sharedlink.ts
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration/src/tokens.ts
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration/src/userinfopanel.tsx
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration/style/base.css
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration/style/index.css
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration/style/index.js
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration/style/menu.css
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration/style/sidepanel.css
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration-extension/README.md
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration-extension/package.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration-extension/tsconfig.json
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration-extension/schema/shared-link.json
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration-extension/schema/user-menu-bar.json
+-rw-r--r--   0        0        0     5807 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration-extension/src/collaboration.ts
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration-extension/src/index.ts
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration-extension/src/sharedlink.ts
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration-extension/style/index.css
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/collaboration-extension/style/index.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/docprovider/babel.config.js
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/docprovider/jest.config.js
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/docprovider/package.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/docprovider/tsconfig.json
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/docprovider/tsconfig.test.json
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/docprovider/src/awareness.ts
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/docprovider/src/index.ts
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/docprovider/src/requests.ts
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/docprovider/src/tokens.ts
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/docprovider/src/utils.ts
+-rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/docprovider/src/ydrive.ts
+-rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/docprovider/src/yprovider.ts
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/docprovider/src/__tests__/yprovider.spec.ts
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/docprovider-extension/README.md
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/docprovider-extension/package.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/docprovider-extension/tsconfig.json
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/docprovider-extension/src/executor.ts
+-rw-r--r--   0        0        0     9449 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/docprovider-extension/src/filebrowser.ts
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/docprovider-extension/src/index.ts
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/docprovider-extension/style/index.css
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/packages/docprovider-extension/style/index.js
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/LICENSE
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/README.md
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 jupyter_collaboration_ui-1.0.0a2/PKG-INFO
```

### Comparing `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/package.json` & `jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9700757575757577%*

 * *Differences: {"'dependencies'": "{'@jupyter/collaboration': '^3.0.0-alpha.2', '@jupyter/docprovider': "*

 * *                   "'^3.0.0-alpha.2', '@jupyter/ydoc': '^2.0.0', '@jupyterlab/application': "*

 * *                   "'^4.2.0', '@jupyterlab/apputils': '^4.2.0', '@jupyterlab/codemirror': "*

 * *                   "'^4.2.0', '@jupyterlab/statedb': '^4.2.0', '@jupyterlab/translation': "*

 * *                   "'^4.2.0', '@jupyterlab/ui-components': '^4.2.0'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.264cc5bbcf3df5 […]*

```diff
@@ -1,24 +1,24 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter-collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/collaboration": "^3.0.0-alpha.1",
-        "@jupyter/docprovider": "^3.0.0-alpha.1",
-        "@jupyter/ydoc": "^1.1.0-a0",
-        "@jupyterlab/application": "^4.2.0-beta.0",
-        "@jupyterlab/apputils": "^4.2.0-beta.0",
-        "@jupyterlab/codemirror": "^4.2.0-beta.0",
+        "@jupyter/collaboration": "^3.0.0-alpha.2",
+        "@jupyter/docprovider": "^3.0.0-alpha.2",
+        "@jupyter/ydoc": "^2.0.0",
+        "@jupyterlab/application": "^4.2.0",
+        "@jupyterlab/apputils": "^4.2.0",
+        "@jupyterlab/codemirror": "^4.2.0",
         "@jupyterlab/coreutils": "^6.0.5",
         "@jupyterlab/services": "^7.0.5",
-        "@jupyterlab/statedb": "^4.2.0-beta.0",
-        "@jupyterlab/translation": "^4.2.0-beta.0",
-        "@jupyterlab/ui-components": "^4.2.0-beta.0",
+        "@jupyterlab/statedb": "^4.2.0",
+        "@jupyterlab/translation": "^4.2.0",
+        "@jupyterlab/ui-components": "^4.2.0",
         "@lumino/widgets": "^2.1.0",
         "y-protocols": "^1.0.5",
         "y-websocket": "^1.3.15",
         "yjs": "^13.5.40"
     },
     "description": "JupyterLab - Real-Time Collaboration Extension",
     "devDependencies": {
@@ -39,15 +39,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyterlab/jupyter-collaboration",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.0faaa3f9527c21590e28.js",
+            "load": "static/remoteEntry.264cc5bbcf3df58d111b.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../projects/jupyter-collaboration-ui/jupyter_collaboration_ui/labextension",
         "schemaDir": "./schema",
         "sharedPackages": {
             "@codemirror/state": {
@@ -120,9 +120,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration-extension",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "3.0.0-alpha.1"
+    "version": "3.0.0-alpha.2"
 }
```

### Comparing `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/schemas/@jupyter/collaboration-extension/package.json.orig` & `jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/schemas/@jupyter/collaboration-extension/package.json.orig`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9704545454545456%*

 * *Differences: {"'dependencies'": "{'@jupyter/collaboration': '^3.0.0-alpha.2', '@jupyter/docprovider': "*

 * *                   "'^3.0.0-alpha.2', '@jupyter/ydoc': '^2.0.0', '@jupyterlab/application': "*

 * *                   "'^4.2.0', '@jupyterlab/apputils': '^4.2.0', '@jupyterlab/codemirror': "*

 * *                   "'^4.2.0', '@jupyterlab/statedb': '^4.2.0', '@jupyterlab/translation': "*

 * *                   "'^4.2.0', '@jupyterlab/ui-components': '^4.2.0'}",*

 * * "'version'": "'3.0.0-alpha.2'"}*

```diff
@@ -1,24 +1,24 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter-collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/collaboration": "^3.0.0-alpha.1",
-        "@jupyter/docprovider": "^3.0.0-alpha.1",
-        "@jupyter/ydoc": "^1.1.0-a0",
-        "@jupyterlab/application": "^4.2.0-beta.0",
-        "@jupyterlab/apputils": "^4.2.0-beta.0",
-        "@jupyterlab/codemirror": "^4.2.0-beta.0",
+        "@jupyter/collaboration": "^3.0.0-alpha.2",
+        "@jupyter/docprovider": "^3.0.0-alpha.2",
+        "@jupyter/ydoc": "^2.0.0",
+        "@jupyterlab/application": "^4.2.0",
+        "@jupyterlab/apputils": "^4.2.0",
+        "@jupyterlab/codemirror": "^4.2.0",
         "@jupyterlab/coreutils": "^6.0.5",
         "@jupyterlab/services": "^7.0.5",
-        "@jupyterlab/statedb": "^4.2.0-beta.0",
-        "@jupyterlab/translation": "^4.2.0-beta.0",
-        "@jupyterlab/ui-components": "^4.2.0-beta.0",
+        "@jupyterlab/statedb": "^4.2.0",
+        "@jupyterlab/translation": "^4.2.0",
+        "@jupyterlab/ui-components": "^4.2.0",
         "@lumino/widgets": "^2.1.0",
         "y-protocols": "^1.0.5",
         "y-websocket": "^1.3.15",
         "yjs": "^13.5.40"
     },
     "description": "JupyterLab - Real-Time Collaboration Extension",
     "devDependencies": {
@@ -115,9 +115,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration-extension",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "3.0.0-alpha.1"
+    "version": "3.0.0-alpha.2"
 }
```

### Comparing `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/341.2e8e5b6b71bf13a327e4.js` & `jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/static/722.0acbe11e1d6267433136.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 "use strict";
 (self.webpackChunk_jupyter_collaboration_extension = self.webpackChunk_jupyter_collaboration_extension || []).push([
-    [341, 722], {
+    [722, 341], {
         9341: (e, s, t) => {
             t.r(s), t.d(s, {
                 ICollaborativeDrive: () => v,
                 WebSocketAwarenessProvider: () => c,
                 WebSocketProvider: () => p,
                 YDrive: () => u
             });
@@ -42,17 +42,17 @@
                         t = i.xv();
                     i.zd(t, o.CHAT), i.Qj(t, JSON.stringify(s)), this.ws.send(i.Fo(t))
                 }
                 _onUserChanged(e) {
                     this._awareness.setLocalStateField("user", e.identity)
                 }
             }
-            var h = t(7655),
-                d = t(8824),
-                l = t(8440),
+            var h = t(8702),
+                d = t(7861),
+                l = t(5923),
                 _ = t(7262);
             class p {
                 constructor(e) {
                     this._onConnectionClosed = e => {
                         1003 === e.code && (console.error("Document provider closed:", e.reason), (0, l.showErrorMessage)(this._trans.__("Document session error"), e.reason, [l.Dialog.okButton()]), this._sharedModel.dispose())
                     }, this._onSync = e => {
                         var s;
```

### Comparing `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/422.c33fd4bf2f8b13b1f430.js` & `jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/static/422.c33fd4bf2f8b13b1f430.js`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/44.0ba472088663f425d307.js` & `jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/static/44.0dea17119570f524d364.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -15,16 +15,16 @@
                 showSharedLinkDialog: () => L
             });
             var r = n(7262);
             const s = new r.Token("@jupyter/collaboration:IUserMenu"),
                 o = new r.Token("@jupyter/collaboration:IGlobalAwareness");
             var a = n(3345),
                 i = n(5256),
-                l = n(8440),
-                c = n(7655);
+                l = n(5923),
+                c = n(8702);
             const d = "jp-Collaborator";
             class u extends i.Panel {
                 constructor(e, t, n) {
                     super({}), this._onAwarenessChanged = () => {
                         const e = this._awareness.getStates(),
                             t = [];
                         e.forEach(((e, n) => {
@@ -249,15 +249,15 @@
                         parent: document.body
                     })]
                 });
 
             function x(e) {
                 return [f.of(e), C]
             }
-            var j = n(2126),
+            var j = n(1527),
                 A = n(4873);
             class I extends i.MenuBar.Renderer {
                 constructor(e) {
                     super(), this._user = e
                 }
                 renderItem(e) {
                     const t = this.createItemClass(e),
@@ -293,15 +293,15 @@
                 }
             }
             class P extends i.Menu {
                 constructor(e) {
                     super(e)
                 }
             }
-            var E = n(2844);
+            var E = n(265);
             async function L({
                 translator: e
             }) {
                 const t = (null != e ? e : E.nullTranslator).load("collaboration"),
                     n = c.PageConfig.getToken(),
                     r = new URL(c.URLExt.normalize(c.PageConfig.getUrl({
                         workspace: c.PageConfig.defaultWorkspace
```

### Comparing `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/722.542e750613dbd427da59.js` & `jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/static/341.2c1235edd98d4fcf3370.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 "use strict";
 (self.webpackChunk_jupyter_collaboration_extension = self.webpackChunk_jupyter_collaboration_extension || []).push([
-    [722, 341], {
+    [341, 722], {
         9341: (e, s, t) => {
             t.r(s), t.d(s, {
                 ICollaborativeDrive: () => v,
                 WebSocketAwarenessProvider: () => c,
                 WebSocketProvider: () => p,
                 YDrive: () => u
             });
@@ -42,17 +42,17 @@
                         t = i.xv();
                     i.zd(t, o.CHAT), i.Qj(t, JSON.stringify(s)), this.ws.send(i.Fo(t))
                 }
                 _onUserChanged(e) {
                     this._awareness.setLocalStateField("user", e.identity)
                 }
             }
-            var h = t(7655),
-                d = t(8824),
-                l = t(8440),
+            var h = t(8702),
+                d = t(7861),
+                l = t(5923),
                 _ = t(7262);
             class p {
                 constructor(e) {
                     this._onConnectionClosed = e => {
                         1003 === e.code && (console.error("Document provider closed:", e.reason), (0, l.showErrorMessage)(this._trans.__("Document session error"), e.reason, [l.Dialog.okButton()]), this._sharedModel.dispose())
                     }, this._onSync = e => {
                         var s;
```

### Comparing `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/784.1e2f345c812db2777387.js` & `jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/static/784.1e2f345c812db2777387.js`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/842.5f0d12cba5fc800873b2.js` & `jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/static/842.733246f866c208234c5d.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,24 +1,24 @@
 "use strict";
 (self.webpackChunk_jupyter_collaboration_extension = self.webpackChunk_jupyter_collaboration_extension || []).push([
     [842], {
         4842: (e, r, a) => {
             a.r(r), a.d(r, {
                 default: () => x
             });
-            var t = a(8440),
-                o = a(7623),
-                n = a(9835),
-                s = a(2126),
-                i = a(7655),
-                l = a(8824),
-                c = a(2824),
-                d = a(2844),
+            var t = a(5923),
+                o = a(2350),
+                n = a(3438),
+                s = a(1527),
+                i = a(8702),
+                l = a(7861),
+                c = a(8101),
+                d = a(265),
                 u = a(5256),
-                p = a(7435),
+                p = a(7202),
                 m = a(2206),
                 b = a(7784);
             const y = {
                     id: "@jupyter/collaboration-extension:userMenu",
                     description: "Provide connected user menu.",
                     requires: [],
                     provides: p.IUserMenu,
```

### Comparing `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/944.0167e5870ff1c1e28b32.js` & `jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/static/944.0167e5870ff1c1e28b32.js`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/952.e3c8e98af75bf2e2b0f2.js` & `jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/static/952.e3c8e98af75bf2e2b0f2.js`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/remoteEntry.0faaa3f9527c21590e28.js` & `jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/static/remoteEntry.264cc5bbcf3df58d111b.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, o, n, i, l, u, d, f, c, s, p, h, b, v, m, y, g, j, w = {
+    var e, r, t, a, o, n, i, l, f, u, d, s, c, p, h, b, v, m, y, g, j, w = {
             1998: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(422), t.e(784), t.e(206), t.e(394), t.e(242), t.e(824), t.e(842)]).then((() => () => t(4842))),
-                        "./extension": () => Promise.all([t.e(422), t.e(784), t.e(206), t.e(394), t.e(242), t.e(824), t.e(842)]).then((() => () => t(4842))),
+                        "./index": () => Promise.all([t.e(422), t.e(784), t.e(206), t.e(956), t.e(454), t.e(861), t.e(842)]).then((() => () => t(4842))),
+                        "./extension": () => Promise.all([t.e(422), t.e(784), t.e(206), t.e(956), t.e(454), t.e(861), t.e(842)]).then((() => () => t(4842))),
                         "./style": () => t.e(944).then((() => () => t(5944)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     n = (e, r) => {
                         if (t.S) {
@@ -43,73 +43,73 @@
         }), r
     }, S.d = (e, r) => {
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
-        44: "0ba472088663f425d307",
-        206: "7108eced39c49eb27106",
-        242: "f38d53af901815a08cb5",
-        262: "d6f92031996231d96ae8",
-        341: "2e8e5b6b71bf13a327e4",
-        349: "e89d95e45f94f06ccdb1",
-        394: "c889587484bcd2ab8dd1",
+        44: "0dea17119570f524d364",
+        206: "4f6141430fe8a637acf8",
+        262: "c416027c81179d6df17b",
+        341: "2c1235edd98d4fcf3370",
+        349: "b9ee23822f0ee74805cd",
         422: "c33fd4bf2f8b13b1f430",
-        722: "542e750613dbd427da59",
+        454: "fec1d8839904b6275579",
+        722: "0acbe11e1d6267433136",
         784: "1e2f345c812db2777387",
-        824: "7eeac4763f58845a00cd",
-        842: "5f0d12cba5fc800873b2",
+        842: "733246f866c208234c5d",
+        861: "6251d06572b376d5c061",
         944: "0167e5870ff1c1e28b32",
-        952: "e3c8e98af75bf2e2b0f2"
+        952: "e3c8e98af75bf2e2b0f2",
+        956: "2542140616ac1e4f58bd"
     } [e] + ".js?v=" + {
-        44: "0ba472088663f425d307",
-        206: "7108eced39c49eb27106",
-        242: "f38d53af901815a08cb5",
-        262: "d6f92031996231d96ae8",
-        341: "2e8e5b6b71bf13a327e4",
-        349: "e89d95e45f94f06ccdb1",
-        394: "c889587484bcd2ab8dd1",
+        44: "0dea17119570f524d364",
+        206: "4f6141430fe8a637acf8",
+        262: "c416027c81179d6df17b",
+        341: "2c1235edd98d4fcf3370",
+        349: "b9ee23822f0ee74805cd",
         422: "c33fd4bf2f8b13b1f430",
-        722: "542e750613dbd427da59",
+        454: "fec1d8839904b6275579",
+        722: "0acbe11e1d6267433136",
         784: "1e2f345c812db2777387",
-        824: "7eeac4763f58845a00cd",
-        842: "5f0d12cba5fc800873b2",
+        842: "733246f866c208234c5d",
+        861: "6251d06572b376d5c061",
         944: "0167e5870ff1c1e28b32",
-        952: "e3c8e98af75bf2e2b0f2"
+        952: "e3c8e98af75bf2e2b0f2",
+        956: "2542140616ac1e4f58bd"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyter/collaboration-extension:", S.l = (t, a, o, n) => {
         if (e[t]) e[t].push(a);
         else {
             var i, l;
             if (void 0 !== o)
-                for (var u = document.getElementsByTagName("script"), d = 0; d < u.length; d++) {
-                    var f = u[d];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
-                        i = f;
+                for (var f = document.getElementsByTagName("script"), u = 0; u < f.length; u++) {
+                    var d = f[u];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
+                        i = d;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, S.nc && i.setAttribute("nonce", S.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [a];
-            var c = (r, a) => {
-                    i.onerror = i.onload = null, clearTimeout(s);
+            var s = (r, a) => {
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(a))), r) return r(a)
                 },
-                s = setTimeout(c.bind(null, void 0, {
+                c = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = c.bind(null, i.onerror), i.onload = c.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, S.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -130,16 +130,16 @@
                             l = o[r];
                         (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
-                    u = [];
-                return "default" === t && (l("@jupyter/collaboration-extension", "3.0.0-alpha.1", (() => Promise.all([S.e(422), S.e(784), S.e(206), S.e(394), S.e(242), S.e(824), S.e(842)]).then((() => () => S(4842))))), l("@jupyter/collaboration", "3.0.0-alpha.1", (() => Promise.all([S.e(206), S.e(262), S.e(394), S.e(44), S.e(242)]).then((() => () => S(2044))))), l("@jupyter/docprovider", "3.0.0-alpha.1", (() => Promise.all([S.e(422), S.e(262), S.e(394), S.e(349), S.e(824), S.e(341)]).then((() => () => S(9341))))), l("y-websocket", "1.5.4", (() => Promise.all([S.e(422), S.e(784), S.e(952), S.e(206)]).then((() => () => S(2952)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                    f = [];
+                return "default" === t && (l("@jupyter/collaboration-extension", "3.0.0-alpha.2", (() => Promise.all([S.e(422), S.e(784), S.e(206), S.e(956), S.e(454), S.e(861), S.e(842)]).then((() => () => S(4842))))), l("@jupyter/collaboration", "3.0.0-alpha.2", (() => Promise.all([S.e(206), S.e(262), S.e(956), S.e(44), S.e(454)]).then((() => () => S(2044))))), l("@jupyter/docprovider", "3.0.0-alpha.2", (() => Promise.all([S.e(422), S.e(262), S.e(956), S.e(349), S.e(861), S.e(341)]).then((() => () => S(9341))))), l("y-websocket", "1.5.4", (() => Promise.all([S.e(422), S.e(784), S.e(952), S.e(206)]).then((() => () => S(2952)))))), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -175,105 +175,105 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var a = 1, n = 1; n < e.length; n++) a--, t += "u" == (typeof(l = e[n]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, l);
             return t
         }
         var i = [];
         for (n = 1; n < e.length; n++) {
             var l = e[n];
-            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : o(l))
+            i.push(0 === l ? "not(" + f() + ")" : 1 === l ? "(" + f() + " || " + f() + ")" : 2 === l ? i.pop() + " " + i.pop() : o(l))
         }
-        return u();
+        return f();
 
-        function u() {
+        function f() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, n = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 o = a < 0;
             o && (a = -a - 1);
-            for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var d, f, c = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(d = r[i]))[0])) return !u || ("u" == c ? l > a && !o : "" == c != o);
-                if ("u" == f) {
-                    if (!u || "u" != c) return !1
-                } else if (u)
-                    if (c == f)
+            for (var i = 0, l = 1, f = !0;; l++, i++) {
+                var u, d, s = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(u = r[i]))[0])) return !f || ("u" == s ? l > a && !o : "" == s != o);
+                if ("u" == d) {
+                    if (!f || "u" != s) return !1
+                } else if (f)
+                    if (s == d)
                         if (l <= a) {
-                            if (d != e[l]) return !1
+                            if (u != e[l]) return !1
                         } else {
-                            if (o ? d > e[l] : d < e[l]) return !1;
-                            d != e[l] && (u = !1)
+                            if (o ? u > e[l] : u < e[l]) return !1;
+                            u != e[l] && (f = !1)
                         }
-                else if ("s" != c && "n" != c) {
+                else if ("s" != s && "n" != s) {
                     if (o || l <= a) return !1;
-                    u = !1, l--
+                    f = !1, l--
                 } else {
-                    if (l <= a || f < c != o) return !1;
-                    u = !1
-                } else "s" != c && "n" != c && (u = !1, l--)
+                    if (l <= a || d < s != o) return !1;
+                    f = !1
+                } else "s" != s && "n" != s && (f = !1, l--)
             }
         }
-        var s = [],
-            p = s.pop.bind(s);
+        var c = [],
+            p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? n(h, r) : !p())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? n(h, r) : !p())
         }
         return !!p()
     }, i = (e, r) => {
         var t = S.S[e];
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
-    }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(a) + ")", d = (e, r, t, a) => {
+    }, f = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(a) + ")", u = (e, r, t, a) => {
         var o = l(e, t);
-        return n(a, o) || c(u(e, t, o, a)), s(e[t][o])
-    }, f = (e, r, t) => {
+        return n(a, o) || s(f(e, t, o, a)), c(e[t][o])
+    }, d = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !n(t, r) || e && !a(e, r) ? e : r), 0)) && o[r]
-    }, c = e => {
+    }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, s = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, a, o) {
+    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, a, o) {
         var n = S.I(r);
         return n && n.then ? n.then(e.bind(e, r, S.S[r], t, a, o)) : e(r, S.S[r], t, a, o)
-    })(((e, r, t, a) => (i(e, t), d(r, 0, t, a)))), b = p(((e, r, t, a, o) => r && S.o(r, t) ? d(r, 0, t, a) : o())), v = p(((e, r, t, a, o) => {
-        var n = r && S.o(r, t) && f(r, t, a);
-        return n ? s(n) : o()
+    })(((e, r, t, a) => (i(e, t), u(r, 0, t, a)))), b = p(((e, r, t, a, o) => r && S.o(r, t) ? u(r, 0, t, a) : o())), v = p(((e, r, t, a, o) => {
+        var n = r && S.o(r, t) && d(r, t, a);
+        return n ? c(n) : o()
     })), m = {}, y = {
         2206: () => h("default", "yjs", [1, 13, 5, 40]),
-        7655: () => h("default", "@jupyterlab/coreutils", [1, 6, 1, 8]),
-        8440: () => h("default", "@jupyterlab/apputils", [1, 4, 2, 8]),
-        2126: () => h("default", "@jupyterlab/ui-components", [1, 4, 1, 8]),
-        2844: () => h("default", "@jupyterlab/translation", [1, 4, 1, 8]),
+        5923: () => h("default", "@jupyterlab/apputils", [1, 4, 3, 0]),
+        8702: () => h("default", "@jupyterlab/coreutils", [1, 6, 2, 0]),
+        265: () => h("default", "@jupyterlab/translation", [1, 4, 2, 0]),
+        1527: () => h("default", "@jupyterlab/ui-components", [1, 4, 2, 0]),
         5256: () => h("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
-        8824: () => h("default", "@jupyterlab/services", [1, 7, 1, 8]),
-        2824: () => h("default", "@jupyterlab/statedb", [1, 4, 1, 8]),
-        7435: () => b("default", "@jupyter/collaboration", [1, 3, 0, 0, , "alpha", 1], (() => Promise.all([S.e(262), S.e(44)]).then((() => () => S(2044))))),
-        7623: () => h("default", "@jupyterlab/codemirror", [1, 4, 1, 8]),
-        9835: () => b("default", "@jupyter/docprovider", [1, 3, 0, 0, , "alpha", 1], (() => Promise.all([S.e(262), S.e(349), S.e(722)]).then((() => () => S(9341))))),
+        7861: () => h("default", "@jupyterlab/services", [1, 7, 2, 0]),
+        2350: () => h("default", "@jupyterlab/codemirror", [1, 4, 2, 0]),
+        3438: () => b("default", "@jupyter/docprovider", [1, 3, 0, 0, , "alpha", 2], (() => Promise.all([S.e(262), S.e(349), S.e(722)]).then((() => () => S(9341))))),
+        7202: () => b("default", "@jupyter/collaboration", [1, 3, 0, 0, , "alpha", 2], (() => Promise.all([S.e(262), S.e(44)]).then((() => () => S(2044))))),
+        8101: () => h("default", "@jupyterlab/statedb", [1, 4, 2, 0]),
         7262: () => h("default", "@lumino/coreutils", [1, 2, 0, 0]),
         195: () => h("default", "@codemirror/state", [1, 6, 2, 0]),
         3345: () => h("default", "react", [1, 18, 2, 0]),
         4873: () => h("default", "@lumino/virtualdom", [1, 2, 0, 0]),
         5024: () => h("default", "@codemirror/view", [1, 6, 9, 6]),
         3560: () => v("default", "y-websocket", [1, 1, 3, 15], (() => Promise.all([S.e(784), S.e(952), S.e(206)]).then((() => () => S(2952))))),
         4602: () => h("default", "@lumino/signaling", [1, 2, 0, 0])
     }, g = {
         44: [195, 3345, 4873, 5024],
         206: [2206],
-        242: [2126, 2844, 5256],
         262: [7262],
         349: [3560, 4602],
-        394: [7655, 8440],
-        824: [8824],
-        842: [2824, 7435, 7623, 9835]
+        454: [265, 1527, 5256],
+        842: [2350, 3438, 7202, 8101],
+        861: [7861],
+        956: [5923, 8702]
     }, j = {}, S.f.consumes = (e, r) => {
         S.o(g, e) && g[e].forEach((e => {
             if (S.o(m, e)) return r.push(m[e]);
             if (!j[e]) {
                 var t = r => {
                     m[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
@@ -297,15 +297,15 @@
         var e = {
             270: 0
         };
         S.f.j = (r, t) => {
             var a = S.o(e, r) ? e[r] : void 0;
             if (0 !== a)
                 if (a) t.push(a[2]);
-                else if (/^(2(06|42|62)|349|394|824)$/.test(r)) e[r] = 0;
+                else if (/^(206|262|349|454|861|956)$/.test(r)) e[r] = 0;
             else {
                 var o = new Promise(((t, o) => a = e[r] = [t, o]));
                 t.push(a[2] = o);
                 var n = S.p + S.u(r),
                     i = new Error;
                 S.l(n, (t => {
                     if (S.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
@@ -314,20 +314,20 @@
                         i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + n + ")", i.name = "ChunkLoadError", i.type = o, i.request = n, a[1](i)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
                 var a, o, [n, i, l] = t,
-                    u = 0;
+                    f = 0;
                 if (n.some((r => 0 !== e[r]))) {
                     for (a in i) S.o(i, a) && (S.m[a] = i[a]);
                     l && l(S)
                 }
-                for (r && r(t); u < n.length; u++) o = n[u], S.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); f < n.length; f++) o = n[f], S.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunk_jupyter_collaboration_extension = self.webpackChunk_jupyter_collaboration_extension || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), S.nc = void 0;
     var x = S(1998);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyter/collaboration-extension"] = x
 })();
```

### Comparing `jupyter_collaboration_ui-1.0.0a1/jupyter_collaboration_ui/labextension/static/third-party-licenses.json` & `jupyter_collaboration_ui-1.0.0a2/jupyter_collaboration_ui/labextension/static/third-party-licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '3.0.0-alpha.2'}, 1: {'versionInfo': '3.0.0-alpha.2'}}"}*

```diff
@@ -1,20 +1,20 @@
 {
     "packages": [
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter/collaboration",
-            "versionInfo": "3.0.0-alpha.1"
+            "versionInfo": "3.0.0-alpha.2"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter/docprovider",
-            "versionInfo": "3.0.0-alpha.1"
+            "versionInfo": "3.0.0-alpha.2"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
             "versionInfo": "6.11.0"
         },
```

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/collaboration/package.json` & `jupyter_collaboration_ui-1.0.0a2/packages/collaboration/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9740384615384615%*

 * *Differences: {"'dependencies'": "{'@jupyter/docprovider': '^3.0.0-alpha.2'}", "'version'": "'3.0.0-alpha.2'"}*

```diff
@@ -2,15 +2,15 @@
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter-collaboration/issues"
     },
     "dependencies": {
         "@codemirror/state": "^6.2.0",
         "@codemirror/view": "^6.7.0",
-        "@jupyter/docprovider": "^3.0.0-alpha.1",
+        "@jupyter/docprovider": "^3.0.0-alpha.2",
         "@jupyterlab/apputils": "^4.0.5",
         "@jupyterlab/coreutils": "^6.0.5",
         "@jupyterlab/services": "^7.0.5",
         "@jupyterlab/ui-components": "^4.0.5",
         "@lumino/coreutils": "^2.1.0",
         "@lumino/virtualdom": "^2.0.0",
         "@lumino/widgets": "^2.1.0",
@@ -63,9 +63,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "3.0.0-alpha.1"
+    "version": "3.0.0-alpha.2"
 }
```

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/collaboratorspanel.tsx` & `jupyter_collaboration_ui-1.0.0a2/packages/collaboration/src/collaboratorspanel.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/components.tsx` & `jupyter_collaboration_ui-1.0.0a2/packages/collaboration/src/components.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/cursors.ts` & `jupyter_collaboration_ui-1.0.0a2/packages/collaboration/src/cursors.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/menu.ts` & `jupyter_collaboration_ui-1.0.0a2/packages/collaboration/src/menu.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/sharedlink.ts` & `jupyter_collaboration_ui-1.0.0a2/packages/collaboration/src/sharedlink.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/tokens.ts` & `jupyter_collaboration_ui-1.0.0a2/packages/collaboration/src/tokens.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/collaboration/src/userinfopanel.tsx` & `jupyter_collaboration_ui-1.0.0a2/packages/collaboration/src/userinfopanel.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/collaboration/style/menu.css` & `jupyter_collaboration_ui-1.0.0a2/packages/collaboration/style/menu.css`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/collaboration/style/sidepanel.css` & `jupyter_collaboration_ui-1.0.0a2/packages/collaboration/style/sidepanel.css`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/package.json` & `jupyter_collaboration_ui-1.0.0a2/packages/collaboration-extension/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9704545454545456%*

 * *Differences: {"'dependencies'": "{'@jupyter/collaboration': '^3.0.0-alpha.2', '@jupyter/docprovider': "*

 * *                   "'^3.0.0-alpha.2', '@jupyter/ydoc': '^2.0.0', '@jupyterlab/application': "*

 * *                   "'^4.2.0', '@jupyterlab/apputils': '^4.2.0', '@jupyterlab/codemirror': "*

 * *                   "'^4.2.0', '@jupyterlab/statedb': '^4.2.0', '@jupyterlab/translation': "*

 * *                   "'^4.2.0', '@jupyterlab/ui-components': '^4.2.0'}",*

 * * "'version'": "'3.0.0-alpha.2'"}*

```diff
@@ -1,24 +1,24 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter-collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/collaboration": "^3.0.0-alpha.1",
-        "@jupyter/docprovider": "^3.0.0-alpha.1",
-        "@jupyter/ydoc": "^1.1.0-a0",
-        "@jupyterlab/application": "^4.2.0-beta.0",
-        "@jupyterlab/apputils": "^4.2.0-beta.0",
-        "@jupyterlab/codemirror": "^4.2.0-beta.0",
+        "@jupyter/collaboration": "^3.0.0-alpha.2",
+        "@jupyter/docprovider": "^3.0.0-alpha.2",
+        "@jupyter/ydoc": "^2.0.0",
+        "@jupyterlab/application": "^4.2.0",
+        "@jupyterlab/apputils": "^4.2.0",
+        "@jupyterlab/codemirror": "^4.2.0",
         "@jupyterlab/coreutils": "^6.0.5",
         "@jupyterlab/services": "^7.0.5",
-        "@jupyterlab/statedb": "^4.2.0-beta.0",
-        "@jupyterlab/translation": "^4.2.0-beta.0",
-        "@jupyterlab/ui-components": "^4.2.0-beta.0",
+        "@jupyterlab/statedb": "^4.2.0",
+        "@jupyterlab/translation": "^4.2.0",
+        "@jupyterlab/ui-components": "^4.2.0",
         "@lumino/widgets": "^2.1.0",
         "y-protocols": "^1.0.5",
         "y-websocket": "^1.3.15",
         "yjs": "^13.5.40"
     },
     "description": "JupyterLab - Real-Time Collaboration Extension",
     "devDependencies": {
@@ -115,9 +115,9 @@
     "typedoc": {
         "displayName": "@jupyter/collaboration-extension",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "3.0.0-alpha.1"
+    "version": "3.0.0-alpha.2"
 }
```

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/src/collaboration.ts` & `jupyter_collaboration_ui-1.0.0a2/packages/collaboration-extension/src/collaboration.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/src/index.ts` & `jupyter_collaboration_ui-1.0.0a2/packages/collaboration-extension/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/collaboration-extension/src/sharedlink.ts` & `jupyter_collaboration_ui-1.0.0a2/packages/collaboration-extension/src/sharedlink.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/docprovider/jest.config.js` & `jupyter_collaboration_ui-1.0.0a2/packages/docprovider/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/docprovider/package.json` & `jupyter_collaboration_ui-1.0.0a2/packages/docprovider/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.970679012345679%*

 * *Differences: {"'dependencies'": "{'@jupyter/ydoc': '^2.0.0'}", "'version'": "'3.0.0-alpha.2'"}*

```diff
@@ -1,14 +1,14 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter-collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/ydoc": "^1.1.0-a0",
+        "@jupyter/ydoc": "^2.0.0",
         "@jupyterlab/coreutils": "^6.0.5",
         "@jupyterlab/services": "^7.0.5",
         "@lumino/coreutils": "^2.1.0",
         "@lumino/disposable": "^2.1.0",
         "@lumino/signaling": "^2.1.0",
         "y-protocols": "^1.0.5",
         "y-websocket": "^1.3.15",
@@ -61,9 +61,9 @@
     ],
     "typedoc": {
         "displayName": "@jupyter/docprovider",
         "entryPoint": "./src/index.ts",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "3.0.0-alpha.1"
+    "version": "3.0.0-alpha.2"
 }
```

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/awareness.ts` & `jupyter_collaboration_ui-1.0.0a2/packages/docprovider/src/awareness.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/requests.ts` & `jupyter_collaboration_ui-1.0.0a2/packages/docprovider/src/requests.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/tokens.ts` & `jupyter_collaboration_ui-1.0.0a2/packages/docprovider/src/tokens.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/ydrive.ts` & `jupyter_collaboration_ui-1.0.0a2/packages/docprovider/src/ydrive.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/docprovider/src/yprovider.ts` & `jupyter_collaboration_ui-1.0.0a2/packages/docprovider/src/yprovider.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/package.json` & `jupyter_collaboration_ui-1.0.0a2/packages/docprovider-extension/package.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9689393939393939%*

 * *Differences: {"'dependencies'": "{'@jupyter/docprovider': '^3.0.0-alpha.2', '@jupyter/ydoc': '^2.0.0', "*

 * *                   "'@jupyterlab/application': '^4.2.0', '@jupyterlab/apputils': '^4.2.0', "*

 * *                   "'@jupyterlab/docregistry': '^4.2.0', '@jupyterlab/filebrowser': '^4.2.0', "*

 * *                   "'@jupyterlab/fileeditor': '^4.2.0', '@jupyterlab/logconsole': '^4.2.0', "*

 * *                   "'@jupyterlab/notebook': '^4.2.0', '@jupyterlab/settingregistry': '^4.2.0', "*

 * *                   "'@jupyterlab/transla […]*

```diff
@@ -1,24 +1,24 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter-collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/docprovider": "^3.0.0-alpha.1",
-        "@jupyter/ydoc": "^1.1.0-a0",
-        "@jupyterlab/application": "^4.2.0-beta.0",
-        "@jupyterlab/apputils": "^4.2.0-beta.0",
-        "@jupyterlab/docregistry": "^4.2.0-beta.0",
-        "@jupyterlab/filebrowser": "^4.2.0-beta.0",
-        "@jupyterlab/fileeditor": "^4.2.0-beta.0",
-        "@jupyterlab/logconsole": "^4.2.0-beta.0",
-        "@jupyterlab/notebook": "^4.2.0-beta.0",
-        "@jupyterlab/settingregistry": "^4.2.0-beta.0",
-        "@jupyterlab/translation": "^4.2.0-beta.0",
+        "@jupyter/docprovider": "^3.0.0-alpha.2",
+        "@jupyter/ydoc": "^2.0.0",
+        "@jupyterlab/application": "^4.2.0",
+        "@jupyterlab/apputils": "^4.2.0",
+        "@jupyterlab/docregistry": "^4.2.0",
+        "@jupyterlab/filebrowser": "^4.2.0",
+        "@jupyterlab/fileeditor": "^4.2.0",
+        "@jupyterlab/logconsole": "^4.2.0",
+        "@jupyterlab/notebook": "^4.2.0",
+        "@jupyterlab/settingregistry": "^4.2.0",
+        "@jupyterlab/translation": "^4.2.0",
         "@lumino/commands": "^2.1.0",
         "y-protocols": "^1.0.5",
         "y-websocket": "^1.3.15",
         "yjs": "^13.5.40"
     },
     "description": "JupyterLab - Collaborative Shared Models",
     "devDependencies": {
@@ -114,9 +114,9 @@
     "typedoc": {
         "displayName": "@jupyter/docprovider-extension",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "3.0.0-alpha.1"
+    "version": "3.0.0-alpha.2"
 }
```

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/src/executor.ts` & `jupyter_collaboration_ui-1.0.0a2/packages/docprovider-extension/src/executor.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/src/filebrowser.ts` & `jupyter_collaboration_ui-1.0.0a2/packages/docprovider-extension/src/filebrowser.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/packages/docprovider-extension/src/index.ts` & `jupyter_collaboration_ui-1.0.0a2/packages/docprovider-extension/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/.gitignore` & `jupyter_collaboration_ui-1.0.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/LICENSE` & `jupyter_collaboration_ui-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/pyproject.toml` & `jupyter_collaboration_ui-1.0.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_collaboration_ui-1.0.0a1/PKG-INFO` & `jupyter_collaboration_ui-1.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyter-collaboration-ui
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: JupyterLab/Jupyter Notebook 7+ extension providing user interface integration for real time collaboration
 Project-URL: Documentation, https://jupyterlab-realtime-collaboration.readthedocs.io/
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-collaboration
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: # Licensing terms
         
         This project is licensed under the terms of the Modified BSD License
```

