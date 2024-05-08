# Comparing `tmp/opensourceleg-2.2.0.tar.gz` & `tmp/opensourceleg-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensourceleg-2.2.0.tar", max compression
+gzip compressed data, was "opensourceleg-3.2.0.tar", max compression
```

## Comparing `opensourceleg-2.2.0.tar` & `opensourceleg-3.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    26526 2024-03-11 16:37:38.238392 opensourceleg-2.2.0/LICENSE
--rw-r--r--   0        0        0     4158 2024-04-11 18:15:50.369362 opensourceleg-2.2.0/README.md
--rw-r--r--   0        0        0      415 2023-10-12 15:36:40.401967 opensourceleg-2.2.0/opensourceleg/__init__.py
--rw-r--r--   0        0        0        0 2023-10-20 14:42:08.002099 opensourceleg-2.2.0/opensourceleg/control/__init__.py
--rw-r--r--   0        0        0     7309 2024-04-22 16:55:56.739331 opensourceleg-2.2.0/opensourceleg/control/compiled_controller.py
--rw-r--r--   0        0        0    15826 2024-04-22 16:55:56.739869 opensourceleg-2.2.0/opensourceleg/control/state_machine.py
--rw-r--r--   0        0        0        0 2023-10-20 14:42:08.002819 opensourceleg-2.2.0/opensourceleg/hardware/__init__.py
--rw-r--r--   0        0        0    34576 2024-05-06 17:40:50.560221 opensourceleg-2.2.0/opensourceleg/hardware/actuators.py
--rw-r--r--   0        0        0    12842 2024-05-06 17:26:49.228964 opensourceleg-2.2.0/opensourceleg/hardware/joints.py
--rw-r--r--   0        0        0    19890 2024-05-06 17:36:59.460237 opensourceleg-2.2.0/opensourceleg/hardware/sensors.py
--rw-r--r--   0        0        0     6501 2024-04-22 16:55:56.743110 opensourceleg-2.2.0/opensourceleg/hardware/thermal.py
--rw-r--r--   0        0        0    14085 2024-05-06 17:36:33.700442 opensourceleg-2.2.0/opensourceleg/osl.py
--rw-r--r--   0        0        0     6352 2024-05-06 17:36:33.057100 opensourceleg-2.2.0/opensourceleg/safety/sensors.py
--rw-r--r--   0        0        0        0 2023-10-20 14:42:08.003682 opensourceleg-2.2.0/opensourceleg/tools/__init__.py
--rw-r--r--   0        0        0     5920 2024-05-06 17:18:03.548467 opensourceleg-2.2.0/opensourceleg/tools/logger.py
--rw-r--r--   0        0        0     4093 2024-04-22 16:55:56.744516 opensourceleg-2.2.0/opensourceleg/tools/units.py
--rw-r--r--   0        0        0    11696 2024-04-22 16:57:48.693201 opensourceleg-2.2.0/opensourceleg/tools/utilities.py
--rw-r--r--   0        0        0     3797 2024-05-06 17:39:28.083443 opensourceleg-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     5329 1970-01-01 00:00:00.000000 opensourceleg-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    26526 2024-03-11 16:37:38.238392 opensourceleg-3.2.0/LICENSE
+-rw-r--r--   0        0        0     4158 2024-04-11 18:15:50.369362 opensourceleg-3.2.0/README.md
+-rw-r--r--   0        0        0      415 2023-10-12 15:36:40.401967 opensourceleg-3.2.0/opensourceleg/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-20 14:42:08.002099 opensourceleg-3.2.0/opensourceleg/control/__init__.py
+-rw-r--r--   0        0        0     7341 2024-05-08 11:49:20.747992 opensourceleg-3.2.0/opensourceleg/control/compiled_controller.py
+-rw-r--r--   0        0        0    22563 2024-05-08 11:49:20.748659 opensourceleg-3.2.0/opensourceleg/control/state_machine.py
+-rw-r--r--   0        0        0        0 2023-10-20 14:42:08.002819 opensourceleg-3.2.0/opensourceleg/hardware/__init__.py
+-rw-r--r--   0        0        0    42079 2024-05-08 12:17:37.503295 opensourceleg-3.2.0/opensourceleg/hardware/actuators.py
+-rw-r--r--   0        0        0    15295 2024-05-08 12:17:37.379637 opensourceleg-3.2.0/opensourceleg/hardware/joints.py
+-rw-r--r--   0        0        0    21325 2024-05-08 11:49:46.500732 opensourceleg-3.2.0/opensourceleg/hardware/sensors.py
+-rw-r--r--   0        0        0     6519 2024-05-08 11:49:20.753173 opensourceleg-3.2.0/opensourceleg/hardware/thermal.py
+-rw-r--r--   0        0        0    17013 2024-05-08 11:49:46.501067 opensourceleg-3.2.0/opensourceleg/osl.py
+-rw-r--r--   0        0        0     6352 2024-05-08 11:49:46.501655 opensourceleg-3.2.0/opensourceleg/safety/sensors.py
+-rw-r--r--   0        0        0        0 2023-10-20 14:42:08.003682 opensourceleg-3.2.0/opensourceleg/tools/__init__.py
+-rw-r--r--   0        0        0     7068 2024-05-08 11:49:46.502069 opensourceleg-3.2.0/opensourceleg/tools/logger.py
+-rw-r--r--   0        0        0     4143 2024-05-08 11:49:20.755662 opensourceleg-3.2.0/opensourceleg/tools/units.py
+-rw-r--r--   0        0        0    13890 2024-05-08 11:56:24.174609 opensourceleg-3.2.0/opensourceleg/tools/utilities.py
+-rw-r--r--   0        0        0     3824 2024-05-08 12:18:27.625254 opensourceleg-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5306 1970-01-01 00:00:00.000000 opensourceleg-3.2.0/PKG-INFO
```

### Comparing `opensourceleg-2.2.0/LICENSE` & `opensourceleg-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opensourceleg-2.2.0/README.md` & `opensourceleg-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `opensourceleg-2.2.0/opensourceleg/control/compiled_controller.py` & `opensourceleg-3.2.0/opensourceleg/control/compiled_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,40 +99,41 @@
         self.inputs = self._input_type()  # type: ignore
 
     def define_outputs(self, output_list: list[Any]) -> None:
         """
         This method defines the output structure to your function.
         See example folder and tutorials for help on using this method.
 
-        Parameters
-        ------------
-        output_list: Output parameters given as a list of [('field_name', field_type)...]
-            field_name is a string you choose as the title of the field.
-            field_type is a type either given by a native c_types value or
-                a custom type defined via the define_type() method.
-                All types can be accessed as CompiledController.types.(type_name)
+        Parameters:
+            output_list: Output parameters given as a list of [('field_name', field_type)...]
+                field_name is a string you choose as the title of the field.
+                field_type is a type either given by a native c_types value or
+                    a custom type defined via the define_type() method.
+                    All types can be accessed as CompiledController.types.(type_name)
         """
         self._output_type = self.define_type("outputs", output_list)
         self.outputs = self._output_type()  # type: ignore
 
     def define_type(self, type_name: str, parameter_list: list[Any]):
         """
         This method defines a new type to be used in the compiled controller.
         After calling this method, the datatype with name type_name will be
         available in my_controller.types.type_name for use.
         See example folder and tutorials for help on using this method.
 
-        Parameters
-        ------------
-        type_name : A string defining the name of your new datatype
-        parameter_list: A list of [('field_name', field_type)...]
-            field_name is a string you choose as the title of the field.
-            field_type is a type either given by a native c_types value or
-                a custom type defined via the define_type() method.
-                All types can be accessed as CompiledController.types.(type_name)
+        Parameters:
+            type_name : A string defining the name of your new datatype
+            parameter_list: A list of [('field_name', field_type)...]
+                field_name is a string you choose as the title of the field.
+                field_type is a type either given by a native c_types value or
+                    a custom type defined via the define_type() method.
+                    All types can be accessed as CompiledController.types.(type_name)
+
+        Returns:
+            Any
 
         Example Usage
         ------------
             my_controller.DefineType('vector3D', [('x', my_controller.types.c_double),
                                                   ('y', my_controller.types.c_double),
                                                   ('z', my_controller.types.c_double)])
         """
@@ -149,18 +150,19 @@
 
     def run(self):
         """
         This method calls the main controller function of the library.
         Under the hood, it calls library_name.main_function_name(*inputs, *outputs),
         where library_name and main_function_name were given in the constructor.
 
-        Parameters -> None
+        Parameters:
+            None
 
         Returns:
-            The output structure as defined by the define_outputs() method.
+            output structure as defined by define_outputs()
 
         Raises:
             ValueError: If define_inputs() or define_outputs() have not been called.
         """
         if self.inputs is None:
             raise ValueError(
                 "Must define input type before calling controller.run(). Use define_inputs() method."
```

### Comparing `opensourceleg-2.2.0/opensourceleg/control/state_machine.py` & `opensourceleg-3.2.0/opensourceleg/control/state_machine.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,27 +19,32 @@
    Add criteria and actions as needed.
 5. Instantiate the `StateMachine` class, add states, events, and transitions, and start the FSM.
 """
 
 
 class State:
     """
-    A class to represent a state in a finite state machine.
-
-    Args:
-        name (str): Name of the state
-        is_knee_active (bool): Whether the knee is active. Default: False
-        knee_stiffness (float): Knee stiffness in Nm/rad
-        knee_damping (float): Knee damping in Nm/rad/sec
-        knee_equilibrium_angle (float): Knee equilibrium angle
-        is_ankle_active (bool): Whether the ankle is active. Default: False
-        ankle_stiffness (float): Ankle stiffness in Nm/rad
-        ankle_damping (float): Ankle damping in Nm/rad/sec
-        ankle_equilibrium_angle (float): Ankle equilibrium angle
-        minimum_time_in_state (float): Minimum time spent in the state in seconds. Default: 2.0
+    Base class for all the states in the state machine. Please note that the knee and ankle
+    impedance parameters are only used if the corresponding joint is active in the state. In addition
+    to the default impedance parameters for each joint, you can also define custom parameters
+    using the set_custom_data method.
+
+    Parameters:
+        name (str): Name of the state. Defaults to state.
+        is_knee_active (bool): If True, the knee joint will be active in this state. Defaults to False.
+        knee_stiffness (float): Stiffness of the knee joint in this state in Nm/rad. Defaults to 0.0.
+        knee_damping (float): Damping of the knee joint in this state in Nm/(rad/s). Defaults to 0.0.
+        knee_equilibrium_angle (float): Equilibrium angle of the knee joint in this state in radians. Defaults to 0.0.
+        is_ankle_active (bool): If True, the ankle joint will be active in this state. Defaults to False.
+        ankle_stiffness (float): Stiffness of the knee joint in this state in Nm/rad. Defaults to 0.0.
+        ankle_damping (float): Damping of the knee joint in this state in Nm/(rad/s). Defaults to 0.0.
+        ankle_equilibrium_angle (float): Equilibrium angle of the knee joint in this state in radians. Defaults to 0.0.
+        minimum_time_in_state (float): Minimum time to be spent in this state in seconds. If the state is exited before
+        this time, the state machine will wait until the minimum time has elapsed before transitioning to the next state.
+        Defaults to 2.0.
 
     Note:
         The knee and ankle impedance parameters are only used if the
         corresponding joint is active. You can also set custom data
         using the `set_custom_data` method.
     """
 
@@ -92,165 +97,208 @@
         pass
 
     def __repr__(self) -> str:
         return f"State[{self._name}]"
 
     def set_minimum_time_spent_in_state(self, time: float) -> None:
         """
-        Set the minimum time spent in the state
+        Sets the minimum time to be spent in this state in seconds.
 
-        Args:
-            time (float): Minimum time spent in the state in seconds
+        Parameters:
+            time (float): Minimum time to be spent in this state in seconds. If the state is
+                          exited before this time, the state machine will wait until the minimum time has
+                          elapsed before transitioning to the next state.
         """
         self._min_time_in_state = time
 
     def set_knee_impedance_paramters(self, theta, k, b) -> None:
         """
-        Set the knee impedance parameters
+        Sets the impedance parameters of the knee joint in this state. The impedance
+        parameters are only used if the knee joint is active in this state.
 
-        Args:
-            theta (float): Equilibrium angle of the knee joint
-            k (float): Stiffness of the knee joint
-            b (float): Damping of the knee joint
+        Parameters:
+            theta (float): Equilibrium angle of the knee joint in this state in radians.
+            k (float): Stiffness of the knee joint in this state in Nm/rad.
+            b (float): Damping of the knee joint in this state in Nm/(rad/s).
 
         Note:
             The knee impedance parameters are only used if the knee is
             active. You can make the knee active by calling the
             `make_knee_active` method.
         """
         self._knee_theta = theta
         self._knee_stiffness = k
         self._knee_damping = b
 
     def set_ankle_impedance_paramters(self, theta, k, b) -> None:
         """
-        Set the ankle impedance parameters
+        Sets the impedance parameters of the ankle joint in this state. The impedance
+        parameters are only used if the ankle joint is active in this state.
 
-        Args:
-            theta (float): Equilibrium angle of the ankle joint
-            k (float): Stiffness of the ankle joint
-            b (float): Damping of the ankle joint
+        Parameters:
+            theta (float): Equilibrium angle of the ankle joint in this state in radians.
+            k (float): Stiffness of the ankle joint in this state in Nm/rad.
+            b (float): Damping of the ankle joint in this state in Nm/(rad/s).
 
         Note:
             The ankle impedance parameters are only used if the ankle is
             active. You can make the ankle active by calling the
             `make_ankle_active` method.
         """
         self._ankle_theta = theta
         self._ankle_stiffness = k
         self._ankle_damping = b
 
     def set_custom_data(self, key: str, value: Any) -> None:
         """
-        Set custom data for the state. The custom data is a dictionary
-        that can be used to store any data you want to associate with
-        the state.
-
-        Args:
-            key (str): Key of the data
-            value (Any): Value of the data
+        Sets a custom data entry for the state. This data can be used to store any
+        additional information that you want to associate with the state. Custom data is stored as a
+        dictionary as key value pairs. Multiple custom data entries can be added to the state.
+
+        Parameters:
+            key (str): Key of the custom data
+            value (Any): Value of the custom data
         """
         self._custom_data[key] = value
 
     def get_custom_data(self, key: str) -> Any:
         """
-        Get custom data for the state. The custom data is a dictionary
-        that can be used to store any data you want to associate with
-        the state.
+        Gets a custom data entry for the state. Please note that if the key does not exist, this method will raise a KeyError.
 
-        Args:
-            key (str): Key of the data
+        Parameters:
+            key (str): Key of the custom data.
 
         Returns:
