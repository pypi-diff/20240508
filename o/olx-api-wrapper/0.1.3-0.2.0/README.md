# Comparing `tmp/olx-api-wrapper-0.1.3.tar.gz` & `tmp/olx-api-wrapper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olx-api-wrapper-0.1.3.tar", last modified: Tue May  7 14:05:19 2024, max compression
+gzip compressed data, was "olx-api-wrapper-0.2.0.tar", last modified: Wed May  8 15:49:30 2024, max compression
```

## Comparing `olx-api-wrapper-0.1.3.tar` & `olx-api-wrapper-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:05:19.962384 olx-api-wrapper-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-07 14:05:12.000000 olx-api-wrapper-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-05-07 14:05:19.958384 olx-api-wrapper-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9802 2024-05-07 14:05:12.000000 olx-api-wrapper-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:05:19.958384 olx-api-wrapper-0.1.3/olx/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-07 14:05:12.000000 olx-api-wrapper-0.1.3/olx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-07 14:05:12.000000 olx-api-wrapper-0.1.3/olx/advert_logo.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-07 14:05:12.000000 olx-api-wrapper-0.1.3/olx/advert_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-07 14:05:12.000000 olx-api-wrapper-0.1.3/olx/adverts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-07 14:05:12.000000 olx-api-wrapper-0.1.3/olx/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-07 14:05:12.000000 olx-api-wrapper-0.1.3/olx/categories_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-07 14:05:12.000000 olx-api-wrapper-0.1.3/olx/cities_districts.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-07 14:05:12.000000 olx-api-wrapper-0.1.3/olx/languages_currencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-07 14:05:12.000000 olx-api-wrapper-0.1.3/olx/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-05-07 14:05:12.000000 olx-api-wrapper-0.1.3/olx/olx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-07 14:05:12.000000 olx-api-wrapper-0.1.3/olx/paid_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-07 14:05:12.000000 olx-api-wrapper-0.1.3/olx/payments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-07 14:05:12.000000 olx-api-wrapper-0.1.3/olx/threads_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-07 14:05:12.000000 olx-api-wrapper-0.1.3/olx/user_business.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-07 14:05:12.000000 olx-api-wrapper-0.1.3/olx/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:05:19.958384 olx-api-wrapper-0.1.3/olx_api_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-05-07 14:05:19.000000 olx-api-wrapper-0.1.3/olx_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-07 14:05:19.000000 olx-api-wrapper-0.1.3/olx_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:05:19.000000 olx-api-wrapper-0.1.3/olx_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 14:05:19.000000 olx-api-wrapper-0.1.3/olx_api_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 14:05:19.000000 olx-api-wrapper-0.1.3/olx_api_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:05:19.962384 olx-api-wrapper-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-07 14:05:12.000000 olx-api-wrapper-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:49:30.476382 olx-api-wrapper-0.2.0/
+-rw-rw-rw-   0        0        0     1071 2024-05-06 17:28:53.000000 olx-api-wrapper-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0    10641 2024-05-08 15:49:30.476382 olx-api-wrapper-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10127 2024-05-08 15:39:31.000000 olx-api-wrapper-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 15:49:30.457783 olx-api-wrapper-0.2.0/olx/
+-rw-rw-rw-   0        0        0      192 2024-05-08 15:42:17.000000 olx-api-wrapper-0.2.0/olx/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-06 13:04:48.000000 olx-api-wrapper-0.2.0/olx/packets.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:49:30.475381 olx-api-wrapper-0.2.0/olx_api_wrapper.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-06 19:26:10.000000 olx-api-wrapper-0.2.0/olx_api_wrapper.egg-info/.gitignore
+-rw-rw-rw-   0        0        0    10641 2024-05-08 15:49:30.000000 olx-api-wrapper-0.2.0/olx_api_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2024-05-08 15:49:30.000000 olx-api-wrapper-0.2.0/olx_api_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 15:49:30.000000 olx-api-wrapper-0.2.0/olx_api_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-08 15:49:30.000000 olx-api-wrapper-0.2.0/olx_api_wrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-08 15:49:30.000000 olx-api-wrapper-0.2.0/olx_api_wrapper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 15:49:30.476382 olx-api-wrapper-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      769 2024-05-08 15:42:11.000000 olx-api-wrapper-0.2.0/setup.py
```

### Comparing `olx-api-wrapper-0.1.3/LICENSE` & `olx-api-wrapper-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2024 Paweł Stawikowski
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright 2024 Paweł Stawikowski
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `olx-api-wrapper-0.1.3/PKG-INFO` & `olx-api-wrapper-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,268 +1,268 @@
-Metadata-Version: 2.1
-Name: olx-api-wrapper
-Version: 0.1.3
-Summary: Unofficial Wrapper for OLX API
-Home-page: https://github.com/Pawikoski/olx-api-wrapper
-Author: Paweł Stawikowski
-Author-email: pawikoski@gmail.com
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
-<a name="readme-top"></a>
-<!--
-*** Thanks for checking out the Best-README-Template. If you have a suggestion
-*** that would make this better, please fork the repo and create a pull request
-*** or simply open an issue with the tag "enhancement".
-*** Don't forget to give the project a star!
-*** Thanks again! Now go create something AMAZING! :D
--->
-
-
-
-<!-- PROJECT SHIELDS -->
-<!--
-*** I'm using markdown "reference style" links for readability.
-*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
-*** See the bottom of this document for the declaration of the reference variables
-*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
-*** https://www.markdownguide.org/basic-syntax/#reference-style-links
--->
-[![Contributors][contributors-shield]][contributors-url]
-[![Forks][forks-shield]][forks-url]
-[![Stargazers][stars-shield]][stars-url]
-[![Issues][issues-shield]][issues-url]
-[![MIT License][license-shield]][license-url]
-[![LinkedIn][linkedin-shield]][linkedin-url]
-
-
-
-<!-- PROJECT LOGO -->
-<br />
-<div align="center">
-  <a href="https://github.com/Pawikoski/olx-api-wrapper">
-    <img src="images/image.png" alt="Logo" height="80">
-  </a>
-
-<h3 align="center">OLX Api Wrapper</h3>
-
-  <p align="center">
-    Simple client for OLX Developer API written in Python
-    <br />
-    <a href="https://github.com/Pawikoski/olx-api-wrapper"><strong>Explore the docs »</strong></a>
-    <br />
-    <br />
-    <a href="https://github.com/Pawikoski/olx-api-wrapper">View Demo</a>
-    ·
-    <a href="https://github.com/Pawikoski/olx-api-wrapper/issues/new?labels=bug&template=bug-report---.md">Report Bug</a>
-    ·
-    <a href="https://github.com/Pawikoski/olx-api-wrapper/issues/new?labels=enhancement&template=feature-request---.md">Request Feature</a>
-  </p>
-</div>
-
-
-
-<!-- TABLE OF CONTENTS -->
-<details>
-  <summary>Table of Contents</summary>
-  <ol>
-    <li>
-      <a href="#about-the-project">About The Project</a>
-      <ul>
-        <li><a href="#built-with">Built With</a></li>
-      </ul>
-    </li>
-    <li>
-      <a href="#getting-started">Getting Started</a>
-      <ul>
-        <li><a href="#prerequisites">Prerequisites</a></li>
-        <li><a href="#installation">Installation</a></li>
-      </ul>
-    </li>
-    <li><a href="#usage">Usage</a></li>
-    <li><a href="#roadmap">Roadmap</a></li>
-    <li><a href="#contributing">Contributing</a></li>
-    <li><a href="#license">License</a></li>
-    <li><a href="#contact">Contact</a></li>
-    <li><a href="#acknowledgments">Acknowledgments</a></li>
-  </ol>
-</details>
-
-
-
-<!-- ABOUT THE PROJECT -->
-## About The Project
-
-OLX API Wrapper: Easy Solution for Working with OLX. With this Python library you can quickly fetch user data, handle adverts with simple CRUD operations, and seamlessly integrate with the OLX API. Simplify your development process and focus on building your app hassle-free.
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-### Built With
-
-* [![Python][Python]][Python-url]
-* [![requests][requests]][requests-url]
-* [![dacite][dacite]][dacite-url]
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-<!-- GETTING STARTED -->
-## Getting Started
-
-In order to use OLX Api you nned to sign in at OLX Developer Portal and create an App.
-More details: https://developer.olx.pl/articles/getting-access-to-api
-
-### Prerequisites
-
-To use this API Wrapper you need to copy Client ID and Client Secret. Store them in the safe place. In your code you can use them as enviroment variables, they sholdn't be hardcoded.
-You can perform actions with API on:
-- OLX PL
-- OLX BG
-- OLX RO
-- OLX PT
-- OLX UA
-- OLX KZ
-  
-By default, all requests are sent to olx.**PL**. To change it you must pass `country_code` argument to every child of Olx class, i.e.:
-```python
-olx.Auth(country_code="bg")
-olx.Adverts(country_code="ro")
-olx.Users(country_code="pt")
-olx.CitiesDistricts(country_code="ua")
-olx.AdvertsStatistics(country_code="kz")
-# etc...
-```
-
-### Installation
-
-1. Install `olx-api-wrapper` package
-   ```sh
-   pip install olx-api-wrapper
-   ```
-2. In order to get access token you need to authenticate with authorization code. [How to get authorization code?](https://developer.olx.pl/api/doc#section/Authentication/Grant-type:-authorization_code)
-   ```python
-   from olx import Auth
-   auth = Auth(
-     client_id="your_client_id",
-     client_secret="your_client_secret",
-   )
-   auth.authenticate(code='authorization_code')
-   access_token = auth.access_token
-   ```
-3. Now you have access token which you will need to have an access to OLX API resources.
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-<!-- USAGE EXAMPLES -->
-## Usage
-
-Using `olx-api-wrapper` in Your Project
-
-Below are examples demonstrating the usage of `olx-api-wrapper` in your project. Please note that you require an access token to execute the actions described below.
-
-Each section from the OLX API documentation corresponds to a separate object within `olx-api-wrapper`. For instance, the section Users in the documentation is represented as olx.Users. Additionally, each endpoint mentioned in the documentation corresponds to a single method. For example, the 'Get user' endpoint becomes the method `olx.Users().get_user(user_id)`.
-
-If a method returns a value, it will be in the form of a dataclass object. This facilitates ease of use and clarity due to type hints. You can access values as properties, for example, `user_values.email`.
-
-This structure provides a convenient and straightforward approach to integrating `olx-api-wrapper` into your project.
-
-=====================================
-
-First of all you need to assign an object you want to use to variable and then use available method of this object. You must to pass `access_token` to every single object.
-
-Prerequisites: Import olx module.
-```python
-import olx
-```
-
-- Show authenticated user info
-  ```python
-  users = olx.Users(access_token='your_access_token')
-  user_info = users.get_authenticated_user()
-  # AuthenticatedUser(id=123, email='john@mail.com', status='confirmed', name='Paweł', phone='123123123', phone_login=None, created_at='2018-01-29 19:48:49', last_login_at='2024-04-26 17:20:48', avatar=None, is_business=True)
-  
-  user_email = user_info.email
-  # john@mail.com
-  ```
-- Get category suggestions for provided ad title
-  ```python
-  categories_and_attributes = olx.CategoriesAttributes(access_token='your_access_token')
-  suggestions = categories_and_attributes.get_category_suggestions(ad_title='Honda Hornet')
-  # [CategorySuggestion(id='1379', name='Szosowo - Turystyczny', path=[CategoryPath(id='5', name='Motoryzacja'), CategoryPath(id='81', name='Motocykle i Skutery')])]
-  ```
-
-<!-- TODO: _For more examples, please refer to the [Documentation](https://example.com)_ -->
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-<!-- CONTRIBUTING -->
-## Contributing
-
-Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
-
-If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
-Don't forget to give the project a star! Thanks again!
-
-1. Fork the Project
-2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
-3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
-4. Push to the Branch (`git push origin feature/AmazingFeature`)
-5. Open a Pull Request
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-<!-- LICENSE -->
-## License
-
-Distributed under the MIT License. See `LICENSE` for more information.
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-<!-- CONTACT -->
-## Contact
-
-Paweł Stawikowski - pawikoski@gmail.com
-
-Project Link: [https://github.com/Pawikoski/olx-api-wrapper](https://github.com/Pawikoski/olx-api-wrapper)
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-
-<!-- MARKDOWN LINKS & IMAGES -->
-<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
-[contributors-shield]: https://img.shields.io/github/contributors/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
-[contributors-url]: https://github.com/Pawikoski/olx-api-wrapper/graphs/contributors
-[forks-shield]: https://img.shields.io/github/forks/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
-[forks-url]: https://github.com/Pawikoski/olx-api-wrapper/network/members
-[stars-shield]: https://img.shields.io/github/stars/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
-[stars-url]: https://github.com/Pawikoski/olx-api-wrapper/stargazers
-[issues-shield]: https://img.shields.io/github/issues/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
-[issues-url]: https://github.com/Pawikoski/olx-api-wrapper/issues
-[license-shield]: https://img.shields.io/github/license/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
-[license-url]: https://github.com/Pawikoski/olx-api-wrapper/blob/master/LICENSE
-[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
-[linkedin-url]: https://linkedin.com/in/paweł-stawikowski
-[product-image]: images/image.png
-[Python]: https://img.shields.io/badge/python-000000?style=for-the-badge&logo=python&logoColor=white
-[Python-url]: https://python.org/
-[dacite]: https://img.shields.io/badge/dacite-20232A?style=for-the-badge&logo=github&logoColor=61DAFB
-[dacite-url]: https://github.com/konradhalas/dacite
-[requests]: https://img.shields.io/badge/requests-35495E?style=for-the-badge&logo=github&logoColor=4FC08D
-[requests-url]: https://github.com/psf/requests
+Metadata-Version: 2.1
+Name: olx-api-wrapper
+Version: 0.2.0
+Summary: Unofficial Wrapper for OLX API
+Home-page: https://github.com/Pawikoski/olx-api-wrapper
+Author: Paweł Stawikowski
+Author-email: pawikoski@gmail.com
+License: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
+<a name="readme-top"></a>
+<!--
+*** Thanks for checking out the Best-README-Template. If you have a suggestion
+*** that would make this better, please fork the repo and create a pull request
+*** or simply open an issue with the tag "enhancement".
+*** Don't forget to give the project a star!
+*** Thanks again! Now go create something AMAZING! :D
+-->
+
+
+
+<!-- PROJECT SHIELDS -->
+<!--
+*** I'm using markdown "reference style" links for readability.
+*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
+*** See the bottom of this document for the declaration of the reference variables
+*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
+*** https://www.markdownguide.org/basic-syntax/#reference-style-links
+-->
+[![Contributors][contributors-shield]][contributors-url]
+[![Forks][forks-shield]][forks-url]
+[![Stargazers][stars-shield]][stars-url]
+[![Issues][issues-shield]][issues-url]
+[![MIT License][license-shield]][license-url]
+[![LinkedIn][linkedin-shield]][linkedin-url]
+
+
+
+<!-- PROJECT LOGO -->
+<br />
+<div align="center">
+  <a href="https://github.com/Pawikoski/olx-api-wrapper">
+    <img src="images/image.png" alt="Logo" height="80">
+  </a>
+
+<h3 align="center">OLX Api Wrapper</h3>
+
+  <p align="center">
+    Simple client for OLX Developer API written in Python
+    <br />
+    <a href="https://github.com/Pawikoski/olx-api-wrapper"><strong>Explore the docs Â»</strong></a>
+    <br />
+    <br />
+    <a href="https://github.com/Pawikoski/olx-api-wrapper">View Demo</a>
+    Â·
+    <a href="https://github.com/Pawikoski/olx-api-wrapper/issues/new?labels=bug&template=bug-report---.md">Report Bug</a>
+    Â·
+    <a href="https://github.com/Pawikoski/olx-api-wrapper/issues/new?labels=enhancement&template=feature-request---.md">Request Feature</a>
+  </p>
+</div>
+
+
+
+<!-- TABLE OF CONTENTS -->
+<details>
+  <summary>Table of Contents</summary>
+  <ol>
+    <li>
+      <a href="#about-the-project">About The Project</a>
+      <ul>
+        <li><a href="#built-with">Built With</a></li>
+      </ul>
+    </li>
+    <li>
+      <a href="#getting-started">Getting Started</a>
+      <ul>
+        <li><a href="#prerequisites">Prerequisites</a></li>
+        <li><a href="#installation">Installation</a></li>
+      </ul>
+    </li>
+    <li><a href="#usage">Usage</a></li>
+    <li><a href="#roadmap">Roadmap</a></li>
+    <li><a href="#contributing">Contributing</a></li>
+    <li><a href="#license">License</a></li>
+    <li><a href="#contact">Contact</a></li>
+    <li><a href="#acknowledgments">Acknowledgments</a></li>
+  </ol>
+</details>
+
+
+
+<!-- ABOUT THE PROJECT -->
+## About The Project
+
+OLX API Wrapper: Easy Solution for Working with OLX. With this Python library you can quickly fetch user data, handle adverts with simple CRUD operations, and seamlessly integrate with the OLX API. Simplify your development process and focus on building your app hassle-free.
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+
+### Built With
+
+* [![Python][Python]][Python-url]
+* [![requests][requests]][requests-url]
+* [![dacite][dacite]][dacite-url]
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+
+<!-- GETTING STARTED -->
+## Getting Started
+
+In order to use OLX Api you nned to sign in at OLX Developer Portal and create an App.
+More details: https://developer.olx.pl/articles/getting-access-to-api
+
+### Prerequisites
+
+To use this API Wrapper you need to copy Client ID and Client Secret. Store them in the safe place. In your code you can use them as enviroment variables, they sholdn't be hardcoded.
+You can perform actions with API on:
+- OLX PL
+- OLX BG
+- OLX RO
+- OLX PT
+- OLX UA
+- OLX KZ
+  
+By default, all requests are sent to olx.**PL**. To change it you must pass `country_code` argument to every child of Olx class, i.e.:
+```python
+olx.partner.Auth(country_code="bg")
+olx.partner.Adverts(country_code="ro")
+olx.partner.Users(country_code="pt")
+olx.partner.CitiesDistricts(country_code="ua")
+olx.partner.AdvertsStatistics(country_code="kz")
+# etc...
+```
+
+### Installation
+
+1. Install `olx-api-wrapper` package
+   ```sh
+   pip install olx-api-wrapper
+   ```
+2. In order to get access token you need to authenticate with authorization code. [How to get authorization code?](https://developer.olx.pl/api/doc#section/Authentication/Grant-type:-authorization_code)
+   ```python
+   from olx.partner import Auth
+   auth = Auth(
+     client_id="your_client_id",
+     client_secret="your_client_secret",
+   )
+   auth.authenticate(code='authorization_code')
+   access_token = auth.access_token
+   ```
+3. Now you have access token which you will need to have an access to OLX API resources.
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+
+<!-- USAGE EXAMPLES -->
+## Usage
+
+Using `olx-api-wrapper` in Your Project
+
+Below are examples demonstrating the usage of `olx-api-wrapper` in your project. Please note that you require an access token to execute the actions described below.
+
+Each section from the OLX API documentation corresponds to a separate object within `olx-api-wrapper`. For instance, the section Users in the documentation is represented as olx.Users. Additionally, each endpoint mentioned in the documentation corresponds to a single method. For example, the 'Get user' endpoint becomes the method `olx.partner.Users().get_user(user_id)`.
+
+If a method returns a value, it will be in the form of a dataclass object. This facilitates ease of use and clarity due to type hints. You can access values as properties, for example, `user_values.email`.
+
+This structure provides a convenient and straightforward approach to integrating `olx-api-wrapper` into your project.
+
+=====================================
+
+First of all you need to assign an object you want to use to variable and then use available method of this object. You must to pass `access_token` to every single object.
+
+Prerequisites: Import olx module.
+```python
+import olx
+```
+
+- Show authenticated user info
+  ```python
+  users = olx.partner.Users(access_token='your_access_token')
+  user_info = users.get_authenticated_user()
+  # AuthenticatedUser(id=123, email='john@mail.com', status='confirmed', name='PaweĹ‚', phone='123123123', phone_login=None, created_at='2018-01-29 19:48:49', last_login_at='2024-04-26 17:20:48', avatar=None, is_business=True)
+  
+  user_email = user_info.email
+  # john@mail.com
+  ```
+- Get category suggestions for provided ad title
+  ```python
+  categories_and_attributes = olx.partner.CategoriesAttributes(access_token='your_access_token')
+  suggestions = categories_and_attributes.get_category_suggestions(ad_title='Honda Hornet')
+  # [CategorySuggestion(id='1379', name='Szosowo - Turystyczny', path=[CategoryPath(id='5', name='Motoryzacja'), CategoryPath(id='81', name='Motocykle i Skutery')])]
+  ```
+
+<!-- TODO: _For more examples, please refer to the [Documentation](https://example.com)_ -->
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+<!-- CONTRIBUTING -->
+## Contributing
+
+Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
+
+If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
+Don't forget to give the project a star! Thanks again!
+
+1. Fork the Project
+2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
+3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
+4. Push to the Branch (`git push origin feature/AmazingFeature`)
+5. Open a Pull Request
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+
+<!-- LICENSE -->
+## License
+
+Distributed under the MIT License. See `LICENSE` for more information.
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+
+<!-- CONTACT -->
+## Contact
+
+PaweĹ‚ Stawikowski - pawikoski@gmail.com
+
+Project Link: [https://github.com/Pawikoski/olx-api-wrapper](https://github.com/Pawikoski/olx-api-wrapper)
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+
+
+<!-- MARKDOWN LINKS & IMAGES -->
+<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
+[contributors-shield]: https://img.shields.io/github/contributors/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
+[contributors-url]: https://github.com/Pawikoski/olx-api-wrapper/graphs/contributors
+[forks-shield]: https://img.shields.io/github/forks/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
+[forks-url]: https://github.com/Pawikoski/olx-api-wrapper/network/members
+[stars-shield]: https://img.shields.io/github/stars/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
+[stars-url]: https://github.com/Pawikoski/olx-api-wrapper/stargazers
+[issues-shield]: https://img.shields.io/github/issues/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
+[issues-url]: https://github.com/Pawikoski/olx-api-wrapper/issues
+[license-shield]: https://img.shields.io/github/license/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
+[license-url]: https://github.com/Pawikoski/olx-api-wrapper/blob/master/LICENSE
+[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
+[linkedin-url]: https://linkedin.com/in/paweĹ‚-stawikowski
+[product-image]: images/image.png
+[Python]: https://img.shields.io/badge/python-000000?style=for-the-badge&logo=python&logoColor=white
+[Python-url]: https://python.org/
+[dacite]: https://img.shields.io/badge/dacite-20232A?style=for-the-badge&logo=github&logoColor=61DAFB
+[dacite-url]: https://github.com/konradhalas/dacite
+[requests]: https://img.shields.io/badge/requests-35495E?style=for-the-badge&logo=github&logoColor=4FC08D
+[requests-url]: https://github.com/psf/requests
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.1.3 Summary: Unofficial
+Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.2.0 Summary: Unofficial
 Wrapper for OLX API Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: PaweÅ Stawikowski Author-email: pawikoski@gmail.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
 [Issues][issues-shield]][issues-url] [![MIT License][license-shield]][license-
 url] [![LinkedIn][linkedin-shield]][linkedin-url]
                                     _[_L_o_g_o_]
                            ******** OOLLXX AAppii WWrraappppeerr ********
             Simple client for OLX Developer API written in Python
-                             _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
+                            _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Ã_?_?Â_?»
 
-                  _V_i_e_w_ _D_e_m_o Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
+                _V_i_e_w_ _D_e_m_o ÃÂ· _R_e_p_o_r_t_ _B_u_g ÃÂ· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _B_u_i_l_t_ _W_i_t_h
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
           o _P_r_e_r_e_q_u_i_s_i_t_e_s
           o _I_n_s_t_a_l_l_a_t_i_o_n
    3. _U_s_a_g_e
@@ -37,49 +37,50 @@
 ## Getting Started In order to use OLX Api you nned to sign in at OLX Developer
 Portal and create an App. More details: https://developer.olx.pl/articles/
 getting-access-to-api ### Prerequisites To use this API Wrapper you need to
 copy Client ID and Client Secret. Store them in the safe place. In your code
 you can use them as enviroment variables, they sholdn't be hardcoded. You can
 perform actions with API on: - OLX PL - OLX BG - OLX RO - OLX PT - OLX UA - OLX
 KZ By default, all requests are sent to olx.**PL**. To change it you must pass
-`country_code` argument to every child of Olx class, i.e.: ```python olx.Auth
-(country_code="bg") olx.Adverts(country_code="ro") olx.Users(country_code="pt")
-olx.CitiesDistricts(country_code="ua") olx.AdvertsStatistics(country_code="kz")
-# etc... ``` ### Installation 1. Install `olx-api-wrapper` package ```sh pip
-install olx-api-wrapper ``` 2. In order to get access token you need to
-authenticate with authorization code. [How to get authorization code?](https://
+`country_code` argument to every child of Olx class, i.e.: ```python
+olx.partner.Auth(country_code="bg") olx.partner.Adverts(country_code="ro")
+olx.partner.Users(country_code="pt") olx.partner.CitiesDistricts
+(country_code="ua") olx.partner.AdvertsStatistics(country_code="kz") # etc...
+``` ### Installation 1. Install `olx-api-wrapper` package ```sh pip install
+olx-api-wrapper ``` 2. In order to get access token you need to authenticate
+with authorization code. [How to get authorization code?](https://
 developer.olx.pl/api/doc#section/Authentication/Grant-type:-authorization_code)
-```python from olx import Auth auth = Auth( client_id="your_client_id",
+```python from olx.partner import Auth auth = Auth( client_id="your_client_id",
 client_secret="your_client_secret", ) auth.authenticate
 (code='authorization_code') access_token = auth.access_token ``` 3. Now you
 have access token which you will need to have an access to OLX API resources.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Usage Using `olx-api-wrapper` in Your Project Below are examples
 demonstrating the usage of `olx-api-wrapper` in your project. Please note that
 you require an access token to execute the actions described below. Each
 section from the OLX API documentation corresponds to a separate object within
 `olx-api-wrapper`. For instance, the section Users in the documentation is
 represented as olx.Users. Additionally, each endpoint mentioned in the
 documentation corresponds to a single method. For example, the 'Get user'
-endpoint becomes the method `olx.Users().get_user(user_id)`. If a method
-returns a value, it will be in the form of a dataclass object. This facilitates
-ease of use and clarity due to type hints. You can access values as properties,
-for example, `user_values.email`. This structure provides a convenient and
-straightforward approach to integrating `olx-api-wrapper` into your project.
-===================================== First of all you need to assign an object
-you want to use to variable and then use available method of this object. You
-must to pass `access_token` to every single object. Prerequisites: Import olx
-module. ```python import olx ``` - Show authenticated user info ```python users
-= olx.Users(access_token='your_access_token') user_info =
-users.get_authenticated_user() # AuthenticatedUser(id=123,
-email='john@mail.com', status='confirmed', name='PaweÅ', phone='123123123',
+endpoint becomes the method `olx.partner.Users().get_user(user_id)`. If a
+method returns a value, it will be in the form of a dataclass object. This
+facilitates ease of use and clarity due to type hints. You can access values as
+properties, for example, `user_values.email`. This structure provides a
+convenient and straightforward approach to integrating `olx-api-wrapper` into
+your project. ===================================== First of all you need to
+assign an object you want to use to variable and then use available method of
+this object. You must to pass `access_token` to every single object.
+Prerequisites: Import olx module. ```python import olx ``` - Show authenticated
+user info ```python users = olx.partner.Users(access_token='your_access_token')
+user_info = users.get_authenticated_user() # AuthenticatedUser(id=123,
+email='john@mail.com', status='confirmed', name='PaweÄ¹â', phone='123123123',
 phone_login=None, created_at='2018-01-29 19:48:49', last_login_at='2024-04-26
 17:20:48', avatar=None, is_business=True) user_email = user_info.email #
 john@mail.com ``` - Get category suggestions for provided ad title ```python
-categories_and_attributes = olx.CategoriesAttributes
+categories_and_attributes = olx.partner.CategoriesAttributes
 (access_token='your_access_token') suggestions =
 categories_and_attributes.get_category_suggestions(ad_title='Honda Hornet') #
 [CategorySuggestion(id='1379', name='Szosowo - Turystyczny', path=[CategoryPath
 (id='5', name='Motoryzacja'), CategoryPath(id='81', name='Motocykle i
 Skutery')])] ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contributing Contributions are what make the open source community such an
@@ -91,15 +92,15 @@
 -b feature/AmazingFeature`) 3. Commit your Changes (`git commit -m 'Add some
 AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
 AmazingFeature`) 5. Open a Pull Request
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## License Distributed under the MIT License. See `LICENSE` for more
 information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Contact PaweÅ Stawikowski - pawikoski@gmail.com Project Link: [https://
+## Contact PaweÄ¹â Stawikowski - pawikoski@gmail.com Project Link: [https://
 github.com/Pawikoski/olx-api-wrapper](https://github.com/Pawikoski/olx-api-
 wrapper)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/Pawikoski/
 olx-api-wrapper.svg?style=for-the-badge [contributors-url]: https://github.com/
 Pawikoski/olx-api-wrapper/graphs/contributors [forks-shield]: https://
 img.shields.io/github/forks/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
@@ -109,15 +110,15 @@
 api-wrapper/stargazers [issues-shield]: https://img.shields.io/github/issues/
 Pawikoski/olx-api-wrapper.svg?style=for-the-badge [issues-url]: https://
 github.com/Pawikoski/olx-api-wrapper/issues [license-shield]: https://
 img.shields.io/github/license/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
 [license-url]: https://github.com/Pawikoski/olx-api-wrapper/blob/master/LICENSE
 [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-
 the-badge&logo=linkedin&colorB=555 [linkedin-url]: https://linkedin.com/in/
-paweÅ-stawikowski [product-image]: images/image.png [Python]: https://
+paweÄ¹â-stawikowski [product-image]: images/image.png [Python]: https://
 img.shields.io/badge/python-000000?style=for-the-
 badge&logo=python&logoColor=white [Python-url]: https://python.org/ [dacite]:
 https://img.shields.io/badge/dacite-20232A?style=for-the-
 badge&logo=github&logoColor=61DAFB [dacite-url]: https://github.com/
 konradhalas/dacite [requests]: https://img.shields.io/badge/requests-
 35495E?style=for-the-badge&logo=github&logoColor=4FC08D [requests-url]: https:/
 /github.com/psf/requests
```

### Comparing `olx-api-wrapper-0.1.3/README.md` & `olx-api-wrapper-0.2.0/olx_api_wrapper.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,253 +1,268 @@
-<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
-<a name="readme-top"></a>
-<!--
-*** Thanks for checking out the Best-README-Template. If you have a suggestion
-*** that would make this better, please fork the repo and create a pull request
-*** or simply open an issue with the tag "enhancement".
-*** Don't forget to give the project a star!
-*** Thanks again! Now go create something AMAZING! :D
--->
-
-
-
-<!-- PROJECT SHIELDS -->
-<!--
-*** I'm using markdown "reference style" links for readability.
-*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
-*** See the bottom of this document for the declaration of the reference variables
-*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
-*** https://www.markdownguide.org/basic-syntax/#reference-style-links
--->
-[![Contributors][contributors-shield]][contributors-url]
-[![Forks][forks-shield]][forks-url]
-[![Stargazers][stars-shield]][stars-url]
-[![Issues][issues-shield]][issues-url]
-[![MIT License][license-shield]][license-url]
-[![LinkedIn][linkedin-shield]][linkedin-url]
-
-
-
-<!-- PROJECT LOGO -->
-<br />
-<div align="center">
-  <a href="https://github.com/Pawikoski/olx-api-wrapper">
-    <img src="images/image.png" alt="Logo" height="80">
-  </a>
-
-<h3 align="center">OLX Api Wrapper</h3>
-
-  <p align="center">
-    Simple client for OLX Developer API written in Python
-    <br />
-    <a href="https://github.com/Pawikoski/olx-api-wrapper"><strong>Explore the docs »</strong></a>
-    <br />
-    <br />
-    <a href="https://github.com/Pawikoski/olx-api-wrapper">View Demo</a>
-    ·
-    <a href="https://github.com/Pawikoski/olx-api-wrapper/issues/new?labels=bug&template=bug-report---.md">Report Bug</a>
-    ·
-    <a href="https://github.com/Pawikoski/olx-api-wrapper/issues/new?labels=enhancement&template=feature-request---.md">Request Feature</a>
-  </p>
-</div>
-
-
-
-<!-- TABLE OF CONTENTS -->
-<details>
-  <summary>Table of Contents</summary>
-  <ol>
-    <li>
-      <a href="#about-the-project">About The Project</a>
-      <ul>
-        <li><a href="#built-with">Built With</a></li>
-      </ul>
-    </li>
-    <li>
-      <a href="#getting-started">Getting Started</a>
-      <ul>
-        <li><a href="#prerequisites">Prerequisites</a></li>
-        <li><a href="#installation">Installation</a></li>
-      </ul>
-    </li>
-    <li><a href="#usage">Usage</a></li>
-    <li><a href="#roadmap">Roadmap</a></li>
-    <li><a href="#contributing">Contributing</a></li>
-    <li><a href="#license">License</a></li>
-    <li><a href="#contact">Contact</a></li>
-    <li><a href="#acknowledgments">Acknowledgments</a></li>
-  </ol>
-</details>
-
-
-
-<!-- ABOUT THE PROJECT -->
-## About The Project
-
-OLX API Wrapper: Easy Solution for Working with OLX. With this Python library you can quickly fetch user data, handle adverts with simple CRUD operations, and seamlessly integrate with the OLX API. Simplify your development process and focus on building your app hassle-free.
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-### Built With
-
-* [![Python][Python]][Python-url]
-* [![requests][requests]][requests-url]
-* [![dacite][dacite]][dacite-url]
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-<!-- GETTING STARTED -->
-## Getting Started
-
-In order to use OLX Api you nned to sign in at OLX Developer Portal and create an App.
-More details: https://developer.olx.pl/articles/getting-access-to-api
-
-### Prerequisites
-
-To use this API Wrapper you need to copy Client ID and Client Secret. Store them in the safe place. In your code you can use them as enviroment variables, they sholdn't be hardcoded.
-You can perform actions with API on:
-- OLX PL
-- OLX BG
-- OLX RO
-- OLX PT
-- OLX UA
-- OLX KZ
-  
-By default, all requests are sent to olx.**PL**. To change it you must pass `country_code` argument to every child of Olx class, i.e.:
-```python
-olx.Auth(country_code="bg")
-olx.Adverts(country_code="ro")
-olx.Users(country_code="pt")
-olx.CitiesDistricts(country_code="ua")
-olx.AdvertsStatistics(country_code="kz")
-# etc...
-```
-
-### Installation
-
-1. Install `olx-api-wrapper` package
-   ```sh
-   pip install olx-api-wrapper
-   ```
-2. In order to get access token you need to authenticate with authorization code. [How to get authorization code?](https://developer.olx.pl/api/doc#section/Authentication/Grant-type:-authorization_code)
-   ```python
-   from olx import Auth
-   auth = Auth(
-     client_id="your_client_id",
-     client_secret="your_client_secret",
-   )
-   auth.authenticate(code='authorization_code')
-   access_token = auth.access_token
-   ```
-3. Now you have access token which you will need to have an access to OLX API resources.
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-<!-- USAGE EXAMPLES -->
-## Usage
-
-Using `olx-api-wrapper` in Your Project
-
-Below are examples demonstrating the usage of `olx-api-wrapper` in your project. Please note that you require an access token to execute the actions described below.
-
-Each section from the OLX API documentation corresponds to a separate object within `olx-api-wrapper`. For instance, the section Users in the documentation is represented as olx.Users. Additionally, each endpoint mentioned in the documentation corresponds to a single method. For example, the 'Get user' endpoint becomes the method `olx.Users().get_user(user_id)`.
-
-If a method returns a value, it will be in the form of a dataclass object. This facilitates ease of use and clarity due to type hints. You can access values as properties, for example, `user_values.email`.
-
-This structure provides a convenient and straightforward approach to integrating `olx-api-wrapper` into your project.
-
-=====================================
-
-First of all you need to assign an object you want to use to variable and then use available method of this object. You must to pass `access_token` to every single object.
-
-Prerequisites: Import olx module.
-```python
-import olx
-```
-
-- Show authenticated user info
-  ```python
-  users = olx.Users(access_token='your_access_token')
-  user_info = users.get_authenticated_user()
-  # AuthenticatedUser(id=123, email='john@mail.com', status='confirmed', name='Paweł', phone='123123123', phone_login=None, created_at='2018-01-29 19:48:49', last_login_at='2024-04-26 17:20:48', avatar=None, is_business=True)
-  
-  user_email = user_info.email
-  # john@mail.com
-  ```
-- Get category suggestions for provided ad title
-  ```python
-  categories_and_attributes = olx.CategoriesAttributes(access_token='your_access_token')
-  suggestions = categories_and_attributes.get_category_suggestions(ad_title='Honda Hornet')
-  # [CategorySuggestion(id='1379', name='Szosowo - Turystyczny', path=[CategoryPath(id='5', name='Motoryzacja'), CategoryPath(id='81', name='Motocykle i Skutery')])]
-  ```
-
-<!-- TODO: _For more examples, please refer to the [Documentation](https://example.com)_ -->
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-<!-- CONTRIBUTING -->
-## Contributing
-
-Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
-
-If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
-Don't forget to give the project a star! Thanks again!
-
-1. Fork the Project
-2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
-3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
-4. Push to the Branch (`git push origin feature/AmazingFeature`)
-5. Open a Pull Request
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-<!-- LICENSE -->
-## License
-
-Distributed under the MIT License. See `LICENSE` for more information.
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-<!-- CONTACT -->
-## Contact
-
-Paweł Stawikowski - pawikoski@gmail.com
-
-Project Link: [https://github.com/Pawikoski/olx-api-wrapper](https://github.com/Pawikoski/olx-api-wrapper)
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-
-<!-- MARKDOWN LINKS & IMAGES -->
-<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
-[contributors-shield]: https://img.shields.io/github/contributors/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
-[contributors-url]: https://github.com/Pawikoski/olx-api-wrapper/graphs/contributors
-[forks-shield]: https://img.shields.io/github/forks/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
-[forks-url]: https://github.com/Pawikoski/olx-api-wrapper/network/members
-[stars-shield]: https://img.shields.io/github/stars/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
-[stars-url]: https://github.com/Pawikoski/olx-api-wrapper/stargazers
-[issues-shield]: https://img.shields.io/github/issues/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
-[issues-url]: https://github.com/Pawikoski/olx-api-wrapper/issues
-[license-shield]: https://img.shields.io/github/license/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
-[license-url]: https://github.com/Pawikoski/olx-api-wrapper/blob/master/LICENSE
-[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
-[linkedin-url]: https://linkedin.com/in/paweł-stawikowski
-[product-image]: images/image.png
-[Python]: https://img.shields.io/badge/python-000000?style=for-the-badge&logo=python&logoColor=white
-[Python-url]: https://python.org/
-[dacite]: https://img.shields.io/badge/dacite-20232A?style=for-the-badge&logo=github&logoColor=61DAFB
-[dacite-url]: https://github.com/konradhalas/dacite
-[requests]: https://img.shields.io/badge/requests-35495E?style=for-the-badge&logo=github&logoColor=4FC08D
-[requests-url]: https://github.com/psf/requests
+Metadata-Version: 2.1
+Name: olx-api-wrapper
+Version: 0.2.0
+Summary: Unofficial Wrapper for OLX API
+Home-page: https://github.com/Pawikoski/olx-api-wrapper
+Author: Paweł Stawikowski
+Author-email: pawikoski@gmail.com
+License: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
+<a name="readme-top"></a>
+<!--
+*** Thanks for checking out the Best-README-Template. If you have a suggestion
+*** that would make this better, please fork the repo and create a pull request
+*** or simply open an issue with the tag "enhancement".
+*** Don't forget to give the project a star!
+*** Thanks again! Now go create something AMAZING! :D
+-->
+
+
+
+<!-- PROJECT SHIELDS -->
+<!--
+*** I'm using markdown "reference style" links for readability.
+*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
+*** See the bottom of this document for the declaration of the reference variables
+*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
+*** https://www.markdownguide.org/basic-syntax/#reference-style-links
+-->
+[![Contributors][contributors-shield]][contributors-url]
+[![Forks][forks-shield]][forks-url]
+[![Stargazers][stars-shield]][stars-url]
+[![Issues][issues-shield]][issues-url]
+[![MIT License][license-shield]][license-url]
+[![LinkedIn][linkedin-shield]][linkedin-url]
+
+
+
+<!-- PROJECT LOGO -->
+<br />
+<div align="center">
+  <a href="https://github.com/Pawikoski/olx-api-wrapper">
+    <img src="images/image.png" alt="Logo" height="80">
+  </a>
+
+<h3 align="center">OLX Api Wrapper</h3>
+
+  <p align="center">
+    Simple client for OLX Developer API written in Python
+    <br />
+    <a href="https://github.com/Pawikoski/olx-api-wrapper"><strong>Explore the docs Â»</strong></a>
+    <br />
+    <br />
+    <a href="https://github.com/Pawikoski/olx-api-wrapper">View Demo</a>
+    Â·
+    <a href="https://github.com/Pawikoski/olx-api-wrapper/issues/new?labels=bug&template=bug-report---.md">Report Bug</a>
+    Â·
+    <a href="https://github.com/Pawikoski/olx-api-wrapper/issues/new?labels=enhancement&template=feature-request---.md">Request Feature</a>
+  </p>
+</div>
+
+
+
+<!-- TABLE OF CONTENTS -->
+<details>
+  <summary>Table of Contents</summary>
+  <ol>
+    <li>
+      <a href="#about-the-project">About The Project</a>
+      <ul>
+        <li><a href="#built-with">Built With</a></li>
+      </ul>
+    </li>
+    <li>
+      <a href="#getting-started">Getting Started</a>
+      <ul>
+        <li><a href="#prerequisites">Prerequisites</a></li>
+        <li><a href="#installation">Installation</a></li>
+      </ul>
+    </li>
+    <li><a href="#usage">Usage</a></li>
+    <li><a href="#roadmap">Roadmap</a></li>
+    <li><a href="#contributing">Contributing</a></li>
+    <li><a href="#license">License</a></li>
+    <li><a href="#contact">Contact</a></li>
+    <li><a href="#acknowledgments">Acknowledgments</a></li>
+  </ol>
+</details>
+
+
+
+<!-- ABOUT THE PROJECT -->
+## About The Project
+
+OLX API Wrapper: Easy Solution for Working with OLX. With this Python library you can quickly fetch user data, handle adverts with simple CRUD operations, and seamlessly integrate with the OLX API. Simplify your development process and focus on building your app hassle-free.
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+
+### Built With
+
+* [![Python][Python]][Python-url]
+* [![requests][requests]][requests-url]
+* [![dacite][dacite]][dacite-url]
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+
+<!-- GETTING STARTED -->
+## Getting Started
+
+In order to use OLX Api you nned to sign in at OLX Developer Portal and create an App.
+More details: https://developer.olx.pl/articles/getting-access-to-api
+
+### Prerequisites
+
+To use this API Wrapper you need to copy Client ID and Client Secret. Store them in the safe place. In your code you can use them as enviroment variables, they sholdn't be hardcoded.
+You can perform actions with API on:
+- OLX PL
+- OLX BG
+- OLX RO
+- OLX PT
+- OLX UA
+- OLX KZ
+  
+By default, all requests are sent to olx.**PL**. To change it you must pass `country_code` argument to every child of Olx class, i.e.:
+```python
+olx.partner.Auth(country_code="bg")
+olx.partner.Adverts(country_code="ro")
+olx.partner.Users(country_code="pt")
+olx.partner.CitiesDistricts(country_code="ua")
+olx.partner.AdvertsStatistics(country_code="kz")
+# etc...
+```
+
+### Installation
+
+1. Install `olx-api-wrapper` package
+   ```sh
+   pip install olx-api-wrapper
+   ```
+2. In order to get access token you need to authenticate with authorization code. [How to get authorization code?](https://developer.olx.pl/api/doc#section/Authentication/Grant-type:-authorization_code)
+   ```python
+   from olx.partner import Auth
+   auth = Auth(
+     client_id="your_client_id",
+     client_secret="your_client_secret",
+   )
+   auth.authenticate(code='authorization_code')
+   access_token = auth.access_token
+   ```
+3. Now you have access token which you will need to have an access to OLX API resources.
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+
+<!-- USAGE EXAMPLES -->
+## Usage
+
+Using `olx-api-wrapper` in Your Project
+
+Below are examples demonstrating the usage of `olx-api-wrapper` in your project. Please note that you require an access token to execute the actions described below.
+
+Each section from the OLX API documentation corresponds to a separate object within `olx-api-wrapper`. For instance, the section Users in the documentation is represented as olx.Users. Additionally, each endpoint mentioned in the documentation corresponds to a single method. For example, the 'Get user' endpoint becomes the method `olx.partner.Users().get_user(user_id)`.
+
+If a method returns a value, it will be in the form of a dataclass object. This facilitates ease of use and clarity due to type hints. You can access values as properties, for example, `user_values.email`.
+
+This structure provides a convenient and straightforward approach to integrating `olx-api-wrapper` into your project.
+
+=====================================
+
+First of all you need to assign an object you want to use to variable and then use available method of this object. You must to pass `access_token` to every single object.
+
+Prerequisites: Import olx module.
+```python
+import olx
+```
+
+- Show authenticated user info
+  ```python
+  users = olx.partner.Users(access_token='your_access_token')
+  user_info = users.get_authenticated_user()
+  # AuthenticatedUser(id=123, email='john@mail.com', status='confirmed', name='PaweĹ‚', phone='123123123', phone_login=None, created_at='2018-01-29 19:48:49', last_login_at='2024-04-26 17:20:48', avatar=None, is_business=True)
+  
+  user_email = user_info.email
+  # john@mail.com
+  ```
+- Get category suggestions for provided ad title
+  ```python
+  categories_and_attributes = olx.partner.CategoriesAttributes(access_token='your_access_token')
+  suggestions = categories_and_attributes.get_category_suggestions(ad_title='Honda Hornet')
+  # [CategorySuggestion(id='1379', name='Szosowo - Turystyczny', path=[CategoryPath(id='5', name='Motoryzacja'), CategoryPath(id='81', name='Motocykle i Skutery')])]
+  ```
+
+<!-- TODO: _For more examples, please refer to the [Documentation](https://example.com)_ -->
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+<!-- CONTRIBUTING -->
+## Contributing
+
+Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
+
+If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
+Don't forget to give the project a star! Thanks again!
+
+1. Fork the Project
+2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
+3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
+4. Push to the Branch (`git push origin feature/AmazingFeature`)
+5. Open a Pull Request
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+
+<!-- LICENSE -->
+## License
+
+Distributed under the MIT License. See `LICENSE` for more information.
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+
+<!-- CONTACT -->
+## Contact
+
+PaweĹ‚ Stawikowski - pawikoski@gmail.com
+
+Project Link: [https://github.com/Pawikoski/olx-api-wrapper](https://github.com/Pawikoski/olx-api-wrapper)
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+
+
+<!-- MARKDOWN LINKS & IMAGES -->
+<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
+[contributors-shield]: https://img.shields.io/github/contributors/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
+[contributors-url]: https://github.com/Pawikoski/olx-api-wrapper/graphs/contributors
+[forks-shield]: https://img.shields.io/github/forks/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
+[forks-url]: https://github.com/Pawikoski/olx-api-wrapper/network/members
+[stars-shield]: https://img.shields.io/github/stars/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
+[stars-url]: https://github.com/Pawikoski/olx-api-wrapper/stargazers
+[issues-shield]: https://img.shields.io/github/issues/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
+[issues-url]: https://github.com/Pawikoski/olx-api-wrapper/issues
+[license-shield]: https://img.shields.io/github/license/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
+[license-url]: https://github.com/Pawikoski/olx-api-wrapper/blob/master/LICENSE
+[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
+[linkedin-url]: https://linkedin.com/in/paweĹ‚-stawikowski
+[product-image]: images/image.png
+[Python]: https://img.shields.io/badge/python-000000?style=for-the-badge&logo=python&logoColor=white
+[Python-url]: https://python.org/
+[dacite]: https://img.shields.io/badge/dacite-20232A?style=for-the-badge&logo=github&logoColor=61DAFB
+[dacite-url]: https://github.com/konradhalas/dacite
+[requests]: https://img.shields.io/badge/requests-35495E?style=for-the-badge&logo=github&logoColor=4FC08D
+[requests-url]: https://github.com/psf/requests
```

#### html2text {}

```diff
@@ -1,17 +1,23 @@
-[![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
-shield]][issues-url] [![MIT License][license-shield]][license-url] [![LinkedIn]
-[linkedin-shield]][linkedin-url]
+Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.2.0 Summary: Unofficial
+Wrapper for OLX API Home-page: https://github.com/Pawikoski/olx-api-wrapper
+Author: PaweÅ Stawikowski Author-email: pawikoski@gmail.com License: MIT
+Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
+Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Description-Content-Type: text/markdown
+License-File: LICENSE [![Contributors][contributors-shield]][contributors-url]
+[![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
+[Issues][issues-shield]][issues-url] [![MIT License][license-shield]][license-
+url] [![LinkedIn][linkedin-shield]][linkedin-url]
                                     _[_L_o_g_o_]
                            ******** OOLLXX AAppii WWrraappppeerr ********
             Simple client for OLX Developer API written in Python
-                             _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
+                            _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Ã_?_?Â_?»
 
-                  _V_i_e_w_ _D_e_m_o Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
+                _V_i_e_w_ _D_e_m_o ÃÂ· _R_e_p_o_r_t_ _B_u_g ÃÂ· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _B_u_i_l_t_ _W_i_t_h
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
           o _P_r_e_r_e_q_u_i_s_i_t_e_s
           o _I_n_s_t_a_l_l_a_t_i_o_n
    3. _U_s_a_g_e
@@ -31,49 +37,50 @@
 ## Getting Started In order to use OLX Api you nned to sign in at OLX Developer
 Portal and create an App. More details: https://developer.olx.pl/articles/
 getting-access-to-api ### Prerequisites To use this API Wrapper you need to
 copy Client ID and Client Secret. Store them in the safe place. In your code
 you can use them as enviroment variables, they sholdn't be hardcoded. You can
 perform actions with API on: - OLX PL - OLX BG - OLX RO - OLX PT - OLX UA - OLX
 KZ By default, all requests are sent to olx.**PL**. To change it you must pass
-`country_code` argument to every child of Olx class, i.e.: ```python olx.Auth
-(country_code="bg") olx.Adverts(country_code="ro") olx.Users(country_code="pt")
-olx.CitiesDistricts(country_code="ua") olx.AdvertsStatistics(country_code="kz")
-# etc... ``` ### Installation 1. Install `olx-api-wrapper` package ```sh pip
-install olx-api-wrapper ``` 2. In order to get access token you need to
-authenticate with authorization code. [How to get authorization code?](https://
+`country_code` argument to every child of Olx class, i.e.: ```python
+olx.partner.Auth(country_code="bg") olx.partner.Adverts(country_code="ro")
+olx.partner.Users(country_code="pt") olx.partner.CitiesDistricts
+(country_code="ua") olx.partner.AdvertsStatistics(country_code="kz") # etc...
+``` ### Installation 1. Install `olx-api-wrapper` package ```sh pip install
+olx-api-wrapper ``` 2. In order to get access token you need to authenticate
+with authorization code. [How to get authorization code?](https://
 developer.olx.pl/api/doc#section/Authentication/Grant-type:-authorization_code)
-```python from olx import Auth auth = Auth( client_id="your_client_id",
+```python from olx.partner import Auth auth = Auth( client_id="your_client_id",
 client_secret="your_client_secret", ) auth.authenticate
 (code='authorization_code') access_token = auth.access_token ``` 3. Now you
 have access token which you will need to have an access to OLX API resources.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Usage Using `olx-api-wrapper` in Your Project Below are examples
 demonstrating the usage of `olx-api-wrapper` in your project. Please note that
 you require an access token to execute the actions described below. Each
 section from the OLX API documentation corresponds to a separate object within
 `olx-api-wrapper`. For instance, the section Users in the documentation is
 represented as olx.Users. Additionally, each endpoint mentioned in the
 documentation corresponds to a single method. For example, the 'Get user'
-endpoint becomes the method `olx.Users().get_user(user_id)`. If a method
-returns a value, it will be in the form of a dataclass object. This facilitates
-ease of use and clarity due to type hints. You can access values as properties,
-for example, `user_values.email`. This structure provides a convenient and
-straightforward approach to integrating `olx-api-wrapper` into your project.
-===================================== First of all you need to assign an object
-you want to use to variable and then use available method of this object. You
-must to pass `access_token` to every single object. Prerequisites: Import olx
-module. ```python import olx ``` - Show authenticated user info ```python users
-= olx.Users(access_token='your_access_token') user_info =
-users.get_authenticated_user() # AuthenticatedUser(id=123,
-email='john@mail.com', status='confirmed', name='PaweÅ', phone='123123123',
+endpoint becomes the method `olx.partner.Users().get_user(user_id)`. If a
+method returns a value, it will be in the form of a dataclass object. This
+facilitates ease of use and clarity due to type hints. You can access values as
+properties, for example, `user_values.email`. This structure provides a
+convenient and straightforward approach to integrating `olx-api-wrapper` into
+your project. ===================================== First of all you need to
+assign an object you want to use to variable and then use available method of
+this object. You must to pass `access_token` to every single object.
+Prerequisites: Import olx module. ```python import olx ``` - Show authenticated
+user info ```python users = olx.partner.Users(access_token='your_access_token')
+user_info = users.get_authenticated_user() # AuthenticatedUser(id=123,
+email='john@mail.com', status='confirmed', name='PaweÄ¹â', phone='123123123',
 phone_login=None, created_at='2018-01-29 19:48:49', last_login_at='2024-04-26
 17:20:48', avatar=None, is_business=True) user_email = user_info.email #
 john@mail.com ``` - Get category suggestions for provided ad title ```python
-categories_and_attributes = olx.CategoriesAttributes
+categories_and_attributes = olx.partner.CategoriesAttributes
 (access_token='your_access_token') suggestions =
 categories_and_attributes.get_category_suggestions(ad_title='Honda Hornet') #
 [CategorySuggestion(id='1379', name='Szosowo - Turystyczny', path=[CategoryPath
 (id='5', name='Motoryzacja'), CategoryPath(id='81', name='Motocykle i
 Skutery')])] ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contributing Contributions are what make the open source community such an
@@ -85,15 +92,15 @@
 -b feature/AmazingFeature`) 3. Commit your Changes (`git commit -m 'Add some
 AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
 AmazingFeature`) 5. Open a Pull Request
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## License Distributed under the MIT License. See `LICENSE` for more
 information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Contact PaweÅ Stawikowski - pawikoski@gmail.com Project Link: [https://
+## Contact PaweÄ¹â Stawikowski - pawikoski@gmail.com Project Link: [https://
 github.com/Pawikoski/olx-api-wrapper](https://github.com/Pawikoski/olx-api-
 wrapper)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/Pawikoski/
 olx-api-wrapper.svg?style=for-the-badge [contributors-url]: https://github.com/
 Pawikoski/olx-api-wrapper/graphs/contributors [forks-shield]: https://
 img.shields.io/github/forks/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
@@ -103,15 +110,15 @@
 api-wrapper/stargazers [issues-shield]: https://img.shields.io/github/issues/
 Pawikoski/olx-api-wrapper.svg?style=for-the-badge [issues-url]: https://
 github.com/Pawikoski/olx-api-wrapper/issues [license-shield]: https://
 img.shields.io/github/license/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
 [license-url]: https://github.com/Pawikoski/olx-api-wrapper/blob/master/LICENSE
 [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-
 the-badge&logo=linkedin&colorB=555 [linkedin-url]: https://linkedin.com/in/
-paweÅ-stawikowski [product-image]: images/image.png [Python]: https://
+paweÄ¹â-stawikowski [product-image]: images/image.png [Python]: https://
 img.shields.io/badge/python-000000?style=for-the-
 badge&logo=python&logoColor=white [Python-url]: https://python.org/ [dacite]:
 https://img.shields.io/badge/dacite-20232A?style=for-the-
 badge&logo=github&logoColor=61DAFB [dacite-url]: https://github.com/
 konradhalas/dacite [requests]: https://img.shields.io/badge/requests-
 35495E?style=for-the-badge&logo=github&logoColor=4FC08D [requests-url]: https:/
 /github.com/psf/requests
```

### Comparing `olx-api-wrapper-0.1.3/olx_api_wrapper.egg-info/PKG-INFO` & `olx-api-wrapper-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,268 +1,253 @@
-Metadata-Version: 2.1
-Name: olx-api-wrapper
-Version: 0.1.3
-Summary: Unofficial Wrapper for OLX API
-Home-page: https://github.com/Pawikoski/olx-api-wrapper
-Author: Paweł Stawikowski
-Author-email: pawikoski@gmail.com
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
-<a name="readme-top"></a>
-<!--
-*** Thanks for checking out the Best-README-Template. If you have a suggestion
-*** that would make this better, please fork the repo and create a pull request
-*** or simply open an issue with the tag "enhancement".
-*** Don't forget to give the project a star!
-*** Thanks again! Now go create something AMAZING! :D
--->
-
-
-
-<!-- PROJECT SHIELDS -->
-<!--
-*** I'm using markdown "reference style" links for readability.
-*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
-*** See the bottom of this document for the declaration of the reference variables
-*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
-*** https://www.markdownguide.org/basic-syntax/#reference-style-links
--->
-[![Contributors][contributors-shield]][contributors-url]
-[![Forks][forks-shield]][forks-url]
-[![Stargazers][stars-shield]][stars-url]
-[![Issues][issues-shield]][issues-url]
-[![MIT License][license-shield]][license-url]
-[![LinkedIn][linkedin-shield]][linkedin-url]
-
-
-
-<!-- PROJECT LOGO -->
-<br />
-<div align="center">
-  <a href="https://github.com/Pawikoski/olx-api-wrapper">
-    <img src="images/image.png" alt="Logo" height="80">
-  </a>
-
-<h3 align="center">OLX Api Wrapper</h3>
-
-  <p align="center">
-    Simple client for OLX Developer API written in Python
-    <br />
-    <a href="https://github.com/Pawikoski/olx-api-wrapper"><strong>Explore the docs »</strong></a>
-    <br />
-    <br />
-    <a href="https://github.com/Pawikoski/olx-api-wrapper">View Demo</a>
-    ·
-    <a href="https://github.com/Pawikoski/olx-api-wrapper/issues/new?labels=bug&template=bug-report---.md">Report Bug</a>
-    ·
-    <a href="https://github.com/Pawikoski/olx-api-wrapper/issues/new?labels=enhancement&template=feature-request---.md">Request Feature</a>
-  </p>
-</div>
-
-
-
-<!-- TABLE OF CONTENTS -->
-<details>
-  <summary>Table of Contents</summary>
-  <ol>
-    <li>
-      <a href="#about-the-project">About The Project</a>
-      <ul>
-        <li><a href="#built-with">Built With</a></li>
-      </ul>
-    </li>
-    <li>
-      <a href="#getting-started">Getting Started</a>
-      <ul>
-        <li><a href="#prerequisites">Prerequisites</a></li>
-        <li><a href="#installation">Installation</a></li>
-      </ul>
-    </li>
-    <li><a href="#usage">Usage</a></li>
-    <li><a href="#roadmap">Roadmap</a></li>
-    <li><a href="#contributing">Contributing</a></li>
-    <li><a href="#license">License</a></li>
-    <li><a href="#contact">Contact</a></li>
-    <li><a href="#acknowledgments">Acknowledgments</a></li>
-  </ol>
-</details>
-
-
-
-<!-- ABOUT THE PROJECT -->
-## About The Project
-
-OLX API Wrapper: Easy Solution for Working with OLX. With this Python library you can quickly fetch user data, handle adverts with simple CRUD operations, and seamlessly integrate with the OLX API. Simplify your development process and focus on building your app hassle-free.
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-### Built With
-
-* [![Python][Python]][Python-url]
-* [![requests][requests]][requests-url]
-* [![dacite][dacite]][dacite-url]
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-<!-- GETTING STARTED -->
-## Getting Started
-
-In order to use OLX Api you nned to sign in at OLX Developer Portal and create an App.
-More details: https://developer.olx.pl/articles/getting-access-to-api
-
-### Prerequisites
-
-To use this API Wrapper you need to copy Client ID and Client Secret. Store them in the safe place. In your code you can use them as enviroment variables, they sholdn't be hardcoded.
-You can perform actions with API on:
-- OLX PL
-- OLX BG
-- OLX RO
-- OLX PT
-- OLX UA
-- OLX KZ
-  
-By default, all requests are sent to olx.**PL**. To change it you must pass `country_code` argument to every child of Olx class, i.e.:
-```python
-olx.Auth(country_code="bg")
-olx.Adverts(country_code="ro")
-olx.Users(country_code="pt")
-olx.CitiesDistricts(country_code="ua")
-olx.AdvertsStatistics(country_code="kz")
-# etc...
-```
-
-### Installation
-
-1. Install `olx-api-wrapper` package
-   ```sh
-   pip install olx-api-wrapper
-   ```
-2. In order to get access token you need to authenticate with authorization code. [How to get authorization code?](https://developer.olx.pl/api/doc#section/Authentication/Grant-type:-authorization_code)
-   ```python
-   from olx import Auth
-   auth = Auth(
-     client_id="your_client_id",
-     client_secret="your_client_secret",
-   )
-   auth.authenticate(code='authorization_code')
-   access_token = auth.access_token
-   ```
-3. Now you have access token which you will need to have an access to OLX API resources.
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-<!-- USAGE EXAMPLES -->
-## Usage
-
-Using `olx-api-wrapper` in Your Project
-
-Below are examples demonstrating the usage of `olx-api-wrapper` in your project. Please note that you require an access token to execute the actions described below.
-
-Each section from the OLX API documentation corresponds to a separate object within `olx-api-wrapper`. For instance, the section Users in the documentation is represented as olx.Users. Additionally, each endpoint mentioned in the documentation corresponds to a single method. For example, the 'Get user' endpoint becomes the method `olx.Users().get_user(user_id)`.
-
-If a method returns a value, it will be in the form of a dataclass object. This facilitates ease of use and clarity due to type hints. You can access values as properties, for example, `user_values.email`.
-
-This structure provides a convenient and straightforward approach to integrating `olx-api-wrapper` into your project.
-
-=====================================
-
-First of all you need to assign an object you want to use to variable and then use available method of this object. You must to pass `access_token` to every single object.
-
-Prerequisites: Import olx module.
-```python
-import olx
-```
-
-- Show authenticated user info
-  ```python
-  users = olx.Users(access_token='your_access_token')
-  user_info = users.get_authenticated_user()
-  # AuthenticatedUser(id=123, email='john@mail.com', status='confirmed', name='Paweł', phone='123123123', phone_login=None, created_at='2018-01-29 19:48:49', last_login_at='2024-04-26 17:20:48', avatar=None, is_business=True)
-  
-  user_email = user_info.email
-  # john@mail.com
-  ```
-- Get category suggestions for provided ad title
-  ```python
-  categories_and_attributes = olx.CategoriesAttributes(access_token='your_access_token')
-  suggestions = categories_and_attributes.get_category_suggestions(ad_title='Honda Hornet')
-  # [CategorySuggestion(id='1379', name='Szosowo - Turystyczny', path=[CategoryPath(id='5', name='Motoryzacja'), CategoryPath(id='81', name='Motocykle i Skutery')])]
-  ```
-
-<!-- TODO: _For more examples, please refer to the [Documentation](https://example.com)_ -->
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-<!-- CONTRIBUTING -->
-## Contributing
-
-Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
-
-If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
-Don't forget to give the project a star! Thanks again!
-
-1. Fork the Project
-2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
-3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
-4. Push to the Branch (`git push origin feature/AmazingFeature`)
-5. Open a Pull Request
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-<!-- LICENSE -->
-## License
-
-Distributed under the MIT License. See `LICENSE` for more information.
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-<!-- CONTACT -->
-## Contact
-
-Paweł Stawikowski - pawikoski@gmail.com
-
-Project Link: [https://github.com/Pawikoski/olx-api-wrapper](https://github.com/Pawikoski/olx-api-wrapper)
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-
-<!-- MARKDOWN LINKS & IMAGES -->
-<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
-[contributors-shield]: https://img.shields.io/github/contributors/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
-[contributors-url]: https://github.com/Pawikoski/olx-api-wrapper/graphs/contributors
-[forks-shield]: https://img.shields.io/github/forks/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
-[forks-url]: https://github.com/Pawikoski/olx-api-wrapper/network/members
-[stars-shield]: https://img.shields.io/github/stars/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
-[stars-url]: https://github.com/Pawikoski/olx-api-wrapper/stargazers
-[issues-shield]: https://img.shields.io/github/issues/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
-[issues-url]: https://github.com/Pawikoski/olx-api-wrapper/issues
-[license-shield]: https://img.shields.io/github/license/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
-[license-url]: https://github.com/Pawikoski/olx-api-wrapper/blob/master/LICENSE
-[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
-[linkedin-url]: https://linkedin.com/in/paweł-stawikowski
-[product-image]: images/image.png
-[Python]: https://img.shields.io/badge/python-000000?style=for-the-badge&logo=python&logoColor=white
-[Python-url]: https://python.org/
-[dacite]: https://img.shields.io/badge/dacite-20232A?style=for-the-badge&logo=github&logoColor=61DAFB
-[dacite-url]: https://github.com/konradhalas/dacite
-[requests]: https://img.shields.io/badge/requests-35495E?style=for-the-badge&logo=github&logoColor=4FC08D
-[requests-url]: https://github.com/psf/requests
+<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
+<a name="readme-top"></a>
+<!--
+*** Thanks for checking out the Best-README-Template. If you have a suggestion
+*** that would make this better, please fork the repo and create a pull request
+*** or simply open an issue with the tag "enhancement".
+*** Don't forget to give the project a star!
+*** Thanks again! Now go create something AMAZING! :D
+-->
+
+
+
+<!-- PROJECT SHIELDS -->
+<!--
+*** I'm using markdown "reference style" links for readability.
+*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
+*** See the bottom of this document for the declaration of the reference variables
+*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
+*** https://www.markdownguide.org/basic-syntax/#reference-style-links
+-->
+[![Contributors][contributors-shield]][contributors-url]
+[![Forks][forks-shield]][forks-url]
+[![Stargazers][stars-shield]][stars-url]
+[![Issues][issues-shield]][issues-url]
+[![MIT License][license-shield]][license-url]
+[![LinkedIn][linkedin-shield]][linkedin-url]
+
+
+
+<!-- PROJECT LOGO -->
+<br />
+<div align="center">
+  <a href="https://github.com/Pawikoski/olx-api-wrapper">
+    <img src="images/image.png" alt="Logo" height="80">
+  </a>
+
+<h3 align="center">OLX Api Wrapper</h3>
+
+  <p align="center">
+    Simple client for OLX Developer API written in Python
+    <br />
+    <a href="https://github.com/Pawikoski/olx-api-wrapper"><strong>Explore the docs »</strong></a>
+    <br />
+    <br />
+    <a href="https://github.com/Pawikoski/olx-api-wrapper">View Demo</a>
+    ·
+    <a href="https://github.com/Pawikoski/olx-api-wrapper/issues/new?labels=bug&template=bug-report---.md">Report Bug</a>
+    ·
+    <a href="https://github.com/Pawikoski/olx-api-wrapper/issues/new?labels=enhancement&template=feature-request---.md">Request Feature</a>
+  </p>
+</div>
+
+
+
+<!-- TABLE OF CONTENTS -->
+<details>
+  <summary>Table of Contents</summary>
+  <ol>
+    <li>
+      <a href="#about-the-project">About The Project</a>
+      <ul>
+        <li><a href="#built-with">Built With</a></li>
+      </ul>
+    </li>
+    <li>
+      <a href="#getting-started">Getting Started</a>
+      <ul>
+        <li><a href="#prerequisites">Prerequisites</a></li>
+        <li><a href="#installation">Installation</a></li>
+      </ul>
+    </li>
+    <li><a href="#usage">Usage</a></li>
+    <li><a href="#roadmap">Roadmap</a></li>
+    <li><a href="#contributing">Contributing</a></li>
+    <li><a href="#license">License</a></li>
+    <li><a href="#contact">Contact</a></li>
+    <li><a href="#acknowledgments">Acknowledgments</a></li>
+  </ol>
+</details>
+
+
+
+<!-- ABOUT THE PROJECT -->
+## About The Project
+
+OLX API Wrapper: Easy Solution for Working with OLX. With this Python library you can quickly fetch user data, handle adverts with simple CRUD operations, and seamlessly integrate with the OLX API. Simplify your development process and focus on building your app hassle-free.
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+
+### Built With
+
+* [![Python][Python]][Python-url]
+* [![requests][requests]][requests-url]
+* [![dacite][dacite]][dacite-url]
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+
+<!-- GETTING STARTED -->
+## Getting Started
+
+In order to use OLX Api you nned to sign in at OLX Developer Portal and create an App.
+More details: https://developer.olx.pl/articles/getting-access-to-api
+
+### Prerequisites
+
+To use this API Wrapper you need to copy Client ID and Client Secret. Store them in the safe place. In your code you can use them as enviroment variables, they sholdn't be hardcoded.
+You can perform actions with API on:
+- OLX PL
+- OLX BG
+- OLX RO
+- OLX PT
+- OLX UA
+- OLX KZ
+  
+By default, all requests are sent to olx.**PL**. To change it you must pass `country_code` argument to every child of Olx class, i.e.:
+```python
+olx.partner.Auth(country_code="bg")
+olx.partner.Adverts(country_code="ro")
+olx.partner.Users(country_code="pt")
+olx.partner.CitiesDistricts(country_code="ua")
+olx.partner.AdvertsStatistics(country_code="kz")
+# etc...
+```
+
+### Installation
+
+1. Install `olx-api-wrapper` package
+   ```sh
+   pip install olx-api-wrapper
+   ```
+2. In order to get access token you need to authenticate with authorization code. [How to get authorization code?](https://developer.olx.pl/api/doc#section/Authentication/Grant-type:-authorization_code)
+   ```python
+   from olx.partner import Auth
+   auth = Auth(
+     client_id="your_client_id",
+     client_secret="your_client_secret",
+   )
+   auth.authenticate(code='authorization_code')
+   access_token = auth.access_token
+   ```
+3. Now you have access token which you will need to have an access to OLX API resources.
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+
+<!-- USAGE EXAMPLES -->
+## Usage
+
+Using `olx-api-wrapper` in Your Project
+
+Below are examples demonstrating the usage of `olx-api-wrapper` in your project. Please note that you require an access token to execute the actions described below.
+
+Each section from the OLX API documentation corresponds to a separate object within `olx-api-wrapper`. For instance, the section Users in the documentation is represented as olx.Users. Additionally, each endpoint mentioned in the documentation corresponds to a single method. For example, the 'Get user' endpoint becomes the method `olx.partner.Users().get_user(user_id)`.
+
+If a method returns a value, it will be in the form of a dataclass object. This facilitates ease of use and clarity due to type hints. You can access values as properties, for example, `user_values.email`.
+
+This structure provides a convenient and straightforward approach to integrating `olx-api-wrapper` into your project.
+
+=====================================
+
+First of all you need to assign an object you want to use to variable and then use available method of this object. You must to pass `access_token` to every single object.
+
+Prerequisites: Import olx module.
+```python
+import olx
+```
+
+- Show authenticated user info
+  ```python
+  users = olx.partner.Users(access_token='your_access_token')
+  user_info = users.get_authenticated_user()
+  # AuthenticatedUser(id=123, email='john@mail.com', status='confirmed', name='Paweł', phone='123123123', phone_login=None, created_at='2018-01-29 19:48:49', last_login_at='2024-04-26 17:20:48', avatar=None, is_business=True)
+  
+  user_email = user_info.email
+  # john@mail.com
+  ```
+- Get category suggestions for provided ad title
+  ```python
+  categories_and_attributes = olx.partner.CategoriesAttributes(access_token='your_access_token')
+  suggestions = categories_and_attributes.get_category_suggestions(ad_title='Honda Hornet')
+  # [CategorySuggestion(id='1379', name='Szosowo - Turystyczny', path=[CategoryPath(id='5', name='Motoryzacja'), CategoryPath(id='81', name='Motocykle i Skutery')])]
+  ```
+
+<!-- TODO: _For more examples, please refer to the [Documentation](https://example.com)_ -->
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+<!-- CONTRIBUTING -->
+## Contributing
+
+Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
+
+If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
+Don't forget to give the project a star! Thanks again!
+
+1. Fork the Project
+2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
+3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
+4. Push to the Branch (`git push origin feature/AmazingFeature`)
+5. Open a Pull Request
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+
+<!-- LICENSE -->
+## License
+
+Distributed under the MIT License. See `LICENSE` for more information.
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+
+<!-- CONTACT -->
+## Contact
+
+Paweł Stawikowski - pawikoski@gmail.com
+
+Project Link: [https://github.com/Pawikoski/olx-api-wrapper](https://github.com/Pawikoski/olx-api-wrapper)
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+
+
+<!-- MARKDOWN LINKS & IMAGES -->
+<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
+[contributors-shield]: https://img.shields.io/github/contributors/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
+[contributors-url]: https://github.com/Pawikoski/olx-api-wrapper/graphs/contributors
+[forks-shield]: https://img.shields.io/github/forks/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
+[forks-url]: https://github.com/Pawikoski/olx-api-wrapper/network/members
+[stars-shield]: https://img.shields.io/github/stars/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
+[stars-url]: https://github.com/Pawikoski/olx-api-wrapper/stargazers
+[issues-shield]: https://img.shields.io/github/issues/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
+[issues-url]: https://github.com/Pawikoski/olx-api-wrapper/issues
+[license-shield]: https://img.shields.io/github/license/Pawikoski/olx-api-wrapper.svg?style=for-the-badge
+[license-url]: https://github.com/Pawikoski/olx-api-wrapper/blob/master/LICENSE
+[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
+[linkedin-url]: https://linkedin.com/in/paweł-stawikowski
+[product-image]: images/image.png
+[Python]: https://img.shields.io/badge/python-000000?style=for-the-badge&logo=python&logoColor=white
+[Python-url]: https://python.org/
+[dacite]: https://img.shields.io/badge/dacite-20232A?style=for-the-badge&logo=github&logoColor=61DAFB
+[dacite-url]: https://github.com/konradhalas/dacite
+[requests]: https://img.shields.io/badge/requests-35495E?style=for-the-badge&logo=github&logoColor=4FC08D
+[requests-url]: https://github.com/psf/requests
```

#### html2text {}

```diff
@@ -1,17 +1,11 @@
-Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.1.3 Summary: Unofficial
-Wrapper for OLX API Home-page: https://github.com/Pawikoski/olx-api-wrapper
-Author: PaweÅ Stawikowski Author-email: pawikoski@gmail.com License: MIT
-Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
-Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Description-Content-Type: text/markdown
-License-File: LICENSE [![Contributors][contributors-shield]][contributors-url]
-[![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
-[Issues][issues-shield]][issues-url] [![MIT License][license-shield]][license-
-url] [![LinkedIn][linkedin-shield]][linkedin-url]
+[![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
+shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
+shield]][issues-url] [![MIT License][license-shield]][license-url] [![LinkedIn]
+[linkedin-shield]][linkedin-url]
                                     _[_L_o_g_o_]
                            ******** OOLLXX AAppii WWrraappppeerr ********
             Simple client for OLX Developer API written in Python
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 
                   _V_i_e_w_ _D_e_m_o Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 Table of Contents
@@ -37,49 +31,50 @@
 ## Getting Started In order to use OLX Api you nned to sign in at OLX Developer
 Portal and create an App. More details: https://developer.olx.pl/articles/
 getting-access-to-api ### Prerequisites To use this API Wrapper you need to
 copy Client ID and Client Secret. Store them in the safe place. In your code
 you can use them as enviroment variables, they sholdn't be hardcoded. You can
 perform actions with API on: - OLX PL - OLX BG - OLX RO - OLX PT - OLX UA - OLX
 KZ By default, all requests are sent to olx.**PL**. To change it you must pass
-`country_code` argument to every child of Olx class, i.e.: ```python olx.Auth
-(country_code="bg") olx.Adverts(country_code="ro") olx.Users(country_code="pt")
-olx.CitiesDistricts(country_code="ua") olx.AdvertsStatistics(country_code="kz")
-# etc... ``` ### Installation 1. Install `olx-api-wrapper` package ```sh pip
-install olx-api-wrapper ``` 2. In order to get access token you need to
-authenticate with authorization code. [How to get authorization code?](https://
+`country_code` argument to every child of Olx class, i.e.: ```python
+olx.partner.Auth(country_code="bg") olx.partner.Adverts(country_code="ro")
+olx.partner.Users(country_code="pt") olx.partner.CitiesDistricts
+(country_code="ua") olx.partner.AdvertsStatistics(country_code="kz") # etc...
+``` ### Installation 1. Install `olx-api-wrapper` package ```sh pip install
+olx-api-wrapper ``` 2. In order to get access token you need to authenticate
+with authorization code. [How to get authorization code?](https://
 developer.olx.pl/api/doc#section/Authentication/Grant-type:-authorization_code)
-```python from olx import Auth auth = Auth( client_id="your_client_id",
+```python from olx.partner import Auth auth = Auth( client_id="your_client_id",
 client_secret="your_client_secret", ) auth.authenticate
 (code='authorization_code') access_token = auth.access_token ``` 3. Now you
 have access token which you will need to have an access to OLX API resources.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Usage Using `olx-api-wrapper` in Your Project Below are examples
 demonstrating the usage of `olx-api-wrapper` in your project. Please note that
 you require an access token to execute the actions described below. Each
 section from the OLX API documentation corresponds to a separate object within
 `olx-api-wrapper`. For instance, the section Users in the documentation is
 represented as olx.Users. Additionally, each endpoint mentioned in the
 documentation corresponds to a single method. For example, the 'Get user'
-endpoint becomes the method `olx.Users().get_user(user_id)`. If a method
-returns a value, it will be in the form of a dataclass object. This facilitates
-ease of use and clarity due to type hints. You can access values as properties,
-for example, `user_values.email`. This structure provides a convenient and
-straightforward approach to integrating `olx-api-wrapper` into your project.
-===================================== First of all you need to assign an object
-you want to use to variable and then use available method of this object. You
-must to pass `access_token` to every single object. Prerequisites: Import olx
-module. ```python import olx ``` - Show authenticated user info ```python users
-= olx.Users(access_token='your_access_token') user_info =
-users.get_authenticated_user() # AuthenticatedUser(id=123,
+endpoint becomes the method `olx.partner.Users().get_user(user_id)`. If a
+method returns a value, it will be in the form of a dataclass object. This
+facilitates ease of use and clarity due to type hints. You can access values as
+properties, for example, `user_values.email`. This structure provides a
+convenient and straightforward approach to integrating `olx-api-wrapper` into
+your project. ===================================== First of all you need to
+assign an object you want to use to variable and then use available method of
+this object. You must to pass `access_token` to every single object.
+Prerequisites: Import olx module. ```python import olx ``` - Show authenticated
+user info ```python users = olx.partner.Users(access_token='your_access_token')
+user_info = users.get_authenticated_user() # AuthenticatedUser(id=123,
 email='john@mail.com', status='confirmed', name='PaweÅ', phone='123123123',
 phone_login=None, created_at='2018-01-29 19:48:49', last_login_at='2024-04-26
 17:20:48', avatar=None, is_business=True) user_email = user_info.email #
 john@mail.com ``` - Get category suggestions for provided ad title ```python
-categories_and_attributes = olx.CategoriesAttributes
+categories_and_attributes = olx.partner.CategoriesAttributes
 (access_token='your_access_token') suggestions =
 categories_and_attributes.get_category_suggestions(ad_title='Honda Hornet') #
 [CategorySuggestion(id='1379', name='Szosowo - Turystyczny', path=[CategoryPath
 (id='5', name='Motoryzacja'), CategoryPath(id='81', name='Motocykle i
 Skutery')])] ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contributing Contributions are what make the open source community such an
```

