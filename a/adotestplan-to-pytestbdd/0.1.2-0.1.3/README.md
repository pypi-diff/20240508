# Comparing `tmp/adotestplan_to_pytestbdd-0.1.2.tar.gz` & `tmp/adotestplan_to_pytestbdd-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adotestplan_to_pytestbdd-0.1.2.tar", max compression
+gzip compressed data, was "adotestplan_to_pytestbdd-0.1.3.tar", max compression
```

## Comparing `adotestplan_to_pytestbdd-0.1.2.tar` & `adotestplan_to_pytestbdd-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1079 2024-05-03 14:05:10.785592 adotestplan_to_pytestbdd-0.1.2/LICENSE
--rw-r--r--   0        0        0     4515 2024-05-03 14:05:10.785592 adotestplan_to_pytestbdd-0.1.2/README.md
--rw-r--r--   0        0        0      399 2024-05-03 14:05:10.785592 adotestplan_to_pytestbdd-0.1.2/adotestplan_to_pytestbdd/__init__.py
--rw-r--r--   0        0        0    50743 2024-05-03 14:05:10.785592 adotestplan_to_pytestbdd-0.1.2/adotestplan_to_pytestbdd/ado_test_plan.py
--rw-r--r--   0        0        0     2040 2024-05-03 14:05:10.785592 adotestplan_to_pytestbdd-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5967 1970-01-01 00:00:00.000000 adotestplan_to_pytestbdd-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-05-07 17:05:57.637521 adotestplan_to_pytestbdd-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4515 2024-05-07 17:05:57.637521 adotestplan_to_pytestbdd-0.1.3/README.md
+-rw-r--r--   0        0        0      399 2024-05-07 17:05:57.637521 adotestplan_to_pytestbdd-0.1.3/adotestplan_to_pytestbdd/__init__.py
+-rw-r--r--   0        0        0    51582 2024-05-07 17:05:57.637521 adotestplan_to_pytestbdd-0.1.3/adotestplan_to_pytestbdd/ado_test_plan.py
+-rw-r--r--   0        0        0      348 2024-05-07 17:05:57.637521 adotestplan_to_pytestbdd-0.1.3/adotestplan_to_pytestbdd/exceptions.py
+-rw-r--r--   0        0        0     2040 2024-05-07 17:05:57.641522 adotestplan_to_pytestbdd-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5967 1970-01-01 00:00:00.000000 adotestplan_to_pytestbdd-0.1.3/PKG-INFO
```

### Comparing `adotestplan_to_pytestbdd-0.1.2/LICENSE` & `adotestplan_to_pytestbdd-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adotestplan_to_pytestbdd-0.1.2/README.md` & `adotestplan_to_pytestbdd-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `adotestplan_to_pytestbdd-0.1.2/adotestplan_to_pytestbdd/ado_test_plan.py` & `adotestplan_to_pytestbdd-0.1.3/adotestplan_to_pytestbdd/ado_test_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,21 @@
     WorkItemTrackingProcessClient
 from bs4 import BeautifulSoup
 from gherlint.linter import GherkinLinter
 from msrest.authentication import BasicAuthentication
 from thefuzz import fuzz
 from timebudget import timebudget
 
+from adotestplan_to_pytestbdd.exceptions import (InvalidGherkinError,
+                                                 InvalidParameterError,
+                                                 InvalidStepError,
+                                                 MissingFixturesError,
+                                                 NoTestSuiteError,
+                                                 OrderOfOperationsError)
+
 
 @dataclass
 class Step:
     id: int = 0
     text: str = ""
     revision: int = 0
 
@@ -335,17 +342,17 @@
                     f"No scenarios created for {feature} in {self.plan_id}. Check tags!")
 
     @timebudget
     def write_feature_files(self):
         '''this test plan populates a directory with BDD formatted feature files.
             it gets those feature files from an internal object self.bdd_tp, so that
             is assumed to have been populated previously'''
-
         if not self.bdd_tp.features:
-            raise ValueError("BDD Test Plan has not been initialized")
+            raise OrderOfOperationsError(
+                "BDD Test Plan has not been initialized")
         if os.path.exists(self.out_dir):
             # if it exists delete it and all files in it
             shutil.rmtree(self.out_dir)
 
         os.makedirs(self.out_dir)
 
         logging.info("BEGIN FEATURE FILE WRITE")
@@ -509,15 +516,15 @@
             else:
                 logging.info(
                     f"\t\tDefined fixture: \t\t{top_loc} - {top_best_match}")
         return missing_fixtures
 
     def _validate_generated_feature_against_pytest_fixtures(self, feature):
         if not os.path.exists(f"{self.out_dir}/{feature}"):
-            raise ValueError(
+            raise OSError(
                 f"Cannot validate {feature} as it is not found on disk")
         generated = self._generate_pytestbdd_for_feature(feature)
 
         fixtures_under_test = self._collect_needed_fixtures(generated)
         if len(self._defined_fixtures):
             logging.info(f"Checking fixture existence for {feature}")
             missing_fixtures = False
@@ -538,15 +545,15 @@
             logging.error(
                 f"No defined fixtures found. needed: {fixtures_under_test}")
             missing_fixtures = True
 
         if not missing_fixtures:
             logging.debug("All fixtures present")
         else:
-            raise ValueError("Missing Fixture definitions")
+            raise MissingFixturesError("Missing Fixture definitions")
 
     @timebudget
     def _generate_pytestbdd_for_feature(self, feature):
         output = subprocess.run(
             ["pytest-bdd",
              "generate",
              f"{self.out_dir}/{feature}"],
@@ -564,22 +571,28 @@
         test_filename = "test_" + test_name + ".py"
         with open(f"{self.out_dir}/{test_filename}", "w") as test_file:
             for i in scenario_runners:
                 test_file.write(f"{i}\n")
 
     def _get_list_of_feature_files(self):
         if self.out_dir is None:
-            raise ValueError(
+            raise OrderOfOperationsError(
                 f"You have not yet populated the features, \
                     or written out the feature files for {self.plan_id}")
-        files = [f for f in os.listdir(self.out_dir) if os.path.isfile(
-            os.path.join(self.out_dir, f))]
+        try:
+            files = [f for f in os.listdir(self.out_dir) if os.path.isfile(
+                os.path.join(self.out_dir, f))]
+        except FileNotFoundError:
+            raise OrderOfOperationsError(
+                f"You have not yet populated the features, \
+                    or written out the feature files for {self.plan_id} \
+                        in directory {self.out_dir}")
 
         if not len(files):
-            raise ValueError(
+            raise OrderOfOperationsError(
                 f"No feature files to generate runners for plan {self.plan_id}")
         return files
 
     def validate_pytestbdd_runners_against_feature_files(self):
         self._defined_fixtures = self._collect_defined_fixtures()
         for feature in self._get_list_of_feature_files():
             self._validate_generated_feature_against_pytest_fixtures(feature)
@@ -642,35 +655,35 @@
         '''This subroutine gets the ADO Rest API object TestPlan
             given a test plan ID'''
         if self.project is not None and self.plan_id is not None:
             self.test_plan = self.test_plan_client.get_test_plan_by_id(
                 project=self.project, plan_id=self.plan_id)
             self.test_plan: TestPlan
         else:
-            raise ValueError(
+            raise OrderOfOperationsError(
                 "You have not configured a project and Test Plan ID")
 
     @timebudget
     def _get_azure_test_suites(self):
         '''this subroutine populates self._azure_test_suites with
             a list of ADO REST API TestSuite objects'''
         temp = self.test_plan_client.get_test_suites_for_plan(
             project=self.project, plan_id=self.plan_id)
         if not len(temp):
-            raise ValueError(
+            raise NoTestSuiteError(
                 f"Found no test suites for {self.plan_id} under project{self.project}")
         for test_suite in temp:
             test_suite: TestSuite  # typehinting for autocompletion
 
             if test_suite.name != self.test_plan.name:
                 logging.info(
                     f"Adding test suite {test_suite.name} to {self.plan_id}")
                 self._azure_test_suites.append(test_suite)
         if not len(self._azure_test_suites):
-            raise ValueError(
+            raise NoTestSuiteError(
                 f"Found no populated test suites for {self.plan_id} under {self.project}")
 
     @timebudget
     def _get_azure_test_cases_for_test_suite(self, test_suite_id):
         '''this subroutine popluates a list of ADO
             REST API TestCase objects'''
         return self.test_client.get_test_cases(
@@ -875,28 +888,28 @@
             nonshared_parameter_table = work_item.fields['Microsoft.VSTS.TCM.Parameters']
         except KeyError:
             # a shared param, likely. process elsewhere
             return
         try:
             parameter_data_source = work_item.fields['Microsoft.VSTS.TCM.LocalDataSource']
         except KeyError:
-            raise ValueError(
+            raise InvalidParameterError(
                 f"Non-Shared parameter on {work_item.id} has no values")
         try:
             params = ET.fromstring(nonshared_parameter_table).findall('param')
         except ET.ParseError:
             # its just a string ID, shared param likely. process elsewhere.
             return
         try:
             tables = ET.fromstring(parameter_data_source).findall('Table1')
         except ET.ParseError:
             # a shared param, likely. process elsewhere
             return
         if not len(tables):
-            raise ValueError(
+            raise InvalidParameterError(
                 "non-shared parameter on {work_item.id} has no table contents")
         for param in params:  # not sure how fragile this is...
             param_name = param.attrib['name']
             for table in tables:
                 for elem in table:
                     tag = elem.tag  # don't need the @ here
                     if param_name == tag:
@@ -922,15 +935,15 @@
         return elements_list
 
     def _ado_to_pytest_bdd_notation(self, content: str, parent_id: int):
         # replace the azure devops "@" notation for shared parameters
         # with the pytest-bdd <variable> notation
         words = content.split(" ")
         if words[0].lower() not in self.valid_starters:
-            raise ValueError(
+            raise InvalidGherkinError(
                 f"{parent_id} step \"{content}\" does not start with one of {self.valid_starters}")  # noqa: E501
         for word in words:
             if "@" in word:
                 updated_word = word.replace("@", "")
                 if "<" == updated_word[0] or ">" == updated_word[-1]:
                     logging.warning(f"You don't need to put the <> characters in your shared parameter ({updated_word}) - that is added programatically ({parent_id})")  # noqa: E501
                 if updated_word[0] != "<":
@@ -945,15 +958,15 @@
         '''This subroutine iterates through all the steps associated with
             an ADO work item (Specifically a test case type of work item).
             It then returns a dictionary containing those steps.'''
         step_title = 'Microsoft.VSTS.TCM.Steps'
         if step_title in work_item.fields:
             steps = work_item.fields[step_title]
         else:
-            raise ValueError(
+            raise InvalidStepError(
                 f"{work_item.id}::{work_item.fields['System.Title']} has no steps")
 
         # now that we know this work item has some steps, lets see if they are
         # shared or unshared
         steps_for_item = []
         root = ET.fromstring(steps)
         all_elements = self._collect_steps_and_comprefs(root)
@@ -1160,15 +1173,15 @@
                             graph.add_node(pydot.Node(
                                 step, label=step, shape="box"))
                         if not graph.get_edge([scenario_id, step]):
                             graph.add_edge(pydot.Edge(scenario_id, step))
 
             graph.write_svg(f"{self.plan_id}.svg")
         else:
-            raise ValueError("No Features to graph!")
+            raise OrderOfOperationsError("No Features to graph!")
 
     def validate(self):
         # right now this just prints to stdout
         # we should figure out a couple things with it.
         # 1) redirect the stdout to logging, or another more robust
         #       recording destination
         # 2) return an error code if any linting issues are found
```

### Comparing `adotestplan_to_pytestbdd-0.1.2/pyproject.toml` & `adotestplan_to_pytestbdd-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "adotestplan-to-pytestbdd"
-version = "0.1.2"
+version = "0.1.3"
 description = "Utility for translating AzureDevOps Test Plans to Gherkin Feature file and Pytest-BDD runners"
 authors = [
     "David VanKampen <david.vankampen@bissell.com>",
     "Tristan VanFossen <tristan.vanfossen@bissell.com>"
 ]
 readme = "README.md"
 repository = 'https://github.com/bissell-homecare-inc/adotestplan-to-pytestbdd'
```

### Comparing `adotestplan_to_pytestbdd-0.1.2/PKG-INFO` & `adotestplan_to_pytestbdd-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adotestplan-to-pytestbdd
-Version: 0.1.2
+Version: 0.1.3
 Summary: Utility for translating AzureDevOps Test Plans to Gherkin Feature file and Pytest-BDD runners
 Home-page: https://github.com/bissell-homecare-inc/adotestplan-to-pytestbdd
 Keywords: ADO,AzureDevOps,BDD
 Author: David VanKampen
 Author-email: david.vankampen@bissell.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