-            Any: Value of the data
+            Any: Value of the custom data
         """
         return self._custom_data[key]
 
     def on_entry(self, callback: Callable[[Any], None]) -> None:
+        """
+        Adds a function or callback to be called when the state is entered.
+
+        Parameters:
+            callback (Callable[[Any], None]): Function to be called when the state is entered.
+        """
         self._entry_callbacks.append(callback)
 
     def on_exit(self, callback: Callable[[Any], None]) -> None:
+        """
+        Adds a function or callback to be called when the state is exited.
+
+        Parameters:
+            callback (Callable[[Any], None]): Function to be called when the state is exited.
+        """
         self._exit_callbacks.append(callback)
 
     def start(self, data: Any) -> None:
+        """
+
+        Parameters:
+            data (Any): Any custom data that you'd like to pass to the state's entry callbacks.
+        """
         self._time_entered = time.time()
         for c in self._entry_callbacks:
             c(data)
 
     def stop(self, data: Any) -> None:
+        """
+        Stops the state by calling all of its exit callbacks in the order they were added.
+
+        Parameters:
+            data (Any): Any custom data that you'd like to pass to the state's exit callbacks.
+        """
         self._time_exited = time.time()
         for c in self._exit_callbacks:
             c(data)
 
     def make_knee_active(self):
         """
-        Make the knee active
+        Sets the knee joint to be active in this state.
+
+        Parameters:
+            None
 
         Note:
             The knee impedance parameters are only used if the knee is
             active.
         """
         self._is_knee_active = True
 
     def make_ankle_active(self):
         """
-        Make the ankle active
+        Sets the ankle joint to be active in this state.
+
+        Parameters:
+            None
 
         Note:
             The ankle impedance parameters are only used if the ankle is
             active.
         """
         self._is_ankle_active = True
 
     @property
     def name(self) -> str:
+        """name (str): Name of the state."""
         return self._name
 
     @property
     def knee_stiffness(self) -> float:
+        """knee_stiffness (float): Stiffness of the knee joint in this state in Nm/rad."""
         return self._knee_stiffness
 
     @property
     def knee_damping(self) -> float:
+        """knee_damping (float): Damping of the knee joint in this state in Nm/(rad/s)."""
         return self._knee_damping
 
     @property
     def knee_theta(self) -> float:
+        """knee_theta (float): Equilibrium angle of the knee joint in this state in radians."""
         return self._knee_theta
 
     @property
     def ankle_stiffness(self) -> float:
+        """ankle_stiffness (float): Stiffness of the ankle joint in this state in Nm/rad."""
         return self._ankle_stiffness
 
     @property
     def ankle_damping(self) -> float:
+        """ankle_damping (float): Damping of the ankle joint in this state in Nm/(rad/s)."""
         return self._ankle_damping
 
     @property
     def ankle_theta(self) -> float:
+        """ankle_theta (float): Equilibrium angle of the ankle joint in this state in radians."""
         return self._ankle_theta
 
     @property
     def is_knee_active(self) -> bool:
+        """is_knee_active (bool): Is the knee joint set to be active in this state?"""
         return self._is_knee_active
 
     @property
     def is_ankle_active(self) -> bool:
+        """is_ankle_active (bool): Is the ankle joint set to be active in this state?"""
         return self._is_ankle_active
 
     @property
     def minimum_time_spent_in_state(self) -> float:
+        """minimum_time_spent_in_state (float): Minimum time to be spent in this state in seconds."""
         return self._min_time_in_state
 
     @property
     def current_time_in_state(self) -> float:
+        """current_time_in_state (float): Current time spent in this state in seconds."""
         return time.time() - self._time_entered
 
     @property
     def time_spent_in_state(self) -> float:
+        """time_spent_in_state (float): Total time spent in this state in seconds."""
         return self._time_exited - self._time_entered
 
 
 class Idle(State):
     def __init__(self) -> None:
         self._name = "idle"
         super().__init__(name=self._name)
@@ -258,24 +306,22 @@
     @property
     def status(self) -> str:
         return self._name
 
 
 class Event:
     """
-    Event class
+    Base class for all the events in the state machine. An event is an unique identifier that
+    corresponds to a transition in the state machine.
+
+    Parameters:
+        name (str): Name of the event.
     """
 
     def __init__(self, name) -> None:
-        """
-        Parameters
-        ----------
-        name : str
-            The name of the event.
-        """
         self._name = name
 
     def __eq__(self, __o) -> bool:
         if __o.name == self._name:
             return True
         else:
             return False
@@ -284,20 +330,30 @@
         return not self.__eq__
 
     def __repr__(self) -> str:
         return f"Event[{self._name}]"
 
     @property
     def name(self):
+        """name (str): Name of the event."""
         return self._name
 
 
 class Transition:
     """
-    Transition class
+    Base class for all the transitions in the state machine. A transition is a directed link between
+    two states in the state machine. A transition is tied to an event and is triggered only when the
+    callback function returns True.
+
+    Parameters:
+        event (Event): Event corresponding to the transition.
+        source (State): Source state of the transition.
+        destination (State): Destination state of the transition.
+        callback (Callable[[Any], bool]): A callback function that returns a boolean value, which
+        determines whether the transition should be triggered.
     """
 
     def __init__(
         self,
         event: Event,
         source: State,
         destination: State,
@@ -315,29 +371,47 @@
 
     def __repr__(self) -> str:
         return (
             f"Transition[{self._source_state.name} -> {self._destination_state.name}]"
         )
 
     def add_criteria(self, callback: Callable[[Any], bool]) -> None:
+        """
+        Adds a criteria to the transition. The transition will be triggered only if all the criteria are met.
+
+        Parameters:
+            callback (Callable[[Any], bool]): A callback function that returns a boolean
+                                              value, which determines whether the transition should be triggered.
+        """
         self._criteria = callback
 
     def add_action(self, callback: Callable[[Any], Any]) -> None:
+        """
+        Adds an action to the transition. This function will be called when the transition is triggered.
+
+        Parameters:
+            callback (Callable[[Any], Any]): Function or callback to be called when the
+                                             transition is triggered.
+
+        """
         self._action = callback
 
     @property
     def event(self) -> Event:
+        """event (Event): Event corresponding to the transition."""
         return self._event
 
     @property
     def source_state(self) -> State:
+        """source_state (State): Source state of the transition."""
         return self._source_state
 
     @property
     def destination_state(self) -> State:
+        """destination_state (State): Destination state of the transition."""
         return self._destination_state
 
 
 class FromToTransition(Transition):
     def __init__(
         self,
         event: Event,
@@ -380,34 +454,26 @@
 
         else:
             return self._from
 
 
 class StateMachine:
     """
-    State Machine class
+    A Finite State Machine (FSM) class to design and implement state machines for controlling
+    the Open-Source Leg or any other hardware system.
+
+    Parameters:
+
+    osl (Any): Open-Source Leg instance or any other hardware object to be
+               controlled. This object should ideally have all the necessary control methods and sensor data.
+               Defaults to none.
+    spoof (bool): If True, the state machine will spoof the state transitions--ie, it will not check
+                  the criteria for transitioning but will instead transition after the minimum time spent in state
+                  has elapsed. This is useful for testing.
 
-    Parameters
-    ----------
-    osl : Any
-        The OpenSourceLeg object.
-    spoof : bool
-        If True, the state machine will spoof the state transitions--ie, it will not
-        check the criteria for transitioning but will instead transition after the
-        minimum time spent in state has elapsed. This is useful for testing.
-        Defaults to False.
-
-    Attributes
-    ----------
-    current_state : State
-        The current state of the state machine.
-    states : list[State]
-        The list of states in the state machine.
-    is_spoofing : bool
-        Whether or not the state machine is spoofing the state transitions.
     """
 
     def __init__(self, osl=None, spoof: bool = False) -> None:
         # State Machine Variables
         self._states: list[State] = []
         self._events: list[Event] = []
         self._transitions: list[FromToTransition] = []
@@ -423,54 +489,59 @@
         self._spoof: bool = spoof
 
     def __repr__(self) -> str:
         return f"StateMachine"
 
     def add_state(self, state: State, initial_state: bool = False) -> None:
         """
-        Add a state to the state machine.
+        Adds a state to the state machine.
+
+        Parameters:
+            state (State): State to be added to the state machine.
+            initial_state (bool): If True, the state will be set as the initial state of the state machine. Defaults to False.
 
-        Parameters
-        ----------
-        state : State
-            The state to be added.
-        initial_state : bool, optional
-            Whether the state is the initial state, by default False
+        Raises:
+            ValueError: If state already exixts in the state machine
         """
         if state in self._states:
             raise ValueError("State already exists.")
 
         self._states.append(state)
 
         if initial_state:
             self._initial_state = state
 
     def add_event(self, event: Event) -> None:
+        """
+        Adds an event to the state machine.
+
+        Parameters:
+            event (Event): Event to be added to the state machine.
+        """
         self._events.append(event)
 
     def add_transition(
         self,
         source: State,
         destination: State,
         event: Event,
         callback: Callable[[Any], bool] = None,
     ) -> Optional[Transition]:
         """
-        Add a transition to the state machine.
+        Adds a transition to the state machine.
+
+        Parameters:
+            source (State): Source state of the transition.
+            destination (State): Destination state of the transition.
+            event (Event): Event to trigger the transition.
+            callback (Callable[[Any], bool]): A callback function that returns a boolean value, which determines whether the transition
+                                              should be triggered. Defaults to None.
 
-        Parameters
-        ----------
-        source : State
-            The source state.
-        destination : State
-            The destination state.
-        event : Event
-            The event that triggers the transition.
-        callback : Callable[[Any], bool], optional
-            A callback function that returns a boolean value, which determines whether the transition is valid, by default None
+        Returns:
+            Optional[Transition]
         """
         transition = None
 
         if (
             source in self._states
             and destination in self._states
             and event in self._events
@@ -479,14 +550,24 @@
                 event=event, source=source, destination=destination, callback=callback
             )
             self._transitions.append(transition)
 
         return transition
 
     def update(self, data: Any = None) -> None:
+        """
+        Updates the state machine. This method should be called in a loop to update
+        the state machine's state and to trigger transitions.
+
+        Parameters:
+            data (Any): Any custom data to be used with the state machine. This data will be passed to the state's exit callbacks.
+
+        Raises:
+            ValueError: It the OSL isn't active
+        """
         validity = False
 
         if not (self._initial_state or self._current_state):
             raise ValueError("OSL isn't active.")
 
         for transition in self._transitions:
             if transition.source_state == self._current_state:
@@ -502,22 +583,40 @@
                 break
 
         if not validity:
             assert self._osl is not None
             self._osl.log.debug(f"Event isn't valid at {self._current_state.name}")
 
     def start(self, data: Any = None) -> None:
+        """
+        Starts the state machine. This method should be called before calling the update method.
+
+        Parameters:
+            data (Any): Any custom data that you'd like to pass to the initial state's entry callbacks.
+
+        Raises:
+            ValueError: If initial state is not set
+        """
         if not self._initial_state:
             raise ValueError("Initial state not set.")
 
         self._current_state = self._initial_state
         self._exited = False
         self._current_state.start(data=data)
 
     def stop(self, data: Any = None) -> None:
+        """
+        Stops the state machine. This method should be called before the state machine goes out of scope.
+
+        Parameters:
+            data (Any): Any custom data that you'd like to pass to the exit state's exit callbacks.
+
+        Raises:
+            ValueError: If the OSL isn't active
+        """
         if not (self._initial_state or self._current_state):
             raise ValueError("OSL isn't active.")
 
         self._current_state.stop(data=data)
         self._current_state = self._exit_state
         self._exited = True
 
@@ -528,23 +627,26 @@
             return False
 
     def spoof(self, spoof: bool) -> None:
         self._spoof = spoof
 
     @property
     def current_state(self):
+        """current_state (State): Current state of the state machine."""
         if self._current_state is None:
             return self._initial_state
         else:
             return self._current_state
 
     @property
     def states(self):
+        """states (list[State]): List of all the states in the state machine."""
         return [state.name for state in self._states]
 
     @property
     def is_spoofing(self):
+        """is_spoofing (bool): True if the state machine is spoofing the state transitions."""
         return self._spoof
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `opensourceleg-2.2.0/opensourceleg/hardware/actuators.py` & `opensourceleg-3.2.0/opensourceleg/hardware/actuators.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import ctypes
 import os
 import time
 from ctypes import c_int
 from dataclasses import dataclass
 
-import flexsea.fx_enums as fxe
+import flexsea.utilities.constants as fx_const
 import numpy as np
 from flexsea.device import Device
 
 from ..tools.logger import Logger
 from .thermal import ThermalModel
 
 """
@@ -43,18 +43,18 @@
 class ControlModes:
     """
     Control modes for the Dephy Actpack.
 
     Available modes are Voltage, Current, Position, Impedance.
     """
 
-    voltage: ctypes.c_int = fxe.FX_VOLTAGE
-    current: ctypes.c_int = fxe.FX_CURRENT
-    position: ctypes.c_int = fxe.FX_POSITION
-    impedance: ctypes.c_int = fxe.FX_IMPEDANCE
+    voltage: ctypes.c_int = fx_const.controllers["voltage"]
+    current: ctypes.c_int = fx_const.controllers["current"]
+    position: ctypes.c_int = fx_const.controllers["position"]
+    impedance: ctypes.c_int = fx_const.controllers["impedance"]
 
     def __repr__(self) -> str:
         return f"ControlModes"
 
 
 @dataclass
 class Gains:
@@ -105,19 +105,19 @@
 DEFAULT_CURRENT_GAINS = Gains(kp=40, ki=400, kd=0, K=0, B=0, ff=128)
 
 DEFAULT_IMPEDANCE_GAINS = Gains(kp=40, ki=400, kd=0, K=200, B=400, ff=128)
 
 
 class ActpackMode:
     """
-    Base class for Actpack modes
+    Base class for all Dephy-actpack control modes.
 
-    Args:
-        control_mode (c_int): Control mode
-        device (DephyActpack): Dephy Actpack
+    Parameters:
+        control_mode (c_int): Control mode to be used. Defaults to 2.
+        device (DephyActpack): Dephy's actpack to be controlled.
     """
 
     def __init__(self, control_mode: c_int, device: "DephyActpack") -> None:
 
         self._control_mode: c_int = control_mode
         self._device: DephyActpack = device
         self._entry_callback: Callable[[], None] = lambda: None
