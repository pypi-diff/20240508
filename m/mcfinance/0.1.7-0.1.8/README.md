# Comparing `tmp/mcfinance-0.1.7.tar.gz` & `tmp/mcfinance-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcfinance-0.1.7.tar", last modified: Fri Oct 13 19:18:14 2023, max compression
+gzip compressed data, was "mcfinance-0.1.8.tar", last modified: Wed May  8 16:12:48 2024, max compression
```

## Comparing `mcfinance-0.1.7.tar` & `mcfinance-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxrwxrwx   0 kashyap   (1000) kashyap   (1000)        0 2023-10-13 19:18:14.634409 mcfinance-0.1.7/
--rwxrwxrwx   0 kashyap   (1000) kashyap   (1000)     1087 2023-09-14 13:50:36.000000 mcfinance-0.1.7/LICENSE
--rwxrwxrwx   0 kashyap   (1000) kashyap   (1000)     3553 2023-10-13 19:18:14.628078 mcfinance-0.1.7/PKG-INFO
--rwxrwxrwx   0 kashyap   (1000) kashyap   (1000)     3004 2023-10-08 09:40:19.000000 mcfinance-0.1.7/README.md
-drwxrwxrwx   0 kashyap   (1000) kashyap   (1000)        0 2023-10-13 19:18:14.159775 mcfinance-0.1.7/mcfinance.egg-info/
--rwxrwxrwx   0 kashyap   (1000) kashyap   (1000)     3553 2023-10-13 19:18:13.000000 mcfinance-0.1.7/mcfinance.egg-info/PKG-INFO
--rwxrwxrwx   0 kashyap   (1000) kashyap   (1000)      383 2023-10-13 19:18:13.000000 mcfinance-0.1.7/mcfinance.egg-info/SOURCES.txt
--rwxrwxrwx   0 kashyap   (1000) kashyap   (1000)        1 2023-10-13 19:18:13.000000 mcfinance-0.1.7/mcfinance.egg-info/dependency_links.txt
--rwxrwxrwx   0 kashyap   (1000) kashyap   (1000)       45 2023-10-13 19:18:13.000000 mcfinance-0.1.7/mcfinance.egg-info/requires.txt
--rwxrwxrwx   0 kashyap   (1000) kashyap   (1000)       10 2023-10-13 19:18:13.000000 mcfinance-0.1.7/mcfinance.egg-info/top_level.txt
--rwxrwxrwx   0 kashyap   (1000) kashyap   (1000)       38 2023-10-13 19:18:14.636410 mcfinance-0.1.7/setup.cfg
--rwxrwxrwx   0 kashyap   (1000) kashyap   (1000)     1200 2023-10-13 19:18:11.000000 mcfinance-0.1.7/setup.py
-drwxrwxrwx   0 kashyap   (1000) kashyap   (1000)        0 2023-10-13 19:18:13.880858 mcfinance-0.1.7/src/
-drwxrwxrwx   0 kashyap   (1000) kashyap   (1000)        0 2023-10-13 19:18:14.429202 mcfinance-0.1.7/src/mcfinance/
--rwxrwxrwx   0 kashyap   (1000) kashyap   (1000)      157 2023-10-08 07:14:11.000000 mcfinance-0.1.7/src/mcfinance/__init__.py
-drwxrwxrwx   0 kashyap   (1000) kashyap   (1000)        0 2023-10-13 19:18:14.562688 mcfinance-0.1.7/src/mcfinance/data/
--rwxrwxrwx   0 kashyap   (1000) kashyap   (1000)   364493 2023-09-14 09:51:47.000000 mcfinance-0.1.7/src/mcfinance/data/dictbse.json
--rwxrwxrwx   0 kashyap   (1000) kashyap   (1000)   376754 2023-09-14 09:51:47.000000 mcfinance-0.1.7/src/mcfinance/data/dictnse.json
--rwxrwxrwx   0 kashyap   (1000) kashyap   (1000)     2318 2023-10-13 19:06:41.000000 mcfinance-0.1.7/src/mcfinance/extractors.py
--rwxrwxrwx   0 kashyap   (1000) kashyap   (1000)     3976 2023-10-13 19:07:44.000000 mcfinance-0.1.7/src/mcfinance/helper.py
--rwxrwxrwx   0 kashyap   (1000) kashyap   (1000)     2185 2023-10-13 19:06:45.000000 mcfinance-0.1.7/src/mcfinance/retrieval.py
--rwxrwxrwx   0 kashyap   (1000) kashyap   (1000)      481 2023-10-13 19:06:45.000000 mcfinance-0.1.7/src/mcfinance/writer.py
+drwxrwxr-x   0 kashyap   (1000) kashyap   (1000)        0 2024-05-08 16:12:48.928377 mcfinance-0.1.8/
+-rw-rw-r--   0 kashyap   (1000) kashyap   (1000)     1066 2024-02-23 10:20:40.000000 mcfinance-0.1.8/LICENSE
+-rw-r--r--   0 kashyap   (1000) kashyap   (1000)     3265 2024-05-08 16:12:48.928377 mcfinance-0.1.8/PKG-INFO
+-rw-rw-r--   0 kashyap   (1000) kashyap   (1000)     2592 2024-05-08 15:44:08.000000 mcfinance-0.1.8/README.md
+drwxrwxr-x   0 kashyap   (1000) kashyap   (1000)        0 2024-05-08 16:12:48.924377 mcfinance-0.1.8/mcfinance.egg-info/
+-rw-r--r--   0 kashyap   (1000) kashyap   (1000)     3265 2024-05-08 16:12:48.000000 mcfinance-0.1.8/mcfinance.egg-info/PKG-INFO
+-rw-rw-r--   0 kashyap   (1000) kashyap   (1000)      428 2024-05-08 16:12:48.000000 mcfinance-0.1.8/mcfinance.egg-info/SOURCES.txt
+-rw-rw-r--   0 kashyap   (1000) kashyap   (1000)        1 2024-05-08 16:12:48.000000 mcfinance-0.1.8/mcfinance.egg-info/dependency_links.txt
+-rw-rw-r--   0 kashyap   (1000) kashyap   (1000)       60 2024-05-08 16:12:48.000000 mcfinance-0.1.8/mcfinance.egg-info/requires.txt
+-rw-rw-r--   0 kashyap   (1000) kashyap   (1000)       10 2024-05-08 16:12:48.000000 mcfinance-0.1.8/mcfinance.egg-info/top_level.txt
+-rw-rw-r--   0 kashyap   (1000) kashyap   (1000)       38 2024-05-08 16:12:48.928377 mcfinance-0.1.8/setup.cfg
+-rw-rw-r--   0 kashyap   (1000) kashyap   (1000)     1188 2024-05-08 16:05:13.000000 mcfinance-0.1.8/setup.py
+drwxrwxr-x   0 kashyap   (1000) kashyap   (1000)        0 2024-05-08 16:12:48.920377 mcfinance-0.1.8/src/
+drwxrwxr-x   0 kashyap   (1000) kashyap   (1000)        0 2024-05-08 16:12:48.924377 mcfinance-0.1.8/src/mcfinance/
+-rw-rw-r--   0 kashyap   (1000) kashyap   (1000)      154 2024-05-07 04:02:41.000000 mcfinance-0.1.8/src/mcfinance/__init__.py
+drwxrwxr-x   0 kashyap   (1000) kashyap   (1000)        0 2024-05-08 16:12:48.924377 mcfinance-0.1.8/src/mcfinance/data/
+-rw-rw-r--   0 kashyap   (1000) kashyap   (1000)   364493 2024-02-23 10:20:40.000000 mcfinance-0.1.8/src/mcfinance/data/dictbse.json
+-rw-rw-r--   0 kashyap   (1000) kashyap   (1000)   376754 2024-02-23 10:20:40.000000 mcfinance-0.1.8/src/mcfinance/data/dictnse.json
+-rw-rw-r--   0 kashyap   (1000) kashyap   (1000)     2257 2024-05-08 15:16:34.000000 mcfinance-0.1.8/src/mcfinance/extractors.py
+-rw-rw-r--   0 kashyap   (1000) kashyap   (1000)     3944 2024-05-08 15:37:32.000000 mcfinance-0.1.8/src/mcfinance/helper.py
+-rw-rw-r--   0 kashyap   (1000) kashyap   (1000)     2240 2024-05-08 16:11:53.000000 mcfinance-0.1.8/src/mcfinance/retrieval.py
+-rw-rw-r--   0 kashyap   (1000) kashyap   (1000)      468 2024-02-23 10:20:40.000000 mcfinance-0.1.8/src/mcfinance/writer.py
+drwxrwxr-x   0 kashyap   (1000) kashyap   (1000)        0 2024-05-08 16:12:48.924377 mcfinance-0.1.8/tests/
+-rw-rw-r--   0 kashyap   (1000) kashyap   (1000)      444 2024-05-07 04:12:34.000000 mcfinance-0.1.8/tests/test0.py
+-rw-rw-r--   0 kashyap   (1000) kashyap   (1000)      476 2024-05-07 04:23:37.000000 mcfinance-0.1.8/tests/test1.py
+-rw-rw-r--   0 kashyap   (1000) kashyap   (1000)      567 2024-05-08 15:23:21.000000 mcfinance-0.1.8/tests/test2.py
```

### Comparing `mcfinance-0.1.7/PKG-INFO` & `mcfinance-0.1.8/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,108 +1,94 @@
 Metadata-Version: 2.1
 Name: mcfinance
