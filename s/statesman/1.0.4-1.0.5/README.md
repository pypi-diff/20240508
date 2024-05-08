# Comparing `tmp/statesman-1.0.4.tar.gz` & `tmp/statesman-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statesman-1.0.4.tar", max compression
+gzip compressed data, was "statesman-1.0.5.tar", max compression
```

## Comparing `statesman-1.0.4.tar` & `statesman-1.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-11-20 20:25:39.721551 statesman-1.0.4/LICENSE
--rw-r--r--   0        0        0    28891 2023-11-20 20:25:39.725551 statesman-1.0.4/README.md
--rw-r--r--   0        0        0     1604 2023-11-20 20:25:39.725551 statesman-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    63111 2023-11-20 20:25:39.725551 statesman-1.0.4/statesman.py
--rw-r--r--   0        0        0    29642 1970-01-01 00:00:00.000000 statesman-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-08 14:31:29.288242 statesman-1.0.5/LICENSE
+-rw-r--r--   0        0        0    28891 2024-05-08 14:31:29.288242 statesman-1.0.5/README.md
+-rw-r--r--   0        0        0     1603 2024-05-08 14:31:29.288242 statesman-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    63170 2024-05-08 14:31:29.288242 statesman-1.0.5/statesman.py
+-rw-r--r--   0        0        0    29638 1970-01-01 00:00:00.000000 statesman-1.0.5/PKG-INFO
```

### Comparing `statesman-1.0.4/LICENSE` & `statesman-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `statesman-1.0.4/README.md` & `statesman-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `statesman-1.0.4/pyproject.toml` & `statesman-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "statesman"
-version = "1.0.4"
+version = "1.0.5"
 description = "A modern state machine library."
 authors = ["Blake Watters <blake@opsani.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/opsani/statesman"
 repository = "https://github.com/opsani/statesman"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
-pydantic = "^1.7.1"
+pydantic = "^2.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 pytest-asyncio = "^0.20.0"
 devtools = "^0.6.1"
 pytest-mock = "^3.10.0"
 isort = "^5.8.0"
@@ -62,8 +62,8 @@
 
 # enable everything that starts from `flake8-`
 "flake8-*" = ["+*"]
 
 [tool.flakehell.exceptions."statesman_test.py"]
 pycodestyle = ["-*"]
 pyflakes = ["-*"]
-flake8-docstrings = ["-*"]
+flake8-docstrings = ["-*"]
```

### Comparing `statesman-1.0.4/statesman.py` & `statesman-1.0.5/statesman.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,28 +202,28 @@
 
     @classmethod
     def active(cls) -> 'State':
         """Return a temporary state object that represents the active state at
         a future point in time."""
         return State(name='__active__', description='The active state at transition time.')
 
-    @pydantic.validator('name', 'description', pre=True)
+    @pydantic.field_validator('name', 'description', mode='before')
     @classmethod
-    def _value_from_base_states(cls, value: Union[str, StateEnum], field) -> str:
+    def _value_from_base_states(cls, value: Union[str, StateEnum], info: pydantic.ValidationInfo) -> str:
         """Extract the appropriate value for the model field from a States
         enumeration value.
 
         States objects are serialized differently than typical Enum
         values in Pydantic. The name field is used to populate the state
         name and the value populates the description.
         """
         if isinstance(value, StateEnum):
-            if field.name == 'name':
+            if info.field_name == 'name':
                 return value.name
-            elif field.name == 'description':
+            elif info.field_name == 'description':
                 return value.value
 
         return value
 
     def __init__(self, name: str, description: Optional[str] = None) -> None:
         super().__init__(name=name, description=description)
 
@@ -284,15 +284,15 @@
         transition_type: An optional type specifying how the transition triggered by the event should be performed.
         return_type: The type of results returned when the event is triggered.
     """
     name: str
     description: Optional[str] = None
     sources: List[Union[None, State]]
     target: State
-    transition_type: Optional['Transition.Types']
+    transition_type: Optional['Transition.Types'] = None
     return_type: Type['Result'] = pydantic.Field(default=bool)
 
     @property
     def actions(self) -> List[Action]:
         """Return a list of actions attached to the event."""
         return self._actions.copy()
 
@@ -1007,15 +1007,15 @@
         else:
             type_ = Transition.Types.external
 
         values.setdefault('type', type_)
 
         return values
 
-    @pydantic.root_validator()
+    @pydantic.root_validator(skip_on_failure=True)
     @classmethod
     def _validate_type(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         type_ = values['type']
         if type_ in (Transition.Types.internal, Transition.Types.self):
             assert values['target'] == values['source'], 'source and target states must be the same for internal or self transitions'
         elif type_ == Transition.Types.external:
             assert values['target'] != values['source'], 'source and target states cannot be the same for external transitions'
@@ -1383,15 +1383,15 @@
     def clear_history(self) -> None:
         """Clear the history of recorded transitions."""
         self._transitions.clear()
 
 
 class SequencingMixin(pydantic.BaseModel):
     """A mixin that provides state transition sequencing functionality."""
-    __private_attributes__ = {'_queue': pydantic.PrivateAttr(collections.deque())}
+    _queue = pydantic.PrivateAttr(default_factory=collections.deque)
 
     def sequence(self, *coroutines: List[Coroutine[Any, Any, Transition]]) -> None:
         """Sequence a series of coroutines that trigger state transitions.
 
         The coroutines passed may be invocations of `enter_state`, `trigger_event`,
         or a decorated event function. The coroutines are awaited as they are dequeued
         via calls to the `next_transition` method.
@@ -1484,8 +1484,8 @@
     """Temporarily override the value of the `entry` setting on a StateMachine object.
     """
     original = obj._config.state_entry
     obj._config.state_entry = entry
     try:
         yield obj
     finally:
-        obj._config.state_entry = original
+        obj._config.state_entry = original
```

### Comparing `statesman-1.0.4/PKG-INFO` & `statesman-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: statesman
-Version: 1.0.4
+Version: 1.0.5
 Summary: A modern state machine library.
 Home-page: https://github.com/opsani/statesman
 License: Apache-2.0
 Author: Blake Watters
 Author-email: blake@opsani.com
 Requires-Python: >=3.8,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pydantic (>=1.7.1,<2.0.0)
+Requires-Dist: pydantic (>=2.4,<3.0)
 Project-URL: Repository, https://github.com/opsani/statesman
 Description-Content-Type: text/markdown
 
 # statesman
 
 ![Run Tests](https://github.com/opsani/statesman/workflows/Run%20Tests/badge.svg)
 [![license](https://img.shields.io/github/license/opsani/statesman.svg)](https://github.com/opsani/statesman/blob/master/LICENSE)
```