@@ -135,50 +135,52 @@
 
     def __repr__(self) -> str:
         return f"ActpackMode[{self._control_mode}]"
 
     @property
     def mode(self) -> c_int:
         """
-        Control mode
+        Control mode being used.
 
         Returns:
-            c_int: Control mode
+            c_int
+
         """
         return self._control_mode
 
     @property
     def has_gains(self) -> bool:
         """
-        Whether the mode has gains
+        True if the control mode has gains.
 
         Returns:
-            bool: True if the mode has gains, False otherwise
+            bool
+
         """
         return self._has_gains
 
     def enter(self) -> None:
         """
-        Calls the entry callback
+        Calls the entry callback of the control mode.
         """
         self._entry_callback()
 
     def exit(self) -> None:
         """
-        Calls the exit callback
+        Calls the exit callback of the control mode.
         """
         self._exit_callback()
 
     def transition(self, to_state: "ActpackMode") -> None:
         """
-        Transition to another mode. Calls the exit callback of the current mode
-        and the entry callback of the new mode.
+        Transition to another control mode. Calls the exit callback of the current control
+        mode and the entry callback of the new control mode.
 
-        Args:
-            to_state (ActpackMode): Mode to transition to
+        Parameters:
+            to_state (ActpackMode): The control mode to transition to.
         """
         self.exit()
         to_state.enter()
 
     def _set_voltage(self, voltage: int) -> None:
         """
         This method should be implemented by the child class. It should set the q axis voltage.
@@ -195,162 +197,281 @@
         """
         This method should be implemented by the child class. It should set the motor position.
         """
         pass
 
 
 class VoltageMode(ActpackMode):
+    """
+    Voltage control mode for Dephy-actpack.
+
+    Parameters:
+        device (DephyActpack): Dephy's actpack to be controlled.
+    """
+
     def __init__(self, device: "DephyActpack") -> None:
         super().__init__(control_mode=CONTROL_MODE.voltage, device=device)
         self._entry_callback = self._entry
         self._exit_callback = self._exit
 
     def _entry(self) -> None:
+        """
+        Writes a debug log message stating that the voltage mode is being entered
+        and sets the control mode to voltage.
+
+        Parameters:
+            None
+
+        """
         self._device._log.debug(msg=f"[Actpack] Entering Voltage mode.")
 
     def _exit(self) -> None:
+        """
+        Sets the voltage to 0, sleeps for 100ms, and writes a debug log message
+        stating that the voltage mode is being exited.
+
+        Parameters:
+            None
+
+        """
         self._device._log.debug(msg=f"[Actpack] Exiting Voltage mode.")
-        self._set_voltage(voltage=0)
+        self._device.stop_motor()
         time.sleep(0.1)
 
     def _set_voltage(self, voltage: int) -> None:
-        self._device.send_motor_command(
-            ctrl_mode=self.mode,
-            value=voltage,
-        )
+        """
+        Sets the q-axis voltage to the given value.
+
+        Parameters:
+            voltage (int): Q-axis voltage to be set in mV
+
+        """
+        self._device.command_motor_voltage(value=voltage)
 
 
 class CurrentMode(ActpackMode):
+    """
+    Current control mode for Dephy-actpack.
+
+    Parameters:
+        device (DephyActpack): Dephy's actpack to be controlled.
+
+    """
+
     def __init__(self, device: "DephyActpack") -> None:
         super().__init__(control_mode=CONTROL_MODE.current, device=device)
         self._entry_callback = self._entry
         self._exit_callback = self._exit
 
     def _entry(self) -> None:
+        """
+        Writes a debug log message stating that the current mode is being entered,
+        sets default gains if none are set, and sets the q-axis current to 0.
+
+        Parameters:
+            None
+        """
         self._device._log.debug(msg=f"[Actpack] Entering Current mode.")
 
         if not self.has_gains:
             self._set_gains()
 
         self._set_current(current=0)
 
     def _exit(self) -> None:
+        """
+        Sets the voltage to 0, sleeps for 1/frequency of the device, and writes a debug
+        log message stating that the current mode is being exited.
+
+        Parameters:
+            None
+        """
         self._device._log.debug(msg=f"[Actpack] Exiting Current mode.")
-        self._device.send_motor_command(ctrl_mode=CONTROL_MODE.voltage, value=0)
+        self._device.stop_motor()
         time.sleep(1 / self._device.frequency)
 
     def _set_gains(
         self,
         kp: int = DEFAULT_CURRENT_GAINS.kp,
         ki: int = DEFAULT_CURRENT_GAINS.ki,
         ff: int = DEFAULT_CURRENT_GAINS.ff,
     ) -> None:
+        """
+        Sets the gains for the current control mode.
+
+        Parameters:
+            kp (int): Proportional gain. Defaults to 40.
+            ki (int): Integral gain. Defaults to 400.
+            ff (int): The feed-forward gain. Defaults to 128.
+
+        """
 
         assert 0 <= kp <= 80, "kp must be between 0 and 80"
         assert 0 <= ki <= 800, "ki must be between 0 and 800"
         assert 0 <= ff <= 128, "ff must be between 0 and 128"
 
         self._device.set_gains(kp=kp, ki=ki, kd=0, k=0, b=0, ff=ff)
         self._has_gains = True
 
     def _set_current(self, current: int) -> None:
-        """Sets the Q-axis current of the motor
+        """
+        Sets the q-axis current to the given value.
 
-        Args:
-            current (int): _description_
+        Parameters:
+            current (int): Q-axis current to be set in mA
         """
-        self._device.send_motor_command(
-            ctrl_mode=self.mode,
-            value=current,
-        )
+        self._device.command_motor_current(value=current)
 
 
 class PositionMode(ActpackMode):
+    """
+    Position control mode for Dephy-actpack.
+
+    Parameters:
+        device (DephyActpack): Dephy's actpack to be controlled.
+
+    """
+
     def __init__(self, device: "DephyActpack") -> None:
         super().__init__(control_mode=CONTROL_MODE.position, device=device)
         self._entry_callback = self._entry
         self._exit_callback = self._exit
 
     def _entry(self) -> None:
+        """
+        Writes a debug log message stating that the position mode is being entered,
+        sets default gains if none are set, and sets the motor position to current position.
+
+        Parameters:
+            None
+        """
+
         self._device._log.debug(msg=f"[Actpack] Entering Position mode.")
 
         if not self.has_gains:
             self._set_gains()
 
         self._device.set_motor_position(self._device.motor_position)
 
     def _exit(self) -> None:
+        """
+        Sets the voltage to 0, sleeps for 1/frequency of the device, and writes a debug
+        log message stating that the position mode is being exited.
+
+        Parameters:
+            None
+        """
+
         self._device._log.debug(msg=f"[Actpack] Exiting Position mode.")
-        self._device.send_motor_command(ctrl_mode=CONTROL_MODE.voltage, value=0)
+        self._device.stop_motor()
         time.sleep(0.1)
 
     def _set_gains(
         self,
         kp: int = DEFAULT_POSITION_GAINS.kp,
         ki: int = DEFAULT_POSITION_GAINS.ki,
         kd: int = DEFAULT_POSITION_GAINS.kd,
         ff: int = DEFAULT_POSITION_GAINS.ff,
     ) -> None:
+        """
+        Sets the gains for the position control mode.
+
+        Parameters:
+            kp (int): Proportional gain. Defaults to 50.
+            ki (int): Integral gain. Defaults to 0.
+            kd (int): Derivative gain. Defaults to 0.
+            ff (int): Feedforward gain. Defaults to 0.
+        """
 
         assert 0 <= kp <= 1000, "kp must be between 0 and 1000"
         assert 0 <= ki <= 1000, "ki must be between 0 and 1000"
         assert 0 <= kd <= 1000, "kd must be between 0 and 1000"
 
         self._device.set_gains(kp=kp, ki=ki, kd=kd, k=0, b=0, ff=ff)
         self._has_gains = True
 
     def _set_motor_position(self, counts: int) -> None:
-        """Sets the motor position
+        """
+        Sets the motor position to the given value.
 
-        Args:
-            counts (int): position in counts
+        Parameters:
+            counts (int): Motor position to be set in counts
         """
-        self._device.send_motor_command(
-            ctrl_mode=self.mode,
-            value=counts,
-        )
+        self._device.command_motor_position(value=counts)
 
 
 class ImpedanceMode(ActpackMode):
+    """
+    Impedance control mode for Dephy-actpack.
+
+    Parameters:
+        device (DephyActpack): Dephy's actpack to be controlled.
+
+    """
+
     def __init__(self, device: "DephyActpack") -> None:
         super().__init__(control_mode=CONTROL_MODE.impedance, device=device)
         self._entry_callback = self._entry
         self._exit_callback = self._exit
 
     def _entry(self) -> None:
+        """
+        Writes a debug log message stating that the impedance mode is being
+        entered, sets default gains if none are set, and sets the motor position to current position.
+
+        Parameters:
+            None
+        """
+
         self._device._log.debug(msg=f"[Actpack] Entering Impedance mode.")
         if not self.has_gains:
             self._set_gains()
 
         self._device.set_motor_position(self._device.motor_position)
 
     def _exit(self) -> None:
+        """
+        Sets the voltage to 0, sleeps for 1/frequency of the device, and writes a debug
+        log message stating that the position mode is being exited.
+
+        Parameters:
+            None
+        """
+
         self._device._log.debug(msg=f"[Actpack] Exiting Impedance mode.")
-        self._device.send_motor_command(ctrl_mode=CONTROL_MODE.voltage, value=0)
+        self._device.stop_motor()
         time.sleep(1 / self._device.frequency)
 
     def _set_motor_position(self, counts: int) -> None:
-        """Sets the motor position
+        """
+        Sets the motor position to the given value.
 
-        Args:
-            counts (int): position in counts
+        Parameters:
+            counts (int): Motor position to be set in counts.
         """
-        self._device.send_motor_command(
-            ctrl_mode=self.mode,
-            value=counts,
-        )
+        self._device.command_motor_impedance(value=counts)
 
     def _set_gains(
         self,
         kp: int = DEFAULT_IMPEDANCE_GAINS.kp,
         ki: int = DEFAULT_IMPEDANCE_GAINS.ki,
         K: int = DEFAULT_IMPEDANCE_GAINS.K,
         B: int = DEFAULT_IMPEDANCE_GAINS.B,
         ff: int = DEFAULT_IMPEDANCE_GAINS.ff,
     ) -> None:
+        """
+        Sets the gains for the impedance control mode.
+
+        Parameters:
+            kp (int): Proportional gain. Defaults to 40
+            ki (int): Integral gain. Defaults to 400
+            K (int): The stiffness gain for impedance control mode. Defaults to 200
+            B (int): The damping gain for impedance control mode. Defaults to 400
+            ff (int): The feed-forward gain. Defaults to 128
+        """
 
         assert 0 <= kp <= 80, "kp must be between 0 and 80"
         assert 0 <= ki <= 800, "ki must be between 0 and 800"
         assert 0 <= ff <= 128, "ff must be between 0 and 128"
         assert 0 <= K, "K must be greater than 0"
         assert 0 <= B, "B must be greater than 0"
 
@@ -384,56 +505,55 @@
         self.impedance = ImpedanceMode(device=device)
 
     def __repr__(self) -> str:
         return f"ActpackControlModes"
 
 
 class DephyActpack(Device):
-    """Class for the Dephy Actpack
-
-    Args:
-        Device (_type_): _description_
-
-    Raises:
-        KeyError: _description_
-        ValueError: _description_
-        KeyError: _description_
-
-    Returns:
-        _type_: _description_
+    """
+    Class for Dephy's actpack. Inherits from Dephy's flexsea device. It contains various helper
+    functions to control the actpack. It also contains opensourceleg libary's control modes
+    framework.
+
+    Parameters:
+        name (str): Name to be given to the actpack. Defaults to DephyActpack.
+        firmware_version (str): Compatible version of the actpack that will be used. Defaults to 7.2.0.
+        port (str): Port to which the actpack is connected. Defaults to /dev/ttyACM0.
+        baud_rate (int): Baud rate of the actpack. Defaults to 230400.
+        frequency (int): Frequency of the actpack. Defaults to 500.
+        logger (Logger): Logger instance to be used for logging.
+        debug_level (int): Debug level to be used for Dephy Actpack's logging routine. Defaults to 0.
+        dephy_log (bool): If True, Dephy Actpack's logging routine will be enabled in addition to the default opensourceleg's logging routine. Defaults to False.
+        stop_motor_on_disconnect (bool): If True, the motor will be stopped when the actpack is disconnected. Defaults to False.
     """
 
     def __init__(
         self,
         name: str = "DephyActpack",
+        firmware_version: str = "7.2.0",
         port: str = "/dev/ttyACM0",
         baud_rate: int = 230400,
         frequency: int = 500,
         logger: Logger = Logger(),
         debug_level: int = 0,
         dephy_log: bool = False,
+        stop_motor_on_disconnect: bool = False,
     ) -> None:
-        """
-        Initializes the Actpack class
 
-        Args:
-            name (str): _description_. Defaults to "DephyActpack".
-            port (str): _description_
-            baud_rate (int): _description_. Defaults to 230400.
-            frequency (int): _description_. Defaults to 500.
-            logger (Logger): _description_
-            debug_level (int): _description_. Defaults to 0.
-            dephy_log (bool): _description_. Defaults to False.
-        """
-        super().__init__(port=port, baud_rate=baud_rate)
+        super().__init__(
+            firmwareVersion=firmware_version,
+            port=port,
+            baudRate=baud_rate,
+            stopMotorOnDisconnect=stop_motor_on_disconnect,
+        )
         self._debug_level: int = debug_level
         self._dephy_log: bool = dephy_log
         self._frequency: int = frequency
         self._data: Any = None
-        self._name: str = name
+        self._actuator_name: str = name
 
         self._log: Logger = logger
         self._state = None
 
         self._encoder_map = None
 
         self._motor_zero_position = 0.0
@@ -453,47 +573,63 @@
         self._thermal_scale: float = 1.0
 
         self.control_modes: ActpackControlModes = ActpackControlModes(device=self)
 
         self._mode: ActpackMode = self.control_modes.voltage
 
     def __repr__(self) -> str:
-        return f"DephyActpack[{self._name}]"
+        return f"DephyActpack[{self._actuator_name}]"
 
     def start(self) -> None:
+        """
+        Starts the actpack by opening the serial port, setting the frequency, and
+        entering the default control mode, which is voltage mode.
+
+        Parameters:
+            None
+        """
         try:
-            self.open(
-                freq=self._frequency,
-                log_level=self._debug_level,
-                log_enabled=self._dephy_log,
-            )
+            self.open()
         except OSError as e:
             print("\n")
             self._log.error(
                 msg=f"[{self.__repr__()}] Need admin previleges to open the port '{self.port}'. \n\nPlease run the script with 'sudo' command or add the user to the dialout group.\n"
             )
             os._exit(status=1)
 
+        self.start_streaming(self._frequency)
         time.sleep(0.1)
         self._data = self.read()
         self._mode.enter()
 
     def stop(self) -> None:
+        """
+        Sets the control mode to voltage mode, sets the voltage to 0, and closes the
+        device.
+
+        Parameters:
+            None
+        """
+
         self.set_mode(mode=self.control_modes.voltage)
-        self.set_voltage(value=0)
+        self.stop_motor()
 
         time.sleep(0.1)
         self.close()
 
     def update(self) -> None:
         """
