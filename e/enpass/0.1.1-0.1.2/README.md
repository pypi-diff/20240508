# Comparing `tmp/enpass-0.1.1.tar.gz` & `tmp/enpass-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enpass-0.1.1.tar", last modified: Tue May  7 22:05:24 2024, max compression
+gzip compressed data, was "enpass-0.1.2.tar", last modified: Tue May  7 22:30:42 2024, max compression
```

## Comparing `enpass-0.1.1.tar` & `enpass-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 alesh      (501) staff       (20)        0 2024-05-07 22:05:24.207851 enpass-0.1.1/
--rw-r--r--   0 alesh      (501) staff       (20)     1070 2024-05-06 23:00:22.000000 enpass-0.1.1/LICENSE
--rw-r--r--   0 alesh      (501) staff       (20)       20 2024-05-06 23:03:08.000000 enpass-0.1.1/MANIFEST.in
--rw-r--r--   0 alesh      (501) staff       (20)     2412 2024-05-07 22:05:24.207671 enpass-0.1.1/PKG-INFO
--rw-r--r--   0 alesh      (501) staff       (20)     1847 2024-05-07 21:55:19.000000 enpass-0.1.1/README.md
-drwxr-xr-x   0 alesh      (501) staff       (20)        0 2024-05-07 22:05:24.206893 enpass-0.1.1/enpass/
--rw-r--r--   0 alesh      (501) staff       (20)      178 2024-05-07 02:48:10.000000 enpass-0.1.1/enpass/__init__.py
--rw-r--r--   0 alesh      (501) staff       (20)     1318 2024-05-07 02:30:24.000000 enpass-0.1.1/enpass/base.py
--rw-r--r--   0 alesh      (501) staff       (20)     1469 2024-05-07 16:59:17.000000 enpass-0.1.1/enpass/entropy.py
-drwxr-xr-x   0 alesh      (501) staff       (20)        0 2024-05-07 22:05:24.207475 enpass-0.1.1/enpass.egg-info/
--rw-r--r--   0 alesh      (501) staff       (20)     2412 2024-05-07 22:05:24.000000 enpass-0.1.1/enpass.egg-info/PKG-INFO
--rw-r--r--   0 alesh      (501) staff       (20)      210 2024-05-07 22:05:24.000000 enpass-0.1.1/enpass.egg-info/SOURCES.txt
--rw-r--r--   0 alesh      (501) staff       (20)        1 2024-05-07 22:05:24.000000 enpass-0.1.1/enpass.egg-info/dependency_links.txt
--rw-r--r--   0 alesh      (501) staff       (20)        7 2024-05-07 22:05:24.000000 enpass-0.1.1/enpass.egg-info/top_level.txt
--rw-r--r--   0 alesh      (501) staff       (20)       38 2024-05-07 22:05:24.207889 enpass-0.1.1/setup.cfg
--rw-r--r--   0 alesh      (501) staff       (20)      777 2024-05-07 22:04:05.000000 enpass-0.1.1/setup.py
+drwxr-xr-x   0 alesh      (501) staff       (20)        0 2024-05-07 22:30:42.945864 enpass-0.1.2/
+-rw-r--r--   0 alesh      (501) staff       (20)     1070 2024-05-06 23:00:22.000000 enpass-0.1.2/LICENSE
+-rw-r--r--   0 alesh      (501) staff       (20)       20 2024-05-06 23:03:08.000000 enpass-0.1.2/MANIFEST.in
+-rw-r--r--   0 alesh      (501) staff       (20)     2399 2024-05-07 22:30:42.945668 enpass-0.1.2/PKG-INFO
+-rw-r--r--   0 alesh      (501) staff       (20)     1834 2024-05-07 22:21:11.000000 enpass-0.1.2/README.md
+drwxr-xr-x   0 alesh      (501) staff       (20)        0 2024-05-07 22:30:42.944973 enpass-0.1.2/enpass/
+-rw-r--r--   0 alesh      (501) staff       (20)      178 2024-05-07 02:48:10.000000 enpass-0.1.2/enpass/__init__.py
+-rw-r--r--   0 alesh      (501) staff       (20)     1318 2024-05-07 02:30:24.000000 enpass-0.1.2/enpass/base.py
+-rw-r--r--   0 alesh      (501) staff       (20)     1469 2024-05-07 16:59:17.000000 enpass-0.1.2/enpass/entropy.py
+drwxr-xr-x   0 alesh      (501) staff       (20)        0 2024-05-07 22:30:42.945496 enpass-0.1.2/enpass.egg-info/
+-rw-r--r--   0 alesh      (501) staff       (20)     2399 2024-05-07 22:30:42.000000 enpass-0.1.2/enpass.egg-info/PKG-INFO
+-rw-r--r--   0 alesh      (501) staff       (20)      210 2024-05-07 22:30:42.000000 enpass-0.1.2/enpass.egg-info/SOURCES.txt
+-rw-r--r--   0 alesh      (501) staff       (20)        1 2024-05-07 22:30:42.000000 enpass-0.1.2/enpass.egg-info/dependency_links.txt
+-rw-r--r--   0 alesh      (501) staff       (20)        7 2024-05-07 22:30:42.000000 enpass-0.1.2/enpass.egg-info/top_level.txt
+-rw-r--r--   0 alesh      (501) staff       (20)       38 2024-05-07 22:30:42.945912 enpass-0.1.2/setup.cfg
+-rw-r--r--   0 alesh      (501) staff       (20)      797 2024-05-07 22:30:30.000000 enpass-0.1.2/setup.py
```

### Comparing `enpass-0.1.1/LICENSE` & `enpass-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `enpass-0.1.1/PKG-INFO` & `enpass-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enpass
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple entropy password validator.
 Home-page: https://github.com/Aresshu/enpass
 Author: Andres Ordonez
 License: MIT
 Keywords: entropy password validator strength
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -31,38 +31,38 @@
 ```
 ## Quick Start
 `calc_entropy` calculates the entropy of a password in bits.
     
 Entropy equation = log2(B^L) 
 `B = Base; L = Length`
 ```python
-    from enpass import *
+    import enpass as ep
 
     password = 'P@SSW0RD!'
 
     #Calculates the entropy of a password in bits.
-    entropy = enpass.calc_entopy(password)
+    entropy = ep.calc_entopy(password)
 ```
 `validate` checks if the password's entropy meets the specified minimum requirement.
 
 Passwords should ideally be > 60.
 Great Passwords should be between 70-90.
 ```python
     min_entropy = 60.0
     # Checks if the password's entropy meets the specified minimum requirement.
-    validate = enpass.validate(entropy, min_entropy)
+    validate = ep.validate(entropy, min_entropy)
 ```
 `estimate_bruteforce_time` assumes that cracking time scales linearly with the number of possible combinations.
 
 While this might hold for straightforward brute-force attacks, more sophisticated attacks,
 such as dictionary attacks or those exploiting weaknesses in password hashing algorithms, may have different time complexities.
 ```python
     guesses_per_second = 100_000_000
     # Estimates the amount of time required to brute-force a password 
-    time_brute_estimate = enpass.estimate_bruteforce_time(entropy, guesses_per_second)
+    time_brute_estimate = ep.estimate_bruteforce_time(entropy, guesses_per_second)
 ```
 ## Roadmap
 - [x] Entropy Calculator
 - [x] Brute-Force Estimate
 - [ ] Scoring
 - [ ] Feedback
 - [ ] Throttling/Hashing Brute-Force Estimate