-Version: 0.1.7
+Version: 0.1.8
 Summary: Money control financial data extractor-Requires python 3.7+
-Home-page: UNKNOWN
 Author: 05kashyap-ragha1992
 Author-email: <aryankashyapnaveen@gmail.com>
-License: UNKNOWN
 Keywords: python,financial,extractor,data
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: bs4
+Requires-Dist: html5lib
+Requires-Dist: lxml
+Requires-Dist: matplotlib
+Requires-Dist: requests
+Requires-Dist: openpyxl
+Requires-Dist: PyQt5
 
 
-# mcfinance
-
-Developed by ragha1992 and 05kashyap
-
-## Description:
-
-Extract financial data from the money control website using the company name, BSE or NSE number.
-Export any selected data into either pandas dataframe or excel sheet with ease!
-### .
-
-*Disclaimer*: We are in no way affiliated with moneycontrol.com
- 
-## Usage:
-### Initialise company details:
-#### Create an Extractor instance with company name/ BSE/ NSE ID and/or number of years(default), required documents(default), and filepath to write documents(default current directory).
-
-```python
-from mcfinance import Extractor
-```
-```python
-Company = Extractor(user_input= "Company_name")
-```
-or input the BSE listing number(int) (number can be used as input directly)
-```python
-Company = Extractor(user_input= BSEnumber)
-```
-or input the NSE listing code (code can be used as input directly)
-```python
-Company = Extractor(user_input= "NSEcode")
-```
-```python
-#years and docs are default
-Company = Extractor(user_input= "Company_name",years = 10, docs = ["balance sheet", "profit loss"], filepath = "/files")
-```
-any of the inputs can be changed later on as per user convenience
-```python
-Company.set_inputs(years = 6)
-```
-We can view the initialised details using: 
-```python
-print(Company)
-```
-output:
-```
-Extractor object, name is Company_name, number of years is 10, documents are ["balancesheet", "profit loss"]
-```
-
-### Export company details as excel file (default)
-#### The get_info() function can be used to extract and store company data in an excel file. The file will be stored in the current filepath or the user defined filepath as per object initialisation 
-
-```python
-Company.get_info()
-```
-or
-```python
-Company.get_info(option = 1)
-```
-
-### Export company details into pandas data frame
-
-```python
-DataFrame1, DataFrame2, DataFrame3 = Company.get_info(option = 0)
-```
-### Plot certain attribute over selected years using matplotlib
-#### The plotter() function can be used to show the companies attribute from a certain document over the selected period of time using a line graph from the matplotlib library. The function accepts a single required arguement for the attribute selection. 
-
-```python
-company.plotter("certain file attribute of the document")
-```
-#### Usage example: 
-
-```python
-cmp = Extractor("TCS", years = 10, docs = ["ratios"])
-cmp.plotter("EV/EBITDA (X)")
-```
-output:
-
-![image](https://github.com/05kashyap/moneycontrol_financial-extractor/assets/120780494/f5be744e-e065-4b03-b6df-2ca7e765c4b2)
-
-### We can also plot the data of multiple companies on the same graph for comparison purposes
-```python
-company1 = Extractor("TCS", years = 10, docs = ["ratios"])
-company2 = Extractor("Infosys", years = 10, docs = ["ratios"])
-Extractor.cmp_plot(comp = [company1, company2], attributes = "EV/EBITDA (X)")
-```
-output:
-
-![image](https://github.com/05kashyap/mcfinance/assets/120780494/294f8313-2876-4751-9485-18517dccb0d3)
+# mcfinance
 
+### Developed by 05kashyap and ragha1992
+### PyPI stats:
+[![Downloads](https://static.pepy.tech/badge/mcfinance)](https://pepy.tech/project/mcfinance)
+## Description:
 
+Extract financial data from the money control website using the company name, BSE or NSE number.
+Export any selected data into either pandas dataframe or excel sheet with ease!
+### .
+
+*Disclaimer*: We are in no way affiliated with moneycontrol.com
+ 
+## Usage:
+```python
+pip install mcfinance
+```
+### Initialise company details:
+#### Create an Extractor instance with company name/ BSE/ NSE ID (required) and/or number of years(default), required documents(default), and filepath to write documents(default current directory).
+
+```python
+from mcfinance import Extractor
+Company = Extractor(user_input= "Company_name")
+#years and docs are default
+Company = Extractor(user_input= "Company_name",years = 10, docs = ["balance sheet", "profit loss"], filepath = "/files")
+```
+any of the inputs can be changed later on as per user convenience
+```python
+Company.set_inputs(years = 6)
+```
+### Export company details as excel file (default)
+#### The get_info() function can be used to extract and store company data in an excel file. The file will be stored in the current filepath or the user defined filepath as per object initialisation 
+
+```python
+Company.get_info()
+```
+or
+```python
+Company.get_info(option = 1)
+```
+
+### Export company details into pandas data frame
+
+```python
+DataFrame1, DataFrame2, DataFrame3 = Company.get_info(option = 0)
+```
+### Plot certain attribute over selected years using matplotlib
+#### The plotter() function can be used to show the companies attribute from a certain document over the selected period of time using a line graph from the matplotlib library. The function accepts a single required arguement for the attribute selection. 
+
+```python
+company.plotter("certain file attribute of the document")
+```
+#### Usage example: 
+
+```python
+cmp = Extractor("TCS", years = 10, docs = ["ratios"])
+cmp.plotter("EV/EBITDA (X)")
+```
+output:
+
+![image](https://github.com/05kashyap/moneycontrol_financial-extractor/assets/120780494/f5be744e-e065-4b03-b6df-2ca7e765c4b2)
+
+### We can also plot the data of multiple companies on the same graph for comparison purposes
+```python
+company1 = Extractor("TCS", years = 10, docs = ["ratios"])
+company2 = Extractor("Infosys", years = 10, docs = ["ratios"])
+Extractor.cmp_plot(comp = [company1, company2], attributes = "EV/EBITDA (X)")
+```
+output:
+
+![image](https://github.com/05kashyap/mcfinance/assets/120780494/294f8313-2876-4751-9485-18517dccb0d3)
```

### Comparing `mcfinance-0.1.7/README.md` & `mcfinance-0.1.8/mcfinance.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,88 +1,94 @@
-# mcfinance
-
-Developed by ragha1992 and 05kashyap
-
-## Description:
-
-Extract financial data from the money control website using the company name, BSE or NSE number.
-Export any selected data into either pandas dataframe or excel sheet with ease!
-### .
-
-*Disclaimer*: We are in no way affiliated with moneycontrol.com
- 
-## Usage:
-### Initialise company details:
-#### Create an Extractor instance with company name/ BSE/ NSE ID and/or number of years(default), required documents(default), and filepath to write documents(default current directory).
-
-```python
-from mcfinance import Extractor
-```
-```python
-Company = Extractor(user_input= "Company_name")
-```
-or input the BSE listing number(int) (number can be used as input directly)
-```python
-Company = Extractor(user_input= BSEnumber)
-```
-or input the NSE listing code (code can be used as input directly)
-```python
-Company = Extractor(user_input= "NSEcode")
-```
-```python
-#years and docs are default
-Company = Extractor(user_input= "Company_name",years = 10, docs = ["balance sheet", "profit loss"], filepath = "/files")
-```
-any of the inputs can be changed later on as per user convenience
-```python
-Company.set_inputs(years = 6)
-```
-We can view the initialised details using: 
-```python
-print(Company)
-```
-output:
-```
-Extractor object, name is Company_name, number of years is 10, documents are ["balancesheet", "profit loss"]
-```
-
-### Export company details as excel file (default)
-#### The get_info() function can be used to extract and store company data in an excel file. The file will be stored in the current filepath or the user defined filepath as per object initialisation 
-
-```python
-Company.get_info()
-```
-or
-```python
-Company.get_info(option = 1)
-```
-
-### Export company details into pandas data frame
-
-```python
-DataFrame1, DataFrame2, DataFrame3 = Company.get_info(option = 0)
-```
-### Plot certain attribute over selected years using matplotlib
-#### The plotter() function can be used to show the companies attribute from a certain document over the selected period of time using a line graph from the matplotlib library. The function accepts a single required arguement for the attribute selection. 
-
-```python
-company.plotter("certain file attribute of the document")
-```
-#### Usage example: 
-
-```python
-cmp = Extractor("TCS", years = 10, docs = ["ratios"])
-cmp.plotter("EV/EBITDA (X)")
-```
-output:
-
-![image](https://github.com/05kashyap/moneycontrol_financial-extractor/assets/120780494/f5be744e-e065-4b03-b6df-2ca7e765c4b2)
-
-### We can also plot the data of multiple companies on the same graph for comparison purposes
-```python
-company1 = Extractor("TCS", years = 10, docs = ["ratios"])
-company2 = Extractor("Infosys", years = 10, docs = ["ratios"])
-Extractor.cmp_plot(comp = [company1, company2], attributes = "EV/EBITDA (X)")
-```
-output:
-
-![image](https://github.com/05kashyap/mcfinance/assets/120780494/294f8313-2876-4751-9485-18517dccb0d3)
+Metadata-Version: 2.1
+Name: mcfinance
+Version: 0.1.8
+Summary: Money control financial data extractor-Requires python 3.7+
+Author: 05kashyap-ragha1992
+Author-email: <aryankashyapnaveen@gmail.com>
+Keywords: python,financial,extractor,data
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: bs4
+Requires-Dist: html5lib
+Requires-Dist: lxml
+Requires-Dist: matplotlib
+Requires-Dist: requests
+Requires-Dist: openpyxl
+Requires-Dist: PyQt5
+
+
+# mcfinance
+
+### Developed by 05kashyap and ragha1992
+### PyPI stats:
+[![Downloads](https://static.pepy.tech/badge/mcfinance)](https://pepy.tech/project/mcfinance)
+## Description:
+
+Extract financial data from the money control website using the company name, BSE or NSE number.
+Export any selected data into either pandas dataframe or excel sheet with ease!
+### .
+
+*Disclaimer*: We are in no way affiliated with moneycontrol.com
+ 
+## Usage:
+```python
+pip install mcfinance
+```
+### Initialise company details:
+#### Create an Extractor instance with company name/ BSE/ NSE ID (required) and/or number of years(default), required documents(default), and filepath to write documents(default current directory).
+
+```python
+from mcfinance import Extractor
+Company = Extractor(user_input= "Company_name")
+#years and docs are default
+Company = Extractor(user_input= "Company_name",years = 10, docs = ["balance sheet", "profit loss"], filepath = "/files")
+```
+any of the inputs can be changed later on as per user convenience
+```python
+Company.set_inputs(years = 6)
+```
+### Export company details as excel file (default)
+#### The get_info() function can be used to extract and store company data in an excel file. The file will be stored in the current filepath or the user defined filepath as per object initialisation 
+
+```python
+Company.get_info()
+```
+or
+```python
+Company.get_info(option = 1)
+```
+
+### Export company details into pandas data frame
+
+```python
+DataFrame1, DataFrame2, DataFrame3 = Company.get_info(option = 0)
+```
+### Plot certain attribute over selected years using matplotlib
+#### The plotter() function can be used to show the companies attribute from a certain document over the selected period of time using a line graph from the matplotlib library. The function accepts a single required arguement for the attribute selection. 
+
+```python
+company.plotter("certain file attribute of the document")
+```
+#### Usage example: 
+
+```python
+cmp = Extractor("TCS", years = 10, docs = ["ratios"])
+cmp.plotter("EV/EBITDA (X)")
+```
+output:
+
+![image](https://github.com/05kashyap/moneycontrol_financial-extractor/assets/120780494/f5be744e-e065-4b03-b6df-2ca7e765c4b2)
+
+### We can also plot the data of multiple companies on the same graph for comparison purposes
+```python
+company1 = Extractor("TCS", years = 10, docs = ["ratios"])
+company2 = Extractor("Infosys", years = 10, docs = ["ratios"])
+Extractor.cmp_plot(comp = [company1, company2], attributes = "EV/EBITDA (X)")
+```
+output:
+
+![image](https://github.com/05kashyap/mcfinance/assets/120780494/294f8313-2876-4751-9485-18517dccb0d3)
```

### Comparing `mcfinance-0.1.7/setup.py` & `mcfinance-0.1.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from setuptools import setup, find_packages
-import codecs
-import os
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
-    long_description = "\n" + fh.read()
-
-
-VERSION = "0.1.7"
-DESCRIPTION = "Money control financial data extractor-Requires python 3.7+"
-LONG_DESCRIPTION = long_description
-
-setup(name="mcfinance",
-      version=VERSION,
-      author="05kashyap-ragha1992",
-      author_email="<aryankashyapnaveen@gmail.com>",
-      description=DESCRIPTION,
-      long_description_content_type = "text/markdown",
-      long_description= LONG_DESCRIPTION,
-      packages=['mcfinance'],
-      package_dir={'mcfinance': 'src/mcfinance'},
-      package_data={'mcfinance': ['data/*.json']},
-      install_requires = ['pandas', 'bs4', 'html5lib', 'lxml','matplotlib','requests'],
-      keywords=['python','financial','extractor','data'],
-      classifiers=["Development Status :: 3 - Alpha",
-                   "Intended Audience :: Developers",
-                   "Programming Language :: Python :: 3.11",
-                   "Operating System :: Microsoft :: Windows",
-                   ]
+from setuptools import setup, find_packages
+import codecs
+import os
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
+    long_description = "\n" + fh.read()
+
+
+VERSION = "0.1.8"
+DESCRIPTION = "Money control financial data extractor-Requires python 3.7+"
+LONG_DESCRIPTION = long_description
+
+setup(name="mcfinance",
+      version=VERSION,
+      author="05kashyap-ragha1992",
+      author_email="<aryankashyapnaveen@gmail.com>",
+      description=DESCRIPTION,
+      long_description_content_type = "text/markdown",
+      long_description= LONG_DESCRIPTION,
+      packages=['mcfinance'],
+      package_dir={'mcfinance': 'src/mcfinance'},
+      package_data={'mcfinance': ['data/*.json']},
+      install_requires = ['pandas', 'bs4', 'html5lib', 'lxml','matplotlib','requests','openpyxl','PyQt5'],
+      keywords=['python','financial','extractor','data'],
+      classifiers=["Development Status :: 3 - Alpha",
+                   "Intended Audience :: Developers",
+                   "Programming Language :: Python :: 3.11",
+                   "Operating System :: Microsoft :: Windows",
+                   ]
       )
```

### Comparing `mcfinance-0.1.7/src/mcfinance/data/dictbse.json` & `mcfinance-0.1.8/src/mcfinance/data/dictbse.json`

 * *Files identical despite different names*

### Comparing `mcfinance-0.1.7/src/mcfinance/data/dictnse.json` & `mcfinance-0.1.8/src/mcfinance/data/dictnse.json`

 * *Files identical despite different names*

### Comparing `mcfinance-0.1.7/src/mcfinance/extractors.py` & `mcfinance-0.1.8/src/mcfinance/extractors.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-import pandas as pd
-import os,sys
-from cachetools import cached, TTLCache
-SCRIPT_DIR = os.path.dirname(os.path.abspath(__file__))
-sys.path.append(os.path.dirname(SCRIPT_DIR))
-from mcfinance import retrieval
-
-report_cache = TTLCache(maxsize=100, ttl=3600) 
-
-@cached(cache=report_cache)
-def prd(url, period, last, trm, a) -> pd.DataFrame:
-    '''Retrieve data for multiple years'''
-    if period > a or period//5 == trm:
-        df = retrieval.retinfo(url)
-        df.drop(df.columns[[0,len(df.columns)-1]], inplace = True, axis=1)
-        if(period == a+5 and last == 0):
-            return df
-        else:
-            df.drop(columns = df.columns[-last:], inplace = True, axis=1)
-        return df
-
-def search_gen(search_term, period) -> pd.DataFrame:
-    '''Handles retrieval of data and generation of urls'''
-    term = period%5
-    last = 5 - period
-    #generate datafrane from the search term
-    url = retrieval.urlfinder(search_term)
-    urls = []
-    urls = []
-    for i in range(2,5):
-        urlt = url + "/" + str(i) + "#" + url.split('/')[6]
-        urls.append(urlt)
-    #cleaning up the tables
-    df1 = retrieval.retinfo(url)
-    df1.drop(df1.columns[len(df1.columns)-1], inplace = True, axis = 1)
-    if(period == 5 and last == 0):
-        fdf = df1
-        return fdf
-    elif period < 5:
-        df1.drop(columns = df1.columns[-last:], inplace = True, axis=1)
-    fdf = df1
-    i=1
-    a = 5
-    for url in urls:
-        df = None
-        try:
-            df = prd(url, period, last, i, a)
-        except Exception as e:
-            print(e)
-            return fdf
-        fdf = pd.concat([fdf, df], join="inner", ignore_index=True, axis=1)
-        i+=1
-        a+=5
-    
-    fdf = fdf.drop(fdf.iloc[:, period+1:],axis = 1)
-
-    return fdf
-
-def plo(attribute, search_term, period):
-    print("plotting...")
-    df = search_gen(search_term, period)
-    col_names = df.loc[0, :].values.flatten().tolist()
-    X = col_names[1:]
-    X.reverse()
-    if(df[df.columns[0]] == attribute).any():
-        rows = df.loc[df[df.columns[0]] == attribute].squeeze().tolist()
-    else:
-        raise Exception("attribute does not exist in this file")
-        return
-    Y = rows[1:]
-    Y.reverse()
-    Y = [float(i) for i in Y]
+import pandas as pd
+import os,sys
+from cachetools import cached, TTLCache
+SCRIPT_DIR = os.path.dirname(os.path.abspath(__file__))
+sys.path.append(os.path.dirname(SCRIPT_DIR))
+from mcfinance import retrieval
+
+report_cache = TTLCache(maxsize=100, ttl=3600) 
+
+@cached(cache=report_cache)
+def prd(url, period, last, trm, a) -> pd.DataFrame:
+    '''Retrieve data for multiple years'''
+    if period > a or period//5 == trm:
+        df = retrieval.retinfo(url)
+        df.drop(df.columns[[0,len(df.columns)-1]], inplace = True, axis=1)
+        if(period == a+5 and last == 0):
+            return df
+        else:
+            df.drop(columns = df.columns[-last:], inplace = True, axis=1)
+        return df
+
+def search_gen(search_term, period) -> pd.DataFrame:
+    '''Handles retrieval of data and generation of urls'''
+    term = period%5
+    last = 5 - period
+    #generate datafrane from the search term
+    url = retrieval.urlfinder(search_term)
+    urls = []
+    for i in range(2,5):
+        urlt = url + "/" + str(i) + "#" + url.split('/')[6]
+        urls.append(urlt)
+    #cleaning up the tables
+    df1 = retrieval.retinfo(url)
+    df1.drop(df1.columns[len(df1.columns)-1], inplace = True, axis = 1)
+    if(period == 5 and last == 0):
+        fdf = df1
+        return fdf
+    elif period < 5:
+        df1.drop(columns = df1.columns[-last:], inplace = True, axis=1)
+    fdf = df1
+    i=1
+    a = 5
+    for url in urls:
+        df = None
+        try:
+            df = prd(url, period, last, i, a)
+        except Exception as e:
+            print(e)
+            return fdf
+        fdf = pd.concat([fdf, df], join="inner", ignore_index=True, axis=1)
+        i+=1
+        a+=5
+    
+    fdf = fdf.drop(fdf.iloc[:, period+1:],axis = 1)
+    
+    return fdf
+
+def plo(attribute, search_term, period):
+    print("plotting...")
+    df = search_gen(search_term, period)
+    col_names = df.loc[0, :].values.flatten().tolist()
+    print(col_names)
+    X = col_names[1:]
+    X.reverse()
+    if(df[df.columns[0]] == attribute).any():
+        rows = df.loc[df[df.columns[0]] == attribute].squeeze().tolist()
+    else:
+        raise Exception("attribute does not exist in this file")
+        return
+    Y = rows[1:]
+    Y.reverse()
+    Y = [float(i) for i in Y]
     return X,Y
```

### Comparing `mcfinance-0.1.7/src/mcfinance/retrieval.py` & `mcfinance-0.1.8/src/mcfinance/retrieval.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,74 @@
-from cachetools import cached, TTLCache
-from bs4 import BeautifulSoup
-import requests
-import time
-import pandas as pd
-import json
-import importlib.resources
-
-url_cache = TTLCache(maxsize=100, ttl=3600) 
-
-def pr_request(url, proxies):
-    for proxy in proxies:
-        try:
-            page = requests.get(
-            url, proxies={"http": proxy, "https": proxy})
-    
-            # Prints Proxy server IP address if proxy is alive.
-            print("Status OK, Output:", page.text)
-    
-        except OSError as e:
-            # Proxy returns Connection error
-            print(e)    
-
-@cached(cache=url_cache)
-def urlfinder(search_term):
-    '''Find google search results'''
-    results = 5
-    
-    page = requests.get(f"http://www.google.com/search?q={search_term}&num={results}")
-    while(page.status_code == 429):
-        time.sleep(5)
-        page = requests.get(f"http://www.google.com/search?q={search_term}&num={results}")
-        if(page.status_code ==200):
-            break
-
-    soup1 = BeautifulSoup(page.content, "html5lib")
-    links = soup1.findAll("a")
-    for link in links :
-        link_href = link.get('href')
-        if "url?q=" in link_href and not "webcache" in link_href:
-            link_g = link.get('href').split("?q=")[1].split("&sa=U")[0]
-            return link_g
-        
-def retinfo(url) -> pd.DataFrame:
-    '''Extract tables from a url'''
-    new_url = url.replace("https", "http")
-    url = requests.get(new_url)
-    dfs = None
-    
-    try:
-        dfs = pd.read_html(url.text)
-    
-    except(ValueError):
-        return pd.DataFrame()
-    
-    df = dfs[0]
-    return df
-
-def comp_name(ticker):
-   
-    if isinstance(ticker, int):
-        ticker = str(ticker)
-    if ticker.isnumeric() and len(ticker) == 6:
-        with importlib.resources.open_text("mcfinance.data", "dictbse.json") as f:
-            dictbse = json.load(f)
-        return dictbse[ticker]
-    elif ticker.isupper():
-        with importlib.resources.open_text("mcfinance.data", "dictnse.json") as f:
-            dictnse = json.load(f)
-        return dictnse[ticker]        
-    else:
+from cachetools import cached, TTLCache
+from bs4 import BeautifulSoup
+from io import StringIO
+import requests
+import time
+import pandas as pd
+import json
+import importlib.resources
+
+url_cache = TTLCache(maxsize=100, ttl=3600) 
+
+def pr_request(url, proxies):
+    for proxy in proxies:
+        try:
+            page = requests.get(
+            url, proxies={"http": proxy, "https": proxy})
+    
+            # Prints Proxy server IP address if proxy is alive.
+            print("Status OK, Output:", page.text)
+    
+        except OSError as e:
+            # Proxy returns Connection error
+            print(e)    
+
+@cached(cache=url_cache)
+def urlfinder(search_term):
+    '''Find google search results'''
+    results = 5
+    
+    page = requests.get(f"http://www.google.com/search?q={search_term}&num={results}")
+    while(page.status_code == 429):
+        time.sleep(5)
+        page = requests.get(f"http://www.google.com/search?q={search_term}&num={results}")
+        if(page.status_code ==200):
+            break
+
+    soup1 = BeautifulSoup(page.content, "html5lib")
+    links = soup1.findAll("a")
+    for link in links :
+        link_href = link.get('href')
+        if "moneycontrol.com" in link_href and "url?q=" in link_href and not "webcache" in link_href:
+            link_g = link.get('href').split("?q=")[1].split("&sa=U")[0]
+            return link_g
+        
+def retinfo(url) -> pd.DataFrame:
+    '''Extract tables from a url'''
+    new_url = url.replace("https", "http")
+    url = requests.get(new_url)
+    dfs = None
+    
+    try:
+        html_string = StringIO(url.text)
+        dfs = pd.read_html(html_string)
+    
+    except(ValueError):
+        return pd.DataFrame()
+    
+    df = dfs[0]
+    return df
+
+def comp_name(ticker):
+   
+    if isinstance(ticker, int):
+        ticker = str(ticker)
+    if ticker.isnumeric() and len(ticker) == 6:
+        with importlib.resources.open_text("mcfinance.data", "dictbse.json") as f:
+            dictbse = json.load(f)
+        return dictbse[ticker]
+    elif ticker.isupper() and ' ' not in ticker:
+        with importlib.resources.open_text("mcfinance.data", "dictnse.json") as f:
+            dictnse = json.load(f)
+        return dictnse[ticker]        
+    else:
         return ticker
```

