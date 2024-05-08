# Comparing `tmp/deps-manager-1.0.2.tar.gz` & `tmp/deps-manager-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deps-manager-1.0.2.tar", last modified: Sat Apr  6 05:34:33 2024, max compression
+gzip compressed data, was "deps-manager-1.0.3.tar", last modified: Wed May  8 19:10:08 2024, max compression
```

## Comparing `deps-manager-1.0.2.tar` & `deps-manager-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-04-06 05:34:33.599907 deps-manager-1.0.2/
--rw-r--r--   0 harshadatupe   (501) staff       (20)      276 2024-04-06 05:34:33.599568 deps-manager-1.0.2/PKG-INFO
--rw-r--r--   0 harshadatupe   (501) staff       (20)     2347 2024-04-06 05:24:23.000000 deps-manager-1.0.2/README.md
-drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-04-06 05:34:33.597495 deps-manager-1.0.2/deps_manager/
--rw-r--r--   0 harshadatupe   (501) staff       (20)        0 2024-04-06 02:20:53.000000 deps-manager-1.0.2/deps_manager/__init__.py
--rw-r--r--   0 harshadatupe   (501) staff       (20)     2615 2024-04-06 02:20:53.000000 deps-manager-1.0.2/deps_manager/dependencies.py
--rw-r--r--   0 harshadatupe   (501) staff       (20)     2484 2024-04-06 05:33:17.000000 deps-manager-1.0.2/deps_manager/main.py
--rw-r--r--   0 harshadatupe   (501) staff       (20)      405 2024-04-06 02:20:53.000000 deps-manager-1.0.2/deps_manager/utils.py
-drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-04-06 05:34:33.599003 deps-manager-1.0.2/deps_manager.egg-info/
--rw-r--r--   0 harshadatupe   (501) staff       (20)      276 2024-04-06 05:34:33.000000 deps-manager-1.0.2/deps_manager.egg-info/PKG-INFO
--rw-r--r--   0 harshadatupe   (501) staff       (20)      333 2024-04-06 05:34:33.000000 deps-manager-1.0.2/deps_manager.egg-info/SOURCES.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)        1 2024-04-06 05:34:33.000000 deps-manager-1.0.2/deps_manager.egg-info/dependency_links.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)       55 2024-04-06 05:34:33.000000 deps-manager-1.0.2/deps_manager.egg-info/entry_points.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)        6 2024-04-06 05:34:33.000000 deps-manager-1.0.2/deps_manager.egg-info/requires.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)       13 2024-04-06 05:34:33.000000 deps-manager-1.0.2/deps_manager.egg-info/top_level.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)       38 2024-04-06 05:34:33.599981 deps-manager-1.0.2/setup.cfg
--rw-r--r--   0 harshadatupe   (501) staff       (20)      535 2024-04-06 05:33:04.000000 deps-manager-1.0.2/setup.py
+drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-08 19:10:08.167495 deps-manager-1.0.3/
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      297 2024-05-08 19:10:08.167222 deps-manager-1.0.3/PKG-INFO
+-rw-r--r--   0 harshadatupe   (501) staff       (20)     2347 2024-04-06 05:24:23.000000 deps-manager-1.0.3/README.md
+drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-08 19:10:08.165547 deps-manager-1.0.3/deps_manager/
+-rw-r--r--   0 harshadatupe   (501) staff       (20)        0 2024-04-06 02:20:53.000000 deps-manager-1.0.3/deps_manager/__init__.py
+-rw-r--r--   0 harshadatupe   (501) staff       (20)     8993 2024-05-08 18:53:47.000000 deps-manager-1.0.3/deps_manager/dependencies.py
+-rw-r--r--   0 harshadatupe   (501) staff       (20)     3000 2024-05-08 19:08:21.000000 deps-manager-1.0.3/deps_manager/main.py
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      405 2024-04-06 02:20:53.000000 deps-manager-1.0.3/deps_manager/utils.py
+drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-08 19:10:08.166746 deps-manager-1.0.3/deps_manager.egg-info/
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      297 2024-05-08 19:10:08.000000 deps-manager-1.0.3/deps_manager.egg-info/PKG-INFO
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      333 2024-05-08 19:10:08.000000 deps-manager-1.0.3/deps_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)        1 2024-05-08 19:10:08.000000 deps-manager-1.0.3/deps_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)       55 2024-05-08 19:10:08.000000 deps-manager-1.0.3/deps_manager.egg-info/entry_points.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)       12 2024-05-08 19:10:08.000000 deps-manager-1.0.3/deps_manager.egg-info/requires.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)       13 2024-05-08 19:10:08.000000 deps-manager-1.0.3/deps_manager.egg-info/top_level.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)       38 2024-05-08 19:10:08.167571 deps-manager-1.0.3/setup.cfg
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      551 2024-05-08 19:05:20.000000 deps-manager-1.0.3/setup.py
```

### Comparing `deps-manager-1.0.2/README.md` & `deps-manager-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `deps-manager-1.0.2/deps_manager/main.py` & `deps-manager-1.0.3/deps_manager/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 def common_options(function):
     """
     Decorator to define common click options.
     """
     function = click.option('-v', '--venv_path', prompt="Enter the path to the virtual environment",
                             help="Path to the virtual environment")(function)
     function = click.option('-l', '--language', prompt="Enter the language", type=click.Choice(['python', 'cpp']),
-                            help="Project Language to manage the dependencies")(function)
+                            help="Project language to manage the dependencies")(function)
     return function
 
 def requirements_option(function):
     """
     Decorator for the requirements file option.
     """
     return click.option('-r', '--requirements_file', prompt="Enter the requirements.txt file name", required=True,
@@ -66,10 +66,24 @@
 @common_options
 @click.option('-lf', '--lock_file', prompt="Enter the lock file name with its absolute path", required=True,
               help="Name of the lock file to lock and save dependencies")
 def lock(venv_path, language, lock_file):
     """Generate a lock file for dependencies."""
     lock_dependencies(lock_file, language, venv_path)
 
+@cli.command()
+@common_options
+def remove_unused(venv_path, language):
+    """Remove unused dependencies."""
+    remove_unused_dependencies(language, venv_path)
+
+@cli.command()
+@click.option('-td', '--tests_dir', required=True,
+              prompt="Enter the tests directory name of the project",
+              help="Name of the directory containing the project's tests")
+def containerize_and_test(language, tests_dir):
+    """Containerize and run the tests."""
+    containerize_and_run_tests(language, tests_dir)
+
 
 if __name__ == '__main__':
     cli()
```

### Comparing `deps-manager-1.0.2/setup.py` & `deps-manager-1.0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='deps-manager',
-    version='1.0.2',
+    version='1.0.3',
     author="Harshada Tupe",
     author_email="harshadatupe8@gmail.com",
     license="MIT",
     packages=find_packages(),
     classifiers=["Programming Language :: Python :: 3 :: Only",
                  "Operating System :: OS Independent"],
     python_requires='>=3.8',
     entry_points={
         'console_scripts': [
             'deps-manager = deps_manager.main:cli',
         ],
     },
     install_requires=[
-        'click', 
+        'click',
+        'conan',
     ],
 )
```