-        Queries the latest values from the actpack.
-        Also updates thermal model.
+        Updates the actpack's attributes by reading the actpack's data stream if the
+        actpack is connected and open. It also updates the actpack's thermal model.
+
+        Parameters:
+            None
         """
-        if self.is_streaming:
+
+        if self.streaming:
             self._data = self.read()
             self._thermal_model.T_c = self.case_temperature
             self._thermal_scale = self._thermal_model.update_and_get_scale(
                 dt=(1 / self._frequency),
                 motor_current=self.motor_current,
             )
 
@@ -504,14 +640,21 @@
                     )
         else:
             self._log.warning(
                 msg=f"[{self.__repr__()}] Please open() the device before streaming data."
             )
 
     def set_mode(self, mode: ActpackMode) -> None:
+        """
+        Sets the control mode to the given mode.
+
+        Parameters:
+            mode (ActpackMode): Control mode to be set.
+        """
+
         if type(mode) in [VoltageMode, CurrentMode, PositionMode, ImpedanceMode]:
             self._mode.transition(to_state=mode)
             self._mode = mode
 
         else:
             self._log.warning(msg=f"[{self.__repr__()}] Mode {mode} not found")
             return
@@ -544,22 +687,23 @@
         self,
         kp: int = DEFAULT_POSITION_GAINS.kp,
         ki: int = DEFAULT_POSITION_GAINS.ki,
         kd: int = DEFAULT_POSITION_GAINS.kd,
         ff: int = DEFAULT_POSITION_GAINS.ff,
     ) -> None:
         """
-        Sets the position gains in arbitrary Dephy units.
+        Sets the gains for the position control mode.
 
         Args:
             kp (int): The proportional gain
             ki (int): The integral gain
             kd (int): The derivative gain
             ff (int): The feedforward gain
         """
+
         if self._mode != self.control_modes.position:
             self._log.warning(
                 msg=f"[{self.__repr__()}] Cannot set position gains in mode {self._mode}"
             )
             return
 
         self._mode._set_gains(kp=kp, ki=ki, kd=kd, ff=ff)  # type: ignore
@@ -567,20 +711,21 @@
     def set_current_gains(
         self,
         kp: int = DEFAULT_CURRENT_GAINS.kp,
         ki: int = DEFAULT_CURRENT_GAINS.ki,
         ff: int = DEFAULT_CURRENT_GAINS.ff,
     ) -> None:
         """
-        Sets the current gains in arbitrary Dephy units.
+        Sets the gains for the current control mode. If no gains are provided, default
+        gains will be used.
 
-        Args:
-            kp (int): The proportional gain
-            ki (int): The integral gain
-            ff (int): The feedforward gain
+        Parameters:
+            kp (int): Proportional gain for the current control mode. Defaults to 40
+            ki(int): Integral gain for the current control mode. Defaults to 400
+            ff (int): Feedforward gain for the current control mode. Defaults to 128.
         """
         if self._mode != self.control_modes.current:
             self._log.warning(
                 f"[{self.__repr__()}] Cannot set current gains in mode {self._mode}"
             )
             return
 
@@ -591,91 +736,96 @@
         kp: int = DEFAULT_IMPEDANCE_GAINS.kp,
         ki: int = DEFAULT_IMPEDANCE_GAINS.ki,
         K: int = DEFAULT_IMPEDANCE_GAINS.K,
         B: int = DEFAULT_IMPEDANCE_GAINS.B,
         ff: int = DEFAULT_IMPEDANCE_GAINS.ff,
     ) -> None:
         """
-        Sets the impedance gains in arbitrary actpack units.
-        See Dephy's webpage for conversions or use other library methods that handle conversion for you.
-
-        Args:
-            kp (int): The proportional gain
-            ki (int): The integral gain
-            K (int): The spring constant
-            B (int): The damping constant
-            ff (int): The feedforward gain
+        Sets the gains for the impedance control mode in arbitary Dephy actpack
+        units. Please refer to Dephy's documentation for more information. You can also use set
+        impedance in SI units using the Joint module.
+
+        Parameters:
+            kp (int): Proportional gain for impedance control mode. Defaults to 40.
+            ki (int): Integral gain for impedance control mode. Defaults to 400.
+            K (int): The stiffness gain for impedance control mode. Defaults to 200.
+            B (int): The damping gain for impedance control mode. Defaults to 400.
+            ff (int): The feed-forward gain for the impedance control mode. Defaults to 128.
         """
+
         if self._mode != self.control_modes.impedance:
             self._log.warning(
                 msg=f"[{self.__repr__()}] Cannot set impedance gains in mode {self._mode}"
             )
             return
 
         self._mode._set_gains(kp=kp, ki=ki, K=K, B=B, ff=ff)  # type: ignore
 
     def set_voltage(self, value: float) -> None:
         """
-        Sets the q axis voltage in mV
+        Sets the voltage to the given value in mV.
 
-        Args:
-            value (float): The voltage to set in mv
+        Parameters:
+            value (float): Voltage to be set in mV.
         """
         if self._mode != self.control_modes.voltage:
             self._log.warning(
                 msg=f"[{self.__repr__()}] Cannot set voltage in mode {self._mode}"
             )
             return
 
         self._mode._set_voltage(
             int(value),
         )
 
     def set_current(self, value: float) -> None:
         """
-        Sets the q axis current in mA
+        Sets the current to the given value in mA.
 
-        Args:
-            value (float): The current to set in mA
+        Parameters:
+            value (float): Current to be set in mA.
         """
+
         if self._mode != self.control_modes.current:
             self._log.warning(
                 msg=f"[{self.__repr__()}] Cannot set current in mode {self._mode}"
             )
             return
 
         self._mode._set_current(
             int(value),
         )
 
     def set_motor_torque(self, torque: float) -> None:
         """
-        Sets the motor torque in Nm.
+        Sets the motor torque to the given value in Nm.
 
-        Args:
-            torque (float): The torque to set in Nm.
+        Parameters:
+            torque (float): Motor torque to be set in Nm.
         """
+
         if self._mode != self.control_modes.current:
             self._log.warning(
                 msg=f"[{self.__repr__()}] Cannot set motor_torque in mode {self._mode}"
             )
             return
 
         self._mode._set_current(
             int(torque / NM_PER_MILLIAMP),
         )
 
     def set_motor_position(self, position: float) -> None:
         """
-        Sets the motor position in radians.
-        If in impedance mode, this sets the equilibrium angle in radians.
+        Sets the motor position to the given value in radians. If the actpack is in
+        impedance mode, this method sets the equilibrium position.
 
-        Args:
-            position (float): The position to set
+        Parameters:
+            position (float): Motor position to be set in radians.
         """
+
         if self._mode not in [
             self.control_modes.position,
             self.control_modes.impedance,
         ]:
             self._log.warning(
                 msg=f"[{self.__repr__()}] Cannot set motor position in mode {self._mode}"
             )
@@ -724,234 +874,233 @@
     @property
     def joint_direction(self) -> float:
         """Joint direction: 1 or -1"""
         return self._joint_direction
 
     @property
     def battery_voltage(self) -> float:
-        """Battery voltage in mV."""
+        """battery_voltage (float): Battery current in mV."""
         if self._data is not None:
-            return float(self._data.batt_volt)
+            return float(self._data["batt_volt"])
         else:
             return 0.0
 
     @property
     def battery_current(self) -> float:
-        """Battery current in mA."""
+        """
+        battery_current (float): Battery current in mA. Measured using actpack's onboard current
+        sensor.
+        """
         if self._data is not None:
-            return float(self._data.batt_curr)
+            return float(self._data["batt_curr"])
         else:
             return 0.0
 
     @property
     def motor_voltage(self) -> float:
-        """Q-axis motor voltage in mV."""
+        """motor_voltage (float): Q-axis voltage in mV."""
         if self._data is not None:
-            return float(self._data.mot_volt)
+            return float(self._data["mot_volt"])
         else:
             return 0.0
 
     @property
     def motor_current(self) -> float:
-        """Q-axis motor current in mA."""
+        """motor_current (float): Motor current in mA. Measured using actpack's onboard current
+        sensor."""
         if self._data is not None:
-            return float(self._data.mot_cur)
+            return float(self._data["mot_cur"])
         else:
             return 0.0
 
     @property
     def motor_torque(self) -> float:
-        """
-        Torque at motor output in Nm.
-        This is calculated using the motor current and torque constant.
-        """
+        """motor_torque (float): Motor torque in Nm."""
         if self._data is not None:
-            return float(self._data.mot_cur * NM_PER_MILLIAMP)
+            return float(self._data["mot_cur"] * NM_PER_MILLIAMP)
         else:
             return 0.0
 
     @property
     def motor_position(self) -> float:
-        """Angle of the motor in radians."""
+        """motor_position (float): Motor's position in radians as measured by the motor's encoder.
+        This is the position of the motor with respect to the motor's zero position."""
         if self._data is not None:
             return (
-                float(self._data.mot_ang * RAD_PER_COUNT)
+                float(self._data["mot_ang"] * RAD_PER_COUNT)
                 - self._motor_zero_position
                 - self.motor_offset
             )
         else:
             return 0.0
 
     @property
     def motor_encoder_counts(self) -> int:
-        """Raw reading from motor encoder in counts."""
-        return int(self._data.mot_ang)
+        """motor_encoder_counts (int): Raw reading from motor encoder in counts."""
+        return int(self._data["mot_ang"])
 
     @property
     def joint_encoder_counts(self) -> int:
-        """Raw reading from joint encoder in counts."""
-        return int(self._data.ank_ang)
+        """joint_encoder_counts (int): Raw reading from joint encoder in counts."""
+        return int(self._data["ank_ang"])
 
     @property
     def motor_velocity(self) -> float:
-        """Motor velocity in rad/s."""
+        """motor_velocity (float): Motor's velocity in rad/s as measured by the motor's encoder."""
         if self._data is not None:
-            return int(self._data.mot_vel) * RAD_PER_DEG
+            return int(self._data["mot_vel"]) * RAD_PER_DEG
         else:
             return 0.0
 
     @property
     def motor_acceleration(self) -> float:
-        """Motor acceleration in rad/s^2."""
+        """motor_acceleration (float): Motor's acceleration in rad/s^2 as measured by the motor's encoder."""
         if self._data is not None:
-            return float(self._data.mot_acc)
+            return float(self._data["mot_acc"])
         else:
             return 0.0
 
     @property
     def joint_position(self) -> float:
-        """Measured angle from the joint encoder in radians."""
+        """joint_position (float): Joint position in radians as measured by the joint encoder. This is
+        the position of the joint with respect to the joint's zero position."""
         if self._data is not None:
             if self.encoder_map is not None:
-                return float(self.encoder_map(self._data.ank_ang))
+                return float(self.encoder_map(self._data["ank_ang"]))
             else:
                 return (
-                    float(self._data.ank_ang * RAD_PER_COUNT)
+                    float(self._data["ank_ang"] * RAD_PER_COUNT)
                     - self.joint_zero_position
                     - self.joint_offset
                 ) * self.joint_direction
         else:
             return 0.0
 
     @property
     def joint_velocity(self) -> float:
-        """Measured velocity from the joint encoder in rad/s."""
+        """joint_velocity (float): Joint velocity in rad/s as measured by the joint encoder."""
         if self._data is not None:
-            return float(self._data.ank_vel * RAD_PER_COUNT)
+            return float(self._data["ank_vel"] * RAD_PER_COUNT)
         else:
             return 0.0
 
     @property
     def case_temperature(self) -> float:
-        """Case temperature in celsius."""
+        """case_temperature (float): Temperature of the actpack's case in degrees Celsius."""
         if self._data is not None:
-            return float(self._data.temperature)
+            return float(self._data["temperature"])
         else:
             return 0.0
 
     @property
     def winding_temperature(self) -> float:
         """
-        ESTIMATED temperature of the windings in celsius.
-        This is calculated based on the thermal model using motor current.
+        winding_temperature (float): Estimated temperature of the actpack's windings in degrees
+        Celcius using the actpack's thermal model.
         """
         if self._data is not None:
             return float(self._thermal_model.T_w)
         else:
             return 0.0
 
     @property
     def thermal_scaling_factor(self) -> float:
         """
-        Scale factor to use in torque control, in [0,1].
-        If you scale the torque command by this factor, the motor temperature will never exceed max allowable temperature.
-        For a proof, see paper referenced in thermal model.
+        thermal_scaling_factor (float): Scale factor to scale the torque in torque control, in
+        [0,1]. If you scale the torque command by this factor, the motor temperature will never exceed
+        max allowable temperature.
         """
         return float(self._thermal_scale)
 
     @property
     def genvars(self):
-        """Dephy's 'genvars' object."""
+        """genvars (np.array(shape=6)): Raw general variables from the actpack. These are used by
+        the load cell amplifier when it is connected to the actpack instead of the RPi's GPIO pins.
+        """
         if self._data is not None:
             return np.array(
                 object=[
-                    self._data.genvar_0,
-                    self._data.genvar_1,
-                    self._data.genvar_2,
-                    self._data.genvar_3,
-                    self._data.genvar_4,
-                    self._data.genvar_5,
+                    self._data["genvar_0"],
+                    self._data["genvar_1"],
+                    self._data["genvar_2"],
+                    self._data["genvar_3"],
+                    self._data["genvar_4"],
+                    self._data["genvar_5"],
                 ]
             )
         else:
             return np.zeros(shape=6)
 
     @property
     def accelx(self) -> float:
         """
-        Acceleration in x direction in m/s^2.
-        Measured using actpack's onboard IMU.
+        accelx (float): Acceleration in X direction in m/s^2.
         """
         if self._data is not None:
-            return float(self._data.accelx * M_PER_SEC_SQUARED_ACCLSB)
+            return float(self._data["accelx"] * M_PER_SEC_SQUARED_ACCLSB)
         else:
             return 0.0
 
     @property
     def accely(self) -> float:
         """
-        Acceleration in y direction in m/s^2.
-        Measured using actpack's onboard IMU.
+        accely (float): Acceleration in Y direction in m/s^2.
         """
         if self._data is not None:
-            return float(self._data.accely * M_PER_SEC_SQUARED_ACCLSB)
+            return float(self._data["accely"] * M_PER_SEC_SQUARED_ACCLSB)
         else:
             return 0.0
 
     @property
     def accelz(self) -> float:
         """
-        Acceleration in z direction in m/s^2.
-        Measured using actpack's onboard IMU.
+        accelz (float): Acceleration in Z direction in m/s^2.
         """
         if self._data is not None:
-            return float(self._data.accelz * M_PER_SEC_SQUARED_ACCLSB)
+            return float(self._data["accelz"] * M_PER_SEC_SQUARED_ACCLSB)
         else:
             return 0.0
 
     @property
     def gyrox(self) -> float:
         """
-        Angular velocity in x direction in rad/s.
-        Measured using actpack's onboard IMU.
+        gyrox (float): Angular velocity in X direction in rad/s.
         """
         if self._data is not None:
-            return float(self._data.gyrox * RAD_PER_SEC_GYROLSB)
+            return float(self._data["gyrox"] * RAD_PER_SEC_GYROLSB)
         else:
             return 0.0
 
     @property
     def gyroy(self) -> float:
         """
-        Angular velocity in y direction in rad/s.
-        Measured using actpack's onboard IMU.
+        gyroy (float): Angular velocity in Y direction in rad/s.
         """
         if self._data is not None:
-            return float(self._data.gyroy * RAD_PER_SEC_GYROLSB)
+            return float(self._data["gyroy"] * RAD_PER_SEC_GYROLSB)
         else:
             return 0.0
 
     @property
     def gyroz(self) -> float:
         """
-        Angular velocity in z direction in rad/s.
-        Measured using actpack's onboard IMU.
+        gyroz (float): Angular velocity in Z direction in rad/s.
         """
         if self._data is not None:
-            return float(self._data.gyroz * RAD_PER_SEC_GYROLSB)
+            return float(self._data["gyroz"] * RAD_PER_SEC_GYROLSB)
         else:
             return 0.0
 
 
 # MockDephyActpack class definition for testing
 # MockData class definition for testing without a data stream
 class MockData:
     def __init__(
         self,
-        batt_volt=30,
+        batt_volt=0,
         batt_curr=0,
         mot_volt=0,
         mot_cur=0,
         mot_ang=0,
         ank_ang=0,
         mot_vel=0,
         mot_acc=0,
@@ -1007,38 +1156,54 @@
     some of the methods to allow for testing without a device, and adds
     attributes used to determine if the methods were called properly.
     """
 
     def __init__(
         self,
         name: str = "MockDephyActpack",
+        firmware_version: str = "7.2.0",
         port: str = "/dev/ttyACM0",
         baud_rate: int = 230400,
         frequency: int = 500,
         logger: Logger = Logger(),
         debug_level: int = 0,
         dephy_log: bool = False,
+        stop_motor_on_disconnect: bool = False,
     ) -> None:
-        """
-        Initializes the MockDephyActpack class
 
-        Args:
-            name (str): _description_. Defaults to "MockDephyActpack".
-            port (str): _description_
-            baud_rate (int): _description_. Defaults to 230400.
-            frequency (int): _description_. Defaults to 500.
-            logger (Logger): _description_
-            debug_level (int): _description_. Defaults to 0.
-            dephy_log (bool): _description_. Defaults to False.
-        """
         self._debug_level: int = debug_level
         self._dephy_log: bool = dephy_log
         self._frequency: int = frequency
-        self._data: MockData = MockData()
-        self._name: str = name
+        self._data: dict[str, float] = {
+            "batt_volt": 0,
+            "batt_curr": 0,
+            "mot_volt": 0,
+            "mot_cur": 0,
+            "mot_ang": 0,
+            "ank_ang": 0,
+            "mot_vel": 0,
+            "mot_acc": 0,
+            "ank_vel": 0,
+            "temperature": 25,
+            "genvar_0": 0,
+            "genvar_1": 0,
+            "genvar_2": 0,
+            "genvar_3": 0,
+            "genvar_4": 0,
+            "genvar_5": 0,
+            "accelx": 0,
+            "accely": 0,
+            "accelz": 0,
+            "gyrox": 0,
+            "gyroy": 0,
+            "gyroz": 0,
+        }
+        self._actuator_name: str = name
+
+        self.id: str = "1.0.0"
 
         self._log: Logger = logger
         self._state = None
 
         # New attributes to be used for testing
 
         # This is used in the open() method to display the port the device should be connected to
@@ -1054,15 +1219,14 @@
             "kd": 0,
             "k": 0,
             "b": 0,
             "ff": 0,
         }
 
         # This is used in the read() method to indicate a data stream
-        self.is_streaming: bool = False
 
         self._encoder_map = None
 
         self._motor_zero_position = 0.0
         self._joint_zero_position = 0.0
 
         self._joint_offset = 0.0
@@ -1076,62 +1240,108 @@
             temp_limit_case=70,
             soft_border_C_case=10,
         )
 
         self.control_modes: ActpackControlModes = ActpackControlModes(device=self)
         self._mode: ActpackMode = self.control_modes.voltage
 
+        self._clib: MockClib = MockClib()
+
     # Overrides the open method to function without a device
-    def open(self, freq, log_level, log_enabled):
+    def open(self):
         self._log.debug(msg=f"[{self.__repr__()}] Opening Device at {self.port}")
-        self.is_streaming = True
+        self.start_streaming(100)
 
     # Overrides the send_motor_command method to set the new _motor_command attribute
     def send_motor_command(self, ctrl_mode, value):
         self._motor_command = (
             f"[{self.__repr__()}] Control Mode: {ctrl_mode}, Value: {value}"
         )
 
+    # Overrides the command_motor_current method to set the new _motor_command attribute
+    def command_motor_current(self, value):
+        self._motor_command = (
+            f"[{self.__repr__()}] Control Mode: c_int(2), Value: {value}"
+        )
+
+    # Overrides the command_motor_current method to set the new _motor_command attribute
+    def command_motor_voltage(self, value):
+        self._motor_command = (
+            f"[{self.__repr__()}] Control Mode: c_int(1), Value: {value}"
+        )
+
+    # Overrides the command_motor_current method to set the new _motor_command attribute
+    def command_motor_position(self, value):
+        self._motor_command = (
+            f"[{self.__repr__()}] Control Mode: c_int(0), Value: {value}"
+        )
+
+    # Overrides the command_motor_current method to set the new _motor_command attribute
+    def command_motor_impedance(self, value):
+        self._motor_command = (
+            f"[{self.__repr__()}] Control Mode: c_int(3), Value: {value}"
+        )
+
     # Overrides the set_gains method to set the gains in the new _gains attribute
     def set_gains(self, kp, ki, kd, k, b, ff):
         self._gains["kp"] = kp
         self._gains["ki"] = ki
         self._gains["kd"] = kd
         self._gains["k"] = k
         self._gains["b"] = b
         self._gains["ff"] = ff
 
     # Overrides the read method to modify the data incrementally instead of through a device data stream
     def read(self):
-        small_noise = np.random.normal(0, 0.01)
 
-        self._data.batt_volt += small_noise
-        self._data.batt_curr += 0.0
-        self._data.mot_volt += 0.0
-        self._data.mot_cur += 0.0
-        self._data.mot_ang += 0.0
-        self._data.ank_ang += 0.0
-        self._data.mot_vel += small_noise
-        self._data.mot_acc += small_noise
-        self._data.ank_vel += small_noise
-        self._data.temperature += small_noise
-        self._data.genvar_0 += 0.0
-        self._data.genvar_1 += 0.0
-        self._data.genvar_2 += 0.0
-        self._data.genvar_3 += 0.0
-        self._data.genvar_4 += 0.0
-        self._data.genvar_5 += 0.0
-        self._data.accelx += small_noise
-        self._data.accely += small_noise
-        self._data.accelz += small_noise
-        self._data.gyrox += small_noise
-        self._data.gyroy += small_noise
-        self._data.gyroz += small_noise
+        self._data["batt_volt"] += 15
+        self._data["batt_curr"] += 15
+        self._data["mot_volt"] += 15
+        self._data["mot_cur"] += 15
+        self._data["mot_ang"] += 15
+        self._data["ank_ang"] += 15
+        self._data["mot_vel"] += 15
+        self._data["mot_acc"] += 15
+        self._data["ank_vel"] += 15
+        self._data["temperature"] += 15
+        self._data["genvar_0"] += 15
+        self._data["genvar_1"] += 15
+        self._data["genvar_2"] += 15
+        self._data["genvar_3"] += 15
+        self._data["genvar_4"] += 15
+        self._data["genvar_5"] += 15
+        self._data["accelx"] += 15
+        self._data["accely"] += 15
+        self._data["accelz"] += 15
+        self._data["gyrox"] += 15
+        self._data["gyroy"] += 15
+        self._data["gyroz"] += 15
         return self._data
 
+    def stop_motor(self):
+        self.command_motor_voltage(0)
+
+    def set_streaming(self):
+        self.streaming = True
+
     # Overrides the close method to do nothing
     def close(self):
         pass
 
+    @property
+    def connected(self) -> bool:
+        return True
+
+
+class MockClib:
+    def __init__(self) -> None:
+        a: bool = False
+
+    def fxIsOpen(self, val) -> bool:
+        return True
+
+    def fxIsStreaming(self, id) -> bool:
+        return True
+
 
 if __name__ == "__main__":
     pass
```

### Comparing `opensourceleg-2.2.0/opensourceleg/hardware/joints.py` & `opensourceleg-3.2.0/opensourceleg/hardware/joints.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 import os
 import time
 
 import numpy as np
 
 from ..tools.logger import Logger
 from .actuators import (
@@ -29,74 +31,102 @@
 4. Home the joint using the `home` method.
 5. Access joint information using properties such as name, gear ratio, and temperature.
 6. For testing without hardware, create a `MockJoint` instance.'
 """
 
 
 class Joint(DephyActpack):
+    """
+    Base class for reading sensor data from and controlling robotic joints using Dephy's actpack
+    (support for more actuators will be added in the future).
+
+    Parameters:
+        name (str): Name of the joint. Defaults to knee.
+        firmware_version (str): Firmware version of the actpack. Defaults to 7.2.0.
+        port (str): Port to which the actpack is connected. Defaults to None.
+        baud_rate(int): Baud rate of the actpack. Defaults to 230400.
+        gear_ratio (float): Gear ratio of the joint. Defaults to 1.0.
+        has_loadcell (bool): Is the load cell conneced to the corresponding Defaults to False.
+        actpack? If True, the load cell data will be read from the actpack and not from the RPi's GPIO
+        pins.
+        debug_level(int): Debug level to be used for the actpack's logging routine. Defaults to 0.
+        dephy_log (bool): If True, Dephy Actpack's logging routine will be Defaults to False.
+        enabled in addition to the default opensourceleg's logging routine.
+        logger (Logger): Logger instance to be used for logging. If no logger is provided, a new
+        logger will be used.
+        stop_motor_on_disconnect (bool): If True, the motor will be stopped when the actpack is
+        disconnected. Defaults to False.
+    """
+
     def __init__(
         self,
         name: str = "knee",
+        firmware_version: str = "7.2.0",
         port: str = "/dev/ttyACM0",
         baud_rate: int = 230400,
         frequency: int = 500,
         gear_ratio: float = 41.4999,
         has_loadcell: bool = False,
         logger: Logger = Logger(),
         debug_level: int = 0,
         dephy_log: bool = False,
+        stop_motor_on_disconnect: bool = False,
     ) -> None:
 
         super().__init__(
             name=name,
+            firmware_version=firmware_version,
             port=port,
             baud_rate=baud_rate,
             frequency=frequency,
             logger=logger,
             debug_level=debug_level,
             dephy_log=dephy_log,
+            stop_motor_on_disconnect=stop_motor_on_disconnect,
         )
 
         self._gear_ratio: float = gear_ratio
         self._is_homed: bool = False
         self._has_loadcell: bool = has_loadcell
 
         self._motor_zero_pos = 0.0
         self._joint_zero_pos = 0.0
 
+        self._encoder_map = None
+
         self._max_temperature: float = MAX_CASE_TEMPERATURE
 
         if "knee" in name.lower() or "ankle" in name.lower():
-            self._name: str = name
+            self.actuator_name: str = name
         else:
             self._log.warning(msg=f"[{self.__repr__()}] Invalid joint name: {name}")
             return
 
-        if os.path.isfile(path=f"./{self._name}_encoder_map.npy"):
-            coefficients = np.load(file=f"./{self._name}_encoder_map.npy")
-            self.set_encoder_map(np.polynomial.polynomial.Polynomial(coef=coefficients))
+        if os.path.isfile(path=f"./{self.actuator_name}_encoder_map.npy"):
+            coefficients = np.load(file=f"./{self.actuator_name}_encoder_map.npy")
+            self._encoder_map = np.polynomial.polynomial.Polynomial(coef=coefficients)  # type: ignore
         else:
             self._log.debug(
-                msg=f"[{self._name}] No encoder map found. Please run the make_encoder_map routine if you need more accurate joint position."
+                msg=f"[{self.actuator_name}] No encoder map found. Please run the make_encoder_map routine if you need more accurate joint position."
             )
 
     def home(
         self,
         homing_voltage: int = 2000,
         homing_frequency: int = 100,
     ) -> None:
         """
 
-        This method homes the joint by moving it to the zero position.
-        The zero position is defined as the position where the joint is fully extended.
-        This method will also make an encoder map if one does not exist.
-
-        Args:
-            homing_voltage (int): voltage in mV to use for homing
-            homing_frequency (int): frequency in Hz to use for homing
+        This method homes the joint by moving it to the zero position. The zero
+        position is defined as the position where the joint is fully extended. This method will also
+        make an encoder map if one does not exist.
+
+        Parameters:
+            homing_voltage (int): Voltage to be used for homing the joint in mV. Defaults to 2000
+            homing_frequency (int): Frequency to be used for homing the joint in Hz. Defaults to 100.
         """
 
         is_homing = True
 
         CURRENT_THRESHOLD = 5000
         VELOCITY_THRESHOLD = 0.001
 
@@ -136,49 +166,52 @@
         self.set_joint_zero_position(position=self.joint_position)
 
         time.sleep(0.1)
 
         _zero_pos: int = 0
         _zero_pos_joint: int = 0
 
-        if "ankle" in self._name.lower():
+        if "ankle" in self._actuator_name.lower():
             self.set_joint_direction(-1.0)
             self.set_joint_offset(-np.deg2rad(30))
             self.set_motor_offset(np.deg2rad(30) * self.gear_ratio)
         else:
             self.set_joint_direction(-1.0)
             self.set_joint_offset(0.0)
             self.set_motor_offset(0.0)
 
         self._is_homed = True
-        self._log.info(f"[{self._name}] Homing complete.")
+        self._log.info(f"[{self._actuator_name}] Homing complete.")
 
     def make_encoder_map(self, overwrite=False) -> None:
         """
         This method makes a lookup table to calculate the position measured by the joint encoder.
         This is necessary because the magnetic output encoders are nonlinear.
         By making the map while the joint is unloaded, joint position calculated by motor position * gear ratio
         should be the same as the true joint position.
 
         Output from this function is a file containing a_i values parameterizing the map
 
         Eqn: position = sum from i=0^5 (a_i*counts^i)
 
+        Parameters:
+            None
+
         Author: Kevin Best
                 U-M Locolab | Neurobionics Lab
                 Gitub: tkevinbest, https://github.com/tkevinbest
         """
 
         if not self.is_homed:
             self._log.warning(
                 msg=f"[{self.__repr__()}] Please home the joint before making the encoder map."
             )
             return
 
-        if os.path.exists(f"./{self._name}_encoder_map.npy") and not overwrite:
+        if os.path.exists(f"./{self._actuator_name}_encoder_map.npy") and not overwrite:
             self._log.info(
                 msg=f"[{self.__repr__()}] Encoder map exists. Skipping encoder map creation."
             )
             return
 
         self.set_mode(mode=self.control_modes.current)
         self.set_current_gains()
@@ -217,65 +250,68 @@
         _power = np.arange(4.0)
         _a_mat = np.array(_joint_encoder_array).reshape(-1, 1) ** _power
         _beta = np.linalg.lstsq(_a_mat, _output_position_array, rcond=None)
         _coeffs = _beta[0]
 
         self.set_encoder_map(np.polynomial.polynomial.Polynomial(coef=_coeffs))
 
-        np.save(file=f"./{self._name}_encoder_map.npy", arr=_coeffs)
+        np.save(file=f"./{self._actuator_name}_encoder_map.npy", arr=_coeffs)
         self._log.info(msg=f"[{self.__repr__()}] Encoder map saved.")
 
     def set_max_temperature(self, temperature: float) -> None:
         """
-        Set the maximum temperature of the motor.
+        Sets the maximum allowable temperature for the joint in degrees C. If the
+        joint's temperature exceeds this value, the joint will be safely exited.
 
-        Args:
-            temperature (float): temperature in degrees Celsius
+        Parameters:
+            temperature (float): Maximum allowable temperature in degrees C.
         """
+
         self._max_temperature = temperature
 
     def set_output_torque(self, torque: float) -> None:
         """
-        Set the output torque of the joint.
-        This is the torque that is applied to the joint, not the motor.
+        Set the output torque of the joint. That is, the prescribed torque here will be
+        scaled into motor torque using the gear ratio.
 
-        Args:
-            torque (float): torque in N_m
+        Parameters:
+            torque (float): Torque to be set in Nm.
         """
         self.set_motor_torque(torque=torque / self.gear_ratio)
 
     def set_output_position(self, position: float) -> None:
         """
-        Set the output position of the joint.
-        This is the desired position of the joint, not the motor.
-        This method automatically handles scaling by the gear raito.
+        Set the output position of the joint. This is the desired position of the joint, not
+        the motor. This method automatically handles scaling by the gear raito.
 
-        Args:
-            position (float): position in radians
+        Parameters:
+            position (float): Position to be set in radians.
         """
+
         self.set_motor_position(position=position * self.gear_ratio)
 
     def set_motor_impedance(
         self,
         kp: int = 40,
         ki: int = 400,
         K: float = 0.08922,
         B: float = 0.0038070,
         ff: int = 128,
     ) -> None:
         """
-        Set the impedance gains of the motor in real units: Nm/rad and Nm/rad/s.
+        Sets the impedance control gains for the joint in SI units: Nm/rad and Nm/(rad/s).
 
-        Args:
+        Parameters:
             kp (int): Proportional gain. Defaults to 40.
             ki (int): Integral gain. Defaults to 400.
-            K (float): Spring constant. Defaults to 0.08922 Nm/rad.
-            B (float): Damping constant. Defaults to 0.0038070 Nm/rad/s.
+            K (float): Spring constant. Defaults to 0.08922.
+            B (float): Damping constant. Defaults to 0.0038070.
             ff (int): Feedforward gain. Defaults to 128.
         """
+
         self.set_impedance_gains(
             kp=kp,
             ki=ki,
             K=int(K * NM_PER_RAD_TO_K),
             B=int(B * NM_S_PER_RAD_TO_B),
             ff=ff,
         )
@@ -286,112 +322,123 @@
         ki: int = 400,
         K: float = 100.0,
         B: float = 3.0,
         ff: int = 128,
     ) -> None:
         """
         Set the impedance gains of the joint in real units: Nm/rad and Nm/rad/s.
-        This sets the impedance at the output and automatically scales based on gear raitos.
+        This sets the impedance at the output and automatically scales based on gear ratios.
 
         Conversion:
             K_motor = K_joint / (gear_ratio ** 2)
             B_motor = B_joint / (gear_ratio ** 2)
 
-        Args:
+        Parameters:
             kp (int): Proportional gain. Defaults to 40.
             ki (int): Integral gain. Defaults to 400.
-            K (float): Spring constant. Defaults to 100 Nm/rad.
-            B (float): Damping constant. Defaults to 3.0 Nm/rad/s.
+            K (float): Spring constant. Defaults to 100.0.
+            B (float): Damping constant. Defaults to 3.0.
             ff (int): Feedforward gain. Defaults to 128.
         """
