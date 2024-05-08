# Comparing `tmp/mini-maze-0.1.1.tar.gz` & `tmp/mini_maze-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mini-maze-0.1.1.tar", last modified: Thu Mar 21 17:45:48 2024, max compression
+gzip compressed data, was "dist\mini_maze-0.1.2.tar", last modified: Tue May  7 19:27:48 2024, max compression
```

## Comparing `mini-maze-0.1.1.tar` & `mini_maze-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 17:45:48.332412 mini-maze-0.1.1/
--rw-rw-rw-   0        0        0     1087 2024-03-17 06:34:52.000000 mini-maze-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     3989 2024-03-21 17:45:48.331412 mini-maze-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3480 2024-03-21 05:34:56.000000 mini-maze-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-03-21 17:45:48.332412 mini-maze-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      846 2024-03-21 17:40:23.000000 mini-maze-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-21 17:45:48.318411 mini-maze-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-03-21 17:45:48.324412 mini-maze-0.1.1/src/mini_maze/
--rw-rw-rw-   0        0        0       84 2024-03-17 08:18:43.000000 mini-maze-0.1.1/src/mini_maze/__init__.py
--rw-rw-rw-   0        0        0     3818 2024-03-21 05:11:08.000000 mini-maze-0.1.1/src/mini_maze/maze_generator.py
--rw-rw-rw-   0        0        0     3380 2024-03-21 05:29:59.000000 mini-maze-0.1.1/src/mini_maze/mini_maze.py
-drwxrwxrwx   0        0        0        0 2024-03-21 17:45:48.330412 mini-maze-0.1.1/src/mini_maze.egg-info/
--rw-rw-rw-   0        0        0     3989 2024-03-21 17:45:48.000000 mini-maze-0.1.1/src/mini_maze.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2024-03-21 17:45:48.000000 mini-maze-0.1.1/src/mini_maze.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 17:45:48.000000 mini-maze-0.1.1/src/mini_maze.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-03-21 17:45:48.000000 mini-maze-0.1.1/src/mini_maze.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-21 17:45:48.000000 mini-maze-0.1.1/src/mini_maze.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 19:27:48.824565 mini_maze-0.1.2/
+-rw-rw-rw-   0        0        0     1087 2024-03-17 06:34:52.000000 mini_maze-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3986 2024-05-07 19:27:48.823564 mini_maze-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3480 2024-03-21 05:34:56.000000 mini_maze-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-07 19:27:48.824565 mini_maze-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      844 2024-05-07 19:27:44.000000 mini_maze-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 19:27:48.804565 mini_maze-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 19:27:48.815564 mini_maze-0.1.2/src/mini_maze/
+-rw-rw-rw-   0        0        0       84 2024-03-24 13:05:29.000000 mini_maze-0.1.2/src/mini_maze/__init__.py
+-rw-rw-rw-   0        0        0     6158 2024-03-31 20:27:58.000000 mini_maze-0.1.2/src/mini_maze/maze.py
+-rw-rw-rw-   0        0        0     3818 2024-03-24 14:39:37.000000 mini_maze-0.1.2/src/mini_maze/maze_generator.py
+-rw-rw-rw-   0        0        0     2932 2024-03-31 20:27:37.000000 mini_maze-0.1.2/src/mini_maze/mini_maze-updated.py
+-rw-rw-rw-   0        0        0     3646 2024-04-10 05:30:50.000000 mini_maze-0.1.2/src/mini_maze/mini_maze.py
+drwxrwxrwx   0        0        0        0 2024-05-07 19:27:48.822565 mini_maze-0.1.2/src/mini_maze.egg-info/
+-rw-rw-rw-   0        0        0     3986 2024-05-07 19:27:48.000000 mini_maze-0.1.2/src/mini_maze.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2024-05-07 19:27:48.000000 mini_maze-0.1.2/src/mini_maze.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 19:27:48.000000 mini_maze-0.1.2/src/mini_maze.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-07 19:27:48.000000 mini_maze-0.1.2/src/mini_maze.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-07 19:27:48.000000 mini_maze-0.1.2/src/mini_maze.egg-info/top_level.txt
```

### Comparing `mini-maze-0.1.1/LICENSE` & `mini_maze-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mini-maze-0.1.1/PKG-INFO` & `mini_maze-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mini-maze
-Version: 0.1.1
+Version: 0.1.2
 Summary: A mini-maze environment for reinforcement learning experiments
