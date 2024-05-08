# Comparing `tmp/cellworld_gym-0.0.91.tar.gz` & `tmp/cellworld_gym-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellworld_gym-0.0.91.tar", last modified: Thu May  2 17:22:08 2024, max compression
+gzip compressed data, was "cellworld_gym-0.0.96.tar", last modified: Wed May  8 18:39:59 2024, max compression
```

## Comparing `cellworld_gym-0.0.91.tar` & `cellworld_gym-0.0.96.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 17:22:08.254638 cellworld_gym-0.0.91/
--rw-rw-rw-   0        0        0       35 2024-05-02 17:22:07.000000 cellworld_gym-0.0.91/MANIFEST.in
--rw-rw-rw-   0        0        0      455 2024-05-02 17:22:08.253638 cellworld_gym-0.0.91/PKG-INFO
--rw-rw-rw-   0        0        0       40 2024-05-02 17:22:07.000000 cellworld_gym-0.0.91/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 17:22:08.193639 cellworld_gym-0.0.91/cellworld_gym/
--rw-rw-rw-   0        0        0       40 2024-05-02 17:22:07.000000 cellworld_gym-0.0.91/cellworld_gym/README.md
--rw-rw-rw-   0        0        0       73 2024-05-01 14:24:56.000000 cellworld_gym-0.0.91/cellworld_gym/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 17:22:08.217638 cellworld_gym-0.0.91/cellworld_gym/__pycache__/
--rw-rw-rw-   0        0        0      251 2024-05-01 23:56:14.000000 cellworld_gym-0.0.91/cellworld_gym/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     4221 2024-04-25 16:59:59.000000 cellworld_gym-0.0.91/cellworld_gym/__pycache__/core.cpython-312.pyc
--rw-rw-rw-   0        0        0     2221 2024-04-25 16:59:42.000000 cellworld_gym-0.0.91/cellworld_gym/core.py
-drwxrwxrwx   0        0        0        0 2024-05-02 17:22:08.244638 cellworld_gym-0.0.91/cellworld_gym/envs/
--rw-rw-rw-   0        0        0      504 2024-05-01 14:24:32.000000 cellworld_gym-0.0.91/cellworld_gym/envs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 17:22:08.250638 cellworld_gym-0.0.91/cellworld_gym/envs/__pycache__/
--rw-rw-rw-   0        0        0      725 2024-05-01 23:56:14.000000 cellworld_gym-0.0.91/cellworld_gym/envs/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     9658 2024-05-01 23:56:14.000000 cellworld_gym-0.0.91/cellworld_gym/envs/__pycache__/bot_evade.cpython-312.pyc
--rw-rw-rw-   0        0        0    10736 2024-05-01 23:56:18.000000 cellworld_gym-0.0.91/cellworld_gym/envs/__pycache__/dual_evade.cpython-312.pyc
--rw-rw-rw-   0        0        0     9750 2024-05-01 23:56:18.000000 cellworld_gym-0.0.91/cellworld_gym/envs/__pycache__/oasis.cpython-312.pyc
--rw-rw-rw-   0        0        0     5728 2024-05-02 17:21:49.000000 cellworld_gym-0.0.91/cellworld_gym/envs/bot_evade.py
--rw-rw-rw-   0        0        0     7316 2024-05-02 17:22:03.000000 cellworld_gym-0.0.91/cellworld_gym/envs/dual_evade.py
--rw-rw-rw-   0        0        0     5960 2024-05-02 17:22:03.000000 cellworld_gym-0.0.91/cellworld_gym/envs/oasis.py
--rw-rw-rw-   0        0        0     1636 2024-05-02 17:22:07.000000 cellworld_gym-0.0.91/cellworld_gym/license.txt
--rw-rw-rw-   0        0        0      180 2024-05-02 17:22:07.000000 cellworld_gym-0.0.91/cellworld_gym/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-02 17:22:08.252647 cellworld_gym-0.0.91/cellworld_gym.egg-info/
--rw-rw-rw-   0        0        0      455 2024-05-02 17:22:08.000000 cellworld_gym-0.0.91/cellworld_gym.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      818 2024-05-02 17:22:08.000000 cellworld_gym-0.0.91/cellworld_gym.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 17:22:08.000000 cellworld_gym-0.0.91/cellworld_gym.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-02 17:22:08.000000 cellworld_gym-0.0.91/cellworld_gym.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       19 2024-05-02 17:22:08.000000 cellworld_gym-0.0.91/cellworld_gym.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-02 17:22:08.000000 cellworld_gym-0.0.91/cellworld_gym.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 17:22:08.254638 cellworld_gym-0.0.91/setup.cfg
--rw-rw-rw-   0        0        0      652 2024-05-02 17:22:07.000000 cellworld_gym-0.0.91/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 18:39:59.618233 cellworld_gym-0.0.96/
+-rw-rw-rw-   0        0        0       35 2024-05-08 18:39:58.000000 cellworld_gym-0.0.96/MANIFEST.in
+-rw-rw-rw-   0        0        0      455 2024-05-08 18:39:59.617235 cellworld_gym-0.0.96/PKG-INFO
+-rw-rw-rw-   0        0        0       40 2024-05-08 18:39:58.000000 cellworld_gym-0.0.96/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 18:39:59.555231 cellworld_gym-0.0.96/cellworld_gym/
+-rw-rw-rw-   0        0        0       40 2024-05-08 18:39:58.000000 cellworld_gym-0.0.96/cellworld_gym/README.md
+-rw-rw-rw-   0        0        0       73 2024-05-01 14:24:56.000000 cellworld_gym-0.0.96/cellworld_gym/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 18:39:59.583233 cellworld_gym-0.0.96/cellworld_gym/__pycache__/
+-rw-rw-rw-   0        0        0      251 2024-05-01 23:56:14.000000 cellworld_gym-0.0.96/cellworld_gym/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4221 2024-04-25 16:59:59.000000 cellworld_gym-0.0.96/cellworld_gym/__pycache__/core.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2221 2024-04-25 16:59:42.000000 cellworld_gym-0.0.96/cellworld_gym/core.py
+drwxrwxrwx   0        0        0        0 2024-05-08 18:39:59.609235 cellworld_gym-0.0.96/cellworld_gym/envs/
+-rw-rw-rw-   0        0        0      504 2024-05-01 14:24:32.000000 cellworld_gym-0.0.96/cellworld_gym/envs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 18:39:59.615231 cellworld_gym-0.0.96/cellworld_gym/envs/__pycache__/
+-rw-rw-rw-   0        0        0      725 2024-05-01 23:56:14.000000 cellworld_gym-0.0.96/cellworld_gym/envs/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9658 2024-05-01 23:56:14.000000 cellworld_gym-0.0.96/cellworld_gym/envs/__pycache__/bot_evade.cpython-312.pyc
+-rw-rw-rw-   0        0        0    10736 2024-05-01 23:56:18.000000 cellworld_gym-0.0.96/cellworld_gym/envs/__pycache__/dual_evade.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9750 2024-05-01 23:56:18.000000 cellworld_gym-0.0.96/cellworld_gym/envs/__pycache__/oasis.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5728 2024-05-03 17:03:10.000000 cellworld_gym-0.0.96/cellworld_gym/envs/bot_evade.py
+-rw-rw-rw-   0        0        0     8043 2024-05-08 14:24:11.000000 cellworld_gym-0.0.96/cellworld_gym/envs/dual_evade.py
+-rw-rw-rw-   0        0        0     5960 2024-05-03 17:03:21.000000 cellworld_gym-0.0.96/cellworld_gym/envs/oasis.py
+-rw-rw-rw-   0        0        0     1636 2024-05-08 18:39:58.000000 cellworld_gym-0.0.96/cellworld_gym/license.txt
+-rw-rw-rw-   0        0        0      180 2024-05-08 18:39:58.000000 cellworld_gym-0.0.96/cellworld_gym/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 18:39:59.616247 cellworld_gym-0.0.96/cellworld_gym.egg-info/
+-rw-rw-rw-   0        0        0      455 2024-05-08 18:39:59.000000 cellworld_gym-0.0.96/cellworld_gym.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      818 2024-05-08 18:39:59.000000 cellworld_gym-0.0.96/cellworld_gym.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 18:39:59.000000 cellworld_gym-0.0.96/cellworld_gym.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-08 18:39:59.000000 cellworld_gym-0.0.96/cellworld_gym.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       19 2024-05-08 18:39:59.000000 cellworld_gym-0.0.96/cellworld_gym.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-08 18:39:59.000000 cellworld_gym-0.0.96/cellworld_gym.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 18:39:59.618233 cellworld_gym-0.0.96/setup.cfg
+-rw-rw-rw-   0        0        0      652 2024-05-08 18:39:58.000000 cellworld_gym-0.0.96/setup.py
```

### Comparing `cellworld_gym-0.0.91/cellworld_gym/__pycache__/core.cpython-312.pyc` & `cellworld_gym-0.0.96/cellworld_gym/__pycache__/core.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_gym-0.0.91/cellworld_gym/core.py` & `cellworld_gym-0.0.96/cellworld_gym/core.py`

 * *Files identical despite different names*

### Comparing `cellworld_gym-0.0.91/cellworld_gym/envs/__pycache__/__init__.cpython-312.pyc` & `cellworld_gym-0.0.96/cellworld_gym/envs/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_gym-0.0.91/cellworld_gym/envs/__pycache__/bot_evade.cpython-312.pyc` & `cellworld_gym-0.0.96/cellworld_gym/envs/__pycache__/bot_evade.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_gym-0.0.91/cellworld_gym/envs/__pycache__/dual_evade.cpython-312.pyc` & `cellworld_gym-0.0.96/cellworld_gym/envs/__pycache__/dual_evade.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_gym-0.0.91/cellworld_gym/envs/__pycache__/oasis.cpython-312.pyc` & `cellworld_gym-0.0.96/cellworld_gym/envs/__pycache__/oasis.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_gym-0.0.91/cellworld_gym/envs/bot_evade.py` & `cellworld_gym-0.0.96/cellworld_gym/envs/bot_evade.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -80,14 +80,15 @@
         return self.observation
 
     def set_action(self, action: int):
         self.model.prey.set_destination(self.action_list[action])
 
     def __step__(self):
         with pulsekit.CodeBlock("botevadeenv.__step__"):