+
         self.set_motor_impedance(
             kp=kp,
             ki=ki,
             K=K / (self.gear_ratio**2),
             B=B / (self.gear_ratio**2),
             ff=ff,
         )
 
     @property
-    def name(self) -> str:
-        return self._name
+    def joint_name(self) -> str:
+        """name (str): Name of the joint."""
+        return self._actuator_name
 
     @property
     def gear_ratio(self) -> float:
+        """gear_ratio (float): Gear ratio of the joint."""
         return self._gear_ratio
 
     @property
     def max_temperature(self) -> float:
-        """Max allowed temperature of the actuator case in celsius."""
+        """max_temperature (float): Maximum allowable temperature of the actuator in degrees C."""
         return self._max_temperature
 
     @property
     def is_homed(self) -> bool:
-        """Indicates if the homing routine has been called yet."""
+        """is_homed (bool): True if the joint has been homed."""
         return self._is_homed
 
     @property
+    def encoder_map(self):
+        """encoder_map (np.array): Polynomial coefficients defining the joint encoder map from counts
+        to radians."""
+        return self._encoder_map
+
+    @property
     def output_position(self) -> float:
         """
-        Position of the output in radians.
-        This is calculated by scaling the motor angle with the gear ratio.
-        Note that this method does not consider compliance from an SEA.
+        output_position (float): Position of the output in radians. This is calculated by scaling the
+        motor angle with the gear ratio. Note that this method does not consider the presence of an
+        SEA.
         """
         return self.motor_position / self.gear_ratio
 
     @property
     def output_velocity(self) -> float:
         """
-        Velocity of the output in radians.
-        This is calculated by scaling the motor angle with the gear ratio.
-        Note that this method does not consider compliance from an SEA.
+        output_velocity (float): Velocity of the output in radians. This is calculated by scaling the
+        motor angle with the gear ratio. Note that this method does not consider the presence of an
+        SEA.
         """
         return self.motor_velocity / self.gear_ratio
 
     @property
     def joint_torque(self) -> float:
         """
-        Torque at the joint output in Nm.
-        This is calculated using motor current, k_t, and the gear ratio.
+        joint_torque (float): Torque at the joint output in Nm. This is calculated using motor
+        current, k_t, and the gear ratio.
         """
         return self.motor_torque * self.gear_ratio
 
 
 class MockJoint(Joint, MockDephyActpack):
     """
     Mock Joint class for testing the Joint class\n
     Inherits everything from the Joint class and the MockDephyActpack class
     except for the Joint constructor.
     """
 
     def __init__(
         self,
         name: str = "knee",
+        firmware_version: str = "7.2.0",
         port: str = "/dev/ttyACM0",
         baud_rate: int = 230400,
         frequency: int = 500,
         gear_ratio: float = 41.4999,
         has_loadcell: bool = False,
         logger: Logger = Logger(),
         debug_level: int = 0,
         dephy_log: bool = False,
+        stop_motor_on_disconnect: bool = False,
     ) -> None:
 
-        MockDephyActpack.__init__(self, name, port)
+        MockDephyActpack.__init__(self, name=name, port=port)
         self._gear_ratio: float = gear_ratio
         self._is_homed: bool = False
         self._has_loadcell: bool = has_loadcell
 
         self._motor_zero_pos = 0.0
         self._joint_zero_pos = 0.0
 
         self._max_temperature: float = MAX_CASE_TEMPERATURE
 
         if "knee" in name.lower() or "ankle" in name.lower():
-            self._name: str = name
+            self._actuator_name: str = name
         else:
             self._log.warning(msg=f"[{self.__repr__()}] Invalid joint name: {name}")
             return
 
 
 if __name__ == "__main__":
     joint = MockJoint()
```

### Comparing `opensourceleg-2.2.0/opensourceleg/hardware/sensors.py` & `opensourceleg-3.2.0/opensourceleg/hardware/sensors.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,16 +28,20 @@
 8. Obtain IMU data using the `get_data` method.
 
 """
 
 
 class StrainAmp:
     """
-    A class to directly manage the 6ch strain gauge amplifier over I2C.
-    An instance of this class is created by the loadcell class.
+    A class to interface with the 6ch strain gauge amplifier over I2C/RPi GPIO.
+
+    Parameters:
+        bus (int): I2C bus to be used. If no bus is provided, the default bus will be used.
+        I2C_addr (str): I2C address of the strain gauge amplifier. Defaults to 0x66.
+
     Author: Mitry Anderson
     """
 
     # register numbers for the "ezi2c" interface on the strainamp
     # found in source code here: https://github.com/JFDuval/flexsea-strain/tree/dev
     MEM_R_CH1_H = 8
     MEM_R_CH1_L = 9
@@ -63,90 +67,121 @@
         self.is_streaming = True
         self.data: list[int] = []
         self.failed_reads = 0
 
     def __repr__(self) -> str:
         return f"StrainAmp"
 
-    def read_uncompressed_strain(self):
-        """Used for an older version of the strain amp firmware (at least pre-2017)"""
-        data = []
-        for i in range(self.MEM_R_CH1_H, self.MEM_R_CH6_L + 1):
-            data.append(self._SMBus.read_byte_data(self.addr, i))
+    def _read_compressed_strain(self):
+        """
+        Reads the compressed strain data from the strain gauge amplifier. This
+        method is recommended for a newer version of the strain amplifier firmware (post-2017).
 
-        return self._unpack_uncompressed_strain(data)
+        Parameters:
+            None
+
+        Returns:
+            None
+
+        Raises:
+            Exception: Unresponsive load cell
+
+        """
 
-    def _read_compressed_strain(self):
-        """Used for more recent versions of strain amp firmware"""
         try:
             self.data = self._SMBus.read_i2c_block_data(self.addr, self.MEM_R_CH1_H, 10)
             self.failed_reads = 0
         except OSError as e:
             self.failed_reads += 1
             # print("\n read failed")
             if self.failed_reads >= 5:
                 raise Exception("Load cell unresponsive.")
         # unpack them and return as nparray
         return self._unpack_compressed_strain(self.data)
 
     def update(self):
-        """Called to update data of strain amp. Also returns data.
-        Data is median filtered (max one sample delay) to avoid i2c issues.
         """
+        Updates the strain gauge amplifier's attributes by reading the strain gauge
+        amplifier's data stream if the strain gauge amplifier is connected. The updated data is
+        median filtered (maximum sample delay of one) to avoid I2C issues.
+
+        Parameters:
+            None
+
+        Returns:
+            None
+
+        """
+
         self.genvars[self.indx, :] = self._read_compressed_strain()
         self.indx: int = (self.indx + 1) % 3
         return np.median(a=self.genvars, axis=0)
 
     @staticmethod
     def _unpack_uncompressed_strain(data):
-        """Used for an older version of the strain amp firmware (at least pre-2017)"""
+        """
+        Unpacks the uncompressed strain data. This method is recommended for an
+        older version of the strain amplifier firmware (pre-2017).
+
+        Parameters:
+            data: Uncompressed strain data to be unpacked.
+
+        Returns:
+            None
+
+        """
         ch1 = (data[0] << 8) | data[1]
         ch2 = (data[2] << 8) | data[3]
         ch3 = (data[4] << 8) | data[5]
         ch4 = (data[6] << 8) | data[7]
         ch5 = (data[8] << 8) | data[9]
         ch6 = (data[10] << 8) | data[11]
         return np.array(object=[ch1, ch2, ch3, ch4, ch5, ch6])
 
     @staticmethod
     def _unpack_compressed_strain(data):
-        """Used for more recent versions of strainamp firmware"""
+        """
+        Unpacks the compressed strain data. This method is recommended for a
+        newer version of the strain amplifier firmware (post-2017).
+
+        Parameters:
+            data: Compressed strain data to be unpacked.
+
+        Returns:
+            None
+        """
         return np.array(
             object=[
                 (data[0] << 4) | ((data[1] >> 4) & 0x0F),
                 ((data[1] << 8) & 0x0F00) | data[2],
                 (data[3] << 4) | ((data[4] >> 4) & 0x0F),
                 ((data[4] << 8) & 0x0F00) | data[5],
                 (data[6] << 4) | ((data[7] >> 4) & 0x0F),
                 ((data[7] << 8) & 0x0F00) | data[8],
             ]
         )
 
-    @staticmethod
-    def strain_data_to_wrench(
-        unpacked_strain, loadcell_matrix, loadcell_zero, exc=5, gain=125
-    ):
-        """Converts strain values between 0 and 4095 to a wrench in N and Nm"""
-        loadcell_signed = (unpacked_strain - 2048) / 4095 * exc
-        loadcell_coupled = loadcell_signed * 1000 / (exc * gain)
-        return np.reshape(
-            np.transpose(a=loadcell_matrix.dot(np.transpose(a=loadcell_coupled)))
-            - loadcell_zero,
-            (6,),
-        )
 
-    @staticmethod
-    def wrench_to_strain_data(measurement, loadcell_matrix, exc=5, gain=125):
-        """Wrench in N and Nm to the strain values that would give that wrench"""
-        loadcell_coupled = (np.linalg.inv(loadcell_matrix)).dot(measurement)
-        loadcell_signed = loadcell_coupled * (exc * gain) / 1000
-        return ((loadcell_signed / exc) * 4095 + 2048).round(0).astype(int)
+class Loadcell:
+    """
+    Class to interface with the load cell. It contains various helper functions to read the load cell
+    data and convert it to forces and moments.
 
+    Parameters:
+        dephy_mode (bool): Is the load cell connected to the actpack? If True, the
+        load cell data will be read from the actpack and not from the RPi's GPIO pins. Defaults to False.
+        joint (Joint): Joint to which the load cell is connected. Defaults to None.
+        amp_gain (float): Amplifier gain of the load cell strain amplifier. Defaults to 125.0.
+        exc (float): Excitation voltage of the load cell strain amplifier. Defaults to False.
+        loadcell_matrix (np.ndarray(6, 6)): Calibration matrix for the load cell.
+        This matrix is used to convert the load cell's raw data to forces and moments. Defaults to None.
+        logger (Logger): Logger instance to be used for logging. If no logger is provided,
+        a new logger will be used. Defaults to None
+    """
 
