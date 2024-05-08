# Comparing `tmp/smartschoolapi_tkbstudios-1.1.1.tar.gz` & `tmp/smartschoolapi_tkbstudios-1.2.0.tar.gz`

## Comparing `smartschoolapi_tkbstudios-1.1.1.tar` & `smartschoolapi_tkbstudios-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,23 @@
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.1/.env.example
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.1/requirements.txt
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.1/.github/workflows/publishpkg.yml
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.1/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.1/examples/get_courses.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.1/examples/get_grades.py
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.1/examples/get_planner.py
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.1/examples/list_messages.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.1/examples/websocket_client.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.1/src/smartschoolapi_tkbstudios/__init__.py
--rw-r--r--   0        0        0    19200 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.1/src/smartschoolapi_tkbstudios/smartschool.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.1/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.1/LICENSE
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.1/README.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.2.0/.env.example
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.2.0/requirements.txt
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.2.0/.github/workflows/publishpkg.yml
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.2.0/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.2.0/examples/delete_message_by_id.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.2.0/examples/example_boilerplate.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.2.0/examples/get_courses.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.2.0/examples/get_grades.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.2.0/examples/get_helpdesk_tickets.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.2.0/examples/get_live_sessions.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.2.0/examples/get_planner.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.2.0/examples/get_school_courses.py
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.2.0/examples/get_upload_zone.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.2.0/examples/intradesk.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.2.0/examples/list_messages.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.2.0/examples/websocket_client.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.2.0/src/smartschoolapi_tkbstudios/__init__.py
+-rw-r--r--   0        0        0    25175 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.2.0/src/smartschoolapi_tkbstudios/smartschool.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.2.0/LICENSE
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.2.0/README.md
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.2.0/PKG-INFO
```

### Comparing `smartschoolapi_tkbstudios-1.1.1/.github/workflows/publishpkg.yml` & `smartschoolapi_tkbstudios-1.2.0/.github/workflows/publishpkg.yml`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-# This workflow will upload a Python Package using Twine when a release is created
-# For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python#publishing-to-package-registries
-
-# This workflow uses actions that are not certified by GitHub.
-# They are provided by a third-party and are governed by
-# separate terms of service, privacy policy, and support
-# documentation.
-
-name: Upload Python Package
-
-on:
-  release:
-    types: [published]
-
-permissions:
-  contents: read
-
-jobs:
-  deploy:
-
-    runs-on: ubuntu-latest
-
-    steps:
-    - uses: actions/checkout@v4
-    - name: Set up Python
-      uses: actions/setup-python@v3
-      with:
-        python-version: '3.12'
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install build
-    - name: Build package
-      run: python -m build
-    - name: Publish package
-      uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
-      with:
-        user: __token__
-        password: ${{ secrets.PYPI_API_TOKEN }}
+# This workflow will upload a Python Package using Twine when a release is created
+# For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python#publishing-to-package-registries
+
+# This workflow uses actions that are not certified by GitHub.
+# They are provided by a third-party and are governed by
+# separate terms of service, privacy policy, and support
+# documentation.
+
+name: Upload Python Package
+
+on:
+  release:
+    types: [published]
+
+permissions:
+  contents: read
+
+jobs:
+  deploy:
+
+    runs-on: ubuntu-latest
+
+    steps:
+    - uses: actions/checkout@v4
+    - name: Set up Python
+      uses: actions/setup-python@v3
+      with:
+        python-version: '3.12'
+    - name: Install dependencies
+      run: |
+        python -m pip install --upgrade pip
+        pip install build
+    - name: Build package
+      run: python -m build
+    - name: Publish package
+      uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
+      with:
+        user: __token__
+        password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `smartschoolapi_tkbstudios-1.1.1/examples/get_courses.py` & `smartschoolapi_tkbstudios-1.2.0/examples/get_school_courses.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,30 @@
-"""
-Get courses example
-"""
-import os
-import logging
-import dotenv
-import smartschoolapi_tkbstudios as smsapi
-
-
-if __name__ == '__main__':
-    dotenv.load_dotenv()
-
-    smart_school_client = smsapi.SmartSchoolClient(
-        domain=os.getenv('SMARTSCHOOL_DOMAIN'),
-        loglevel=logging.DEBUG,
-    )
-    smart_school_client.phpsessid = os.getenv('SMARTSCHOOL_PHPSESSID')
-    smart_school_client.pid = os.getenv('SMARTSCHOOL_PID')
-    smart_school_client.user_id = os.getenv('SMARTSCHOOL_USER_ID')
-    smart_school_client.platform_id = os.getenv('SMARTSCHOOL_PLATFORM_ID')
-
-    courses = smart_school_client.get_courses()
-
-    print("Your courses:")
-    for course in courses:
-        print(f"{course['id']} - {course['name']} - {course['teacher']}")
+"""
+Get school courses example
+"""
+import os
+import logging
+import dotenv
+import smartschoolapi_tkbstudios as smsapi
+
+
+if __name__ == '__main__':
+    dotenv.load_dotenv()
+
+    smart_school_client = smsapi.SmartSchoolClient(
+        domain=os.getenv('SMARTSCHOOL_DOMAIN'),
+        loglevel=logging.DEBUG,
+    )
+    smart_school_client.phpsessid = os.getenv('SMARTSCHOOL_PHPSESSID')
+    smart_school_client.pid = os.getenv('SMARTSCHOOL_PID')
+    smart_school_client.user_id = os.getenv('SMARTSCHOOL_USER_ID')
+    smart_school_client.platform_id = os.getenv('SMARTSCHOOL_PLATFORM_ID')
+
+    smart_school_client.check_if_authenticated()
+
+    courses = smart_school_client.get_school_courses()
+
+    print("Your courses:")
+    for course in courses:
+        print(f"{course['id']}: "
+              f"{course['name']} "
+              f"({'visible' if course['isVisible'] else 'hidden'})")
```

### Comparing `smartschoolapi_tkbstudios-1.1.1/examples/get_grades.py` & `smartschoolapi_tkbstudios-1.2.0/examples/get_grades.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,62 @@
-"""
-Get grades example
-"""
-import os
-import logging
-import dotenv
-import smartschoolapi_tkbstudios as smsapi
-
-
-def format_grade(grade_to_format):
-    """
-    Format grade
-    """
-    course_name = grade_to_format['courses'][0]['name']
-    grade_name = grade_to_format['name']
-    grade_percentage = grade_to_format['graphic']['value']
-    grade_description = grade_to_format['graphic']['description']
-    grade_date = grade_to_format['date']
-    grade_available_since_date = grade_to_format['availabilityDate']
-    teacher_name = grade_to_format['gradebookOwner']['name']['startingWithLastName']
-    period_name = grade_to_format['period']['name']
-    period_active = bool(grade_to_format['period']['isActive'])
-
-    feedbacks = grade_to_format.get('feedbacks', [])
-    feedback_str = ""
-    for feedback in feedbacks:
-        student_name = feedback['student']['name']['startingWithLastName']
-        teacher_name = feedback['teacher']['name']['startingWithLastName']
-        feedback_text = feedback['text']
-        feedback_str += f"\nFeedback for {student_name} from {teacher_name}:\n  {feedback_text}\n"
-
-    return f"Course: {course_name}\n" \
-           f"Grade: {grade_name}\n" \
-           f"Grade: {grade_percentage}{'%' if isinstance(grade_percentage, int) else ''}" \
-           f" - {grade_description}\n" \
-           f"Date: {grade_date}\n" \
-           f"Available since: {grade_available_since_date}\n" \
-           f"Teacher: {teacher_name}\n" \
-           f"Period: {period_name}{' - Active period!' if period_active else ''}\n" \
-           f"{f"Feedbacks: {feedback_str}" if feedback_str else ''}"
-
-
-if __name__ == '__main__':
-    dotenv.load_dotenv()
-
-    smart_school_client = smsapi.SmartSchoolClient(
-        domain=os.getenv('SMARTSCHOOL_DOMAIN'),
-        loglevel=logging.DEBUG,
-    )
-    smart_school_client.phpsessid = os.getenv('SMARTSCHOOL_PHPSESSID')
-    smart_school_client.pid = os.getenv('SMARTSCHOOL_PID')
-    smart_school_client.user_id = os.getenv('SMARTSCHOOL_USER_ID')
-    smart_school_client.platform_id = os.getenv('SMARTSCHOOL_PLATFORM_ID')
-
-    grades = smart_school_client.get_results()
-
-    for grade in reversed(grades):
-        formatted_grade = format_grade(grade)
-        print(formatted_grade)
-        print("\n")
+"""
+Get grades example
+"""
+import os
+import logging
+import dotenv
+import smartschoolapi_tkbstudios as smsapi
+
+
+def format_grade(grade_to_format):
+    """
+    Format grade
+    """
+    course_name = grade_to_format['courses'][0]['name']
+    grade_name = grade_to_format['name']
+    grade_percentage = grade_to_format['graphic']['value']
+    grade_description = grade_to_format['graphic']['description']
+    grade_date = grade_to_format['date']
+    grade_available_since_date = grade_to_format['availabilityDate']
+    teacher_name = grade_to_format['gradebookOwner']['name']['startingWithLastName']
+    period_name = grade_to_format['period']['name']
+    period_active = bool(grade_to_format['period']['isActive'])
+
+    feedbacks = grade_to_format.get('feedbacks', [])
+    feedback_str = ""
+    for feedback in feedbacks:
+        student_name = feedback['student']['name']['startingWithLastName']
+        teacher_name = feedback['teacher']['name']['startingWithLastName']
+        feedback_text = feedback['text']
+        feedback_str += f"\nFeedback for {student_name} from {teacher_name}:\n  {feedback_text}\n"
+
+    return f"Course: {course_name}\n" \
+           f"Grade: {grade_name}\n" \
+           f"Grade: {grade_percentage}{'%' if isinstance(grade_percentage, int) else ''}" \
+           f" - {grade_description}\n" \
+           f"Date: {grade_date}\n" \
+           f"Available since: {grade_available_since_date}\n" \
+           f"Teacher: {teacher_name}\n" \
+           f"Period: {period_name}{' - Active period!' if period_active else ''}\n" \
+           f"{f"Feedbacks: {feedback_str}" if feedback_str else ''}"
+
+
+if __name__ == '__main__':
+    dotenv.load_dotenv()
+
+    smart_school_client = smsapi.SmartSchoolClient(
+        domain=os.getenv('SMARTSCHOOL_DOMAIN'),
+        loglevel=logging.DEBUG,
+    )
+    smart_school_client.phpsessid = os.getenv('SMARTSCHOOL_PHPSESSID')
+    smart_school_client.pid = os.getenv('SMARTSCHOOL_PID')
+    smart_school_client.user_id = os.getenv('SMARTSCHOOL_USER_ID')
+    smart_school_client.platform_id = os.getenv('SMARTSCHOOL_PLATFORM_ID')
+
+    smart_school_client.check_if_authenticated()
+
+    grades = smart_school_client.get_results()
+
+    for grade in reversed(grades):
+        formatted_grade = format_grade(grade)
+        print(formatted_grade)
+        print("\n")
```

### Comparing `smartschoolapi_tkbstudios-1.1.1/examples/websocket_client.py` & `smartschoolapi_tkbstudios-1.2.0/examples/delete_message_by_id.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-"""
-Websocket client example
-"""
-import os
-import logging
-import dotenv
-import smartschoolapi_tkbstudios as smsapi
-
-
-def received_message_callback(message_data):
-    """
-    Callback function
-    """
-    print(f"Received message: {message_data}")
-
-
-if __name__ == '__main__':
-    dotenv.load_dotenv()
-
-    smart_school_client = smsapi.SmartSchoolClient(
-        domain=os.getenv('SMARTSCHOOL_DOMAIN'),
-        loglevel=logging.DEBUG,
-    )
-    smart_school_client.phpsessid = os.getenv('SMARTSCHOOL_PHPSESSID')
-    smart_school_client.pid = os.getenv('SMARTSCHOOL_PID')
-    smart_school_client.user_id = os.getenv('SMARTSCHOOL_USER_ID')
-    smart_school_client.platform_id = os.getenv('SMARTSCHOOL_PLATFORM_ID')
-    smart_school_client.received_message_callback = received_message_callback
-
-    smart_school_client.run_websocket()
+"""
+Delete message example
+How to use:
+python `examples/delete_message_by_id.py 123`
+where 123 is the message id
+
+"""
+import os
+import logging
+import sys
+import dotenv
+from smartschoolapi_tkbstudios import SmartSchoolClient
+
+if __name__ == '__main__':
+    dotenv.load_dotenv()
+
+    if len(sys.argv) != 2:
+        print("Usage: python examples/delete_message_by_id.py <message_id>")
+        sys.exit(1)
+
+    message_id = int(sys.argv[1])
+
+    smart_school_client = SmartSchoolClient(
+        domain=os.getenv('SMARTSCHOOL_DOMAIN'),
+        loglevel=logging.DEBUG,
+    )
+    smart_school_client.phpsessid = os.getenv('SMARTSCHOOL_PHPSESSID')
+    smart_school_client.pid = os.getenv('SMARTSCHOOL_PID')
+    smart_school_client.user_id = os.getenv('SMARTSCHOOL_USER_ID')
+    smart_school_client.platform_id = os.getenv('SMARTSCHOOL_PLATFORM_ID')
+
+    smart_school_client.check_if_authenticated()
+
+    messages = smart_school_client.delete_message_by_id(message_id)
```

### Comparing `smartschoolapi_tkbstudios-1.1.1/PKG-INFO` & `smartschoolapi_tkbstudios-1.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: smartschoolapi_tkbstudios
-Version: 1.1.1
+Version: 1.2.0
 Summary: A python package to interact with SmartSchool, a Belgian School Management System
 Project-URL: Homepage, https://github.com/tkbstudios/SmartSchoolPyClient
 Project-URL: Issues, https://github.com/tkbstudios/SmartSchoolPyClient/issues
 Author-email: TKB Studios <tkbstudios@mail.tkbstudios.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 
 # SmartSchool Client
 I made this library to communicate with smartschool for some reason.  
 I was able to bind it with a voice assistant to tell me when I get a new message. (Home Assistant for reference)
 
 # How to use
```

