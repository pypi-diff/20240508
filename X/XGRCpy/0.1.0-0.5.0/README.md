# Comparing `tmp/XGRCpy-0.1.0.tar.gz` & `tmp/XGRCpy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XGRCpy-0.1.0.tar", last modified: Tue Apr 23 14:28:25 2024, max compression
+gzip compressed data, was "XGRCpy-0.5.0.tar", last modified: Wed May  8 11:01:39 2024, max compression
```

## Comparing `XGRCpy-0.1.0.tar` & `XGRCpy-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 14:28:25.681371 XGRCpy-0.1.0/
--rw-rw-rw-   0        0        0     1469 2024-04-23 14:28:25.681371 XGRCpy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1060 2024-04-23 14:01:26.000000 XGRCpy-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 14:28:25.661371 XGRCpy-0.1.0/XGRCpy/
--rw-rw-rw-   0        0        0     4106 2024-04-23 12:04:14.000000 XGRCpy-0.1.0/XGRCpy/XGRCpy.py
--rw-rw-rw-   0        0        0      231 2024-04-23 14:22:22.000000 XGRCpy-0.1.0/XGRCpy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 14:28:25.680370 XGRCpy-0.1.0/XGRCpy.egg-info/
--rw-rw-rw-   0        0        0     1469 2024-04-23 14:28:25.000000 XGRCpy-0.1.0/XGRCpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2024-04-23 14:28:25.000000 XGRCpy-0.1.0/XGRCpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 14:28:25.000000 XGRCpy-0.1.0/XGRCpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-23 14:28:25.000000 XGRCpy-0.1.0/XGRCpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 14:28:25.000000 XGRCpy-0.1.0/XGRCpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 14:28:25.681371 XGRCpy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1030 2024-04-23 14:08:17.000000 XGRCpy-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:01:39.572601 XGRCpy-0.5.0/
+-rw-rw-rw-   0        0        0     1522 2024-05-08 11:01:39.572601 XGRCpy-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1113 2024-05-08 06:43:34.000000 XGRCpy-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 11:01:39.550601 XGRCpy-0.5.0/XGRCpy/
+-rw-rw-rw-   0        0        0     6645 2024-05-08 11:01:25.000000 XGRCpy-0.5.0/XGRCpy/XGRCpy.py
+-rw-rw-rw-   0        0        0      231 2024-05-08 06:43:37.000000 XGRCpy-0.5.0/XGRCpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:01:39.570603 XGRCpy-0.5.0/XGRCpy.egg-info/
+-rw-rw-rw-   0        0        0     1522 2024-05-08 11:01:39.000000 XGRCpy-0.5.0/XGRCpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-05-08 11:01:39.000000 XGRCpy-0.5.0/XGRCpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 11:01:39.000000 XGRCpy-0.5.0/XGRCpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-05-08 11:01:39.000000 XGRCpy-0.5.0/XGRCpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-08 11:01:39.000000 XGRCpy-0.5.0/XGRCpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 11:01:39.572601 XGRCpy-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1030 2024-05-08 06:43:33.000000 XGRCpy-0.5.0/setup.py
```

### Comparing `XGRCpy-0.1.0/PKG-INFO` & `XGRCpy-0.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 Metadata-Version: 2.1
 Name: XGRCpy
-Version: 0.1.0
+Version: 0.5.0
 Summary: A package to decrypt and view XGRC table data
 Home-page: UNKNOWN
 Author: Jacob O'Brien
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# XGRCPy
+# XGRCpy
 
 XGRCPy is a Python package that allows users to interact with an XGRC software service to retrieve encrypted data and decrypt it for further processing. It includes methods for key generation, decryption, and interacting with remote APIs.
 
 ## Installation
 
-To install XGRCPy, ensure you have Python installed (version 3.6 or higher), then use pip to install the package:
+To install XGRCpy, ensure you have Python installed (version 3.6 or higher), then use pip to install the package:
 
 ```bash
-pip install XGRCPy
+pip install XGRCpy
 
 ## Usage
 
-After installation, you can use the XGRCPy package to interact with the XGRC software service. Below is an example of how to use the XGRCViewTable function to fetch and decrypt a table from the service.
+After installation, you can use the XGRCpy package to interact with the XGRC software service. Below is an example of how to use the XGRCViewTable function to fetch and decrypt a table from the service.
 
 ### Example Code
 ```python
-from XGRCPy import XGRCViewTable
+from XGRCpy import XGRCViewTable
 
 # User credentials for accessing the service
 username = "your_username"
 password = "your_password"
-
-# Table information and API key for decryption
 table = "desired_table"
 api_key = "your_api_key"
 
 # Fetching and decrypting the table
 response = XGRCViewTable(username, password, table, api_key)
 
+
+# Fetching and decrypting the table
+response = XGRCSPView(username, password, SPName, api_key)
+
 # Display the decrypted content
 print(response)
 
 