-class Loadcell:
     def __init__(
         self,
         dephy_mode: bool = False,
         joint: Joint = None,
         amp_gain: float = 125.0,
         exc: float = 5.0,
         loadcell_matrix=None,
@@ -177,22 +212,33 @@
         self._zeroed = False
         self._log: Logger = logger  # type: ignore
 
     def __repr__(self) -> str:
         return f"Loadcell"
 
     def reset(self):
+        """
+        Resets the load cell's zero offset.
+
+        Parameters:
+            None
+        """
         self._zeroed = False
         self._loadcell_zero = np.zeros(shape=(1, 6), dtype=np.double)
 
     def update(self, loadcell_zero=None) -> None:
         """
-        Queries the loadcell for the latest data.
-        Latest data can then be accessed via properties, e.g. loadcell.Fx.
+        Updates the load cell's attributes by reading and converting the load cell's
+        data. You can access the load cell forces and moments using the loadcell attributes like
+        loadcell.fx, loadcell.mx, etc.
+
+        Parameters:
+            loadcell_zero (np.array): Zero offset of the load cell. Defaults to None.
         """
+
         if self._is_dephy:
             loadcell_signed = (
                 (self._joint.genvars - self._offset) / self._adc_range * self._exc
             )
         else:
             assert self._lc is not None
             loadcell_signed = (
@@ -222,17 +268,23 @@
             for safety_attribute_name in self._safety_attributes:
                 self._log.debug(
                     msg=f"[{self.__repr__()}] Safety mechanism in-place for {safety_attribute_name}: {getattr(self, safety_attribute_name)}"
                 )
 
     def initialize(self, number_of_iterations: int = 2000) -> None:
         """
-        Obtains the initial loadcell reading (aka) loadcell_zero.
-        This is automatically subtraced off for subsequent calls of the update method.
+        Initializes the load cell's zero offset by taking the average of the load cell's raw
+        data over a given number of iterations.
+
+        Parameters:
+            number_of_iterations (int): Number of iterations to be used. Defaults to 2000.
+                                        for the load cell's zero offset calibration.
+
         """
+
         ideal_loadcell_zero = np.zeros(shape=(1, 6), dtype=np.double)
 
         if not self._zeroed:
             self._log.info(
                 f"[{self.__repr__()}] Initiating zeroing routine, please ensure that there is no ground contact force."
             )
             time.sleep(1)
@@ -266,72 +318,64 @@
             == "y"
         ):
             self.reset()
             self.initialize()
 
     @property
     def is_zeroed(self) -> bool:
-        """Indicates if load cell zeroing routine has been called."""
+        """is_zeroed (bool): True if the load cell zeroing routine has been successfully completed."""
         return self._zeroed
 
     @property
     def fx(self):
         """
-        Latest force in the x (medial/lateral) direction in Newtons.
-        If using the standard OSL setup, this is positive towards the user's right.
+        fx (float): Force in the x direction in N.
         """
         return self.loadcell_data[0]
 
     @property
     def fy(self):
         """
-        Latest force in the y (anterior/posterior) direction in Newtons.
-        If using the standard OSL setup, this is positive in the posterior direction.
+        fy (float): Force in the y direction in N.
         """
         return self.loadcell_data[1]
 
     @property
     def fz(self):
         """
-        Latest force in the z (vertical) direction in Newtons.
-        If using the standard OSL setup, this should be positive downwards.
-        i.e. quiet standing on the OSL should give a negative Fz.
+        fz (float): Force in the z direction in N.
         """
         return self.loadcell_data[2]
 
     @property
     def mx(self):
         """
-        Latest moment about the x (medial/lateral) axis in Nm.
-        If using the standard OSL setup, this axis is positive towards the user's right.
+        mx (float): Moment in the x direction in Nm.
         """
         return self.loadcell_data[3]
 
     @property
     def my(self):
         """
-        Latest moment about the y (anterior/posterior) axis in Nm.
-        If using the standard OSL setup, this axis is positive in the posterior direction.
+        my (float) Moment in the y direction in Nm.
         """
         return self.loadcell_data[4]
 
     @property
     def mz(self):
         """
-        Latest moment about the z (vertical) axis in Nm.
-        If using the standard OSL setup, this axis is positive towards the ground.
+        mz (float): Moment in the z direction in Nm.
+
         """
         return self.loadcell_data[5]
 
     @property
     def loadcell_data(self):
         """
-        Returns a vector of the latest loadcell data.
-        [Fx, Fy, Fz, Mx, My, Mz]
-        Forces in N, moments in Nm.
+        loadcell_data (np.array(6)): Raw vector of the load cell data i.e. [fx, fy, fz, mx, my, mz]. Forces are in N and moments are in Nm.
         """
         if self._loadcell_data is not None:
             return self._loadcell_data[0]
         else:
             return [0.0, 0.0, 0.0, 0.0, 0.0, 0.0]
 
 
@@ -483,29 +527,39 @@
     """z direction acceleration in g"""
     imu_time_sta: float = 0
     imu_filter_gps_time_week_num: float = 0
 
 
 class IMULordMicrostrain:
     """
-    Sensor class for the Lord Microstrain IMU.
+    Base class to interface with the Lord Microstrain IMU.
     Requires the MSCL library from Lord Microstrain (see below for install instructions).
 
     As configured, this class returns euler angles (rad), angular rates (rad/s), and accelerations (g).
 
+    Parameters:
+        port (str): Port to which the IMU is connected. If no port is provided, the default port will be used. Defaults to /dev/ttyUSB0.
+        baud_rate (int): Baud rate of the IMU. Defaults to 921600.
+        timeout (int): Timeout for reading data from the IMU in milliseconds. Defaults to 500.
+        sample_rate (int): Sample rate of the IMU in Hz. Defaults to 100.
+
     Example:
         imu = IMULordMicrostrain()
         imu.start_streaming()
         while in loop:
             imu.get_data()
         imu.stop_streaming()
 
     Resources:
         * To install, download the pre-built package for raspian at https://github.com/LORD-MicroStrain/MSCL/tree/master
         * Full documentation for their library can be found at https://lord-microstrain.github.io/MSCL/Documentation/MSCL%20API%20Documentation/index.html.
+
+    Author: Kevin Best
+            U-M Locolab | Neurobionics Lab
+            Gitub: tkevinbest, https://github.com/tkevinbest
     """
 
     def __init__(
         self, port=r"/dev/ttyUSB0", baud_rate=921600, timeout=500, sample_rate=100
     ):
         import sys
 
@@ -557,23 +611,41 @@
         )  # Clean the internal circular buffer.
         self.imu_data = IMUDataClass()
 
     def __repr__(self) -> str:
         return f"IMULordMicrostrain"
 
     def start_streaming(self):
+        """
+        Starts streaming data from the IMU.
+
+        Parameters:
+            None
+        """
+
         self.imu.resume()
 
     def stop_streaming(self):
+        """
+        Stops streaming data from the IMU.
+
+        Paramters:
+            None
+        """
+
         self.imu.setToIdle()
 
     def get_data(self):
         """
-        Get IMU data from the Lord Microstrain IMU
+        Get data from the Lord Microstrain IMU
+
+        Parameters:
+            None
         """
+
         imu_packets = self.imu.getDataPackets(self.timeout)
         if len(imu_packets):
             # Read all the information from the first packet as float.
             raw_imu_data = {
                 data_point.channelName(): data_point.as_float()
                 for data_point in imu_packets[-1].data()
             }
```

### Comparing `opensourceleg-2.2.0/opensourceleg/hardware/thermal.py` & `opensourceleg-3.2.0/opensourceleg/hardware/thermal.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         R: Resistance
 
     Implementation:
         1: The model is updated at every time step with the current and the ambient temperature.
         2: The model can be used to predict the temperature of the winding and the case at any time step.
         3: The model can also be used to scale the torque based on the temperature of the winding and the case.
 
-    Args:
+    Parameters:
         ambient (float): Ambient temperature in Celsius. Defaults to 21.
         params (dict): Dictionary of parameters. Defaults to dict().
         temp_limit_windings (float): Maximum temperature of the windings in Celsius. Defaults to 115.
         soft_border_C_windings (float): Soft border of the windings in Celsius. Defaults to 15.
         temp_limit_case (float): Maximum temperature of the case in Celsius. Defaults to 80.
         soft_border_C_case (float): Soft border of the case in Celsius. Defaults to 5.
 
@@ -84,15 +84,15 @@
     def __repr__(self) -> str:
         return f"ThermalModel"
 
     def update(self, dt: float = 1 / 200, motor_current: float = 0) -> None:
         """
         Updates the temperature of the winding and the case based on the current and the ambient temperature.
 
-        Args:
+        Parameters:
             dt (float): Time step in seconds. Defaults to 1/200.
             motor_current (float): Motor current in mA. Defaults to 0.
 
         Dynamics:
             1: self.C_w * d self.T_w /dt = (I^2)R + (self.T_c-self.T_w)/self.R_WC
             2: self.C_c * d self.T_c /dt = (self.T_w-self.T_c)/self.R_WC + (self.T_w-self.T_a)/self.R_CA
         """
@@ -110,15 +110,15 @@
         self.T_w += dt * dTw_dt
         self.T_c += dt * dTc_dt
 
     def update_and_get_scale(self, dt, motor_current: float = 0, FOS: float = 1.0):
         """
         Updates the temperature of the winding and the case based on the current and the ambient temperature and returns the scale factor for the torque.
 
-        Args:
+        Parameters:
             dt (float): Time step in seconds.
             motor_current (float): Motor current in mA. Defaults to 0.
             FOS (float): Factor of safety. Defaults to 3.0.
 
         Returns:
             float: Scale factor for the torque.
```

### Comparing `opensourceleg-2.2.0/opensourceleg/safety/sensors.py` & `opensourceleg-3.2.0/opensourceleg/safety/sensors.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-2.2.0/opensourceleg/tools/logger.py` & `opensourceleg-3.2.0/opensourceleg/tools/logger.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,19 +30,21 @@
 is instantiated.
 
 """
 
 
 class Logger(logging.Logger):
     """
-    Logger class is a class that logs attributes from a class to a csv file
+    Custom logger class to log debug information and data to a csv file.
+    This class inherits from the logging.Logger class and adds additional methods.
 
-    Methods:
-        __init__(self, container: object, file_path: str, logger: logging.Logger = None) -> None
-        log(self) -> None
+    Parameters:
+        file_path (str): path to save the log file. If you want to save the log file in the
+                         current working directory, use './' followed by the file name. Defaults to ./osl.
+        log_format (str): Format of the log message. Defaults to [%(asctime)s] %(levelname)s: %(message)s.
     """
 
     def __init__(
         self,
         file_path: str = "./osl",
         log_format: str = "[%(asctime)s] %(levelname)s: %(message)s",
     ) -> None:
@@ -87,53 +89,62 @@
         self._is_logging = False
 
     def __repr__(self) -> str:
         return f"Logger"
 
     def set_file_level(self, level: str = "DEBUG") -> None:
         """
-        Sets the level of the logger
+        Sets the file level of the logger. Anything below this level will not be logged to
+        the .log file. There are five standard levels: DEBUG, INFO, WARNING, ERROR, and CRITICAL.
+        DEBUG is the lowest level and CRITICAL is the highest level.
 
-        Args:
-            level (str): Level of the logger
+        Parameters:
+            level (str): Level of the logger. Defaults to DEBUG.
         """
         if level not in self._log_levels.keys():
             self.warning(msg=f"Invalid logging level: {level}")
 
         self._file_handler.setLevel(level=self._log_levels[level])
 
     def set_stream_level(self, level: str = "INFO") -> None:
         """
-        Sets the level of the logger
+        Sets the stream level of the logger. Anything below this level will not be logged to
+        the console. There are five standard levels: DEBUG, INFO, WARNING, ERROR, and CRITICAL.
+        DEBUG is the lowest level and CRITICAL is the highest level.
 
-        Args:
-            level (str): Level of the logger
+        Parameter:
+            level (str): Level to be set for the logger's stream. Defaults to INFO
         """
         if level not in self._log_levels.keys():
             self.warning(msg=f"Invalid logging level: {level}")
 
         self._stream_handler.setLevel(level=self._log_levels[level])
 
     def add_attributes(
         self, container: Union[object, dict[Any, Any]], attributes: list[str]
     ) -> None:
         """
-        Adds class instance and attributes to log
+        Adds the attributes to be logged to the logger.
 
-        Args:
-            container (object, dict): Container can either be an object (instance of a class)
-                or a Dict containing the attributes to be logged.
-            attributes (list[str]): List of attributes to log
+        Parameters:
+            container (Union[object, dict[Any, Any]]): Class instance or dictionary to log the attributes
+                                                       from. Defaults to None.
+            attributes (list[str]): List of attribute names to log. The attribute names should be strings
+                                    and should match the attribute names of the class instance or dictionary. Defaults to None.
         """
         self._containers.append(container)
         self._attributes.append(attributes)
 
     def data(self) -> None:
         """
-        Logs the attributes of the class instance to the csv file
+        Logs the data from the added attributes to a csv file. This csv file
+        will be saved at the file path specified in the constructor.
+
+        Parameters:
+            None
         """
         header_data = []
         data = []
 
         if not self._is_logging:
             for container, attributes in zip(self._containers, self._attributes):
                 for attribute in attributes:
@@ -160,15 +171,18 @@
                     data.append(getattr(container, attribute))
 
         self._writer.writerow(data)
         self._file.flush()
 
     def close(self) -> None:
         """
-        Closes the csv file
+        Closes the data log file.
+
+        Parameters:
+            None
         """
         self._file.close()
 
 
 if __name__ == "__main__":
     local_logger = Logger(file_path="./test_log")
     local_variable_1 = 100
```

### Comparing `opensourceleg-2.2.0/opensourceleg/tools/units.py` & `opensourceleg-3.2.0/opensourceleg/tools/units.py`

 * *Files 5% similar despite different names*

```diff
@@ -129,17 +129,17 @@
         return f"voltage"
 
 
 def convert_to_default(value: float, from_unit: float) -> float:
     """
     Convert a value from an user unit to the default unit.
 
-    Args:
-        value (float): Value to convert
-        from_unit (float): Unit corresponding to the value that is being converted to the default unit.
+    Parameters:
+        value (float): Value to be converted to the default unit.
+        from_unit (float): Unit of the value to be converted to the default unit.
 
     Returns:
         float: Converted value in default units.
 
     Example:
         >>> convert_to_default(2, units.current.A)
         2000 # returns value in mA, which is the default unit for current
@@ -153,17 +153,17 @@
     return value * from_unit
 
 
 def convert_from_default(value: float, to_unit: float) -> float:
     """
     Convert a value from the default unit to an user unit.
 
-    Args:
-        value (float): Value to convert
-        to_unit (float): Desired unit for the converted value.
+    Parameters:
+        value (float): Value to be converted to the desired unit.
+        to_unit (float): Desired unit of the value to be converted to.
 
     Returns:
         float: Converted value in desired unit.
 
     Example:
 
         >>> convert_from_default(2000, units.current.A)