```

### Comparing `enpass-0.1.1/README.md` & `enpass-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,38 +14,38 @@
 ```
 ## Quick Start
 `calc_entropy` calculates the entropy of a password in bits.
     
 Entropy equation = log2(B^L) 
 `B = Base; L = Length`
 ```python
-    from enpass import *
+    import enpass as ep
 
     password = 'P@SSW0RD!'
 
     #Calculates the entropy of a password in bits.
-    entropy = enpass.calc_entopy(password)
+    entropy = ep.calc_entopy(password)
 ```
 `validate` checks if the password's entropy meets the specified minimum requirement.
 
 Passwords should ideally be > 60.
 Great Passwords should be between 70-90.
 ```python
     min_entropy = 60.0
     # Checks if the password's entropy meets the specified minimum requirement.
-    validate = enpass.validate(entropy, min_entropy)
+    validate = ep.validate(entropy, min_entropy)
 ```
 `estimate_bruteforce_time` assumes that cracking time scales linearly with the number of possible combinations.
 
 While this might hold for straightforward brute-force attacks, more sophisticated attacks,
 such as dictionary attacks or those exploiting weaknesses in password hashing algorithms, may have different time complexities.
 ```python
     guesses_per_second = 100_000_000
     # Estimates the amount of time required to brute-force a password 
