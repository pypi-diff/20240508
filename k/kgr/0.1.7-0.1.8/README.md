# Comparing `tmp/kgr-0.1.7.tar.gz` & `tmp/kgr-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgr-0.1.7.tar", last modified: Sat Apr 13 20:47:50 2024, max compression
+gzip compressed data, was "kgr-0.1.8.tar", last modified: Tue May  7 22:07:09 2024, max compression
```

## Comparing `kgr-0.1.7.tar` & `kgr-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2024-04-13 20:46:37.220586 kgr-0.1.7/LICENSE
--rw-r--r--   0        0        0       73 2024-04-13 20:46:37.220754 kgr-0.1.7/README.md
--rw-r--r--   0        0        0      880 2024-04-13 20:47:50.329691 kgr-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 20:46:37.221089 kgr-0.1.7/src/__init__.py
--rw-r--r--   0        0        0       30 2024-04-13 20:46:37.221251 kgr-0.1.7/src/__main__.py
--rw-r--r--   0        0        0     8952 2024-04-13 20:46:37.221541 kgr-0.1.7/src/lib.py
--rw-r--r--   0        0        0     2046 1970-01-01 00:00:00.000000 kgr-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-13 20:46:37.220586 kgr-0.1.8/LICENSE
+-rw-r--r--   0        0        0       73 2024-04-13 20:46:37.220754 kgr-0.1.8/README.md
+-rw-r--r--   0        0        0      880 2024-05-07 22:07:09.558441 kgr-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-13 20:46:37.221089 kgr-0.1.8/src/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-13 20:46:37.221251 kgr-0.1.8/src/__main__.py
+-rw-r--r--   0        0        0     9024 2024-05-07 22:02:45.239020 kgr-0.1.8/src/lib.py
+-rw-r--r--   0        0        0     2046 1970-01-01 00:00:00.000000 kgr-0.1.8/PKG-INFO
```

### Comparing `kgr-0.1.7/LICENSE` & `kgr-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kgr-0.1.7/pyproject.toml` & `kgr-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "kgr"
-version = "0.1.7"
+version = "0.1.8"
 dependencies = [
     "requests",
     "geopy",
     "bs4",
 ]
 authors = [
     { name = "Dmitry Luschan", email = "dluschan@gmail.com" },
```

### Comparing `kgr-0.1.7/src/lib.py` & `kgr-0.1.8/src/lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,19 +62,19 @@
 			row["WKT"] = f"""POINT ({row["lon"]} {row["lat"]})"""
 			if args.verbosity > 0 and i % 10 == 0 or args.verbosity > 1:
 				print(f"Done: {i:>{width}d}/{len(data)}")
 	return errors
 
 
 def read_data(args):
-	return list(DictReader(open(args.input, newline=''), delimiter=args.delimiter))
+	return list(DictReader(open(args.input, newline='', encoding="UTF-8"), delimiter=args.delimiter))
 
 
 def write_data(data: list, args):
-	with open(args.output, 'w', newline='') as csvfile:
+	with open(args.output, 'w', newline='', encoding="UTF-8") as csvfile:
 		writer = DictWriter(csvfile, fieldnames=data[0].keys())
 		writer.writeheader()
 		for row in data:
 			writer.writerow(row)
 
 
 def create_placemark(row: dict, src_name: str):
@@ -109,15 +109,15 @@
 	name_tag = Document().createElement("name")
 	name_tag.appendChild(Document().createTextNode(args.layout))
 	doc_tag.appendChild(name_tag)
 
 	for row in data:
 		doc_tag.appendChild(create_placemark(row, args.suffix))
 	root.appendChild(doc_tag)
-	print(root.toprettyxml(), file=open(args.output, "w"))
+	print(root.toprettyxml(), file=open(args.output, "w", encoding="UTF-8"))
 
 
 def create_parser():
 	parser = ArgumentParser(description="Miltitool for convert data from https://memopzk.org to Google Maps")
 	subparsers = parser.add_subparsers(dest='command')
 
 	check_parser = subparsers.add_parser('check', description="Check get geocode for single address")
@@ -172,15 +172,15 @@
 	parse_raw_data(data, args)
 	write_data(data, args)
 
 
 def geocode(args):
 	if args.replace:
 		args.output = args.input
-	args.error = open(args.error, "w") if args.error else stderr
+	args.error = open(args.error, "w", encoding="UTF-8") if args.error else stderr
 	
 	data = read_data(args)
 	assert len(data), "Empty data"
 	assert "ФИО" in data[0].keys(), """Error: Missing column "ФИО"! """
 	assert "city" in data[0].keys(), """Error: Missing column "city"! """
 	errors = translate_city_to_geocode(data, args)
 	if not args.quiet:
```

### Comparing `kgr-0.1.7/PKG-INFO` & `kgr-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kgr
-Version: 0.1.7
+Version: 0.1.8
 Summary: Miltitool for convert data from https://memopzk.org to Google Maps
 Author-Email: Dmitry Luschan <dluschan@gmail.com>
 Maintainer-Email: Dmitry Luschan <dluschan@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Dmitry Luschan
```