+            self.step_count += 1
             truncated = (self.step_count >= self.max_step)
             obs = self.__update_observation__()
             reward = self.reward_function(obs)
             self.episode_reward += reward
 
             if self.model.puffed:
                 self.model.puffed = False
@@ -99,15 +100,14 @@
                         "survived": survived,
                         "agents": {}}
                 for agent_name, agent in self.model.agents.items():
                     info["agents"][agent_name] = {}
                     info["agents"][agent_name] = agent.get_stats()
             else:
                 info = {}
-            self.step_count += 1
         return obs, reward, not self.model.running, truncated, info
 
     def replay_step(self, agents_state: typing.Dict[str, AgentState]):
         self.model.set_agents_state(agents_state=agents_state,
                                     delta_t=self.time_step)
         return self.__step__()
```

### Comparing `cellworld_gym-0.0.91/cellworld_gym/envs/dual_evade.py` & `cellworld_gym-0.0.96/cellworld_gym/envs/dual_evade.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,43 +10,65 @@
 from gymnasium import spaces
 
 
 class DualEvadeObservation(Observation):
     fields = ["self_x",
               "self_y",
               "self_direction",
+              "predator_x",
+              "predator_y",
+              "predator_direction",
+              "prey_goal_distance",
+              "predator_prey_distance",
+              "puffed",
+              "puff_cooled_down",
+              "finished"]
+
+
+class DualEvadeObservationWithOther(DualEvadeObservation):
+    fields = ["self_x",
+              "self_y",
+              "self_direction",
               "other_x",
               "other_y",
               "other_direction",
               "predator_x",
               "predator_y",
               "predator_direction",
               "prey_goal_distance",
               "predator_prey_distance",
               "puffed",
               "puff_cooled_down",
               "finished"]
 
 
 class DualEvadeEnv(Env):
