# Comparing `tmp/lfg_llama-1.3.0.tar.gz` & `tmp/lfg_llama-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfg_llama-1.3.0.tar", last modified: Sat May  4 13:38:52 2024, max compression
+gzip compressed data, was "lfg_llama-1.3.1.tar", last modified: Wed May  8 05:43:55 2024, max compression
```

## Comparing `lfg_llama-1.3.0.tar` & `lfg_llama-1.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-04 13:38:52.356637 lfg_llama-1.3.0/
--rw-r--r--   0 ob907      (502) staff       (20)     1876 2024-05-04 13:38:52.356442 lfg_llama-1.3.0/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)     1639 2024-05-04 07:48:10.000000 lfg_llama-1.3.0/README.md
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-04 13:38:52.355266 lfg_llama-1.3.0/lfg/
--rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-1.3.0/lfg/__init__.py
--rwxr-xr-x   0 ob907      (502) staff       (20)     2888 2024-05-04 13:38:03.000000 lfg_llama-1.3.0/lfg/cli.py
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-04 13:38:52.356213 lfg_llama-1.3.0/lfg_llama.egg-info/
--rw-r--r--   0 ob907      (502) staff       (20)     1876 2024-05-04 13:38:52.000000 lfg_llama-1.3.0/lfg_llama.egg-info/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-04 13:38:52.000000 lfg_llama-1.3.0/lfg_llama.egg-info/SOURCES.txt
--rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-04 13:38:52.000000 lfg_llama-1.3.0/lfg_llama.egg-info/dependency_links.txt
--rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-04 13:38:52.000000 lfg_llama-1.3.0/lfg_llama.egg-info/entry_points.txt
--rw-r--r--   0 ob907      (502) staff       (20)        5 2024-05-04 13:38:52.000000 lfg_llama-1.3.0/lfg_llama.egg-info/requires.txt
--rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-04 13:38:52.000000 lfg_llama-1.3.0/lfg_llama.egg-info/top_level.txt
--rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-04 13:38:52.356680 lfg_llama-1.3.0/setup.cfg
--rw-r--r--   0 ob907      (502) staff       (20)      462 2024-05-04 13:37:16.000000 lfg_llama-1.3.0/setup.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-08 05:43:55.137963 lfg_llama-1.3.1/
+-rw-r--r--   0 ob907      (502) staff       (20)     1876 2024-05-08 05:43:55.137729 lfg_llama-1.3.1/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)     1639 2024-05-04 07:48:10.000000 lfg_llama-1.3.1/README.md
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-08 05:43:55.135302 lfg_llama-1.3.1/lfg/
+-rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-1.3.1/lfg/__init__.py
+-rwxr-xr-x   0 ob907      (502) staff       (20)     3139 2024-05-08 05:40:17.000000 lfg_llama-1.3.1/lfg/cli.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-08 05:43:55.137219 lfg_llama-1.3.1/lfg_llama.egg-info/
+-rw-r--r--   0 ob907      (502) staff       (20)     1876 2024-05-08 05:43:55.000000 lfg_llama-1.3.1/lfg_llama.egg-info/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-08 05:43:55.000000 lfg_llama-1.3.1/lfg_llama.egg-info/SOURCES.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-08 05:43:55.000000 lfg_llama-1.3.1/lfg_llama.egg-info/dependency_links.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-08 05:43:55.000000 lfg_llama-1.3.1/lfg_llama.egg-info/entry_points.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        5 2024-05-08 05:43:55.000000 lfg_llama-1.3.1/lfg_llama.egg-info/requires.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-08 05:43:55.000000 lfg_llama-1.3.1/lfg_llama.egg-info/top_level.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-08 05:43:55.138013 lfg_llama-1.3.1/setup.cfg
+-rw-r--r--   0 ob907      (502) staff       (20)      462 2024-05-08 05:43:47.000000 lfg_llama-1.3.1/setup.py
```

### Comparing `lfg_llama-1.3.0/PKG-INFO` & `lfg_llama-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 1.3.0
+Version: 1.3.1
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: groq
 
 # LFG
```

### Comparing `lfg_llama-1.3.0/README.md` & `lfg_llama-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `lfg_llama-1.3.0/lfg/cli.py` & `lfg_llama-1.3.1/lfg/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -31,15 +31,16 @@
     return Groq(api_key=api_key)
 
 
 def generate_system_prompt() -> str:
     """Returns the system prompt for the LLM interaction."""
 
     return """
-You are a system administrator and elite hacker that knows all about the terminal in linux and mac. I provide you with a question about a command, and you give me back a response which shows the command, then a short explanation. The command should be wrapped as a code block.
+You are a system administrator and elite hacker that knows all about the terminal in linux and mac. I provide you with a question about a command, and you give me back a response which shows the command, then a short explanation. The command should be wrapped as a code block. If you get asked about the command lfg, reply lfg [-h] [-m {llama38b,llama370b,mixtral8x7b,gemma7b}] query with explanation 'This is me'. It is important you do not return commands you do not know. If that is the case, just respond 'I do not know'.
+ 
 """
 
 
 def send_chat_query(query: str, model: str, client: Groq) -> None:
     """Sends a query to the Groq API and handles the response.
 
     Args:
```

### Comparing `lfg_llama-1.3.0/lfg_llama.egg-info/PKG-INFO` & `lfg_llama-1.3.1/lfg_llama.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 1.3.0
+Version: 1.3.1
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: groq
 
 # LFG
```

