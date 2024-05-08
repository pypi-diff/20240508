# Comparing `tmp/decoutilities-0.2.2.tar.gz` & `tmp/decoutilities-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoutilities-0.2.2.tar", last modified: Tue May  7 13:01:33 2024, max compression
+gzip compressed data, was "decoutilities-0.2.3.tar", last modified: Wed May  8 08:04:29 2024, max compression
```

## Comparing `decoutilities-0.2.2.tar` & `decoutilities-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 13:01:33.076781 decoutilities-0.2.2/
--rw-rw-rw-   0        0        0     1089 2024-04-26 12:51:10.000000 decoutilities-0.2.2/LICENSE
--rw-rw-rw-   0        0        0    10146 2024-05-07 13:01:33.054928 decoutilities-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     9675 2024-05-07 12:58:21.000000 decoutilities-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 13:01:32.721167 decoutilities-0.2.2/decoutilities/
--rw-rw-rw-   0        0        0     4740 2024-05-07 07:54:09.000000 decoutilities-0.2.2/decoutilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 13:01:32.879109 decoutilities-0.2.2/decoutilities/config/
--rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.2.2/decoutilities/config/__init__.py
--rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.2.2/decoutilities/config/config.py
--rw-rw-rw-   0        0        0     2736 2024-04-30 08:27:33.000000 decoutilities-0.2.2/decoutilities/config/configContainer.py
-drwxrwxrwx   0        0        0        0 2024-05-07 13:01:32.931755 decoutilities-0.2.2/decoutilities/inject/
--rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.2.2/decoutilities/inject/__init__.py
--rw-rw-rw-   0        0        0      483 2024-04-29 13:14:09.000000 decoutilities-0.2.2/decoutilities/inject/injector.py
-drwxrwxrwx   0        0        0        0 2024-05-07 13:01:32.978442 decoutilities-0.2.2/decoutilities/queue/
--rw-rw-rw-   0        0        0     1043 2024-05-07 08:05:33.000000 decoutilities-0.2.2/decoutilities/queue/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 13:01:33.014202 decoutilities-0.2.2/decoutilities.egg-info/
--rw-rw-rw-   0        0        0    10146 2024-05-07 13:01:32.000000 decoutilities-0.2.2/decoutilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      402 2024-05-07 13:01:32.000000 decoutilities-0.2.2/decoutilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 13:01:32.000000 decoutilities-0.2.2/decoutilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-07 13:01:32.000000 decoutilities-0.2.2/decoutilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 13:01:33.076781 decoutilities-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      729 2024-05-07 13:00:25.000000 decoutilities-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:04:29.928145 decoutilities-0.2.3/
+-rw-rw-rw-   0        0        0     1089 2024-04-26 12:51:10.000000 decoutilities-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0    12036 2024-05-08 08:04:29.915233 decoutilities-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11565 2024-05-08 08:01:40.000000 decoutilities-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 08:04:29.473198 decoutilities-0.2.3/decoutilities/
+-rw-rw-rw-   0        0        0     4740 2024-05-07 07:54:09.000000 decoutilities-0.2.3/decoutilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:04:29.710605 decoutilities-0.2.3/decoutilities/config/
+-rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.2.3/decoutilities/config/__init__.py
+-rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.2.3/decoutilities/config/config.py
+-rw-rw-rw-   0        0        0     2736 2024-04-30 08:27:33.000000 decoutilities-0.2.3/decoutilities/config/configContainer.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:04:29.809938 decoutilities-0.2.3/decoutilities/data/
+-rw-rw-rw-   0        0        0      104 2024-05-08 07:57:21.000000 decoutilities-0.2.3/decoutilities/data/__init__.py
+-rw-rw-rw-   0        0        0     2154 2024-05-08 07:56:33.000000 decoutilities-0.2.3/decoutilities/data/dataEncryptor.py
+-rw-rw-rw-   0        0        0     1671 2024-05-08 07:52:43.000000 decoutilities-0.2.3/decoutilities/data/keyManager.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:04:29.839738 decoutilities-0.2.3/decoutilities/inject/
+-rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.2.3/decoutilities/inject/__init__.py
+-rw-rw-rw-   0        0        0      483 2024-04-29 13:14:09.000000 decoutilities-0.2.3/decoutilities/inject/injector.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:04:29.887419 decoutilities-0.2.3/decoutilities/queue/
+-rw-rw-rw-   0        0        0     1043 2024-05-07 08:05:33.000000 decoutilities-0.2.3/decoutilities/queue/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:04:29.901330 decoutilities-0.2.3/decoutilities.egg-info/
+-rw-rw-rw-   0        0        0    12036 2024-05-08 08:04:29.000000 decoutilities-0.2.3/decoutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2024-05-08 08:04:29.000000 decoutilities-0.2.3/decoutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 08:04:29.000000 decoutilities-0.2.3/decoutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-08 08:04:29.000000 decoutilities-0.2.3/decoutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 08:04:29.928145 decoutilities-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-05-08 08:03:28.000000 decoutilities-0.2.3/setup.py
```

### Comparing `decoutilities-0.2.2/LICENSE` & `decoutilities-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.2/PKG-INFO` & `decoutilities-0.2.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: decoutilities
-Version: 0.2.2
-Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
-Author: Hugo Torres
-Author-email: contact@redactado.es
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # decoutilities
 
 A simple python package that allows using decorators for multiple things like easily setting up singleton or config files.
 
 ## Installation
 
 You can install `decoutilities` using pip:
@@ -332,14 +319,62 @@
 
 - `add_item(item)`: Adds an item to the end of the queue.
 - `remove_item()`: Removes and returns the first item in the queue. If the queue is empty, it returns `None`.
 - `check_item()`: Returns the first item in the queue without removing it. If the queue is empty, it returns `None`.
 - `clear_queue()`: Clears all items from the queue.
 - `print_log()`: Prints the log of actions performed on the queue. Each log entry includes the timestamp, action, item, and the size of the queue after the action.
 
+## Data Encryption Module
+
+This module provides a way to encrypt and decrypt data, either in the form of text strings or files. It uses an XOR encryption system with a randomly generated key.
+
+### Classes
+
+The module consists of two main classes:
+
+1. `keyManager`: This class is responsible for generating a unique encryption key. The key is randomly generated each time a `keyManager` instance is created.
+
+2. `dataEncryptor`: This class uses an instance of `keyManager` to encrypt and decrypt data. The data can be a text string or a file.
+
+### Usage
+
+To use this module, you first need to create an instance of `keyManager`:
+
+```python
+key_manager = keyManager()
+```
+
+Next, you can create an instance of `dataEncryptor` using the `keyManager`:
+
+```python
+encryptor = dataEncryptor(key_manager)
+```
+
+Now you can encrypt and decrypt data. To encrypt data, use the `encrypt` method:
+
+```python
+encrypted_data = encryptor.encrypt(source, 'string')  # To encrypt a text string
+encrypted_file = encryptor.encrypt(source, 'file')  # To encrypt a file
+```
+
+To decrypt data, use the `decrypt` method:
+
+```python
+decrypted_data = encryptor.decrypt(encrypted_data, 'string')  # To decrypt a text string
+decrypted_file = encryptor.decrypt(encrypted_file, 'file')  # To decrypt a file
+```
+
+### Key Generation
+
+The key generation process in `keyManager` is designed to be secure. It uses a large random number as the basis for the key, which makes it difficult for an attacker to guess. The length of the key also contributes to its security. The longer the key, the more possible combinations there are, making it harder for an attacker to crack.
+
+### Notes
+
+This module uses XOR encryption, which is not secure for most practical uses. It is recommended to use a more secure encryption algorithm for any data that needs protection in the real world.
+
 ## Experimental Features
 
 All features marked as in `BETA` or being `EXPERIMENTAL` are untested, what means they were only tested below specific condititons and not with all case of uses.
 
 Please report any issues or contribute by making a PR (look for [CONTRIBUTING](CONTRIBUTING) section for details).
 
 ### REMEMBER:
@@ -360,8 +395,8 @@
 - FEATURE: For new features, include a explanation mentioning why it should be inside `decoutilities`.
 - BUGFIX: For general bugfixes.
 - SECURITY: For fixes related with security issues.
 - QoL: For QoL improvements
 
 ## Author
 
-- [Hugo Torres](https://github.com/Reddishye)
+- [Hugo Torres](https://github.com/Reddishye)
```

### Comparing `decoutilities-0.2.2/decoutilities/__init__.py` & `decoutilities-0.2.3/decoutilities/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.2/decoutilities/config/config.py` & `decoutilities-0.2.3/decoutilities/config/config.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.2/decoutilities/config/configContainer.py` & `decoutilities-0.2.3/decoutilities/config/configContainer.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.2/decoutilities/queue/__init__.py` & `decoutilities-0.2.3/decoutilities/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.2/decoutilities.egg-info/PKG-INFO` & `decoutilities-0.2.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.2.2
+Version: 0.2.3
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -332,14 +332,62 @@
 
 - `add_item(item)`: Adds an item to the end of the queue.
 - `remove_item()`: Removes and returns the first item in the queue. If the queue is empty, it returns `None`.
 - `check_item()`: Returns the first item in the queue without removing it. If the queue is empty, it returns `None`.
 - `clear_queue()`: Clears all items from the queue.
 - `print_log()`: Prints the log of actions performed on the queue. Each log entry includes the timestamp, action, item, and the size of the queue after the action.
 
+## Data Encryption Module
+
+This module provides a way to encrypt and decrypt data, either in the form of text strings or files. It uses an XOR encryption system with a randomly generated key.
+
+### Classes
+
+The module consists of two main classes:
+
+1. `keyManager`: This class is responsible for generating a unique encryption key. The key is randomly generated each time a `keyManager` instance is created.
+
+2. `dataEncryptor`: This class uses an instance of `keyManager` to encrypt and decrypt data. The data can be a text string or a file.
+
+### Usage
+
+To use this module, you first need to create an instance of `keyManager`:
+
+```python
+key_manager = keyManager()
+```
+
+Next, you can create an instance of `dataEncryptor` using the `keyManager`:
+
+```python
+encryptor = dataEncryptor(key_manager)
+```
+
+Now you can encrypt and decrypt data. To encrypt data, use the `encrypt` method:
+
+```python
+encrypted_data = encryptor.encrypt(source, 'string')  # To encrypt a text string
+encrypted_file = encryptor.encrypt(source, 'file')  # To encrypt a file
+```
+
+To decrypt data, use the `decrypt` method:
+
+```python
+decrypted_data = encryptor.decrypt(encrypted_data, 'string')  # To decrypt a text string
+decrypted_file = encryptor.decrypt(encrypted_file, 'file')  # To decrypt a file
+```
+
+### Key Generation
+
+The key generation process in `keyManager` is designed to be secure. It uses a large random number as the basis for the key, which makes it difficult for an attacker to guess. The length of the key also contributes to its security. The longer the key, the more possible combinations there are, making it harder for an attacker to crack.
+
+### Notes
+
+This module uses XOR encryption, which is not secure for most practical uses. It is recommended to use a more secure encryption algorithm for any data that needs protection in the real world.
+
 ## Experimental Features
 
 All features marked as in `BETA` or being `EXPERIMENTAL` are untested, what means they were only tested below specific condititons and not with all case of uses.
 
 Please report any issues or contribute by making a PR (look for [CONTRIBUTING](CONTRIBUTING) section for details).
 
 ### REMEMBER:
```

### Comparing `decoutilities-0.2.2/setup.py` & `decoutilities-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
 name='decoutilities',
-version='0.2.2',
+version='0.2.3',
 author='Hugo Torres',
 author_email='contact@redactado.es',
 description='Enhance the readability of your code with decorators and simplify the creation of configuration files.',
 packages=find_packages(include=['decoutilities', 'decoutilities.*']),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
```