+
     def __init__(self,
                  world_name: str,
                  use_lppos: bool,
                  use_predator: bool,
                  max_step: int = 300,
                  reward_function: typing.Callable[[DualEvadeObservation], float] = lambda x: 0,
                  time_step: float = .25,
                  render: bool = False,
                  real_time: bool = False,
-                 end_on_pov_goal: bool = True):
+                 end_on_pov_goal: bool = True,
+                 use_other: bool = True):
         self.max_step = max_step
         self.reward_function = reward_function
         self.time_step = time_step
         self.loader = cwgame.CellWorldLoader(world_name=world_name)
-        self.observation = DualEvadeObservation()
+        self.use_other = use_other
+        if use_other:
+            self.observation = DualEvadeObservationWithOther()
+            self.other_observation = DualEvadeObservationWithOther()
+        else:
+            self.other_observation = DualEvadeObservation()
+            self.observation = DualEvadeObservation()
         self.observation_space = spaces.Box(-np.inf, np.inf, (len(self.observation),), dtype=np.float32)
         self.end_on_pov_goal = end_on_pov_goal
         if use_lppos:
             self.action_list = self.loader.tlppo_action_list
         else:
             self.action_list = self.loader.full_action_list
 
@@ -56,37 +78,37 @@
                                       real_time=real_time,
                                       render=render,
                                       use_predator=use_predator)
         self.prey_trajectory_length = 0
         self.predator_trajectory_length = 0
         self.episode_reward = 0
         self.step_count = 0
