# Comparing `tmp/configuration_maker-0.1.4-py2.py3-none-any.whl.zip` & `tmp/configuration_maker-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2783 bytes, number of entries: 6
--rw-r--r--  2.0 unx       54 b- defN 22-Oct-14 17:23 configuration_maker/__init__.py
--rw-r--r--  2.0 unx     3645 b- defN 22-Oct-14 17:23 configuration_maker/main.py
--rw-r--r--  2.0 unx      339 b- defN 22-Oct-14 17:23 configuration_maker-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Oct-14 17:23 configuration_maker-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 22-Oct-14 17:23 configuration_maker-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      516 b- defN 22-Oct-14 17:23 configuration_maker-0.1.4.dist-info/RECORD
-6 files, 4684 bytes uncompressed, 1837 bytes compressed:  60.8%
+Zip file size: 2800 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       54 b- defN 24-May-08 17:14 configuration_maker/__init__.py
+-rw-r--r--  2.0 unx     3696 b- defN 24-May-08 17:15 configuration_maker/main.py
+-rw-r--r--  2.0 unx      339 b- defN 24-May-08 17:17 configuration_maker-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-08 17:17 configuration_maker-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 24-May-08 17:17 configuration_maker-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      515 b- defN 24-May-08 17:17 configuration_maker-0.1.5.dist-info/RECORD
+6 files, 4716 bytes uncompressed, 1854 bytes compressed:  60.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: configuration_maker/__init__.py
 Comment: 
 
 Filename: configuration_maker/main.py
 Comment: 
 
-Filename: configuration_maker-0.1.4.dist-info/METADATA
+Filename: configuration_maker-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: configuration_maker-0.1.4.dist-info/WHEEL
+Filename: configuration_maker-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: configuration_maker-0.1.4.dist-info/top_level.txt
+Filename: configuration_maker-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: configuration_maker-0.1.4.dist-info/RECORD
+Filename: configuration_maker-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## configuration_maker/main.py

```diff
@@ -29,33 +29,33 @@
         self.path = Path(path).resolve()
         self.path.parent.mkdir(parents=True, exist_ok=True)
         self.keys = config_keys
         self.cli_command = cli_command
         if autoload_env:
             load_dotenv()
             
-    def load(self):
+    def load(self, skip_env=False):
         config = {}
         if self.path.exists():
             try:
                 config = load_json(self.path)
             except json.decoder.JSONDecodeError:
                 self.path.unlink()
         for key in self.keys:
-            value = os.environ.get(key.name, None)
+            value = None if skip_env else os.environ.get(key.name, None)
             if value is None:
                 value = config.get(key.name, None)
             if value is not None:
                 value = key.convert(value)
             config[key.name] = value
 
         return config
     
     def update(self, group=None, reset=False):
-        config = self.load()
+        config = self.load(skip_env=True)
         
         print('\n\n(leave blank to keep existing value)')
         for key in self.keys:
             if key.group == group or group is None:
                 current_value = None
                 if not reset:
                     current_value = config.get(key.name, None)
```