-    time_brute_estimate = enpass.estimate_bruteforce_time(entropy, guesses_per_second)
+    time_brute_estimate = ep.estimate_bruteforce_time(entropy, guesses_per_second)
 ```
 ## Roadmap
 - [x] Entropy Calculator
 - [x] Brute-Force Estimate
 - [ ] Scoring
 - [ ] Feedback
 - [ ] Throttling/Hashing Brute-Force Estimate
```

### Comparing `enpass-0.1.1/enpass/base.py` & `enpass-0.1.2/enpass/base.py`

 * *Files identical despite different names*

### Comparing `enpass-0.1.1/enpass/entropy.py` & `enpass-0.1.2/enpass/entropy.py`

 * *Files identical despite different names*

### Comparing `enpass-0.1.1/enpass.egg-info/PKG-INFO` & `enpass-0.1.2/enpass.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enpass
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple entropy password validator.
 Home-page: https://github.com/Aresshu/enpass
 Author: Andres Ordonez
 License: MIT
 Keywords: entropy password validator strength
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -31,38 +31,38 @@
 ```
 ## Quick Start
 `calc_entropy` calculates the entropy of a password in bits.
     
 Entropy equation = log2(B^L) 
 `B = Base; L = Length`
 ```python
-    from enpass import *
+    import enpass as ep
 
     password = 'P@SSW0RD!'
 
     #Calculates the entropy of a password in bits.
-    entropy = enpass.calc_entopy(password)
+    entropy = ep.calc_entopy(password)
 ```
 `validate` checks if the password's entropy meets the specified minimum requirement.
 
 Passwords should ideally be > 60.
 Great Passwords should be between 70-90.
 ```python
     min_entropy = 60.0
     # Checks if the password's entropy meets the specified minimum requirement.
-    validate = enpass.validate(entropy, min_entropy)
+    validate = ep.validate(entropy, min_entropy)
 ```
 `estimate_bruteforce_time` assumes that cracking time scales linearly with the number of possible combinations.
 
 While this might hold for straightforward brute-force attacks, more sophisticated attacks,
 such as dictionary attacks or those exploiting weaknesses in password hashing algorithms, may have different time complexities.
 ```python
     guesses_per_second = 100_000_000
     # Estimates the amount of time required to brute-force a password 
-    time_brute_estimate = enpass.estimate_bruteforce_time(entropy, guesses_per_second)
+    time_brute_estimate = ep.estimate_bruteforce_time(entropy, guesses_per_second)
 ```
 ## Roadmap
 - [x] Entropy Calculator
 - [x] Brute-Force Estimate
 - [ ] Scoring
 - [ ] Feedback
 - [ ] Throttling/Hashing Brute-Force Estimate
```

### Comparing `enpass-0.1.1/setup.py` & `enpass-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 with open('README.md') as file:
     long_description = file.read()
 
 setup(
     name = 'enpass',
-    version = '0.1.1',
+    version = '0.1.2',
     description = 'Simple entropy password validator.',
     long_description= long_description,
     long_description_content_type = 'text/markdown',
     author = 'Andres Ordonez',
-    packages=['enpass'],
+    packages=find_packages(),
     url='https://github.com/Aresshu/enpass',
     license = 'MIT',
     classifiers = [
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         "Programming Language :: Python",
```