-        self.other_observation = DualEvadeObservation()
         self.prey = self.model.prey_1
         self.other = self.model.prey_2
         self.prey_data = self.model.prey_data_1
         self.other_data = self.model.prey_data_2
         self.other_policy = lambda x: random.randint(0, len(self.action_list) - 1)
 
     def set_other_policy(self, other_policy: typing.Callable[[DualEvadeObservation], int]):
         self.other_policy = other_policy
 
     def __update_observation__(self, observation: DualEvadeObservation, prey, prey_data, other):
         observation.self_x = prey.state.location[0]
         observation.self_y = prey.state.location[1]
         observation.self_direction = math.radians(prey.state.direction)
 
-        if self.model.mouse_visible:
-            observation.other_x = other.state.location[0]
-            observation.other_y = other.state.location[1]
-            observation.other_direction = math.radians(other.state.direction)
-        else:
-            observation.other_x = 0
-            observation.other_y = 0
-            observation.other_direction = 0
+        if self.use_other:
+            if self.model.mouse_visible:
+                observation.other_x = other.state.location[0]
+                observation.other_y = other.state.location[1]
+                observation.other_direction = math.radians(other.state.direction)
+            else:
+                observation.other_x = 0
+                observation.other_y = 0
+                observation.other_direction = 0
 
         if self.model.use_predator and prey_data.predator_visible:
             observation.predator_x = self.model.predator.state.location[0]
             observation.predator_y = self.model.predator.state.location[1]
             observation.predator_direction = math.radians(self.model.predator.state.direction)
         else:
             observation.predator_x = 0
@@ -101,14 +123,15 @@
         return observation
 
     def set_actions(self, action: int, other_action: int):
         self.prey.set_destination(self.action_list[action])
         self.other.set_destination(self.action_list[other_action])
 
     def __step__(self):
+        self.step_count += 1
         truncated = (self.step_count >= self.max_step)
 
         obs = self.__update_observation__(observation=self.observation,
                                           prey=self.prey,
                                           prey_data=self.prey_data,
                                           other=self.other)
         reward = self.reward_function(obs)
@@ -129,15 +152,14 @@
                     "survived": survived,
                     "agents": {}}
             for agent_name, agent in self.model.agents.items():
                 info["agents"][agent_name] = {}
                 info["agents"][agent_name] = agent.get_stats()
         else:
             info = {}
-        self.step_count += 1
         return obs, reward, not self.model.running, truncated, info
 
     def replay_step(self, agents_state: typing.Dict[str, AgentState]):
         self.model.set_agents_state(agents_state=agents_state,
                                     delta_t=self.time_step)
         return self.__step__()
```

### Comparing `cellworld_gym-0.0.91/cellworld_gym/envs/oasis.py` & `cellworld_gym-0.0.96/cellworld_gym/envs/oasis.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -88,14 +88,15 @@
         self.observation.finished = not self.model.running
         return self.observation
 
     def set_action(self, action: int):
         self.model.prey.set_destination(self.action_list[action])
 
     def __step__(self):
+        self.step_count += 1
         truncated = (self.step_count >= self.max_step)
         obs = self.__update_observation__()
         reward = self.reward_function(obs)
         self.episode_reward += reward
 
         if self.model.puffed:
             self.model.puffed = False
@@ -107,15 +108,14 @@
                     "survived": survived,
                     "agents": {}}
             for agent_name, agent in self.model.agents.items():
                 info["agents"][agent_name] = {}
                 info["agents"][agent_name] = agent.get_stats()
         else:
             info = {}
-        self.step_count += 1
         return obs, reward, not self.model.running, truncated, info
 
     def replay_step(self, agents_state: typing.Dict[str, AgentState]):
         self.model.set_agents_state(agents_state=agents_state,
                                     delta_t=self.time_step)
         return self.__step__()
```

### Comparing `cellworld_gym-0.0.91/cellworld_gym/license.txt` & `cellworld_gym-0.0.96/cellworld_gym/license.txt`

 * *Files identical despite different names*

### Comparing `cellworld_gym-0.0.91/cellworld_gym.egg-info/SOURCES.txt` & `cellworld_gym-0.0.96/cellworld_gym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellworld_gym-0.0.91/setup.py` & `cellworld_gym-0.0.96/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,9 +7,9 @@
       author_email='germanespinosa@gmail.com',
       long_description=open('./cellworld_gym/README.md').read() + '\n---\n<small>Package created with Easy-pack</small>\n',
       long_description_content_type='text/markdown',
       packages=['cellworld_gym'],
       install_requires=['cellworld_game', 'gym'],
       license='MIT',
       include_package_data=True,
-      version='0.0.91',
+      version='0.0.96',
       zip_safe=False)
```