```

### Comparing `opensourceleg-2.2.0/opensourceleg/tools/utilities.py` & `opensourceleg-3.2.0/opensourceleg/tools/utilities.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,73 +44,84 @@
 
     def handle_signal(self, signum, frame):
         self.kill_now = True
 
     def get_fade(self):
         # interpolates from 1 to zero with soft fade out
         if self._kill_soon:
-            t = time.time() - self._soft_kill_time
+            t = time.monotonic() - self._soft_kill_time
             if t >= self._fade_time:
                 return 0.0
             return 1.0 - (t / self._fade_time)
         return 1.0
 
     _kill_now = False
     _kill_soon = False
 
     @property
     def kill_now(self):
         if self._kill_now:
             return True
         if self._kill_soon:
-            t = time.time() - self._soft_kill_time
+            t = time.monotonic() - self._soft_kill_time
             if t > self._fade_time:
                 self._kill_now = True
         return self._kill_now
 
     @kill_now.setter
     def kill_now(self, val):
         if val:
             if self._kill_soon:  # if you kill twice, then it becomes immediate
                 self._kill_now = True
             else:
                 if self._fade_time > 0.0:
                     self._kill_soon = True
-                    self._soft_kill_time = time.time()
+                    self._soft_kill_time = time.monotonic()
                 else:
                     self._kill_now = True
         else:
             self._kill_now = False
             self._kill_soon = False
             self._soft_kill_time = None
 
 
 class SoftRealtimeLoop:
     """
-    Soft Realtime Loop---a class designed to allow clean exits from infinite loops
-    with the potential for post-loop cleanup operations executing.
+    A class to create soft real-time loops for running control algorithms. This class was designed to allow clean exits
+    from infinite loops with the potential for executing post-loop cleanup operations. The SoftRealTimeLoop can also be
+    used as a with statement as it has a __enter__ and __exit__ method. Please read the tutorials for more information.
+
+    Parameters:
+        dt (float): Time step to be used for the real-time loop in seconds. Defaults to 0.001
+        fade (float): Fade factor to be used for the real-time loop. Defaults to 0.0.
+        report (bool): If True, the loop will report useful information regarding the loop like the number of cycles,
+        average error in the loop, percentage of time spent sleeping, etc. Defaults to False.
+
+    More Info:
+        Soft Realtime Loop---a class designed to allow clean exits from infinite loops
+        with the potential for post-loop cleanup operations executing.
+
+        The Loop Killer object watches for the key shutdown signals on the UNIX operating system (which runs on the PI)
+        when it detects a shutdown signal, it sets a flag, which is used by the Soft Realtime Loop to stop iterating.
+        Typically, it detects the CTRL-C from your keyboard, which sends a SIGTERM signal.
+
+        the function_in_loop argument to the Soft Realtime Loop's blocking_loop method is the function to be run every loop.
+        A typical usage would set function_in_loop to be a method of an object, so that the object could store program state.
+        See the 'ifmain' for two examples.
 
-    The Loop Killer object watches for the key shutdown signals on the UNIX operating system (which runs on the PI)
-    when it detects a shutdown signal, it sets a flag, which is used by the Soft Realtime Loop to stop iterating.
-    Typically, it detects the CTRL-C from your keyboard, which sends a SIGTERM signal.
-
-    the function_in_loop argument to the Soft Realtime Loop's blocking_loop method is the function to be run every loop.
-    A typical usage would set function_in_loop to be a method of an object, so that the object could store program state.
-    See the 'ifmain' for two examples.
-
-    This library will soon be hosted as a PIP module and added as a python dependency.
-    https://github.com/UM-LoCoLab/NeuroLocoMiddleware/blob/main/SoftRealtimeLoop.py
+        This library will soon be hosted as a PIP module and added as a python dependency.
+        https://github.com/UM-LoCoLab/NeuroLocoMiddleware/blob/main/SoftRealtimeLoop.py
 
     # Author: Gray C. Thomas, Ph.D
     # https://github.com/GrayThomas, https://graythomas.github.io
 
     """
 
     def __init__(self, dt=0.001, report=False, fade=0.0):
-        self.t0 = self.t1 = time.time()
+        self.t0 = self.t1 = time.monotonic()
         self.killer = LoopKiller(fade_time=fade)
         self.dt = dt
         self.ttarg = None
         self.sum_err = 0.0
         self.sum_var = 0.0
         self.sleep_t_agg = 0.0
         self.n = 0
@@ -130,75 +141,91 @@
             print(
                 "\tpercent of time sleeping: %.1f %%"
                 % (self.sleep_t_agg / self.time() * 100.0)
             )
 
     @property
     def fade(self):
+        """fade (float): Fade factor being used for the real-time loop."""
         return self.killer.get_fade()
 
     def run(self, function_in_loop, dt=None):
+        """
+        Runs the real-time loop with the given function.
+
+        Paramaters:
+            function_in_loop (Callable[[Any], Any]): Function to be run within the real-time loop.
+            dt (float): Time step to be used for the real-time loop. If None, the time step given in the
+                        constructor will be used. Defaults to None.
+        """
         if dt is None:
             dt = self.dt
-        self.t0 = self.t1 = time.time() + dt
+        self.t0 = self.t1 = time.monotonic() + dt
         while not self.killer.kill_now:
             ret = function_in_loop()
             if ret == 0:
                 self.stop()
-            while time.time() < self.t1 and not self.killer.kill_now:
+            while time.monotonic() < self.t1 and not self.killer.kill_now:
                 if signal.sigtimedwait(
                     [signal.SIGTERM, signal.SIGINT, signal.SIGHUP], 0
                 ):
                     self.stop()
             self.t1 += dt
 
     def stop(self):
+        """
+        Safely stops the real-time loop's run method and exits the loop.
+
+        Parameters:
+            None
+        """
         self.killer.kill_now = True
 
     def time(self):
-        return time.time() - self.t0
+        return time.monotonic() - self.t0
 
     def time_since(self):
-        return time.time() - self.t1
+        return time.monotonic() - self.t1
 
     def __iter__(self):
-        self.t0 = self.t1 = time.time() + self.dt
+        self.t0 = self.t1 = time.monotonic() + self.dt
         return self
 
     def __next__(self):
         if self.killer.kill_now:
             raise StopIteration
 
         while (
-            time.time() < self.t1 - 2 * PRECISION_OF_SLEEP and not self.killer.kill_now
+            time.monotonic() < self.t1 - 2 * PRECISION_OF_SLEEP
+            and not self.killer.kill_now
         ):
-            t_pre_sleep = time.time()
+            t_pre_sleep = time.monotonic()
             time.sleep(
-                max(PRECISION_OF_SLEEP, self.t1 - time.time() - PRECISION_OF_SLEEP)
+                max(PRECISION_OF_SLEEP, self.t1 - time.monotonic() - PRECISION_OF_SLEEP)
             )
-            self.sleep_t_agg += time.time() - t_pre_sleep
+            self.sleep_t_agg += time.monotonic() - t_pre_sleep
 
-        while time.time() < self.t1 and not self.killer.kill_now:
+        while time.monotonic() < self.t1 and not self.killer.kill_now:
             try:
                 if signal.sigtimedwait(
                     [signal.SIGTERM, signal.SIGINT, signal.SIGHUP], 0
                 ):
                     self.stop()
             except AttributeError:
                 pass
 
         if self.killer.kill_now:
             raise StopIteration
         self.t1 += self.dt
         if self.ttarg is None:
             # inits ttarg on first call
-            self.ttarg = time.time() + self.dt
+            self.ttarg = time.monotonic() + self.dt
             # then skips the first loop
             return self.t1 - self.t0
-        error = time.time() - self.ttarg  # seconds
+        error = time.monotonic() - self.ttarg  # seconds
         self.sum_err += error
         self.sum_var += error**2
         self.n += 1
         self.ttarg += self.dt
         return self.t1 - self.t0
 
 
@@ -230,14 +257,19 @@
     """
     Creates a signal that ramps between 0 and 1 at the specified rate.
     Looks like a trapezoid in the time domain
     Used to slowly enable joint torque for smooth switching at startup.
     Call saturatingRamp.update() to update the value of the ramp and return the value.
     Can also access saturatingRamp.value without updating.
 
+    Parameters:
+        loop_frequency (int): Frequency of the loop in Hz. This is used to calculate the time step for
+        the ramp. Defaults to 100.
+        ramp_time (float): Time to complete the ramp. Defaults to 1.0.
+
     Example usage:
         ramp = saturatingRamp(100, 1.0)
 
         # In loop
             torque = torque * ramp.update(enable_ramp)
 
     Author: Kevin Best
@@ -254,23 +286,21 @@
         self.value = 0.0
 
     def __repr__(self) -> str:
         return f"SaturatingRamp"
 
     def update(self, enable_ramp=False):
         """
-        Updates the ramp value and returns it as a float.
-        If enable_ramp is true, ramp value increases
-        Otherwise decreases.
+        Updates the ramp value and returns the current value of the ramp.
 
         Example usage:
             torque = torque * ramp.update(enable_ramp)
 
-        Args:
-            enable_ramp (bool, optional): If enable_ramp is true, ramp value increases. Defaults to False.
+        Parameters:
+            enable_ramp (bool): If True, the ramp value increases. If False, the ramp value decreases. Defaults to False.
 
         Returns:
             value (float): Scalar between 0 and 1.
         """
         if enable_ramp:
             delta = self.delta_per_update
         else:
@@ -279,15 +309,18 @@
 
         self.value = min(max(self.value, 0), 1)
         return self.value
 
 
 def get_active_ports():
     """
-    Lists active serial ports.
+    Finds and returns the active serial ports. This method is useful to find which port the hardware is connected to.
+
+    Parameters:
+        None
     """
     if sys.platform.startswith("linux") or sys.platform.startswith("cygwin"):
         ports = glob.glob("/dev/tty[A-Za-z]C*")
     elif sys.platform.startswith("darwin"):
         ports = glob.glob("/dev/tty.*")
     elif sys.platform.startswith("win"):
         ports = ["COM%s" % (i + 1) for i in range(256)]
@@ -307,14 +340,21 @@
 
 
 def clamp_within_vector_range(input_value, input_vector):
     """
     This function ensures that input_value remains within the range spanned by the input_vector.
     If the input_value falls outside the vector's bounds, it'll return the appropriate max or min value from the vector.
 
+    Parameters:
+        input_value (float): Value to be clamped within the vector's range.
+        input_vector (list[float]): Vector to be used to clamp the input value.
+
+    Returns:
+        Any
+
     Example:
         clamp_within_vector_range(10, [0,1,2,3]) = 3
         clamp_within_vector_range(-10, [0,1,2,3]) = 0
 
     Author:
         Kevin Best, 8/7/2023
         https://github.com/tkevinbest
@@ -324,33 +364,43 @@
     return max(min(input_value, max_allowed), min_allowed)
 
 
 def get_ctype_args(input_header: str):
     """
     Converts a header file from C string into a list of ctypes arguments.
 
-    Keyword Arguments:
-        inputHeader: string from header file, such as "const struct0_T *thighIMU, double Knee_joint_position,
-          double Ankle_joint_position"
-    returns:
-        ctypes list of the appropriate types for the inputs, such as (ctypes.c_void_p, ctypes.c_double, ctypes.c_double)
+    Parameters:
+        input_header (str): string from header file, such as "const struct0_T *thighIMU, double Knee_joint_position,
+                           double Ankle_joint_position"
+
+    Returns:
+        list[ctypes]: ctypes list of the appropriate types for the inputs, such as (ctypes.c_void_p, ctypes.c_double, ctypes.c_double)
 
     Author: Kevin Best,
     https://github.com/tkevinbest
     """
     input_header_split = input_header.split(",")
 
     arg_list = [get_ctype(token) for token in input_header_split]
     return arg_list
 
 
 def get_ctype(token):
     """
     Converts a single token from a header file into a ctypes argument.
 
+    Parameters:
+        token (float): Single token from a header file, such as 'const'
+
+    Returns:
+        c_type
+
+    Raises:
+        Exception: Invalid Token
+
     Author: Kevin Best, 8/7/2023
     https://github.com/tkevinbest
     """
     if "*" in token:
         out = ctypes.c_void_p
     elif "double" in token:
         out = ctypes.c_double
```

### Comparing `opensourceleg-2.2.0/pyproject.toml` & `opensourceleg-3.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "opensourceleg"
-version = "2.2.0"
+version = "3.2.0"
 description = "An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prostheses."
 readme = "README.md"
 authors = ["Open-source Leg <opensourceleg@gmail.com>"]
-license = "GNU LGPL v2.1"
+license = "GNU LESSER GENERAL PUBLIC LICENSE v2.1"
 repository = "https://github.com/neurobionics/opensourceleg"
 homepage = "https://github.com/neurobionics/opensourceleg"
 
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
 keywords = []  #! Update me
 
 # Pypi classifiers: https://pypi.org/classifiers/
@@ -27,23 +27,23 @@
   "Programming Language :: Python :: 3.9",
 ]
 
 [virtualenvs]
 in-project = true
 
 [tool.poetry.dependencies]
-python = ">=3.9,<4.0.0"
+python = ">=3.11,<4.0.0"
 pyserial = "^3.5"
-flexsea = "^8.0.1"
+flexsea = "^12.0.3"
 smbus2 = "^0.4.2"
 numpy = "^1.24.3"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.1"
-black = {version = ">=22.3,<25.0", allow-prereleases = true}
+black = {version = ">=24.3,<25.0", allow-prereleases = true}
 darglint = "^1.8.1"
 isort = {extras = ["colors"], version = "^5.10.1"}
 mypy = ">=0.991,<1.1"
 mypy-extensions = "^0.4.3"
 pre-commit = "^2.15.0"
 pydocstyle = "^6.1.1"
 pylint = ">=2.13.7,<4.0.0"
```

### Comparing `opensourceleg-2.2.0/PKG-INFO` & `opensourceleg-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: opensourceleg
-Version: 2.2.0
+Version: 3.2.0
 Summary: An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prostheses.
 Home-page: https://github.com/neurobionics/opensourceleg
-License: GNU LGPL v2.1
+License: GNU LESSER GENERAL PUBLIC LICENSE v2.1
 Author: Open-source Leg
 Author-email: opensourceleg@gmail.com
-Requires-Python: >=3.9,<4.0.0
+Requires-Python: >=3.11,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: flexsea (>=8.0.1,<9.0.0)
+Requires-Dist: flexsea (>=12.0.3,<13.0.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pyserial (>=3.5,<4.0)
 Requires-Dist: smbus2 (>=0.4.2,<0.5.0)
 Project-URL: Repository, https://github.com/neurobionics/opensourceleg
 Description-Content-Type: text/markdown
 
 <div align="center">
```