-Home-page: https://github.com/yourusername/mini-maze
+Home-page: https://github.com/mshaocong/mini-maze
 Author: Shaocong Ma
 Author-email: scma0908@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `mini-maze-0.1.1/README.md` & `mini_maze-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mini-maze-0.1.1/setup.py` & `mini_maze-0.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mini-maze',
-    version='0.1.1',
+    version='0.1.2',
     author='Shaocong Ma',
     author_email='scma0908@gmail.com',
     description='A mini-maze environment for reinforcement learning experiments',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url='https://github.com/yourusername/mini-maze',
+    url='https://github.com/mshaocong/mini-maze',
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     include_package_data=True,
     install_requires=[
-        'minigrid>=2.1.0' # List your project's dependencies here
+        'minigrid>=2.1.0'  # List your project's dependencies here
         # e.g., 'numpy', 'gym',
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
```

### Comparing `mini-maze-0.1.1/src/mini_maze/maze_generator.py` & `mini_maze-0.1.2/src/mini_maze/maze_generator.py`

 * *Files identical despite different names*

### Comparing `mini-maze-0.1.1/src/mini_maze/mini_maze.py` & `mini_maze-0.1.2/src/mini_maze/mini_maze-updated.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,31 +3,30 @@
 import random
 from minigrid.core.grid import Grid
 from minigrid.core.mission import MissionSpace
 from minigrid.core.world_object import Goal, Wall
 from minigrid.minigrid_env import MiniGridEnv
 
 from .maze_generator import find_next_state
+from .maze import Maze
 
 
 class MiniMazeEnv(MiniGridEnv):
     def __init__(
             self,
-            maze,
-            start_pos=(1, 1),
-            target_pos=None,
+            maze: Maze,
             max_steps: int | None = None,
             **kwargs,
     ):
-        self.start_pos = start_pos
-        self.target_pos = target_pos
+        self.start_pos = maze.start
+        self.target_pos = maze.goal
         self.maze = maze
 
         mission_space = MissionSpace(mission_func=self._gen_mission)
-        size = max(len(maze), len(maze[0]))
+        size = max( maze.height, maze.width) # max(len(maze), len(maze[0]))
 
         if max_steps is None:
             max_steps = 4 * size ** 2
 
         super().__init__(
             mission_space=mission_space,
             grid_size=size,
@@ -42,34 +41,36 @@
         return "get to the green goal square"
 
     def _gen_grid(self, width, height):
         # Create an empty grid
         self.grid = Grid(width, height)
 
         # Populate the grid based on the input matrix
-        for i, row in enumerate(self.maze):
+        for i, row in enumerate(self.maze.maze):
             for j, item in enumerate(row):
                 if item == 1:  # Wall
                     self.grid.set(j, i, Wall())
 
         i, j = self.target_pos
         self.put_obj(Goal(), j, i)
 
         # Place the agent
         if self.start_pos is not None:
-            self.agent_pos = self.start_pos
+            i, j = self.start_pos
+            self.agent_pos = (j, i)
             self.agent_dir = 0
         else:
             self.place_agent()
 
         self.mission = "get to the green goal square"
 
     def get_optimal_action(self):
         # Evaluate the next state.
-        next_state = find_next_state(self.maze, self.agent_pos, self.target_pos)
+        i, j = self.target_pos
+        next_state = find_next_state(self.maze, self.agent_pos, (j,i))
         assert next_state is not None
         move = {0: (1, 0), 1: (0, 1), 2: (-1, 0), 3: (0, -1)}
         left_dir = self.agent_dir - 1
         if left_dir < 0:
             left_dir += 4
         left_pos = (self.agent_pos[0] + move[left_dir][0], self.agent_pos[1] + move[left_dir][1])
         right_dir = (self.agent_dir + 1) % 4
@@ -81,26 +82,7 @@
         elif next_state[0] == left_pos[0] and next_state[1] == left_pos[1]:
             return 0  # turn left
         elif next_state[0] == right_pos[0] and next_state[1] == right_pos[1]:
             return 1  # turn right
         else:
             return random.choice([0, 1])
 
-
-if __name__ == "__main__":
-    from minigrid.manual_control import ManualControl
-
-    maze = [
-        [1, 1, 1, 1, 1],
-        [1, 0, 0, 1, 1],
-        [1, 0, 1, 0, 1],
-        [1, 0, 0, 0, 1],
-        [1, 1, 1, 1, 1]
-    ]
-
-    start_pos = (1, 1)
-    target_pos = (3, 3)
-    env = MiniMazeEnv(maze, start_pos=start_pos, target_pos=target_pos, render_mode="human")
-
-    # enable manual control for testing
-    manual_control = ManualControl(env, seed=42)
-    manual_control.start()
```

### Comparing `mini-maze-0.1.1/src/mini_maze.egg-info/PKG-INFO` & `mini_maze-0.1.2/src/mini_maze.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mini-maze
-Version: 0.1.1
+Version: 0.1.2
 Summary: A mini-maze environment for reinforcement learning experiments
-Home-page: https://github.com/yourusername/mini-maze
+Home-page: https://github.com/mshaocong/mini-maze
 Author: Shaocong Ma
 Author-email: scma0908@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