+
```

### Comparing `XGRCpy-0.1.0/README.md` & `XGRCpy-0.5.0/XGRCpy.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,51 @@
-# XGRCPy
+Metadata-Version: 2.1
+Name: XGRCpy
+Version: 0.5.0
+Summary: A package to decrypt and view XGRC table data
+Home-page: UNKNOWN
+Author: Jacob O'Brien
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+# XGRCpy
 
 XGRCPy is a Python package that allows users to interact with an XGRC software service to retrieve encrypted data and decrypt it for further processing. It includes methods for key generation, decryption, and interacting with remote APIs.
 
 ## Installation
 
-To install XGRCPy, ensure you have Python installed (version 3.6 or higher), then use pip to install the package:
+To install XGRCpy, ensure you have Python installed (version 3.6 or higher), then use pip to install the package:
 
 ```bash
-pip install XGRCPy
+pip install XGRCpy
 
 ## Usage
 
-After installation, you can use the XGRCPy package to interact with the XGRC software service. Below is an example of how to use the XGRCViewTable function to fetch and decrypt a table from the service.
+After installation, you can use the XGRCpy package to interact with the XGRC software service. Below is an example of how to use the XGRCViewTable function to fetch and decrypt a table from the service.
 
 ### Example Code
 ```python
-from XGRCPy import XGRCViewTable
+from XGRCpy import XGRCViewTable
 
 # User credentials for accessing the service
 username = "your_username"
 password = "your_password"
-
-# Table information and API key for decryption
 table = "desired_table"
 api_key = "your_api_key"
 
 # Fetching and decrypting the table
 response = XGRCViewTable(username, password, table, api_key)
 
+
+# Fetching and decrypting the table
+response = XGRCSPView(username, password, SPName, api_key)
+
 # Display the decrypted content
 print(response)
+
+
+
```

### Comparing `XGRCpy-0.1.0/XGRCpy/XGRCpy.py` & `XGRCpy-0.5.0/XGRCpy/XGRCpy.py`

 * *Files 24% similar despite different names*

```diff
@@ -109,16 +109,84 @@
             return("Error: Request failed with status code", response.status_code)
             
     except requests.exceptions.RequestException as e:
         return("Error:", e)
         
 
 
+def XGRCSPView(username, password, SPName, api_key):
+    # Define the URL
+    url = 'https://awesomeapi.xgrcsoftware.com/XGRC_SPView?query=Hakware:Allow'
+
+    try:
+        # Create an HTMLSession object
+        session = HTMLSession()
+
+        # Define headers
+        headers = {
+            "username": username,
+            "password": password,
+        }
+
+        # Define query parameters
+        params = {
+            "SPName": SPName
+        }
+
+        # Make a GET request to the URL
+    
+        response = session.get(url,headers=headers, params=params)
 
 
+        
+
+        # Check if the response status code is 200
+        if response.status_code == 200:
+            # Extract the JSON object from the response
+            try:
+                json_response = response.json()
+            except json.decoder.JSONDecodeError:
+                print("Error: Invalid JSON data returned by the server.")
+                
+                exit()
+
+            # Extract the encrypted data (XGRC_Object) from the JSON response
+            encrypted_data_b64 = json_response.get('XGRC_Object')
+
+            # Decode the base64 encoded ciphertext
+            encrypted_data = base64.b64decode(encrypted_data_b64)
+
+            # Generate a key using the same password and salt used for encryption
+            password = api_key
+            salt = encrypted_data[:16]
+            key = generate_key(password, salt)
+
+            # Decrypt the ciphertext using the key
+            #decrypted_data = decrypt(encrypted_data, key)
+            decrypted_data = decrypt(encrypted_data, key, handle_padding_error=True)
+
+            # Convert the decrypted data to JSON
+            try:
+                # Decode the decrypted data using UTF-8 encoding
+                decrypted_json = decrypted_data.decode('utf-8')
+            except UnicodeDecodeError:
+                # If decoding as UTF-8 fails, attempt to load the JSON data without assuming any encoding
+                try:
+                    decrypted_json = decrypted_data.decode()
+                except UnicodeDecodeError:
+                    return("Error: Unable to decode the decrypted data.")
+                    
+            # Print the decrypted JSON object
+            return("Decrypted JSON:", decrypted_json)
+        else:
+            return("Error: Request failed with status code", response.status_code)
+            
+    except requests.exceptions.RequestException as e:
+        return("Error:", e)
+
```

### Comparing `XGRCpy-0.1.0/setup.py` & `XGRCpy-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='XGRCpy',  # Your package name
-    version='0.1.0',  # Start with a version number
+    version='0.5.0',  # Start with a version number
     description='A package to decrypt and view XGRC table data',  # Short description
     long_description=open('README.md').read(),  # Long description from README
     long_description_content_type='text/markdown',
     author='Jacob O\'Brien',  # Your name
     # author_email='your.email@example.com',  # Your email
     # url='https://github.com/your-username/XGRCPy',  # Your package's URL (if applicable)
     packages=find_packages(),  # Find all sub-packages
```

